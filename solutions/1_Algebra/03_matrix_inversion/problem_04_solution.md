## Question

Find $A^{-1}$ using the Gauss–Jordan method for

$$
A=
\begin{pmatrix}
1 & 2 \\
3 & 5 \\
\end{pmatrix}.
$$

Show the augmented matrix $[A\mid I]$ after successive operations and explain why obtaining $I$ on the left gives the inverse on the right.

## Solution

The Gauss–Jordan method starts from the augmented matrix $[A\mid I]$ and applies row operations to the whole matrix until the left part becomes $I$.

Starting matrix:

$$
\begin{pmatrix}
1 & 2 & \mid & 1 & 0 \\
3 & 5 & \mid & 0 & 1 \\
\end{pmatrix}
$$

Step 1: $R_2\leftarrow R_2-3R_1$ creates a zero below the first pivot:

$$
\begin{pmatrix}
1 & 2 & \mid & 1 & 0 \\
0 & -1 & \mid & -3 & 1 \\
\end{pmatrix}
$$

Step 2: $R_2\leftarrow -R_2$ makes the second pivot equal to $1$:

$$
\begin{pmatrix}
1 & 2 & \mid & 1 & 0 \\
0 & 1 & \mid & 3 & -1 \\
\end{pmatrix}
$$

Step 3: $R_1\leftarrow R_1-2R_2$ creates a zero above the second pivot:

$$
\begin{pmatrix}
1 & 0 & \mid & -5 & 2 \\
0 & 1 & \mid & 3 & -1 \\
\end{pmatrix}
$$

The left part is now $I$, so the right part is the inverse:

$$
A^{-1}=
\begin{pmatrix}
-5 & 2 \\
3 & -1 \\
\end{pmatrix}.
$$

Why this works: every row operation is the same as multiplying from the left by an elementary matrix $E$. If the operations $E_1,E_2,E_3$ turn $A$ into $I$, then

$$
E_3E_2E_1A=I,
$$

so the product $E=E_3E_2E_1$ satisfies $EA=I$, which means $E=A^{-1}$. The same operations are applied to the right part, which started as $I$, so the right part becomes $E\cdot I=E=A^{-1}$.

## Verification

$$
AA^{-1}=
\begin{pmatrix}
1 & 2 \\
3 & 5 \\
\end{pmatrix}
\begin{pmatrix}
-5 & 2 \\
3 & -1 \\
\end{pmatrix}=
\begin{pmatrix}
-5+6 & 2-2 \\
-15+15 & 6-5 \\
\end{pmatrix}=
\begin{pmatrix}
1 & 0 \\
0 & 1 \\
\end{pmatrix}.
$$

The result also agrees with the $2\times2$ formula: $\det A=5-6=-1$, and $\frac{1}{-1}$ times the matrix with entries $5,-2,-3,1$ gives the same $A^{-1}$.
