## Question

Given

$$
L:(x,y,z)=(2,-1,3)+t(1,2,-2).
$$

State a point on the line and its direction vector, check whether $P=(4,3,-1)$ lies on $L$, and find the point corresponding to $t=-1$.

## Solution

The line is written in the form "point plus $t$ times direction vector":

$$
L:\ (x,y,z)=P_0+t\,v,\qquad P_0=(2,-1,3),\quad v=(1,2,-2).
$$

So the point $P_0=(2,-1,3)$ lies on the line (it corresponds to $t=0$), and $v=(1,2,-2)$ is a direction vector.

**Does $P=(4,3,-1)$ lie on $L$?** The point lies on $L$ exactly when one value of $t$ satisfies all three coordinate equations at once:

$$
\begin{cases}
2+t=4, \\
-1+2t=3, \\
3-2t=-1.
\end{cases}
$$

The first equation gives $t=2$, the second gives $2t=4$, so $t=2$, and the third gives $-2t=-4$, so $t=2$. All three equations give the same value $t=2$, so $P$ lies on $L$. If the values were different, the point would not lie on the line.

Equivalently, $P-P_0=(2,4,-4)=2\,(1,2,-2)$ is a multiple of the direction vector.

**The point for $t=-1$.**

$$
(x,y,z)=(2,-1,3)+(-1)\cdot(1,2,-2)=(2-1,\ -1-2,\ 3+2)=(1,-3,5).
$$

## Verification

Substituting $t=2$ into the parametric equation gives back $P$:

$$
(2,-1,3)+2\cdot(1,2,-2)=(2+2,\ -1+4,\ 3-4)=(4,3,-1).
$$

For $t=-1$, the vector from $P_0$ to $(1,-3,5)$ is $(-1,-2,2)=-v$, which is again a multiple of $v$.
