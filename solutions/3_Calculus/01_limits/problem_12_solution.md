# Exercise 12 — Exponential Function Limit

## Problem Statement

Compute the limit, connect it with the classical limit in Exercise 5, and show the transformation that reduces this expression to that pattern:

$$
\lim_{x\to0}(1+3x)^{1/x}.
$$

## Step-by-Step Solution

### Step 1 — Match the classical limit

For $x$ sufficiently close to $0$, the base $1+3x$ is positive. Rewrite the exponent to expose the classical form:

$$
(1+3x)^{1/x}
=\left((1+3x)^{1/(3x)}\right)^3.
$$

### Step 2 — Change variables

Let $u=3x$. Then $u\to0$ as $x\to0$, and the expression inside parentheses becomes $(1+u)^{1/u}$. The classical limit leading to $e$ gives

$$
\lim_{u\to0}(1+u)^{1/u}=e.
$$

Taking the cube of this limit,

$$
\lim_{x\to0}(1+3x)^{1/x}=e^3.
$$

The factor $3$ in the exponent scaling becomes the third power of the classical limit.

## Final Answer

$$
\lim_{x\to0}(1+3x)^{1/x}=e^3.
$$

## Key Takeaways

- Rewrite the exponent so the base and exponent match $(1+u)^{1/u}$.
- A fixed power outside a limit becomes the same power of the limiting value.