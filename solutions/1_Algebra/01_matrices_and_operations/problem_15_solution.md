## Question

Given

$$
A=
\begin{pmatrix}
1 & 2 & 0 \\
0 & 1 & 1 \\
\end{pmatrix},\quad B=
\begin{pmatrix}
1 & 0 \\
2 & 1 \\
-1 & 3 \\
\end{pmatrix},\quad C=
\begin{pmatrix}
2 & 1 \\
0 & -1 \\
\end{pmatrix}.
$$

Compute $(AB)C$ and $A(BC)$. Compare the results and the number of intermediate operations. Explain what associativity of matrix multiplication means in this example.

## Solution

First path, $(AB)C$. The product $AB$ is $(2\times3)(3\times2)$, so it is $2\times2$:

$$
AB=
\begin{pmatrix}
1\cdot1+2\cdot2+0\cdot(-1) & 1\cdot0+2\cdot1+0\cdot3 \\
0\cdot1+1\cdot2+1\cdot(-1) & 0\cdot0+1\cdot1+1\cdot3 \\
\end{pmatrix}=
\begin{pmatrix}
5 & 2 \\
1 & 4 \\
\end{pmatrix}.
$$

Then

$$
(AB)C=
\begin{pmatrix}
5 & 2 \\
1 & 4 \\
\end{pmatrix}
\begin{pmatrix}
2 & 1 \\
0 & -1 \\
\end{pmatrix}=
\begin{pmatrix}
10 & 3 \\
2 & -3 \\
\end{pmatrix}.
$$

Second path, $A(BC)$. The product $BC$ is $(3\times2)(2\times2)$, so it is $3\times2$:

$$
BC=
\begin{pmatrix}
1 & 0 \\
2 & 1 \\
-1 & 3 \\
\end{pmatrix}
\begin{pmatrix}
2 & 1 \\
0 & -1 \\
\end{pmatrix}=
\begin{pmatrix}
2 & 1 \\
4 & 1 \\
-2 & -4 \\
\end{pmatrix}.
$$

Then

$$
A(BC)=
\begin{pmatrix}
1 & 2 & 0 \\
0 & 1 & 1 \\
\end{pmatrix}
\begin{pmatrix}
2 & 1 \\
4 & 1 \\
-2 & -4 \\
\end{pmatrix}=
\begin{pmatrix}
2+8+0 & 1+2+0 \\
0+4-2 & 0+1-4 \\
\end{pmatrix}=
\begin{pmatrix}
10 & 3 \\
2 & -3 \\
\end{pmatrix}.
$$

Both paths give the same matrix.

Number of operations: multiplying an $m\times n$ matrix by an $n\times p$ matrix needs $m\cdot n\cdot p$ scalar multiplications.

- $(AB)C$: $AB$ needs $2\cdot3\cdot2=12$, then $(AB)C$ needs $2\cdot2\cdot2=8$, in total $20$.
- $A(BC)$: $BC$ needs $3\cdot2\cdot2=12$, then $A(BC)$ needs $2\cdot3\cdot2=12$, in total $24$.

Associativity means that $(AB)C=A(BC)$ whenever the products are defined: the order of the factors must stay the same, but the brackets may be placed in either way. The final result does not depend on the grouping, only the amount of work does. In this example the first path is cheaper, because its intermediate matrix $AB$ is only $2\times2$, while $BC$ is $3\times2$.

## Verification

The two independent calculations produce the same matrix

$$
\begin{pmatrix}
10 & 3 \\
2 & -3 \\
\end{pmatrix},
$$

which confirms $(AB)C=A(BC)$ in this example.
