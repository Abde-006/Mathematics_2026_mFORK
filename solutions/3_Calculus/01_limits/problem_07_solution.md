# Exercise 7 — Limit at a Point and Canceling a Factor

## Problem Statement

Compute the limit and explain why the value of the function at $x=3$ is not needed to determine it.

$$
\lim_{x\to3}\frac{x^2-4x+3}{x-3}.
$$

## Step-by-Step Solution

### Step 1 — Factor the numerator

Find two numbers with product $3$ and sum $-4$, namely $-1$ and $-3$:

$$
x^2-4x+3=(x-1)(x-3).
$$

### Step 2 — Cancel the common factor near $x=3$

For $x\ne3$, cancel the factor $x-3$:

$$
\frac{x^2-4x+3}{x-3}
=\frac{(x-1)(x-3)}{x-3}
=x-1.
$$

The original quotient is undefined at $x=3$, but a limit concerns values arbitrarily close to $3$, not necessarily the value at $3$ itself.

### Step 3 — Take the limit of the simplified expression

$$
\lim_{x\to3}(x-1)=3-1=2.
$$

## Final Answer

$$
\lim_{x\to3}\frac{x^2-4x+3}{x-3}=2.
$$

## Key Takeaways

- Canceling a factor is valid in a punctured neighborhood where that factor is nonzero.
- The limit can exist even when the original function is undefined at the limiting point.