## Question

For

$$
A=
\begin{pmatrix}
1 & 2 & 3 \\
2 & 1 & 0 \\
-1 & 4 & 2 \\
\end{pmatrix}
$$

find $\det A$ by simplifying the matrix with row operations. At each step, indicate whether and how the determinant changes.

## Solution

Operations $R_i\leftarrow R_i+cR_j$ do not change $\det$.

$R_2-2R_1$, $R_3+R_1$, then $R_3+2R_2$:

$$
\begin{pmatrix}
1 & 2 & 3 \\
0 & -3 & -6 \\
0 & 0 & -7
\end{pmatrix},\qquad
\det A=1\cdot(-3)\cdot(-7)=21.
$$

## Verification

Direct expansion: $2-8+27=21$.
