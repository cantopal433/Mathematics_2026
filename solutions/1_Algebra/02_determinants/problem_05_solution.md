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

All three operations below are of the form $R_i\leftarrow R_i+cR_j$ with $i\ne j$. Such an operation does not change the determinant: the determinant is linear in row $i$, so the new determinant equals $\det A$ plus $c$ times the determinant of a matrix in which row $i$ is replaced by row $j$. That second matrix has two equal rows, so its determinant is $0$.

Step 1: $R_2\leftarrow R_2-2R_1$, which gives $(2-2,\ 1-4,\ 0-6)=(0,-3,-6)$:

$$
\begin{pmatrix}
1 & 2 & 3 \\
0 & -3 & -6 \\
-1 & 4 & 2
\end{pmatrix}.
$$

A multiple of row 1 was added to row 2, so the determinant stays equal to $\det A$.

Step 2: $R_3\leftarrow R_3+R_1$, which gives $(-1+1,\ 4+2,\ 2+3)=(0,6,5)$:

$$
\begin{pmatrix}
1 & 2 & 3 \\
0 & -3 & -6 \\
0 & 6 & 5
\end{pmatrix}.
$$

Row 1 was added to row 3, so the determinant again does not change.

Step 3: $R_3\leftarrow R_3+2R_2$, which gives $(0,\ 6-6,\ 5-12)=(0,0,-7)$:

$$
\begin{pmatrix}
1 & 2 & 3 \\
0 & -3 & -6 \\
0 & 0 & -7
\end{pmatrix}.
$$

A multiple of row 2 was added to row 3, so the determinant is still unchanged.

The final matrix is upper triangular, so its determinant is the product of the diagonal entries. Since no step changed the determinant,

$$
\det A=1\cdot(-3)\cdot(-7)=21.
$$

## Verification

Direct cofactor expansion of the original matrix along the first row:

$$
\det A=1\cdot(1\cdot2-0\cdot4)-2\cdot(2\cdot2-0\cdot(-1))+3\cdot(2\cdot4-1\cdot(-1))=2-8+27=21.
$$

This agrees with the result obtained by row operations.
