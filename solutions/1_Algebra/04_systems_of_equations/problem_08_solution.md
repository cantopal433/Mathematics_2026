## Question

Solve by elimination the two systems

$$
\begin{cases}
2x+y=5, \\
x-y=1,
\end{cases}
$$

$$
\begin{cases}
2x+y=1, \\
x-y=4.
\end{cases}
$$

Compare the successive elimination steps. Which part of the calculation is the same in both cases, and why?

## Solution

Both systems have the same coefficient matrix

$$
A=
\begin{pmatrix}
2 & 1 \\
1 & -1 \\
\end{pmatrix},
$$

and differ only in the right-hand sides $b_1=(5,1)^T$ and $b_2=(1,4)^T$. They can be solved together with one augmented matrix that contains both right-hand sides:

$$
\begin{pmatrix}
2 & 1 & \mid & 5 & 1 \\
1 & -1 & \mid & 1 & 4 \\
\end{pmatrix}
$$

Step 1: $R_1\leftrightarrow R_2$ puts the coefficient $1$ in the pivot position:

$$
\begin{pmatrix}
1 & -1 & \mid & 1 & 4 \\
2 & 1 & \mid & 5 & 1 \\
\end{pmatrix}
$$

Step 2: $R_2\leftarrow R_2-2R_1$ eliminates $x$ from the second equation:

$$
\begin{pmatrix}
1 & -1 & \mid & 1 & 4 \\
0 & 3 & \mid & 3 & -7 \\
\end{pmatrix}
$$

Back substitution, column by column:

- first system: $3y=3$, so $y=1$, and $x-y=1$ gives $x=2$,
- second system: $3y=-7$, so $y=-\frac73$, and $x-y=4$ gives $x=4-\frac73=\frac53$.

The solutions are

$$
(x,y)=(2,\ 1)\qquad\mathrm{and}\qquad (x,y)=\left(\frac53,\ -\frac73\right).
$$

**Comparison.** The row operations (the interchange and $R_2-2R_1$) are exactly the same in both systems, and the left part of the matrix goes through the same stages. This happens because the choice of every row operation depends only on the coefficients of the unknowns, that is, only on $A$. The right-hand sides are simply carried along and do not influence which operations are performed. Only the last column and the final back substitution differ.

## Verification

First system with $(2,1)$:

$$
2\cdot2+1=5,\qquad 2-1=1.
$$

Second system with $\left(\frac53,-\frac73\right)$:

$$
2\cdot\frac53-\frac73=\frac{10-7}{3}=1,\qquad \frac53+\frac73=\frac{12}{3}=4.
$$

All four equations hold.
