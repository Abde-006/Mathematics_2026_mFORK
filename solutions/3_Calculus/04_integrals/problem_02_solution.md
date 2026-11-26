# Problem 2. Powers, Roots, and the Domain

## Problem

Compute $\int(2\sqrt{x}+3/x^2-x^{1/3})dx$, determine the domain, and verify.

## Solution

Rewrite the integrand as powers:

$$
2x^{1/2}+3x^{-2}-x^{1/3}.
$$

The square root requires $x\ge0$, and $x^{-2}$ requires $x
e0$, so the original domain is $(0,\infty)$.

### Computation

The power-rule reminder is $\int x^n\,dx=\frac{x^{n+1}}{n+1}+C$ for $n\neq-1$. It raises each identified exponent by one and divides by the new exponent.

$$
\begin{aligned}
\int2x^{1/2}dx&=\frac43x^{3/2},\\
\int3x^{-2}dx&=-3x^{-1},\\
\int-x^{1/3}dx&=-\frac34x^{4/3}.
\end{aligned}
$$

Hence

$$
F(x)=\frac43x^{3/2}-\frac3x-\frac34x^{4/3}+C.
$$

### Verification

Differentiation gives $2x^{1/2}+3x^{-2}-x^{1/3}$, exactly the integrand.

## Final Answer

$$
\frac43x^{3/2}-\frac3x-\frac34x^{4/3}+C,\qquad x>0.
$$
