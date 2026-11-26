## Question

For each of the following systems, perform only as much elimination as necessary to recognize its type:

**System 1**

$$
\begin{cases}
x+y=2, \\
x-y=0,
\end{cases}
$$

**System 2**

$$
\begin{cases}
x+y=2, \\
2x+2y=4,
\end{cases}
$$

**System 3**

$$
\begin{cases}
x+y=2, \\
2x+2y=5.
\end{cases}
$$

For each, justify the classification: one solution, infinitely many solutions, or no solution.

## Solution

In each system one elimination step, which removes $x$ from the second equation, is enough to recognize the type.

**System 1.** The operation $R_2\leftarrow R_2-R_1$ gives

$$
\begin{pmatrix}
1 & 1 & \mid & 2 \\
0 & -2 & \mid & -2 \\
\end{pmatrix}
$$

There are two pivots for two unknowns and no contradiction, so the system has **exactly one solution**. Back substitution gives $y=1$ and $x=1$.

**System 2.** The operation $R_2\leftarrow R_2-2R_1$ gives

$$
\begin{pmatrix}
1 & 1 & \mid & 2 \\
0 & 0 & \mid & 0 \\
\end{pmatrix}
$$

The second row is $0=0$, which is always true: the second equation is twice the first. There is only one pivot, so $y$ is free, and the system has **infinitely many solutions**, $(x,y)=(2-s,\ s)$ with $s\in\mathbb R$.

**System 3.** The operation $R_2\leftarrow R_2-2R_1$ gives

$$
\begin{pmatrix}
1 & 1 & \mid & 2 \\
0 & 0 & \mid & 1 \\
\end{pmatrix}
$$

The second row is $0=1$, which is impossible. The left-hand side of the second equation is twice the first, but the right-hand side is $5\ne2\cdot2$. The system has **no solution**.

Geometrically, System 1 consists of two lines with different slopes that meet in one point, System 2 consists of one line written twice, and System 3 consists of two different parallel lines.

## Verification

System 1: $(1,1)$ gives $1+1=2$ and $1-1=0$. System 2: the points $(2,0)$ and $(0,2)$ both satisfy $x+y=2$ and $2x+2y=4$. System 3: any solution of $x+y=2$ satisfies $2x+2y=4$, never $5$.
