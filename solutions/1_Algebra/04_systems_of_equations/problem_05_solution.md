## Question

For the augmented matrix

$$
\begin{pmatrix}
1 & 2 & -1 & \mid & 3 \\
0 & 1 & 2 & \mid & 1 \\
0 & 0 & 0 & \mid & 0 \\
\end{pmatrix}
$$

determine the number of solutions and write them in parametric form. Explain how you know how many variables may be chosen freely.

## Solution

The matrix is already in row echelon form. With unknowns $x,y,z$ it represents the equations

$$
\begin{cases}
x+2y-z=3, \\
y+2z=1, \\
0=0.
\end{cases}
$$

The last row gives $0=0$, which is always true, so there is no contradiction and the system is consistent.

The pivots are in the columns of $x$ and $y$. The number of variables is $3$ and the number of pivots (the rank) is $2$, so

$$
3-2=1
$$

variable can be chosen freely. The free variable is the one whose column contains no pivot, which is $z$. Since a free variable can take any real value, the system has infinitely many solutions.

Let $z=t$ with $t\in\mathbb R$. Back substitution gives:

- second row: $y+2t=1$, so $y=1-2t$,
- first row: $x+2(1-2t)-t=3$, so $x=3-2+4t+t=1+5t$.

The solutions in parametric form are

$$
(x,y,z)=(1+5t,\ 1-2t,\ t),\qquad t\in\mathbb R.
$$

## Verification

For $t=1$ the point is $(6,-1,1)$:

$$
6+2\cdot(-1)-1=3,\qquad -1+2\cdot1=1.
$$

For $t=0$ the point is $(1,1,0)$:

$$
1+2\cdot1-0=3,\qquad 1+2\cdot0=1.
$$

Both points satisfy the nonzero equations, confirming the parametric solution.
