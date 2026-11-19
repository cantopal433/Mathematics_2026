## Question

Let $A$ and $B$ be invertible $2\times2$ matrices with

$$
\det A=-2,\qquad \det B=3.
$$

Without finding the entries of the matrices, compute

$$
\det\left(B^{-1}A^TB\right).
$$

State the determinant properties you use in order and explain why the factors involving $B$ eventually cancel.

## Solution

The following determinant properties are used, in this order:

1. product rule: $\det(XYZ)=\det X\cdot\det Y\cdot\det Z$ for square matrices of the same size,
2. transpose: $\det(A^T)=\det A$,
3. inverse: $\det(B^{-1})=\dfrac{1}{\det B}$, which follows from $\det(B^{-1})\det B=\det(B^{-1}B)=\det I=1$.

The matrix $B$ is invertible because $\det B=3\ne0$, so $B^{-1}$ exists and all three matrices in the product are $2\times2$.

Applying the product rule:

$$
\det\left(B^{-1}A^TB\right)=\det(B^{-1})\cdot\det(A^T)\cdot\det B.
$$

Replacing $\det(A^T)$ by $\det A$ and $\det(B^{-1})$ by $\dfrac{1}{\det B}$:

$$
\det\left(B^{-1}A^TB\right)=\frac{1}{\det B}\cdot\det A\cdot\det B=\frac13\cdot(-2)\cdot3=-2.
$$

The factors involving $B$ cancel because determinants are ordinary numbers. The matrices $B^{-1}$, $A^T$ and $B$ do not commute in general, but their determinants do, so $\dfrac{1}{\det B}$ and $\det B$ can be brought together, and their product is $1$. Hence the result equals $\det A$ and does not depend on $B$ at all.

## Verification

A concrete example with the given determinants is $A=\mathrm{diag}(-2,1)$ and $B=\mathrm{diag}(3,1)$. Then $B^{-1}=\mathrm{diag}(\frac13,1)$ and $A^T=A$, and products of diagonal matrices are computed entry by entry:

$$
B^{-1}A^TB=\mathrm{diag}\left(\tfrac13\cdot(-2)\cdot3,\ 1\cdot1\cdot1\right)=\mathrm{diag}(-2,1),
$$

whose determinant is $(-2)\cdot1=-2$, in agreement with the result above.
