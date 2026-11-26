# Problem 14. A $0/0$ Limit with Trigonometry

## Problem statement

Compute

$$
\lim_{x\to0}\frac{1-\cos x}{x^2}
$$

without l'Hôpital's rule.

## Named quantities

- $x$ is an angle in radians.
- $u=x/2$ is the half-angle argument.
- $L$ is the requested limit.

## Step 1 - Apply the identity

**Half-angle identity.**

$$
1-\cos x=2\sin^2\left(\frac x2\right).
$$

Because $x^2=4(x/2)^2$,

$$
\begin{aligned}
\frac{1-\cos x}{x^2}
&=\frac{2\sin^2(x/2)}{x^2} \\
&=\frac12\left(\frac{\sin(x/2)}{x/2}\right)^2.
\end{aligned}
$$

## Step 2 - Apply the fundamental limit

**Fundamental trigonometric limit.** This limit tests the ratio of $\sin u$ to its angle $u$ for a small angle in radians and will be used to evaluate the remaining factor.

$$
\lim_{u\to0}\frac{\sin u}{u}=1.
$$

As $x\to0$, $u=x/2\to0$, so

$$
\frac{\sin(x/2)}{x/2}\to1.
$$

Therefore

$$
L=\frac12(1)^2=\frac12.
$$

## Verification

At $x=0.01$ radians,

$$
\frac{1-\cos0.01}{0.0001}\approx0.4999958,
$$

which approaches $1/2$.

## Interpretation

Near zero, $1-\cos x$ is approximately $x^2/2$. Geometrically, this is the quadratic gap below $1$ on the cosine graph.

## Final answer

$$
\frac12
$$
