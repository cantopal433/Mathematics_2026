## Question

Solve

$$
\begin{cases}
x+2y-z=0, \\
2x+4y-2z=0, \\
x-y+2z=0.
\end{cases}
$$

Give all solutions in parametric form and explain why $(0,0,0)$ always satisfies a homogeneous system.

## Solution

A system is homogeneous when all right-hand sides are $0$, so the right-hand side column of the augmented matrix stays $0$ during elimination and can be omitted. The coefficient matrix is reduced:

$$
\begin{pmatrix}
1 & 2 & -1 \\
2 & 4 & -2 \\
1 & -1 & 2 \\
\end{pmatrix}
$$

Step 1: $R_2\leftarrow R_2-2R_1$ and $R_3\leftarrow R_3-R_1$:

$$
\begin{pmatrix}
1 & 2 & -1 \\
0 & 0 & 0 \\
0 & -3 & 3 \\
\end{pmatrix}
$$

The second equation was twice the first, so it became $0=0$ and gives no new information.

Step 2: $R_2\leftrightarrow R_3$ moves the zero row to the bottom:

$$
\begin{pmatrix}
1 & 2 & -1 \\
0 & -3 & 3 \\
0 & 0 & 0 \\
\end{pmatrix}
$$

There are two pivots and three unknowns, so $3-2=1$ variable is free. The column of $z$ has no pivot, so $z$ is chosen as the parameter: $z=t$, $t\in\mathbb R$.

- second row: $-3y+3t=0$, so $y=t$,
- first row: $x+2t-t=0$, so $x=-t$.

All solutions are

$$
(x,y,z)=(-t,\ t,\ t)=t\,(-1,\ 1,\ 1),\qquad t\in\mathbb R.
$$

Geometrically, the solution set is a line through the origin with direction vector $(-1,1,1)$.

**Why $(0,0,0)$ is always a solution.** In a homogeneous system every equation has the form $a_1x+a_2y+a_3z=0$. Substituting $x=y=z=0$ makes every left-hand side equal to $0$, which matches every right-hand side. In matrix form, $A\cdot0=0$ for any matrix $A$. Here $(0,0,0)$ corresponds to the parameter value $t=0$.

## Verification

For $t=1$ the point is $(-1,1,1)$:

$$
-1+2\cdot1-1=0,\qquad 2\cdot(-1)+4\cdot1-2\cdot1=0,\qquad -1-1+2\cdot1=0.
$$

All three equations hold, and by linearity every multiple $t(-1,1,1)$ is also a solution.
