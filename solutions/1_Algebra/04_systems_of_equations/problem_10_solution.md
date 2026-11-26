## Question

Find a polynomial $p(x)=ax^2+bx+c$ whose graph passes through $(0,1)$, $(1,3)$, and $(2,9)$. Reduce the problem to a system of equations and check the result by substituting all three points.

## Solution

The graph of $p$ passes through a point $(x_0,y_0)$ exactly when $p(x_0)=y_0$. Each of the three points gives one linear equation in the unknown coefficients $a,b,c$:

$$
\begin{cases}
p(0)=c=1, \\
p(1)=a+b+c=3, \\
p(2)=4a+2b+c=9.
\end{cases}
$$

In matrix form, with unknowns ordered as $a,b,c$:

$$
\begin{pmatrix}
0 & 0 & 1 & \mid & 1 \\
1 & 1 & 1 & \mid & 3 \\
4 & 2 & 1 & \mid & 9 \\
\end{pmatrix}
$$

The first equation gives $c=1$ immediately. Substituting it into the other two:

$$
\begin{cases}
a+b=2, \\
4a+2b=8.
\end{cases}
$$

Subtracting twice the first of these equations from the second eliminates $b$:

$$
(4a+2b)-2(a+b)=8-4\quad\Longrightarrow\quad 2a=4\quad\Longrightarrow\quad a=2.
$$

Then $b=2-a=0$. The polynomial is

$$
p(x)=2x^2+1.
$$

## Verification

Substituting all three points:

$$
p(0)=2\cdot0+1=1,\qquad p(1)=2\cdot1+1=3,\qquad p(2)=2\cdot4+1=9.
$$

The graph passes through $(0,1)$, $(1,3)$, and $(2,9)$.
