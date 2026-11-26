## Question

The matrices

$$
S=
\begin{pmatrix}
2 & 0 \\
0 & 1 \\
\end{pmatrix},\qquad H=
\begin{pmatrix}
1 & 1 \\
0 & 1 \\
\end{pmatrix}
$$

describe nonuniform scaling and shear. For $T=HS$, find $T^{-1}$ in two ways:

1. first compute $T$, then its inverse,
2. use $(HS)^{-1}=S^{-1}H^{-1}$.

Compare the results. Additionally compute $H^{-1}S^{-1}$ and verify that the incorrect order gives a different matrix. Explain the rule: “when undoing a composition of operations, we undo them from the end.”

## Solution

The separate inverses are needed in both methods. $S$ is diagonal, so its inverse has the reciprocal diagonal entries. $H$ has determinant $1$, and undoing a shear means shearing back:

$$
S^{-1}=
\begin{pmatrix}
\frac12 & 0 \\
0 & 1 \\
\end{pmatrix},\qquad
H^{-1}=
\begin{pmatrix}
1 & -1 \\
0 & 1 \\
\end{pmatrix}.
$$

**Method 1: compute $T$ first.**

$$
T=HS=
\begin{pmatrix}
1 & 1 \\
0 & 1 \\
\end{pmatrix}
\begin{pmatrix}
2 & 0 \\
0 & 1 \\
\end{pmatrix}=
\begin{pmatrix}
2 & 1 \\
0 & 1 \\
\end{pmatrix}.
$$

Then $\det T=2$, and the $2\times2$ formula gives

$$
T^{-1}=\frac12
\begin{pmatrix}
1 & -1 \\
0 & 2 \\
\end{pmatrix}=
\begin{pmatrix}
\frac12 & -\frac12 \\
0 & 1 \\
\end{pmatrix}.
$$

**Method 2: use $(HS)^{-1}=S^{-1}H^{-1}$.**

$$
S^{-1}H^{-1}=
\begin{pmatrix}
\frac12 & 0 \\
0 & 1 \\
\end{pmatrix}
\begin{pmatrix}
1 & -1 \\
0 & 1 \\
\end{pmatrix}=
\begin{pmatrix}
\frac12 & -\frac12 \\
0 & 1 \\
\end{pmatrix}.
$$

Both methods give the same matrix.

**The incorrect order.**

$$
H^{-1}S^{-1}=
\begin{pmatrix}
1 & -1 \\
0 & 1 \\
\end{pmatrix}
\begin{pmatrix}
\frac12 & 0 \\
0 & 1 \\
\end{pmatrix}=
\begin{pmatrix}
\frac12 & -1 \\
0 & 1 \\
\end{pmatrix},
$$

which differs from $T^{-1}$ in the top right entry.

**The rule.** The vector $Tx=H(Sx)$ is produced by first scaling with $S$ and then shearing with $H$. To get back to $x$, the operation performed last must be undone first: remove the shear with $H^{-1}$, then remove the scaling with $S^{-1}$. Written as a product acting on a vector, this is $S^{-1}H^{-1}$, because the matrix closest to the vector acts first. This is the meaning of "when undoing a composition of operations, we undo them from the end".

## Verification

$$
TT^{-1}=
\begin{pmatrix}
2 & 1 \\
0 & 1 \\
\end{pmatrix}
\begin{pmatrix}
\frac12 & -\frac12 \\
0 & 1 \\
\end{pmatrix}=
\begin{pmatrix}
1 & -1+1 \\
0 & 1 \\
\end{pmatrix}=I,
$$

while for the incorrect order

$$
T\,H^{-1}S^{-1}=
\begin{pmatrix}
2 & 1 \\
0 & 1 \\
\end{pmatrix}
\begin{pmatrix}
\frac12 & -1 \\
0 & 1 \\
\end{pmatrix}=
\begin{pmatrix}
1 & -1 \\
0 & 1 \\
\end{pmatrix}\ne I.
$$

So only $S^{-1}H^{-1}$ is the inverse of $T$.
