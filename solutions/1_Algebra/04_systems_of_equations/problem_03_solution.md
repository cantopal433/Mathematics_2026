## Question

Solve or show that the system is inconsistent:

$$
\begin{cases}
x+2y=3, \\
2x+4y=7.
\end{cases}
$$

Show how the contradiction appears in the matrix after elimination and interpret it in terms of equations.

## Solution

The augmented matrix of the system is

$$
\begin{pmatrix}
1 & 2 & \mid & 3 \\
2 & 4 & \mid & 7 \\
\end{pmatrix}
$$

The operation $R_2\leftarrow R_2-2R_1$ eliminates $x$ from the second equation:

$$
\begin{pmatrix}
1 & 2 & \mid & 3 \\
0 & 0 & \mid & 1 \\
\end{pmatrix}
$$

The second row now represents the equation

$$
0\cdot x+0\cdot y=1,\qquad\mathrm{that\ is}\qquad 0=1,
$$

which is false for every choice of $x$ and $y$. A row of the form $(0\ \ 0\mid c)$ with $c\ne0$ is the sign of a contradiction, so the system is inconsistent and has no solution.

Interpretation in terms of equations: the left-hand side of the second equation is exactly twice the left-hand side of the first. If $x+2y=3$, then necessarily $2x+4y=6$, so the second equation $2x+4y=7$ cannot hold at the same time. Geometrically, the two equations describe parallel lines in the plane, $y=\frac{3-x}{2}$ and $y=\frac{7-2x}{4}$, which have the same slope $-\frac12$ but different intercepts, so they never meet.

## Verification

Suppose a solution existed. Multiplying the first equation by $2$ gives $2x+4y=6$, and subtracting this from the second equation gives $0=7-6=1$, a contradiction. This confirms that the system has no solution.
