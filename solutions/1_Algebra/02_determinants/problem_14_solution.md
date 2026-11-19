## Question

Consider the system $Ax=b$, where

$$
A=
\begin{pmatrix}
1 & 2 \\
k & 4 \\
\end{pmatrix}.
$$

For which values of $k$ does the system have exactly one solution for every $b$? For the remaining value, give an example of a right-hand side $b$ for which the system has infinitely many solutions, and an example for which it has no solution.

## Solution

The determinant of the coefficient matrix is

$$
\det A=1\cdot4-2\cdot k=4-2k.
$$

A square system $Ax=b$ has exactly one solution for every right-hand side $b$ if and only if $A$ is invertible, that is, $\det A\ne0$. In that case the solution is $x=A^{-1}b$. Since

$$
4-2k\ne0\quad\Longleftrightarrow\quad k\ne2,
$$

the system has exactly one solution for every $b$ when $k\ne2$.

For the remaining value $k=2$, with $b=(b_1,b_2)^T$, the system is

$$
\begin{cases}
x+2y=b_1, \\
2x+4y=b_2.
\end{cases}
$$

The left-hand side of the second equation is exactly twice the left-hand side of the first. Multiplying the first equation by $2$ gives $2x+4y=2b_1$, so the system can have a solution only if $b_2=2b_1$.

Infinitely many solutions: take $b=(1,2)^T$. Then $b_2=2b_1$, the second equation is just twice the first, and only the condition $x+2y=1$ remains. Choosing $y=s$ freely gives

$$
x=1-2s,\qquad y=s,\qquad s\in\mathbb R.
$$

No solution: take $b=(1,0)^T$. The first equation gives $2x+4y=2$, while the second requires $2x+4y=0$. Both cannot hold, so the system is inconsistent.

## Verification

For $k=2$ and $b=(1,2)^T$, the choices $s=0$ and $s=1$ give $(x,y)=(1,0)$ and $(x,y)=(-1,1)$:

$$
1+2\cdot0=1,\quad 2\cdot1+4\cdot0=2;\qquad -1+2\cdot1=1,\quad 2\cdot(-1)+4\cdot1=2.
$$

Both pairs satisfy the system, so it indeed has more than one solution. For any $k\ne2$, for example $k=0$, $\det A=4\ne0$ and the solution is unique.
