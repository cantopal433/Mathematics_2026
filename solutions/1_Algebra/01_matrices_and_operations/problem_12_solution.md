## Question

Let

$$
A=
\begin{pmatrix}
1 & 1 \\
0 & 1 \\
\end{pmatrix}.
$$

Compute $A^2$, $A^3$, and $A^4$, and use them to formulate a conjecture for $A^n$. Then do not stop after checking one more case: assume the formula is true for $n$, multiply by $A$, and explain why you obtain exactly the formula for $n+1$.

## Solution

Each power is obtained by multiplying the previous one by $A$:

$$
A^2=
\begin{pmatrix}
1 & 1 \\
0 & 1 \\
\end{pmatrix}
\begin{pmatrix}
1 & 1 \\
0 & 1 \\
\end{pmatrix}=
\begin{pmatrix}
1 & 2 \\
0 & 1 \\
\end{pmatrix},
$$

$$
A^3=A^2A=
\begin{pmatrix}
1 & 3 \\
0 & 1 \\
\end{pmatrix},\qquad
A^4=A^3A=
\begin{pmatrix}
1 & 4 \\
0 & 1 \\
\end{pmatrix}.
$$

The diagonal entries stay equal to $1$, the bottom left entry stays $0$, and the top right entry grows by $1$ with each multiplication. This suggests the conjecture

$$
A^n=
\begin{pmatrix}
1 & n \\
0 & 1 \\
\end{pmatrix}\qquad\mathrm{for\ all}\ n\ge1.
$$

The conjecture is proved by induction.

Base case: for $n=1$ the formula gives $A$ itself, so it holds.

Induction step: assume the formula holds for some $n$. Multiplying by $A$ gives

$$
A^{n+1}=A^nA=
\begin{pmatrix}
1 & n \\
0 & 1 \\
\end{pmatrix}
\begin{pmatrix}
1 & 1 \\
0 & 1 \\
\end{pmatrix}=
\begin{pmatrix}
1\cdot1+n\cdot0 & 1\cdot1+n\cdot1 \\
0\cdot1+1\cdot0 & 0\cdot1+1\cdot1 \\
\end{pmatrix}=
\begin{pmatrix}
1 & n+1 \\
0 & 1 \\
\end{pmatrix}.
$$

This is exactly the formula for $n+1$. The only entry that changes is the top right one, where $n$ becomes $n+1$, because the row $(1,\ n)$ multiplied by the column $(1,\ 1)^T$ gives $n+1$. Since the formula holds for $n=1$ and passes from $n$ to $n+1$, it holds for every $n\ge1$.

## Verification

The formula gives $A^2$, $A^3$, $A^4$ with top right entries $2$, $3$, $4$, which matches the direct calculations. One more direct product, $A^5=A^4A$, gives

$$
\begin{pmatrix}
1 & 4 \\
0 & 1 \\
\end{pmatrix}
\begin{pmatrix}
1 & 1 \\
0 & 1 \\
\end{pmatrix}=
\begin{pmatrix}
1 & 5 \\
0 & 1 \\
\end{pmatrix},
$$

which also agrees with the formula.
