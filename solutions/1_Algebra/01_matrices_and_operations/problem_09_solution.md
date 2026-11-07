## Solution

$$
Sx=\begin{pmatrix}2\\ 2\end{pmatrix},\quad RSx=\begin{pmatrix}-2\\ 2\end{pmatrix};\qquad
Rx=\begin{pmatrix}-2\\ 1\end{pmatrix},\quad SRx=\begin{pmatrix}-4\\ 1\end{pmatrix}.
$$

The results differ. In $RSx$ the $x$-coordinate is doubled before rotation; in $SRx$ the vector is rotated first, so the doubling acts on a different component. Scaling is not uniform, so it does not commute with rotation.

## Verification

$RS=\begin{pmatrix}0 & -1\\ 2 & 0\end{pmatrix}\ne SR=\begin{pmatrix}0 & -2\\ 1 & 0\end{pmatrix}$.
