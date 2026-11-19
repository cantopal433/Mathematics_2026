## Question

Given

$$
A=
\begin{pmatrix}
1 & 1 \\
0 & 1 \\
\end{pmatrix},\qquad B=
\begin{pmatrix}
a & b \\
c & d \\
\end{pmatrix}.
$$

Find the conditions on $a,b,c,d$ under which $AB=BA$. Describe the general form of all such matrices $B$.

## Solution

Both products are computed entry by entry, multiplying rows of the first factor by columns of the second:

$$
AB=
\begin{pmatrix}
1 & 1 \\
0 & 1 \\
\end{pmatrix}
\begin{pmatrix}
a & b \\
c & d \\
\end{pmatrix}=
\begin{pmatrix}
a+c & b+d \\
c & d \\
\end{pmatrix},
$$

$$
BA=
\begin{pmatrix}
a & b \\
c & d \\
\end{pmatrix}
\begin{pmatrix}
1 & 1 \\
0 & 1 \\
\end{pmatrix}=
\begin{pmatrix}
a & a+b \\
c & c+d \\
\end{pmatrix}.
$$

Two matrices are equal exactly when all corresponding entries are equal. Comparing the four entries gives:

- top left: $a+c=a$, so $c=0$,
- top right: $b+d=a+b$, so $d=a$,
- bottom left: $c=c$, which holds always,
- bottom right: $d=c+d$, so again $c=0$.

There is no condition on $b$. Therefore $AB=BA$ holds exactly for the matrices

$$
B=
\begin{pmatrix}
a & b \\
0 & a \\
\end{pmatrix}=aI+b
\begin{pmatrix}
0 & 1 \\
0 & 0 \\
\end{pmatrix},\qquad a,b\in\mathbb R.
$$

In words, $B$ must be upper triangular with equal diagonal entries. This family contains, for example, the identity $I$ ($a=1$, $b=0$) and the matrix $A$ itself ($a=b=1$).

## Verification

For $a=2$ and $b=3$:

$$
AB=
\begin{pmatrix}
1 & 1 \\
0 & 1 \\
\end{pmatrix}
\begin{pmatrix}
2 & 3 \\
0 & 2 \\
\end{pmatrix}=
\begin{pmatrix}
2 & 5 \\
0 & 2 \\
\end{pmatrix},\qquad
BA=
\begin{pmatrix}
2 & 3 \\
0 & 2 \\
\end{pmatrix}
\begin{pmatrix}
1 & 1 \\
0 & 1 \\
\end{pmatrix}=
\begin{pmatrix}
2 & 5 \\
0 & 2 \\
\end{pmatrix}.
$$

The two products are equal, as predicted.
