# Problem 8. A Square Root in a Function Limit

## Problem statement

Compute

$$
\lim_{x\to4}\frac{\sqrt{x}-2}{x-4}
$$

by rationalizing the numerator.

## Named quantities

- $x$ is the independent variable.
- $L$ is the requested limit.

## Step 1 - Rationalize

**Rationalization identity.**

$$
(\sqrt{x}-2)(\sqrt{x}+2)=x-4.
$$

This identity transforms the numerator difference into the denominator factor $x-4$.

For $x\ge0$ and $x\neq4$, multiply by $(\sqrt{x}+2)/(\sqrt{x}+2)$:

$$
\begin{aligned}
\frac{\sqrt{x}-2}{x-4}
&=\frac{\sqrt{x}-2}{x-4}\cdot\frac{\sqrt{x}+2}{\sqrt{x}+2} \\
&=\frac{x-4}{(x-4)(\sqrt{x}+2)} \\
&=\frac1{\sqrt{x}+2}.
\end{aligned}
$$

## Step 2 - Substitute $x=4$

$$
L=\frac1{\sqrt4+2}=\frac14.
$$

## Verification

At $x=4.01$, $\sqrt{4.01}\approx2.002498$, so

$$
\frac{2.002498-2}{0.01}\approx0.2498.
$$

At $x=3.99$, the quotient is approximately $0.2502$. Both sides approach $1/4$.

## Interpretation

The limit is the difference quotient for $\sqrt{x}$ at $x=4$. Geometrically, it is the tangent slope $1/(2\sqrt4)=1/4$.

## Final answer

$$
\frac14
$$
