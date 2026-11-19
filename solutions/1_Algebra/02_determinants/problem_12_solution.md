## Question

For

$$
A(t)=
\begin{pmatrix}
1 & 2 & 3 \\
2 & 4 & t \\
0 & 1 & 1 \\
\end{pmatrix}
$$

find the values of $t$ for which the matrix is not invertible.

Before computing the determinant, perform the operation

$$
R_2\leftarrow R_2-2R_1
$$

and use the resulting structure. At the end, explain what special thing happens to the rows for the value of the parameter you found.

## Solution

The operation $R_2\leftarrow R_2-2R_1$ adds a multiple of the first row to the second row, so it does not change the determinant. It gives $(2-2,\ 4-4,\ t-6)=(0,0,t-6)$:

$$
\begin{pmatrix}
1 & 2 & 3 \\
0 & 0 & t-6 \\
0 & 1 & 1 \\
\end{pmatrix}.
$$

The first column now has only one nonzero entry, so the determinant can be expanded along that column:

$$
\det A(t)=1\cdot
\det
\begin{pmatrix}
0 & t-6 \\
1 & 1 \\
\end{pmatrix}=0\cdot1-(t-6)\cdot1=6-t.
$$

A square matrix is not invertible exactly when its determinant is $0$. Here

$$
6-t=0\quad\Longleftrightarrow\quad t=6,
$$

so $A(t)$ is not invertible only for $t=6$ and is invertible for every other value of $t$.

For $t=6$ the transformed second row is $(0,0,0)$. This means that in the original matrix the second row equals twice the first row:

$$
(2,4,6)=2\cdot(1,2,3).
$$

The rows are linearly dependent, which is exactly why the determinant vanishes and the matrix has no inverse.

## Verification

Direct cofactor expansion of $A(t)$ along the first row:

$$
1\cdot(4\cdot1-t\cdot1)-2\cdot(2\cdot1-t\cdot0)+3\cdot(2\cdot1-4\cdot0)=4-t-4+6=6-t.
$$

For example, $t=0$ gives $\det A(0)=6\ne0$, while $t=6$ gives $\det A(6)=0$.
