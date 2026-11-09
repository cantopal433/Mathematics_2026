## Question

Let

$$
S=
\begin{pmatrix}
2 & 0 \\
0 & 1 \\
\end{pmatrix},\qquad R=
\begin{pmatrix}
0 & -1 \\
1 & 0 \\
\end{pmatrix}.
$$

The matrix $S$ describes nonuniform scaling, while $R$ describes a $90^\circ$ counterclockwise rotation.
For

$$
x=
\begin{pmatrix}
1 \\
2 \\
\end{pmatrix}
$$

compute $RSx$ and $SRx$. Compare the results and explain geometrically why the order of these transformations matters.

## Solution

$$
Sx=
\begin{pmatrix}
2 \\
2
\end{pmatrix},\quad
RSx=
\begin{pmatrix}
-2 \\
2
\end{pmatrix};\qquad
Rx=
\begin{pmatrix}
-2 \\
1
\end{pmatrix},\quad
SRx=
\begin{pmatrix}
-4 \\
1
\end{pmatrix}.
$$

The results differ. In $RSx$ the $x$-coordinate is doubled before rotation; in $SRx$ the vector is rotated first, so the doubling acts on a different component. Scaling is not uniform, so it does not commute with rotation.

## Verification

$$
RS=
\begin{pmatrix}
0 & -1 \\
2 & 0
\end{pmatrix}\ne
SR=
\begin{pmatrix}
0 & -2 \\
1 & 0
\end{pmatrix}.
$$
