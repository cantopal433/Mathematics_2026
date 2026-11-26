## Question

For

$$
A=
\begin{pmatrix}
1 & 1 \\
0 & 1 \\
\end{pmatrix},\qquad B=
\begin{pmatrix}
2 & 0 \\
0 & 3 \\
\end{pmatrix}
$$

compute $(AB)^{-1}$ and $B^{-1}A^{-1}$. Check that the results are the same and explain the meaning of the reversed order.

## Solution

**Direct way.** First the product is computed:

$$
AB=
\begin{pmatrix}
1 & 1 \\
0 & 1 \\
\end{pmatrix}
\begin{pmatrix}
2 & 0 \\
0 & 3 \\
\end{pmatrix}=
\begin{pmatrix}
2 & 3 \\
0 & 3 \\
\end{pmatrix}.
$$

Its determinant is $2\cdot3-3\cdot0=6\ne0$, so by the $2\times2$ formula

$$
(AB)^{-1}=\frac16
\begin{pmatrix}
3 & -3 \\
0 & 2 \\
\end{pmatrix}=
\begin{pmatrix}
\frac12 & -\frac12 \\
0 & \frac13 \\
\end{pmatrix}.
$$

**Using the separate inverses.** The matrix $A$ has determinant $1$, and $B$ is diagonal, so its inverse is obtained by inverting the diagonal entries:

$$
A^{-1}=
\begin{pmatrix}
1 & -1 \\
0 & 1 \\
\end{pmatrix},\qquad
B^{-1}=
\begin{pmatrix}
\frac12 & 0 \\
0 & \frac13 \\
\end{pmatrix}.
$$

Then

$$
B^{-1}A^{-1}=
\begin{pmatrix}
\frac12 & 0 \\
0 & \frac13 \\
\end{pmatrix}
\begin{pmatrix}
1 & -1 \\
0 & 1 \\
\end{pmatrix}=
\begin{pmatrix}
\frac12 & -\frac12 \\
0 & \frac13 \\
\end{pmatrix}.
$$

The two results are the same, so $(AB)^{-1}=B^{-1}A^{-1}$ in this example.

**Meaning of the reversed order.** The product $ABx$ first applies $B$ to $x$ and then applies $A$. To undo this, the last operation must be undone first: apply $A^{-1}$ and then $B^{-1}$, which is the product $B^{-1}A^{-1}$. Algebraically,

$$
(AB)(B^{-1}A^{-1})=A(BB^{-1})A^{-1}=AIA^{-1}=AA^{-1}=I.
$$

The order is important: the product in the other order is

$$
A^{-1}B^{-1}=
\begin{pmatrix}
\frac12 & -\frac13 \\
0 & \frac13 \\
\end{pmatrix},
$$

which differs from $(AB)^{-1}$ in the top right entry.

## Verification

$$
(AB)(AB)^{-1}=
\begin{pmatrix}
2 & 3 \\
0 & 3 \\
\end{pmatrix}
\begin{pmatrix}
\frac12 & -\frac12 \\
0 & \frac13 \\
\end{pmatrix}=
\begin{pmatrix}
1 & -1+1 \\
0 & 1 \\
\end{pmatrix}=
\begin{pmatrix}
1 & 0 \\
0 & 1 \\
\end{pmatrix}.
$$

The product is the identity matrix, so the computed inverse is correct.
