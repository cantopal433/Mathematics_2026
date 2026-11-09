## Question

For

$$
A=
\begin{pmatrix}
1 & 2 & 3 \\
4 & 5 & 6 \\
\end{pmatrix},\qquad B=
\begin{pmatrix}
1 & 0 \\
2 & 1 \\
-1 & 3 \\
\end{pmatrix}
$$

compute $A^T$, $B^T$, and $AB$. Then verify in this example that

$$
(AB)^T=B^TA^T.
$$

## Solution

The transpose turns rows into columns:

$$
A^T=
\begin{pmatrix}
1 & 4 \\
2 & 5 \\
3 & 6
\end{pmatrix},\qquad
B^T=
\begin{pmatrix}
1 & 2 & -1 \\
0 & 1 & 3
\end{pmatrix},\qquad
AB=
\begin{pmatrix}
2 & 11 \\
8 & 23
\end{pmatrix}.
$$

## Verification

$$
(AB)^T=
\begin{pmatrix}
2 & 8 \\
11 & 23
\end{pmatrix},\qquad
B^TA^T=
\begin{pmatrix}
2 & 8 \\
11 & 23
\end{pmatrix},
$$

so $(AB)^T=B^TA^T$.
