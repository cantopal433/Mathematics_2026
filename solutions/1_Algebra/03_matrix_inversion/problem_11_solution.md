## Question

For

$$
A(t)=
\begin{pmatrix}
1 & t \\
t & 1 \\
\end{pmatrix}
$$

find all $t$ for which the matrix is invertible, and then give a formula for $A(t)^{-1}$. Explain what happens to this formula at the excluded values.

## Solution

A $2\times2$ matrix is invertible exactly when its determinant is nonzero. Here

$$
\det A(t)=1\cdot1-t\cdot t=1-t^2=(1-t)(1+t).
$$

The determinant is zero only for $t=1$ and $t=-1$, so $A(t)$ is invertible for all $t\ne\pm1$.

For these values, the $2\times2$ formula (swap the diagonal entries, change the sign of the other two, divide by the determinant) gives

$$
A(t)^{-1}=\frac{1}{1-t^2}
\begin{pmatrix}
1 & -t \\
-t & 1 \\
\end{pmatrix},\qquad t\ne\pm1.
$$

At the excluded values the factor $\frac{1}{1-t^2}$ would require division by zero, so the formula has no meaning. This matches the structure of the matrix: for $t=1$ the two rows are equal,

$$
A(1)=
\begin{pmatrix}
1 & 1 \\
1 & 1 \\
\end{pmatrix},
$$

and for $t=-1$ the second row is the negative of the first,

$$
A(-1)=
\begin{pmatrix}
1 & -1 \\
-1 & 1 \\
\end{pmatrix}.
$$

In both cases the rows are linearly dependent, so the matrix is not invertible.

## Verification

For a general $t$:

$$
A(t)
\begin{pmatrix}
1 & -t \\
-t & 1 \\
\end{pmatrix}=
\begin{pmatrix}
1-t^2 & -t+t \\
t-t & -t^2+1 \\
\end{pmatrix}=(1-t^2)I,
$$

so after dividing by $1-t^2$ the product is $I$. For example, for $t=2$ the formula gives $-\frac13$ times the matrix with rows $(1,-2)$ and $(-2,1)$, and multiplying by $A(2)$ gives $-\frac13\cdot(-3)I=I$.
