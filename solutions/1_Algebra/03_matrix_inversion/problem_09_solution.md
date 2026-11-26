## Question

Given

$$
A=
\begin{pmatrix}
1 & 2 \\
0 & 1 \\
\end{pmatrix},\qquad B=
\begin{pmatrix}
3 & 1 \\
2 & 4 \\
\end{pmatrix}.
$$

Solve the equation $AX=B$ for $X$. Before calculating, decide on which side of the equation $A^{-1}$ must be used. Then check the result by computing $AX$.

## Solution

**Which side.** In the equation $AX=B$ the matrix $A$ stands to the left of $X$. Matrix multiplication is not commutative, so $A^{-1}$ must also be multiplied from the left, on both sides of the equation:

$$
A^{-1}AX=A^{-1}B\quad\Longrightarrow\quad X=A^{-1}B.
$$

Multiplying from the right would give $AXA^{-1}=BA^{-1}$, which does not isolate $X$.

**The inverse of $A$.** Here $\det A=1\cdot1-2\cdot0=1\ne0$, so

$$
A^{-1}=
\begin{pmatrix}
1 & -2 \\
0 & 1 \\
\end{pmatrix}.
$$

**The solution.**

$$
X=A^{-1}B=
\begin{pmatrix}
1 & -2 \\
0 & 1 \\
\end{pmatrix}
\begin{pmatrix}
3 & 1 \\
2 & 4 \\
\end{pmatrix}=
\begin{pmatrix}
3-4 & 1-8 \\
2 & 4 \\
\end{pmatrix}=
\begin{pmatrix}
-1 & -7 \\
2 & 4 \\
\end{pmatrix}.
$$

## Verification

$$
AX=
\begin{pmatrix}
1 & 2 \\
0 & 1 \\
\end{pmatrix}
\begin{pmatrix}
-1 & -7 \\
2 & 4 \\
\end{pmatrix}=
\begin{pmatrix}
-1+4 & -7+8 \\
2 & 4 \\
\end{pmatrix}=
\begin{pmatrix}
3 & 1 \\
2 & 4 \\
\end{pmatrix}=B.
$$

The equation $AX=B$ is satisfied.
