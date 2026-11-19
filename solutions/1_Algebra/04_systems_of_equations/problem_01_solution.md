## Question

Write the system

$$
\begin{cases}
2x-y+z=4, \\
x+3y-2z=1, \\
3x+y+z=7.
\end{cases}
$$

in the form $Ax=b$.
Identify the coefficient matrix, the vector of unknowns, and the right-hand side vector. Explain how each row of the matrix corresponds to one equation.

## Solution

A linear system can be written as one matrix equation $Ax=b$. The coefficient matrix $A$ collects the coefficients of the unknowns, the vector $x$ lists the unknowns in a fixed order, and the vector $b$ contains the right-hand sides.

With the unknowns in the order $x,y,z$:

$$
A=
\begin{pmatrix}
2 & -1 & 1 \\
1 & 3 & -2 \\
3 & 1 & 1 \\
\end{pmatrix},\qquad
x=
\begin{pmatrix}
x \\
y \\
z \\
\end{pmatrix},\qquad
b=
\begin{pmatrix}
4 \\
1 \\
7 \\
\end{pmatrix},
$$

so the system is

$$
\begin{pmatrix}
2 & -1 & 1 \\
1 & 3 & -2 \\
3 & 1 & 1 \\
\end{pmatrix}
\begin{pmatrix}
x \\
y \\
z \\
\end{pmatrix}=
\begin{pmatrix}
4 \\
1 \\
7 \\
\end{pmatrix}.
$$

Row $i$ of $A$ contains the coefficients of equation $i$, and column $j$ contains all coefficients of the $j$-th unknown. A missing unknown would appear as a $0$ in its column. In the first equation, $2x-y+z=4$, the coefficients $2$, $-1$, $1$ form the first row of $A$, and the right-hand side $4$ is the first entry of $b$. The same holds for the second and third equations.

## Verification

Multiplying $A$ by $x$ row by column gives back the left-hand sides:

$$
Ax=
\begin{pmatrix}
2x-y+z \\
x+3y-2z \\
3x+y+z \\
\end{pmatrix}.
$$

Setting this equal to $b$ gives exactly the three original equations.
