# Exercise 2 — Different Growth Rates

## Problem Statement

Compute both limits, compare the two cases, and formulate a general observation about how the degrees of the numerator and denominator affect the result:

$$
\lim_{n\to\infty}\frac{3n+1}{n^2+4},
\qquad
\lim_{n\to\infty}\frac{2n^3-n}{5n^2+1}.
$$

## Step-by-Step Solution

### Step 1 — Limit with lower numerator degree

The numerator has degree $1$ and the denominator has degree $2$. Divide both by $n^2$:

$$
\frac{3n+1}{n^2+4}
=\frac{\frac3n+\frac1{n^2}}{1+\frac4{n^2}}.
$$

The numerator tends to $0$ and the denominator tends to $1$, so

$$
\lim_{n\to\infty}\frac{3n+1}{n^2+4}=0.
$$

### Step 2 — Limit with higher numerator degree

Here the numerator has degree $3$ and the denominator has degree $2$. Divide both by $n^2$:

$$
\frac{2n^3-n}{5n^2+1}
=\frac{2n-\frac1n}{5+\frac1{n^2}}.
$$

The denominator tends to $5$, while the numerator grows without bound like $2n$. Thus

$$
\lim_{n\to\infty}\frac{2n^3-n}{5n^2+1}=+\infty.
$$

### Step 3 — Compare the degrees

For these positive leading terms, a numerator degree below the denominator degree gives limit $0$, equal degrees give the ratio of leading coefficients, and a numerator degree above the denominator degree gives unbounded growth. For degree difference greater than zero, the sign of the leading-coefficient ratio determines the direction of divergence.

## Final Answer

$$
\lim_{n\to\infty}\frac{3n+1}{n^2+4}=0,
\qquad
\lim_{n\to\infty}\frac{2n^3-n}{5n^2+1}=+\infty.
$$

## Key Takeaways

- Compare degrees by dividing by the largest relevant power.
- A higher-degree numerator can make the quotient diverge rather than approach a finite number.