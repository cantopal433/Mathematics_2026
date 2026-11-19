## Question

Analyze, depending on the parameter $a$, the system

$$
\begin{cases}
x+y=2, \\
ax+ay=4.
\end{cases}
$$

Among the three possibilities — exactly one solution, infinitely many solutions, no solution — determine which actually occur and for which values of $a$. If one type cannot occur, explain why.

## Solution

The left-hand side of the second equation is $ax+ay=a(x+y)$. The first equation says that $x+y=2$, so any solution must satisfy

$$
a(x+y)=2a.
$$

The second equation requires $a(x+y)=4$, so the system can be consistent only if $2a=4$.

The coefficient matrix and its determinant are

$$
A=
\begin{pmatrix}
1 & 1 \\
a & a \\
\end{pmatrix},\qquad \det A=1\cdot a-1\cdot a=0.
$$

The determinant is $0$ for every value of $a$.

Three cases are possible in principle, and they are checked one by one:

- **Exactly one solution: never.** A $2\times2$ system has a unique solution exactly when $\det A\ne0$. Here $\det A=0$ for every $a$, because the second row of $A$ is always $a$ times the first row. So this case does not occur for any value of $a$.
- **Infinitely many solutions: only for $a=2$.** Then the second equation $2x+2y=4$ is twice the first one and adds no new condition. The system reduces to $x+y=2$, with solutions $(x,y)=(2-s,\ s)$, $s\in\mathbb R$.
- **No solution: for every $a\ne2$.** If $a=0$, the second equation reads $0=4$, which is false. If $a\ne0$ and $a\ne2$, dividing the second equation by $a$ gives $x+y=\frac4a\ne2$, which contradicts the first equation. Geometrically, the two equations describe parallel lines that do not meet.

In summary, infinitely many solutions occur for $a=2$, no solution occurs for $a\ne2$, and exactly one solution never occurs.

## Verification

For $a=2$ the points $(2,0)$ and $(0,2)$ both satisfy $x+y=2$ and $2x+2y=4$, so there is more than one solution. For $a=1$ the system becomes $x+y=2$ and $x+y=4$, which cannot both hold. For $a=0$ the second equation is $0=4$, which is impossible.
