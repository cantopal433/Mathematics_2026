## Question

Find numbers $x,y$ satisfying

$$
x+y=10,\qquad 2x+5y=32.
$$

Solve the system and explain geometrically why the solution is unique.

## Solution

The system is

$$
\begin{cases}
x+y=10, \\
2x+5y=32.
\end{cases}
$$

Subtracting twice the first equation from the second eliminates $x$:

$$
(2x+5y)-2(x+y)=32-20\quad\Longrightarrow\quad 3y=12\quad\Longrightarrow\quad y=4.
$$

Substituting into the first equation gives $x=10-4=6$. The solution is

$$
(x,y)=(6,\ 4).
$$

**Why the solution is unique.** Each equation describes a line in the plane:

$$
y=10-x\qquad\mathrm{and}\qquad y=\frac{32-2x}{5}.
$$

The first line has slope $-1$ and the second has slope $-\frac25$. Lines with different slopes are not parallel, so they intersect in exactly one point, and that point is the unique solution. Algebraically, the coefficient matrix has determinant

$$
\det
\begin{pmatrix}
1 & 1 \\
2 & 5 \\
\end{pmatrix}=5-2=3\ne0,
$$

which also guarantees exactly one solution.

## Verification

$$
6+4=10,\qquad 2\cdot6+5\cdot4=12+20=32.
$$

Both equations hold.
