## Question

Let

$$
F=
\begin{pmatrix}
1 & 1 \\
1 & 0 \\
\end{pmatrix}.
$$

Compute $F^2$, $F^3$, $F^4$, and $F^5$. Compare the numbers obtained with the sequence

$$
0,1,1,2,3,5,8,\ldots
$$

and describe the relationship you observe. Then compute

$$
F
\begin{pmatrix}
a \\
b \\
\end{pmatrix}
$$

and explain how this multiplication performs one recurrence step: it creates the sum of two consecutive terms and keeps one of them for the next step.

## Solution

Each power is obtained by multiplying the previous one by $F$:

$$
F^2=
\begin{pmatrix}
2 & 1 \\
1 & 1 \\
\end{pmatrix},\quad
F^3=
\begin{pmatrix}
3 & 2 \\
2 & 1 \\
\end{pmatrix},\quad
F^4=
\begin{pmatrix}
5 & 3 \\
3 & 2 \\
\end{pmatrix},\quad
F^5=
\begin{pmatrix}
8 & 5 \\
5 & 3 \\
\end{pmatrix}.
$$

For example,

$$
F^3=F^2F=
\begin{pmatrix}
2 & 1 \\
1 & 1 \\
\end{pmatrix}
\begin{pmatrix}
1 & 1 \\
1 & 0 \\
\end{pmatrix}=
\begin{pmatrix}
2+1 & 2+0 \\
1+1 & 1+0 \\
\end{pmatrix}=
\begin{pmatrix}
3 & 2 \\
2 & 1 \\
\end{pmatrix}.
$$

All entries are terms of the Fibonacci sequence $f_0=0,\ f_1=1,\ f_2=1,\ f_3=2,\ f_4=3,\ f_5=5,\ f_6=8,\ldots$, in which every term is the sum of the two previous ones. In each power, three consecutive terms appear:

$$
F^n=
\begin{pmatrix}
f_{n+1} & f_n \\
f_n & f_{n-1} \\
\end{pmatrix}.
$$

For instance, $F^5$ contains $f_6=8$, $f_5=5$ and $f_4=3$.

Multiplying $F$ by a general vector gives

$$
F
\begin{pmatrix}
a \\
b \\
\end{pmatrix}=
\begin{pmatrix}
1\cdot a+1\cdot b \\
1\cdot a+0\cdot b \\
\end{pmatrix}=
\begin{pmatrix}
a+b \\
a \\
\end{pmatrix}.
$$

This is one step of the recurrence. If the vector holds two consecutive terms, $a=f_k$ and $b=f_{k-1}$, then the first entry of the result is their sum $f_k+f_{k-1}=f_{k+1}$, the next term. The second entry keeps $f_k$, so the new vector again holds two consecutive terms and is ready for the next step.

## Verification

Starting from $(f_1,f_0)^T=(1,0)^T$ and applying $F$ repeatedly:

$$
\begin{pmatrix}
1 \\
0 \\
\end{pmatrix}\to
\begin{pmatrix}
1 \\
1 \\
\end{pmatrix}\to
\begin{pmatrix}
2 \\
1 \\
\end{pmatrix}\to
\begin{pmatrix}
3 \\
2 \\
\end{pmatrix}\to
\begin{pmatrix}
5 \\
3 \\
\end{pmatrix}\to
\begin{pmatrix}
8 \\
5 \\
\end{pmatrix}.
$$

The first entries $1,1,2,3,5,8$ are exactly the Fibonacci numbers, in agreement with the entries of $F^2,\ldots,F^5$.
