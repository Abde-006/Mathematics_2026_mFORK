# Exercise 6 — From a Sequence to a Function

## Problem Statement

Compute

$$
\lim_{x\to\infty}\frac{3x^2-x+1}{5x^2+4x-2}.
$$

## Step-by-Step Solution

### Step 1 — Divide by the highest power of $x$

The numerator and denominator have the same degree, $2$. Divide every term by $x^2$:

$$
\frac{3x^2-x+1}{5x^2+4x-2}
=\frac{3-\frac1x+\frac1{x^2}}{5+\frac4x-\frac2{x^2}}.
$$

### Step 2 — Take the limit

As $x\to\infty$, $\frac1x\to0$ and $\frac1{x^2}\to0$. The denominator tends to the nonzero number $5$, so

$$
\lim_{x\to\infty}\frac{3-\frac1x+\frac1{x^2}}{5+\frac4x-\frac2{x^2}}
=\frac35.
$$

The method is the same as for the sequence in Exercise 1: divide by the highest power and retain the ratio of leading coefficients. The variable now ranges over real values rather than integer indices, but the terms of lower degree still become negligible as the argument grows.

## Final Answer

$$
\lim_{x\to\infty}\frac{3x^2-x+1}{5x^2+4x-2}=\frac35.
$$

## Key Takeaways

- The dominant-term method applies to polynomial quotients in both sequences and functions.
- Replacing $n$ by a real variable changes the domain approaching infinity, not the algebraic method.