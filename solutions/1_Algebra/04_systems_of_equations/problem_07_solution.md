## Question

Do not solve all of the following systems completely. For each situation, choose the method that best uses its structure and justify your choice:

1. one system with a triangular coefficient matrix

$$
\begin{cases}
2x-y=3, \\
4y=8;
\end{cases}
$$

2. three systems $Ax=b_i$ with the same invertible matrix $A$, when $A^{-1}$ is already known;
3. one $3\times3$ system for which the inverse matrix is not given and the goal is only to find one solution vector.

For case 1, carry out the chosen method completely. For cases 2 and 3, describe the plan and indicate which part of the computation would be reusable or unnecessary. Do not judge a method by its name alone — refer to the number of right-hand sides and the structure of the matrix.

## Solution

**Case 1: triangular coefficient matrix.** The coefficient matrix

$$
\begin{pmatrix}
2 & -1 \\
0 & 4 \\
\end{pmatrix}
$$

is already upper triangular, so no elimination is needed. The best method is back substitution: solve the last equation first and substitute upward.

From the second equation:

$$
4y=8\quad\Longrightarrow\quad y=2.
$$

Substituting into the first equation:

$$
2x-2=3\quad\Longrightarrow\quad 2x=5\quad\Longrightarrow\quad x=\frac52.
$$

The solution is $(x,y)=\left(\frac52,\ 2\right)$. Computing an inverse or running full elimination here would be unnecessary work, because the triangular structure already gives the answer in two short steps.

**Case 2: three systems $Ax=b_i$ with the same matrix and $A^{-1}$ known.** The best plan is to use the given inverse:

$$
x_i=A^{-1}b_i,\qquad i=1,2,3.
$$

Each solution needs only one matrix-vector product, with no row operations at all. The reusable part is $A^{-1}$, which is the same for all three right-hand sides; the expensive work of inverting $A$ has already been done. Without a known inverse, a good alternative would be to reduce the augmented matrix $[A\mid b_1\ b_2\ b_3]$ once, so that the elimination on $A$ is shared by all three right-hand sides.

**Case 3: one $3\times3$ system, inverse not given, only one solution needed.** The best method is Gaussian elimination on $[A\mid b]$ followed by back substitution. Computing $A^{-1}$ first would be unnecessary: finding the inverse by Gauss–Jordan means reducing $[A\mid I]$, which is like solving the system for three right-hand sides at once, and afterwards a matrix-vector product would still be required. With only one right-hand side, nothing from the inverse would be reused, so direct elimination is cheaper.

In all three cases the choice depends on the structure of the matrix and on the number of right-hand sides, not on the name of the method.

## Verification

Substituting the solution of case 1 into the system:

$$
2\cdot\frac52-2=5-2=3,\qquad 4\cdot2=8.
$$

Both equations hold.
