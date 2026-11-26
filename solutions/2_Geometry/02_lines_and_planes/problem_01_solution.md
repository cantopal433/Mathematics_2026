## Question

Find the equation of the line through $A=(1,2)$ and $B=(4,-1)$ in parametric and general form. Identify a direction vector and an example of a normal vector. Check that both points satisfy the equation you obtain.

## Solution

**Direction vector.** A line through two points has the direction of the vector from one point to the other:

$$
\overrightarrow{AB}=B-A=(4-1,\ -1-2)=(3,-3).
$$

Any nonzero multiple of it is also a direction vector, for example $v=(1,-1)$.

**Parametric form.** A line is described by "a point plus multiples of a direction vector". Starting from $A$:

$$
(x,y)=(1,2)+t\,(3,-3),\qquad t\in\mathbb R,
$$

that is, $x=1+3t$ and $y=2-3t$. The value $t=0$ gives $A$, and $t=1$ gives $A+\overrightarrow{AB}=B$.

**Normal vector.** A normal vector is perpendicular to the direction vector, so its dot product with $(3,-3)$ must be $0$. The vector $n=(1,1)$ works:

$$
(3,-3)\cdot(1,1)=3-3=0.
$$

**General form.** A line with normal vector $n=(a,b)$ has an equation $ax+by+c=0$. With $n=(1,1)$ this is $x+y+c=0$, and the constant $c$ is found by requiring that $A$ lies on the line:

$$
1+2+c=0\quad\Longrightarrow\quad c=-3.
$$

So the general form is

$$
x+y-3=0.
$$

The same result follows by eliminating $t$ from the parametric form: adding $x=1+3t$ and $y=2-3t$ gives $x+y=3$.

## Verification

Both points satisfy the general equation:

$$
A:\ 1+2-3=0,\qquad B:\ 4+(-1)-3=0.
$$

Both points are also obtained from the parametric form, for $t=0$ and $t=1$.
