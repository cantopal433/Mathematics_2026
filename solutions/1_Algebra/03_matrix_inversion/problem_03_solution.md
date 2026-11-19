## Question

For

$$
A=
\begin{pmatrix}
2 & 4 \\
1 & 2 \\
\end{pmatrix}
$$

explain in two ways why $A^{-1}$ does not exist: using the determinant and using dependence between the rows.

## Solution

**First way: the determinant.** A square matrix is invertible if and only if its determinant is different from $0$. For the given matrix

$$
\det A=2\cdot2-4\cdot1=4-4=0.
$$

The determinant is zero, so $A^{-1}$ does not exist. This can also be seen from the $2\times2$ formula, which requires dividing by $\det A$, and division by $0$ is impossible.

**Second way: dependence between the rows.** The first row is twice the second row:

$$
(2,4)=2\cdot(1,2).
$$

The rows are linearly dependent, so the row operation $R_1\leftarrow R_1-2R_2$ produces a zero row:

$$
\begin{pmatrix}
0 & 0 \\
1 & 2 \\
\end{pmatrix}.
$$

A matrix with a zero row can never be reduced to the identity matrix by row operations, so the Gauss–Jordan method cannot produce an inverse. Equivalently, for every matrix $B$, the first row of $AB$ is twice its second row, so $AB$ can never equal $I$, whose rows $(1,0)$ and $(0,1)$ are not proportional.

## Verification

Both approaches agree: the zero determinant and the dependent rows describe the same fact. For example, $A$ sends the nonzero vector $(2,-1)^T$ to zero:

$$
A
\begin{pmatrix}
2 \\
-1 \\
\end{pmatrix}=
\begin{pmatrix}
4-4 \\
2-2 \\
\end{pmatrix}=
\begin{pmatrix}
0 \\
0 \\
\end{pmatrix},
$$

so no matrix can undo $A$, because a matrix applied to the zero vector always gives the zero vector, never $(2,-1)^T$.
