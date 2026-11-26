## Question

For

$$
A=
\begin{pmatrix}
2 & 1 \\
1 & 3 \\
\end{pmatrix},\qquad b=
\begin{pmatrix}
7 \\
8 \\
\end{pmatrix}
$$

solve $Ax=b$ in two ways:

1. using $A^{-1}b$,
2. using Gaussian elimination.

Compare both solutions, the number of essential steps, and state which method was simpler in this example.

## Solution

**Method 1: $x=A^{-1}b$.** The determinant is $\det A=2\cdot3-1\cdot1=5\ne0$, so

$$
A^{-1}=\frac15
\begin{pmatrix}
3 & -1 \\
-1 & 2 \\
\end{pmatrix}
$$

and

$$
x=A^{-1}b=\frac15
\begin{pmatrix}
3\cdot7-1\cdot8 \\
-1\cdot7+2\cdot8 \\
\end{pmatrix}=\frac15
\begin{pmatrix}
13 \\
9 \\
\end{pmatrix}=
\begin{pmatrix}
\frac{13}{5} \\
\frac95 \\
\end{pmatrix}.
$$

**Method 2: Gaussian elimination.** The augmented matrix is

$$
\begin{pmatrix}
2 & 1 & \mid & 7 \\
1 & 3 & \mid & 8 \\
\end{pmatrix}
$$

Interchanging the rows puts the coefficient $1$ in the pivot position, which avoids fractions in the first step:

$$
\begin{pmatrix}
1 & 3 & \mid & 8 \\
2 & 1 & \mid & 7 \\
\end{pmatrix}
$$

Then $R_2\leftarrow R_2-2R_1$:

$$
\begin{pmatrix}
1 & 3 & \mid & 8 \\
0 & -5 & \mid & -9 \\
\end{pmatrix}
$$

Back substitution: $-5y=-9$ gives $y=\frac95$, and then $x=8-3\cdot\frac95=\frac{40-27}{5}=\frac{13}{5}$.

**Comparison.** Both methods give the same solution $(x,y)=\left(\frac{13}{5},\ \frac95\right)$.

- The inverse method needs three essential steps: the determinant, the inverse matrix, and a matrix-vector product with four multiplications.
- Elimination needs two essential steps: one row operation (after an optional row interchange) and a short back substitution.

In this example elimination was simpler, because there is only one right-hand side, and computing the whole inverse is more work than solving one system. The inverse method becomes worthwhile when $A^{-1}$ is already known or when many systems with the same matrix must be solved. In fact, this matrix $A$ is the same as in Exercise 6, so if its inverse from that exercise is reused, the inverse method reduces to a single matrix-vector product.

## Verification

$$
Ax=
\begin{pmatrix}
2 & 1 \\
1 & 3 \\
\end{pmatrix}
\begin{pmatrix}
\frac{13}{5} \\
\frac95 \\
\end{pmatrix}=
\begin{pmatrix}
\frac{26}{5}+\frac95 \\
\frac{13}{5}+\frac{27}{5} \\
\end{pmatrix}=
\begin{pmatrix}
7 \\
8 \\
\end{pmatrix}=b.
$$

The solution satisfies both equations.
