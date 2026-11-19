## Question

Solve using Gaussian elimination:

$$
\begin{cases}
x+y+z=6, \\
2x-y+z=3, \\
x+2y-z=2.
\end{cases}
$$

After solving, substitute the result into all equations and check consistency.

## Solution

Gaussian elimination works on the augmented matrix $[A\mid b]$. Row operations do not change the set of solutions, because each of them can be reversed.

$$
\begin{pmatrix}
1 & 1 & 1 & \mid & 6 \\
2 & -1 & 1 & \mid & 3 \\
1 & 2 & -1 & \mid & 2 \\
\end{pmatrix}
$$

Step 1: $R_2\leftarrow R_2-2R_1$ and $R_3\leftarrow R_3-R_1$ eliminate $x$ from the second and third equations:

$$
\begin{pmatrix}
1 & 1 & 1 & \mid & 6 \\
0 & -3 & -1 & \mid & -9 \\
0 & 1 & -2 & \mid & -4 \\
\end{pmatrix}
$$

Step 2: $R_2\leftrightarrow R_3$ brings the row with coefficient $1$ in front of $y$ to the pivot position, which avoids fractions:

$$
\begin{pmatrix}
1 & 1 & 1 & \mid & 6 \\
0 & 1 & -2 & \mid & -4 \\
0 & -3 & -1 & \mid & -9 \\
\end{pmatrix}
$$

Step 3: $R_3\leftarrow R_3+3R_2$ eliminates $y$ from the third equation:

$$
\begin{pmatrix}
1 & 1 & 1 & \mid & 6 \\
0 & 1 & -2 & \mid & -4 \\
0 & 0 & -7 & \mid & -21 \\
\end{pmatrix}
$$

The matrix is in row echelon form with three pivots, so the system has exactly one solution. Back substitution from the last equation upward:

- third row: $-7z=-21$, so $z=3$,
- second row: $y-2z=-4$, so $y=-4+6=2$,
- first row: $x+y+z=6$, so $x=6-2-3=1$.

The solution is

$$
(x,y,z)=(1,2,3).
$$

## Verification

Substituting into all three original equations:

$$
\begin{aligned}
1+2+3 &= 6, \\
2\cdot1-2+3 &= 3, \\
1+2\cdot2-3 &= 2.
\end{aligned}
$$

All three equations hold, so the system is consistent and $(1,2,3)$ is its solution.
