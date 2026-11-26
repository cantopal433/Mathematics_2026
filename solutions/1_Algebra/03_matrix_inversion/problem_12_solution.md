## Question

It is known that

$$
A^{-1}=
\begin{pmatrix}
2 & -1 \\
-3 & 2 \\
\end{pmatrix}.
$$

Without finding $A$, compute $(3A)^{-1}$, $(A^T)^{-1}$, and $(A^2)^{-1}$. Justify each result using the appropriate property.

## Solution

Each result follows from the definition of the inverse: a matrix $Y$ is the inverse of $X$ if $XY=I$. It is enough to propose a candidate and check this product.

**$(3A)^{-1}$.** The candidate is $\frac13A^{-1}$, because numbers can be moved in front of a matrix product:

$$
(3A)\cdot\frac13A^{-1}=3\cdot\frac13\cdot AA^{-1}=I.
$$

So

$$
(3A)^{-1}=\frac13A^{-1}=
\begin{pmatrix}
\frac23 & -\frac13 \\
-1 & \frac23 \\
\end{pmatrix}.
$$

**$(A^T)^{-1}$.** The candidate is $(A^{-1})^T$. Using the rule $(XY)^T=Y^TX^T$:

$$
A^T(A^{-1})^T=(A^{-1}A)^T=I^T=I.
$$

So the inverse of the transpose is the transpose of the inverse:

$$
(A^T)^{-1}=(A^{-1})^T=
\begin{pmatrix}
2 & -3 \\
-1 & 2 \\
\end{pmatrix}.
$$

**$(A^2)^{-1}$.** The candidate is $(A^{-1})^2$, because

$$
A^2(A^{-1})^2=A\,(AA^{-1})\,A^{-1}=AIA^{-1}=AA^{-1}=I.
$$

So

$$
(A^2)^{-1}=(A^{-1})^2=
\begin{pmatrix}
2 & -1 \\
-3 & 2 \\
\end{pmatrix}
\begin{pmatrix}
2 & -1 \\
-3 & 2 \\
\end{pmatrix}=
\begin{pmatrix}
4+3 & -2-2 \\
-6-6 & 3+4 \\
\end{pmatrix}=
\begin{pmatrix}
7 & -4 \\
-12 & 7 \\
\end{pmatrix}.
$$

None of these steps required knowing $A$ itself.

## Verification

Only for checking, $A$ is recovered as the inverse of $A^{-1}$: since $\det A^{-1}=4-3=1$,

$$
A=
\begin{pmatrix}
2 & 1 \\
3 & 2 \\
\end{pmatrix}.
$$

Squaring gives

$$
A^2=
\begin{pmatrix}
4+3 & 2+2 \\
6+6 & 3+4 \\
\end{pmatrix}=
\begin{pmatrix}
7 & 4 \\
12 & 7 \\
\end{pmatrix},
$$

and

$$
A^2
\begin{pmatrix}
7 & -4 \\
-12 & 7 \\
\end{pmatrix}=
\begin{pmatrix}
7 & 4 \\
12 & 7 \\
\end{pmatrix}
\begin{pmatrix}
7 & -4 \\
-12 & 7 \\
\end{pmatrix}=
\begin{pmatrix}
49-48 & -28+28 \\
84-84 & -48+49 \\
\end{pmatrix}=I.
$$

Similarly, $3A$ times $\frac13A^{-1}$ and $A^T$ times $(A^{-1})^T$ both give $I$, which confirms all three results.
