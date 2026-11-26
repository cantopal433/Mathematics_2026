## Question

Find the equation of the plane through $P=(1,-2,3)$ and perpendicular to $n=(2,1,-1)$. Check the result by substituting the point $P$ and explain the role of the normal vector.

## Solution

**Role of the normal vector.** A point $X=(x,y,z)$ lies in the plane exactly when the vector $X-P$, which joins the given point to $X$, lies in the plane. Every vector in the plane is perpendicular to the normal vector $n$, so the condition is

$$
n\cdot(X-P)=0.
$$

The normal vector therefore fixes the orientation (tilt) of the plane, and the point $P$ fixes its position in space.

**The equation.** With $n=(2,1,-1)$ and $X-P=(x-1,\ y+2,\ z-3)$:

$$
2(x-1)+1\cdot(y+2)-1\cdot(z-3)=0.
$$

Expanding:

$$
2x-2+y+2-z+3=0,
$$

so the plane is

$$
2x+y-z+3=0.
$$

The coefficients of $x$, $y$, $z$ in this general equation are exactly the coordinates of the normal vector $(2,1,-1)$. This is true for every plane: in $ax+by+cz+d=0$ the vector $(a,b,c)$ is normal to the plane.

## Verification

Substituting $P=(1,-2,3)$:

$$
2\cdot1+(-2)-3+3=0.
$$

As an additional check, the point $Q=(0,0,3)$ also satisfies the equation, since $0+0-3+3=0$. The vector $Q-P=(-1,2,0)$ lies in the plane and is indeed perpendicular to $n$:

$$
(-1,2,0)\cdot(2,1,-1)=-2+2+0=0.
$$
