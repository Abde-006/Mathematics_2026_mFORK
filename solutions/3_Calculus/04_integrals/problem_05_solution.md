# Problem 5. The Same Substitution in a Different Context

## Problem

Compute $\int xe^{x^2}dx$ and compare with Problem 4.

## Solution

The inner function is

$$
u=x^2,\qquad du=2x dx,
$$

so $x dx=\frac12du$.

### Computation

The substitution $u=x^2$ gives $du=2x\,dx$, so the exponential rule $\int e^u\,du=e^u+C$ applies after factoring $\frac12$.

$$
\int xe^{x^2}dx
=\frac12\int e^u du
=\frac12e^u+C
=\frac12e^{x^2}+C.
$$

The structure is the same as Problem 4: an inner function $x^2$, an outer power or exponential, and a factor proportional to $dx^2/dx$.

### Verification

$$
\frac d{dx}\left(\frac12e^{x^2}\right)=xe^{x^2}.
$$

## Final Answer

$$
\frac12e^{x^2}+C.
$$
