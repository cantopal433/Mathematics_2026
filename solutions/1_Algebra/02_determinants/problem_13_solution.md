## Question

Compute the determinant

$$
A=
\begin{pmatrix}
1 & 2 & 3 \\
2 & 5 & 7 \\
1 & 0 & 2 \\
\end{pmatrix}
$$

using elimination. Record the effect of every row operation used on the value of the determinant.

## Solution

Elimination uses only operations of the form $R_i\leftarrow R_i+cR_j$ with $i\ne j$. Adding a multiple of one row to another row does not change the determinant, so its value is the same after every step.

Step 1: $R_2\leftarrow R_2-2R_1$, which gives $(2-2,\ 5-4,\ 7-6)=(0,1,1)$:

$$
\begin{pmatrix}
1 & 2 & 3 \\
0 & 1 & 1 \\
1 & 0 & 2 \\
\end{pmatrix}.
$$

Effect on the determinant: none.

Step 2: $R_3\leftarrow R_3-R_1$, which gives $(1-1,\ 0-2,\ 2-3)=(0,-2,-1)$:

$$
\begin{pmatrix}
1 & 2 & 3 \\
0 & 1 & 1 \\
0 & -2 & -1 \\
\end{pmatrix}.
$$

Effect on the determinant: none.

Step 3: $R_3\leftarrow R_3+2R_2$, which gives $(0,\ -2+2,\ -1+2)=(0,0,1)$:

$$
\begin{pmatrix}
1 & 2 & 3 \\
0 & 1 & 1 \\
0 & 0 & 1 \\
\end{pmatrix}.
$$

Effect on the determinant: none.

The final matrix is upper triangular, so its determinant is the product of the diagonal entries. Since no step changed the determinant,

$$
\det A=1\cdot1\cdot1=1.
$$

## Verification

Direct cofactor expansion of the original matrix along the first row:

$$
1\cdot(5\cdot2-7\cdot0)-2\cdot(2\cdot2-7\cdot1)+3\cdot(2\cdot0-5\cdot1)=10+6-15=1.
$$

This agrees with the result obtained by elimination.
