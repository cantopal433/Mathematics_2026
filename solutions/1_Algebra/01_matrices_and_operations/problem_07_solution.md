## Question

For

$$
A=
\begin{pmatrix}
2 & 1 \\
0 & 2 \\
\end{pmatrix}
$$

compute

$$
AI,\qquad IA,\qquad A+0,\qquad A^2,\qquad A^3.
$$

Explain the roles of the matrices $I$ and $0$, and describe the pattern you observe in successive powers of $A$.

## Solution

$I$ is the neutral element of multiplication and $0$ is the neutral element of addition:

$$
AI=IA=A,\qquad A+0=A.
$$

$$
A^2=
\begin{pmatrix}
4 & 4 \\
0 & 4
\end{pmatrix},\qquad
A^3=
\begin{pmatrix}
8 & 12 \\
0 & 8
\end{pmatrix}.
$$

Pattern: the diagonal entries are $2^n$ and the upper right entry is $n\,2^{n-1}$:

$$
A^n=
\begin{pmatrix}
2^n & n\,2^{n-1} \\
0 & 2^n
\end{pmatrix}.
$$

## Verification

For $n=2$: $2\cdot2^1=4$; for $n=3$: $3\cdot2^2=12$, matching the computed powers.
