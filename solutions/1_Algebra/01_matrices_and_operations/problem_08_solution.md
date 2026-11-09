## Question

For

$$
A=
\begin{pmatrix}
1 & 2 & -1 \\
2 & 4 & 1 \\
-1 & 1 & 3 \\
\end{pmatrix}
$$

perform, in order:

1. $R_2\leftarrow R_2-2R_1$,
2. $R_3\leftarrow R_3+R_1$,
3. interchange $R_2$ and $R_3$.

Write the matrix after each step. Then, for each of the three operations, state an operation that reverses it.

## Solution

After $R_2\leftarrow R_2-2R_1$, then $R_3\leftarrow R_3+R_1$, then $R_2\leftrightarrow R_3$:

$$
\begin{pmatrix}
1 & 2 & -1 \\
0 & 0 & 3 \\
-1 & 1 & 3
\end{pmatrix}
\to
\begin{pmatrix}
1 & 2 & -1 \\
0 & 0 & 3 \\
0 & 3 & 2
\end{pmatrix}
\to
\begin{pmatrix}
1 & 2 & -1 \\
0 & 3 & 2 \\
0 & 0 & 3
\end{pmatrix}.
$$

Inverse operations:

- $R_2\leftarrow R_2-2R_1$ is reversed by $R_2\leftarrow R_2+2R_1$,
- $R_3\leftarrow R_3+R_1$ is reversed by $R_3\leftarrow R_3-R_1$,
- $R_2\leftrightarrow R_3$ is reversed by the same interchange.

## Verification

Applying the inverse operations in reverse order returns the original matrix $A$.
