## Question

Consider the system

$$
x_1+x_2=10,\qquad x_2+x_3=8,\qquad x_1-x_3=2.
$$

Solve it and check whether all three equations are independently necessary to describe the solution set. If one follows from the others, show this by calculation.

## Solution

The augmented matrix, with unknowns $x_1,x_2,x_3$, is

$$
\begin{pmatrix}
1 & 1 & 0 & \mid & 10 \\
0 & 1 & 1 & \mid & 8 \\
1 & 0 & -1 & \mid & 2 \\
\end{pmatrix}
$$

Step 1: $R_3\leftarrow R_3-R_1$:

$$
\begin{pmatrix}
1 & 1 & 0 & \mid & 10 \\
0 & 1 & 1 & \mid & 8 \\
0 & -1 & -1 & \mid & -8 \\
\end{pmatrix}
$$

Step 2: $R_3\leftarrow R_3+R_2$:

$$
\begin{pmatrix}
1 & 1 & 0 & \mid & 10 \\
0 & 1 & 1 & \mid & 8 \\
0 & 0 & 0 & \mid & 0 \\
\end{pmatrix}
$$

The last row became $0=0$, so the system is consistent but has only two pivots for three unknowns. The variable $x_3$ is free. Let $x_3=t$, $t\in\mathbb R$:

- second row: $x_2=8-t$,
- first row: $x_1=10-x_2=2+t$.

The solution set is

$$
(x_1,x_2,x_3)=(2+t,\ 8-t,\ t),\qquad t\in\mathbb R,
$$

so the system has infinitely many solutions.

**Are all three equations necessary?** No. Subtracting the second equation from the first gives

$$
(x_1+x_2)-(x_2+x_3)=10-8\quad\Longrightarrow\quad x_1-x_3=2,
$$

which is exactly the third equation. So the third equation follows from the first two and adds no new information; this is why it turned into the zero row during elimination. The first two equations alone already describe the same solution set.

## Verification

For $t=0$ the point is $(2,8,0)$, and for $t=3$ it is $(5,5,3)$:

$$
2+8=10,\quad 8+0=8,\quad 2-0=2;\qquad 5+5=10,\quad 5+3=8,\quad 5-3=2.
$$

Both points satisfy all three equations.
