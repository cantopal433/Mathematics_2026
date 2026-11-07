## Solution

The product of an $m\times n$ and a $p\times q$ matrix is defined only if $n=p$; the result is $m\times q$.

| Product | Sizes | Defined | Result |
|---|---|---|---|
| $AB$ | $(2\times3)(3\times4)$ | yes | $2\times4$ |
| $BA$ | $(3\times4)(2\times3)$ | no, $4\ne2$ | – |
| $BC$ | $(3\times4)(4\times2)$ | yes | $3\times2$ |
| $CB$ | $(4\times2)(3\times4)$ | no, $2\ne3$ | – |
| $AC$ | $(2\times3)(4\times2)$ | no, $3\ne4$ | – |
| $CA$ | $(4\times2)(2\times3)$ | yes | $4\times3$ |
| $AD$ | $(2\times3)(2\times2)$ | no, $3\ne2$ | – |
| $DA$ | $(2\times2)(2\times3)$ | yes | $2\times3$ |

## Verification

In every defined case the inner dimensions agree and the outer dimensions give the result size.
