## Question

Given

$$
A=
\begin{pmatrix}
1 & 2 & 0 \\
0 & 1 & 1 \\
\end{pmatrix},\qquad B=
\begin{pmatrix}
1 & 2 \\
-1 & 0 \\
3 & 1 \\
\end{pmatrix}.
$$

Denote the columns of $B$ by $b_1,b_2$.

1. Compute $Ab_1$ and $Ab_2$.
2. Compute the matrix $AB$.
3. Compare the results and explain why the columns of $AB$ are exactly the vectors $Ab_1$ and $Ab_2$.

## Solution

$$
Ab_1=A
\begin{pmatrix}
1 \\
-1 \\
3
\end{pmatrix}=
\begin{pmatrix}
-1 \\
2
\end{pmatrix},\qquad
Ab_2=A
\begin{pmatrix}
2 \\
0 \\
1
\end{pmatrix}=
\begin{pmatrix}
2 \\
1
\end{pmatrix},
$$

$$
AB=
\begin{pmatrix}
-1 & 2 \\
2 & 1
\end{pmatrix}.
$$

Column $j$ of $AB$ uses only column $j$ of $B$, so it equals $Ab_j$.

## Verification

The columns of $AB$ are exactly $Ab_1$ and $Ab_2$.
