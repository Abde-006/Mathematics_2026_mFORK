# Problem 6. A Logarithm from a Rational Integral

## Problem

Compute $\int2x/(x^2+5)dx$, identify the substitution, and explain the logarithm.

## Solution

Choose

$$
u=x^2+5,\qquad du=2x dx.
$$

This has the form $u'/u$.

### Computation

The logarithm rule $\int du/u=\ln|u|+C$ applies because $du=2x\,dx$ and $u=x^2+5$; this is the derivative-of-the-denominator-over-the-denominator pattern.

$$
\int\frac{2x}{x^2+5}dx
=\int\frac{du}{u}
=\ln|u|+C.
$$

Since $x^2+5>0$, absolute values are unnecessary:

$$
F(x)=\ln(x^2+5)+C.
$$

The logarithm appears because $(\ln u)'=u'/u$.

### Verification

$$
F'(x)=\frac{2x}{x^2+5}.
$$

## Final Answer

$$
\ln(x^2+5)+C.
$$
