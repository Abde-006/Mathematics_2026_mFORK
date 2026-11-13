# Exercise 1 — Dominant Terms in a Sequence

## Problem Statement

Compute the limit and explain why the highest-degree terms determine its value:

$$
\lim_{n\to\infty}\frac{4n^2-3n+1}{2n^2+5n-7}.
$$

## Step-by-Step Solution

### Step 1 — Divide by the highest power of $n$

The numerator and denominator both have degree $2$. Divide every term by $n^2$:

$$
\frac{4n^2-3n+1}{2n^2+5n-7}
=\frac{4-\frac3n+\frac1{n^2}}{2+\frac5n-\frac7{n^2}}.
$$

### Step 2 — Take the limit of each term

As $n\to\infty$, both $\frac1n$ and $\frac1{n^2}$ tend to $0$. The denominator tends to $2$, which is nonzero, so the quotient limit is

$$
\lim_{n\to\infty}
\frac{4-\frac3n+\frac1{n^2}}{2+\frac5n-\frac7{n^2}}
=\frac{4-0+0}{2+0-0}=2.
$$

The terms of highest degree determine the result because the lower-degree terms become negligible after division by $n^2$.

## Final Answer

$$
\lim_{n\to\infty}\frac{4n^2-3n+1}{2n^2+5n-7}=2.
$$

## Key Takeaways

- For a quotient of polynomials of equal degree, the limit is the ratio of the leading coefficients.
- Dividing by the highest power makes the vanishing lower-order terms visible.