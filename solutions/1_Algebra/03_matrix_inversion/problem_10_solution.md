## Question

Given

$$
D=
\begin{pmatrix}
2 & 0 & 0 \\
0 & -3 & 0 \\
0 & 0 & 5 \\
\end{pmatrix},\qquad E=
\begin{pmatrix}
2 & 0 & 0 \\
0 & 0 & 0 \\
0 & 0 & 5 \\
\end{pmatrix}.
$$

Without using Gauss–Jordan elimination, decide which matrix is invertible. For the invertible matrix, give the inverse and check the result by multiplication.

## Solution

The determinant of a diagonal matrix is the product of its diagonal entries, and a matrix is invertible exactly when its determinant is nonzero:

$$
\det D=2\cdot(-3)\cdot5=-30\ne0,\qquad \det E=2\cdot0\cdot5=0.
$$

So $D$ is invertible and $E$ is not. For $E$ this is also visible directly: its second row is a zero row, so for every matrix $X$ the second row of $EX$ is zero, and $EX$ can never equal $I$.

For the invertible matrix $D$, the product of two diagonal matrices is computed entry by entry on the diagonal. To obtain $I$, each diagonal entry must be replaced by its reciprocal:

$$
D^{-1}=
\begin{pmatrix}
\frac12 & 0 & 0 \\
0 & -\frac13 & 0 \\
0 & 0 & \frac15 \\
\end{pmatrix}.
$$

The same idea fails for $E$, because the entry $0$ has no reciprocal.

## Verification

$$
DD^{-1}=
\begin{pmatrix}
2\cdot\frac12 & 0 & 0 \\
0 & (-3)\cdot\left(-\frac13\right) & 0 \\
0 & 0 & 5\cdot\frac15 \\
\end{pmatrix}=
\begin{pmatrix}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & 0 & 1 \\
\end{pmatrix}.
$$

The product is the identity matrix, so the inverse is correct.
