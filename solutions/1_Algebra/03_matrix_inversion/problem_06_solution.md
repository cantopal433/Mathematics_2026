## Question

Solve

$$
Ax=b,
$$

where

$$
A=
\begin{pmatrix}
2 & 1 \\
1 & 3 \\
\end{pmatrix},\qquad b=
\begin{pmatrix}
5 \\
7 \\
\end{pmatrix},
$$

using $x=A^{-1}b$. Then substitute the resulting vector back into the equation and check the result.

## Solution

If $A$ is invertible, multiplying both sides of $Ax=b$ from the left by $A^{-1}$ gives

$$
A^{-1}Ax=A^{-1}b\quad\Longrightarrow\quad x=A^{-1}b.
$$

First the inverse is found with the $2\times2$ formula. The determinant is

$$
\det A=2\cdot3-1\cdot1=5\ne0,
$$

so the inverse exists:

$$
A^{-1}=\frac15
\begin{pmatrix}
3 & -1 \\
-1 & 2 \\
\end{pmatrix}.
$$

Then

$$
x=A^{-1}b=\frac15
\begin{pmatrix}
3 & -1 \\
-1 & 2 \\
\end{pmatrix}
\begin{pmatrix}
5 \\
7 \\
\end{pmatrix}=\frac15
\begin{pmatrix}
15-7 \\
-5+14 \\
\end{pmatrix}=\frac15
\begin{pmatrix}
8 \\
9 \\
\end{pmatrix}=
\begin{pmatrix}
\frac85 \\
\frac95 \\
\end{pmatrix}.
$$

So the solution is $x_1=\frac85$ and $x_2=\frac95$. Since $A$ is invertible, this solution is unique.

## Verification

Substituting the vector back into the equation:

$$
Ax=
\begin{pmatrix}
2 & 1 \\
1 & 3 \\
\end{pmatrix}
\begin{pmatrix}
\frac85 \\
\frac95 \\
\end{pmatrix}=
\begin{pmatrix}
\frac{16}{5}+\frac95 \\
\frac85+\frac{27}{5} \\
\end{pmatrix}=
\begin{pmatrix}
\frac{25}{5} \\
\frac{35}{5} \\
\end{pmatrix}=
\begin{pmatrix}
5 \\
7 \\
\end{pmatrix}=b.
$$

Both equations are satisfied.
