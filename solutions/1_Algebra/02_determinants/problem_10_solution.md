## Question

Without carrying out a full determinant calculation, explain why

$$
\det
\begin{pmatrix}
1 & 2 & 3 \\
2 & 4 & 6 \\
0 & 1 & 5 \\
\end{pmatrix}=0.
$$

Identify a specific dependence between the rows and connect it with noninvertibility of the matrix.

## Solution

$(2,4,6)=2\cdot(1,2,3)$, so after $R_2\leftarrow R_2-2R_1$ the second row is zero and $\det=0$.

The rows are dependent, so the matrix is not invertible.

## Verification

A matrix with a zero row has determinant $0$.
