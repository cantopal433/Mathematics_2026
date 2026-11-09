## Question

For

$$
A=
\begin{pmatrix}
1 & 2 \\
0 & 1 \\
\end{pmatrix},\qquad B=
\begin{pmatrix}
2 & 0 \\
3 & 1 \\
\end{pmatrix}
$$

compute $AB$ and $BA$. Is $AB=BA$? Use this example to explain what noncommutativity of matrix multiplication means.

## Solution

Entry $(i,j)$ of a product is row $i$ of the first matrix times column $j$ of the second:

$$
AB=
\begin{pmatrix}
1\cdot2+2\cdot3 & 1\cdot0+2\cdot1 \\
0\cdot2+1\cdot3 & 0\cdot0+1\cdot1
\end{pmatrix}=
\begin{pmatrix}
8 & 2 \\
3 & 1
\end{pmatrix},\qquad
BA=
\begin{pmatrix}
2 & 4 \\
3 & 7
\end{pmatrix}.
$$

Since $AB\ne BA$, matrix multiplication is not commutative: the order of the factors matters.

## Verification

$\det(AB)=8-6=2$ and $\det(BA)=14-12=2=\det A\cdot\det B$, consistent with both products.
