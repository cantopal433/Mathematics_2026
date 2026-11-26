## Question

The matrix

$$
S=
\begin{pmatrix}
2 & 0 \\
0 & \frac12 \\
\end{pmatrix}
$$

describes a scaling of the plane. Find $S^{-1}$ and explain geometrically what the inverse transformation does. Check the action of the pair $S,S^{-1}$ on one simple vector.

## Solution

The matrix $S$ is diagonal. A diagonal matrix with nonzero diagonal entries is inverted by replacing each diagonal entry with its reciprocal, because the product of two diagonal matrices is computed entry by entry on the diagonal. Here $\det S=2\cdot\frac12=1\ne0$, and

$$
S^{-1}=
\begin{pmatrix}
\frac12 & 0 \\
0 & 2 \\
\end{pmatrix}.
$$

Geometric meaning: $S$ sends $(x,y)$ to $(2x,\ \frac12y)$, so it stretches the plane by the factor $2$ in the horizontal direction and compresses it by the factor $\frac12$ in the vertical direction. The inverse transformation does the opposite: $S^{-1}$ sends $(x,y)$ to $(\frac12x,\ 2y)$, so it compresses horizontally by $\frac12$ and stretches vertically by $2$. Applying one after the other returns every point to its original position.

## Verification

First, the product of the matrices:

$$
SS^{-1}=
\begin{pmatrix}
2\cdot\frac12 & 0 \\
0 & \frac12\cdot2 \\
\end{pmatrix}=
\begin{pmatrix}
1 & 0 \\
0 & 1 \\
\end{pmatrix}.
$$

Then the action on the vector $v=(1,1)^T$:

$$
Sv=
\begin{pmatrix}
2 \\
\frac12 \\
\end{pmatrix},\qquad
S^{-1}(Sv)=
\begin{pmatrix}
\frac12\cdot2 \\
2\cdot\frac12 \\
\end{pmatrix}=
\begin{pmatrix}
1 \\
1 \\
\end{pmatrix}=v.
$$

The pair $S,S^{-1}$ brings the vector back to where it started.
