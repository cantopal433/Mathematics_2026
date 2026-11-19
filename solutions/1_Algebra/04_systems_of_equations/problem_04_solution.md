## Question

Solve

$$
\begin{cases}
x+y+z=2, \\
2x+2y+2z=4, \\
x-y+z=0.
\end{cases}
$$

Give the solution in parametric form, identify a free variable, and for one chosen parameter value check that the resulting point really satisfies the system.

## Solution

The augmented matrix is

$$
\begin{pmatrix}
1 & 1 & 1 & \mid & 2 \\
2 & 2 & 2 & \mid & 4 \\
1 & -1 & 1 & \mid & 0 \\
\end{pmatrix}
$$

Step 1: $R_2\leftarrow R_2-2R_1$ and $R_3\leftarrow R_3-R_1$:

$$
\begin{pmatrix}
1 & 1 & 1 & \mid & 2 \\
0 & 0 & 0 & \mid & 0 \\
0 & -2 & 0 & \mid & -2 \\
\end{pmatrix}
$$

The second row became $0=0$: the second equation is just twice the first, so it gives no new information.

Step 2: $R_2\leftrightarrow R_3$ moves the zero row to the bottom:

$$
\begin{pmatrix}
1 & 1 & 1 & \mid & 2 \\
0 & -2 & 0 & \mid & -2 \\
0 & 0 & 0 & \mid & 0 \\
\end{pmatrix}
$$

There are only two pivots, in the columns of $x$ and $y$, and there is no contradictory row. The column of $z$ has no pivot, so $z$ is a free variable and the system has infinitely many solutions.

From the second row, $-2y=-2$, so $y=1$. Setting $z=t$ with $t\in\mathbb R$, the first row gives $x+1+t=2$, so $x=1-t$. The solution in parametric form is

$$
(x,y,z)=(1-t,\ 1,\ t),\qquad t\in\mathbb R.
$$

## Verification

For the parameter value $t=2$ the point is $(x,y,z)=(-1,1,2)$. Substituting into the original system:

$$
\begin{aligned}
-1+1+2 &= 2, \\
2\cdot(-1)+2\cdot1+2\cdot2 &= 4, \\
-1-1+2 &= 0.
\end{aligned}
$$

All three equations hold, so the point really satisfies the system.
