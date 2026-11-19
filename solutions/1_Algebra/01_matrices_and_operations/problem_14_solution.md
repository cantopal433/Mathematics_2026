## Question

The matrix for a rotation through an angle $\theta$ is

$$
R(\theta)=
\begin{pmatrix}
\cos\theta & -\sin\theta \\
\sin\theta & \cos\theta \\
\end{pmatrix}.
$$

Compute $R(\alpha)R(\beta)$ and, using the angle-sum formulas for sine and cosine, show that

$$
R(\alpha)R(\beta)=R(\alpha+\beta).
$$

Explain the result geometrically.

## Solution

The product is computed row by column:

$$
R(\alpha)R(\beta)=
\begin{pmatrix}
\cos\alpha & -\sin\alpha \\
\sin\alpha & \cos\alpha \\
\end{pmatrix}
\begin{pmatrix}
\cos\beta & -\sin\beta \\
\sin\beta & \cos\beta \\
\end{pmatrix}
$$

$$
=
\begin{pmatrix}
\cos\alpha\cos\beta-\sin\alpha\sin\beta & -\cos\alpha\sin\beta-\sin\alpha\cos\beta \\
\sin\alpha\cos\beta+\cos\alpha\sin\beta & -\sin\alpha\sin\beta+\cos\alpha\cos\beta \\
\end{pmatrix}.
$$

The angle-sum formulas are

$$
\cos(\alpha+\beta)=\cos\alpha\cos\beta-\sin\alpha\sin\beta,\qquad
\sin(\alpha+\beta)=\sin\alpha\cos\beta+\cos\alpha\sin\beta.
$$

The top left and bottom right entries are both $\cos(\alpha+\beta)$, the bottom left entry is $\sin(\alpha+\beta)$, and the top right entry is $-\sin(\alpha+\beta)$. Hence

$$
R(\alpha)R(\beta)=
\begin{pmatrix}
\cos(\alpha+\beta) & -\sin(\alpha+\beta) \\
\sin(\alpha+\beta) & \cos(\alpha+\beta) \\
\end{pmatrix}=R(\alpha+\beta).
$$

Geometrically, $R(\alpha)R(\beta)x$ first rotates the vector $x$ by the angle $\beta$ and then rotates the result by $\alpha$. Two rotations about the origin combine into one rotation by the sum of the angles. Since $\alpha+\beta=\beta+\alpha$, it also follows that $R(\alpha)R(\beta)=R(\beta)R(\alpha)$, so rotations of the plane about the origin commute with each other.

## Verification

For $\alpha=\beta=90^\circ$, using $\cos90^\circ=0$ and $\sin90^\circ=1$:

$$
R(90^\circ)R(90^\circ)=
\begin{pmatrix}
0 & -1 \\
1 & 0 \\
\end{pmatrix}
\begin{pmatrix}
0 & -1 \\
1 & 0 \\
\end{pmatrix}=
\begin{pmatrix}
-1 & 0 \\
0 & -1 \\
\end{pmatrix}=R(180^\circ),
$$

since $\cos180^\circ=-1$ and $\sin180^\circ=0$. Two quarter turns give a half turn, as expected.
