# Problem 4. Substitution as Reversing the Chain Rule

## Problem

Compute $\int2x(x^2+1)^4dx$ by substitution and verify.

## Solution

Choose

$$
u=x^2+1.
$$

Then

$$
du=2x dx,
$$

so the exact differential is present.

### Computation

Substitution reverses the chain rule. With $u=x^2+1$ and $du=2x\,dx$, the power form $\int u^n\,du=\frac{u^{n+1}}{n+1}+C$ applies to $n=4$.

$$
\int2x(x^2+1)^4dx=\int u^4du=\frac{u^5}{5}+C
=\frac{(x^2+1)^5}{5}+C.
$$

### Verification

$$
\frac d{dx}\left[\frac{(x^2+1)^5}{5}\right]
=(x^2+1)^4(2x),
$$

which matches the integrand.

## Final Answer

$$
\frac{(x^2+1)^5}{5}+C.
$$
