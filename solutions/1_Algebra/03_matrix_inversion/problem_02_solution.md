## Question

Find the inverse of

$$
A=
\begin{pmatrix}
3 & 2 \\
5 & 4 \\
\end{pmatrix}
$$

using the formula for a $2\times2$ matrix. At the end, check the result by computing one product with $A$.

## Solution

For a $2\times2$ matrix

$$
A=
\begin{pmatrix}
a & b \\
c & d \\
\end{pmatrix}
$$

with $\det A=ad-bc\ne0$, the inverse is obtained by swapping the diagonal entries, changing the sign of the off-diagonal entries, and dividing by the determinant:

$$
A^{-1}=\frac{1}{ad-bc}
\begin{pmatrix}
d & -b \\
-c & a \\
\end{pmatrix}.
$$

Here $a=3$, $b=2$, $c=5$, $d=4$, so

$$
\det A=3\cdot4-2\cdot5=12-10=2\ne0,
$$

and the inverse exists:

$$
A^{-1}=\frac12
\begin{pmatrix}
4 & -2 \\
-5 & 3 \\
\end{pmatrix}=
\begin{pmatrix}
2 & -1 \\
-\frac52 & \frac32 \\
\end{pmatrix}.
$$

## Verification

The result is checked by multiplying it by $A$:

$$
AA^{-1}=
\begin{pmatrix}
3 & 2 \\
5 & 4 \\
\end{pmatrix}
\begin{pmatrix}
2 & -1 \\
-\frac52 & \frac32 \\
\end{pmatrix}=
\begin{pmatrix}
6-5 & -3+3 \\
10-10 & -5+6 \\
\end{pmatrix}=
\begin{pmatrix}
1 & 0 \\
0 & 1 \\
\end{pmatrix}.
$$

The product is the identity matrix, so the computed inverse is correct.
