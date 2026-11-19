## Question

For

$$
A=
\begin{pmatrix}
2 & 1 \\
1 & 1 \\
\end{pmatrix},\qquad B=
\begin{pmatrix}
1 & -1 \\
-1 & 2 \\
\end{pmatrix}
$$

check, without using a formula, whether $B=A^{-1}$. Compute $AB$ and $BA$ and relate the result to the definition of the inverse.

## Solution

By definition, a matrix $B$ is the inverse of a square matrix $A$ if

$$
AB=I\qquad\mathrm{and}\qquad BA=I,
$$

where $I$ is the identity matrix of the same size. So it is enough to compute both products and compare them with $I$.

Each entry of a product is a row of the first factor times a column of the second:

$$
AB=
\begin{pmatrix}
2 & 1 \\
1 & 1 \\
\end{pmatrix}
\begin{pmatrix}
1 & -1 \\
-1 & 2 \\
\end{pmatrix}=
\begin{pmatrix}
2\cdot1+1\cdot(-1) & 2\cdot(-1)+1\cdot2 \\
1\cdot1+1\cdot(-1) & 1\cdot(-1)+1\cdot2 \\
\end{pmatrix}=
\begin{pmatrix}
1 & 0 \\
0 & 1 \\
\end{pmatrix},
$$

$$
BA=
\begin{pmatrix}
1 & -1 \\
-1 & 2 \\
\end{pmatrix}
\begin{pmatrix}
2 & 1 \\
1 & 1 \\
\end{pmatrix}=
\begin{pmatrix}
1\cdot2+(-1)\cdot1 & 1\cdot1+(-1)\cdot1 \\
(-1)\cdot2+2\cdot1 & (-1)\cdot1+2\cdot1 \\
\end{pmatrix}=
\begin{pmatrix}
1 & 0 \\
0 & 1 \\
\end{pmatrix}.
$$

Both products are equal to $I$, so $B$ satisfies the definition of the inverse and $B=A^{-1}$. Matrix multiplication is not commutative in general, which is why the definition requires both $AB=I$ and $BA=I$; here both conditions hold.

## Verification

As an independent check, $\det A=2\cdot1-1\cdot1=1$ and $\det B=1\cdot2-(-1)\cdot(-1)=1$. Then $\det A\cdot\det B=1=\det I$, which is consistent with $AB=I$.
