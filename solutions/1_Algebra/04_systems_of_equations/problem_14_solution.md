## Question

Compare the systems

$$
\begin{cases}
x+y=2, \\
2x-y=1, \\
3x=3
\end{cases}
$$

and

$$
\begin{cases}
x+y=2, \\
2x-y=1, \\
3x=3.1.
\end{cases}
$$

Check the consistency of each system and explain why a small change in one number can change the type of the system.

## Solution

Both systems have three equations but only two unknowns, so they can be consistent only if all three lines pass through one common point.

The first two equations are the same in both systems. Adding them eliminates $y$:

$$
(x+y)+(2x-y)=2+1\quad\Longrightarrow\quad 3x=3\quad\Longrightarrow\quad x=1,
$$

and then $y=2-x=1$. So any solution of either system must be the point $(1,1)$.

**First system.** The third equation $3x=3$ also gives $x=1$, so the point $(1,1)$ satisfies all three equations. The system is consistent and has exactly one solution, $(x,y)=(1,1)$.

**Second system.** The third equation $3x=3.1$ gives $x=\frac{31}{30}$, but the first two equations force $x=1$. These cannot hold at the same time, so the second system is inconsistent and has no solution.

The same conclusion follows from elimination. The left-hand side of the third equation is the sum of the first two left-hand sides, $3x=(x+y)+(2x-y)$, so the operation $R_3\leftarrow R_3-R_1-R_2$ turns the third row into

$$
0=3-2-1=0\qquad\mathrm{and}\qquad 0=3.1-2-1=0.1
$$

in the first and second system, respectively. The first is always true, while the second is a contradiction.

**Why a small change matters.** In the first system the third equation is not independent: it is exactly the sum of the other two, so its right-hand side must be exactly $2+1=3$. Geometrically, the third line $x=1$ passes through the intersection point of the first two lines. Changing $3$ to $3.1$ moves this line to $x=\frac{31}{30}$, which misses the point $(1,1)$, so the three lines no longer have a common point. For an overdetermined system, consistency depends on an exact equality between numbers, and any change, however small, can destroy it.

## Verification

For the first system, $(1,1)$ gives

$$
1+1=2,\qquad 2-1=1,\qquad 3\cdot1=3.
$$

For the second system, the same point gives $3\cdot1=3\ne3.1$, and no other point satisfies the first two equations.
