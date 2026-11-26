## Question

Analyze the number of solutions depending on $t$:

$$
\begin{cases}
x+y+z=1, \\
x+ty+z=2, \\
x+y+tz=3.
\end{cases}
$$

Use elimination and separately analyze the parameter values for which a standard calculation step ceases to be valid.

## Solution

The augmented matrix is

$$
\begin{pmatrix}
1 & 1 & 1 & \mid & 1 \\
1 & t & 1 & \mid & 2 \\
1 & 1 & t & \mid & 3 \\
\end{pmatrix}
$$

The operations $R_2\leftarrow R_2-R_1$ and $R_3\leftarrow R_3-R_1$ are valid for every $t$:

$$
\begin{pmatrix}
1 & 1 & 1 & \mid & 1 \\
0 & t-1 & 0 & \mid & 1 \\
0 & 0 & t-1 & \mid & 2 \\
\end{pmatrix}
$$

The second and third rows now read

$$
(t-1)y=1,\qquad (t-1)z=2.
$$

The next step is to divide by $t-1$. This step is valid only when $t-1\ne0$, so the case $t=1$ must be analyzed separately.

**Case $t\ne1$.** Dividing is allowed:

$$
y=\frac{1}{t-1},\qquad z=\frac{2}{t-1},
$$

and from the first equation

$$
x=1-y-z=1-\frac{3}{t-1}=\frac{t-4}{t-1}.
$$

The matrix has three pivots, so the system has exactly one solution for every $t\ne1$.

**Case $t=1$.** The second and third rows become

$$
0\cdot y=1,\qquad 0\cdot z=2,
$$

that is, $0=1$ and $0=2$. These are contradictions, so for $t=1$ the system has no solution. This is also visible in the original system: for $t=1$ all three left-hand sides equal $x+y+z$, but the right-hand sides $1$, $2$, $3$ are different.

The case of infinitely many solutions does not occur for any $t$. The coefficient determinant equals $(t-1)^2$, which is zero only for $t=1$, and in that case the system is inconsistent.

## Verification

For $t=2$ the formulas give $(x,y,z)=(-2,\ 1,\ 2)$:

$$
-2+1+2=1,\qquad -2+2\cdot1+2=2,\qquad -2+1+2\cdot2=3.
$$

For $t=4$ they give $(x,y,z)=\left(0,\ \frac13,\ \frac23\right)$:

$$
0+\frac13+\frac23=1,\qquad 0+\frac43+\frac23=2,\qquad 0+\frac13+\frac83=3.
$$

All equations hold in both cases.
