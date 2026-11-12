## Question

Suppose that for a $3\times3$ matrix, $\det A=-4$. Compute

$$
\det(2A),\qquad \det(A^T),\qquad \det(A^2),\qquad \det(-A).
$$

Justify each answer using the appropriate property.

## Solution

**$\det(2A)$.** Multiplying a single row by a number $c$ multiplies the determinant by $c$. The matrix $2A$ is obtained from $A$ by multiplying each of its 3 rows by $2$, so the determinant is multiplied by $2$ three times:

$$
\det(2A)=2^3\det A=8\cdot(-4)=-32.
$$

**$\det(A^T)$.** Transposition turns rows into columns. The determinant can be expanded along a row or along a column with the same result, so transposition does not change it:

$$
\det(A^T)=\det A=-4.
$$

**$\det(A^2)$.** Since $A^2=A\cdot A$, the product rule $\det(XY)=\det X\cdot\det Y$ gives

$$
\det(A^2)=\det A\cdot\det A=(-4)^2=16.
$$

**$\det(-A)$.** The matrix $-A$ is $(-1)\cdot A$, so this is the same rule as for $2A$ with $c=-1$. Each of the 3 rows is multiplied by $-1$, and since $3$ is odd the sign changes:

$$
\det(-A)=(-1)^3\det A=(-1)\cdot(-4)=4.
$$

## Verification

The results can be checked on a concrete $3\times3$ matrix with $\det A=-4$, for example $A=\mathrm{diag}(-4,1,1)$. For a diagonal matrix the determinant is the product of the diagonal entries:

- $2A=\mathrm{diag}(-8,2,2)$, so $\det(2A)=-8\cdot2\cdot2=-32$,
- $A^T=A$, so $\det(A^T)=-4$,
- $A^2=\mathrm{diag}(16,1,1)$, so $\det(A^2)=16$,
- $-A=\mathrm{diag}(4,-1,-1)$, so $\det(-A)=4\cdot(-1)\cdot(-1)=4$.

All four values agree with the results obtained from the properties.
