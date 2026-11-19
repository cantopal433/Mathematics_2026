## Question

Compute

$$
\det
\begin{pmatrix}
1 & 2 & 3 \\
1 & 3 & 4 \\
1 & 4 & 6 \\
\end{pmatrix}
$$

by first performing row operations that create as many zeros as possible. State which operations do not change the determinant.

## Solution

Three types of row operations affect the determinant in different ways:

- adding a multiple of one row to another row does not change the determinant,
- interchanging two rows changes the sign of the determinant,
- multiplying a row by a number $c$ multiplies the determinant by $c$.

Only operations of the first type are used below, so the determinant never changes.

Step 1: $R_2\leftarrow R_2-R_1$ and $R_3\leftarrow R_3-R_1$. Every row starts with $1$, so subtracting the first row creates zeros in the first column:

$$
\begin{pmatrix}
1 & 2 & 3 \\
0 & 1 & 1 \\
0 & 2 & 3 \\
\end{pmatrix}.
$$

The determinant is unchanged, because a multiple of $R_1$ was added to $R_2$ and to $R_3$.

Step 2: $R_3\leftarrow R_3-2R_2$, which gives $(0,\ 2-2,\ 3-2)=(0,0,1)$:

$$
\begin{pmatrix}
1 & 2 & 3 \\
0 & 1 & 1 \\
0 & 0 & 1 \\
\end{pmatrix}.
$$

Again a multiple of another row was added, so the determinant is unchanged.

The matrix is now upper triangular, so its determinant is the product of the diagonal entries:

$$
\det=1\cdot1\cdot1=1.
$$

## Verification

Direct cofactor expansion of the original matrix along the first row:

$$
1\cdot(3\cdot6-4\cdot4)-2\cdot(1\cdot6-4\cdot1)+3\cdot(1\cdot4-3\cdot1)=2-4+3=1.
$$

This agrees with the result obtained by row operations.
