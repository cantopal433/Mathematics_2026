## Question

For

$$
A=
\begin{pmatrix}
1 & 2 & -1 \\
0 & 3 & 4 \\
2 & 1 & 5 \\
\end{pmatrix}
$$

compute $\det A$ using Sarrus' rule. Then perform one simple check using a chosen property of the determinant.

## Solution

Sarrus' rule for a $3\times3$ matrix adds the three products along the diagonals running from top left to bottom right, and subtracts the three products along the diagonals running from top right to bottom left.

Products along the main diagonals:

$$
\begin{aligned}
a_{11}a_{22}a_{33} &= 1\cdot3\cdot5=15, \\
a_{12}a_{23}a_{31} &= 2\cdot4\cdot2=16, \\
a_{13}a_{21}a_{32} &= (-1)\cdot0\cdot1=0.
\end{aligned}
$$

Their sum is $15+16+0=31$.

Products along the opposite diagonals:

$$
\begin{aligned}
a_{13}a_{22}a_{31} &= (-1)\cdot3\cdot2=-6, \\
a_{11}a_{23}a_{32} &= 1\cdot4\cdot1=4, \\
a_{12}a_{21}a_{33} &= 2\cdot0\cdot5=0.
\end{aligned}
$$

Their sum is $-6+4+0=-2$.

Therefore

$$
\det A=31-(-2)=33.
$$

## Verification

As an independent check, the determinant is computed again by cofactor (Laplace) expansion along the first column. This method uses $2\times2$ minors instead of diagonal products, so it does not repeat the Sarrus calculation. Since $a_{21}=0$, only two terms remain:

$$
\det A=1\cdot
\det
\begin{pmatrix}
3 & 4 \\
1 & 5
\end{pmatrix}
+2\cdot
\det
\begin{pmatrix}
2 & -1 \\
3 & 4
\end{pmatrix}
=1\cdot(15-4)+2\cdot(8+3)=11+22=33.
$$

Both methods give $\det A=33$.
