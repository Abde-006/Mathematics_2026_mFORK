# Problem 11. Choose the Method First

## Problem

Choose and apply the appropriate method for $\int\sin(3x)dx$, $\int x\ln x dx$, and $\int x/\sqrt{x^2+1}dx$.

## Solution

### Part 1 - Substitution

For $\int\sin(3x)dx$, let $u=3x$, so $du=3dx$:

$$
\int\sin(3x)dx=-\frac13\cos(3x)+C.
$$

### Part 2 - Integration by parts

For $\int x\ln x dx$, $x$ is easy to integrate and $\ln x$ is easy to differentiate:

$$
u=\ln x,\qquad dv=x dx,
$$

$$
du=\frac1x dx,\qquad v=\frac{x^2}{2}.
$$

Therefore

$$
\begin{aligned}
\int x\ln x dx
&=\frac{x^2}{2}\ln x-\int\frac{x^2}{2}\frac1x dx\\
&=\frac{x^2}{2}\ln x-\frac{x^2}{4}+C.
\end{aligned}
$$

### Part 3 - Substitution

For $\int x/\sqrt{x^2+1}dx$, let $u=x^2+1$, so $du=2x dx$:

$$
\int\frac{x}{\sqrt{x^2+1}}dx
=\frac12\int u^{-1/2}du
=\sqrt u+C
=\sqrt{x^2+1}+C.
$$

Verification:

$$
\frac d{dx}\sqrt{x^2+1}=\frac{x}{\sqrt{x^2+1}}.
$$

## Final Answers

1. $-\frac13\cos(3x)+C$.
2. $\frac{x^2}{2}\ln x-\frac{x^2}{4}+C$.
3. $\sqrt{x^2+1}+C$.
