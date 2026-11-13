# Exercise 11 — An $n$-th Root

## Problem Statement

Compute the limit, explain which term dominates and why, and describe how this comparison differs from comparing the degrees in a quotient of polynomials:

$$
\lim_{n\to\infty}\sqrt[n]{5^n+2^n}.
$$

## Step-by-Step Solution

### Step 1 — Factor out the dominant exponential term

Since $5^n$ grows faster than $2^n$, factor $5^n$ from the expression inside the root:

$$
\sqrt[n]{5^n+2^n}
=\sqrt[n]{5^n\left(1+\left(\frac25\right)^n\right)}.
$$

### Step 2 — Separate the factors

For positive quantities, the $n$-th root of a product is the product of the $n$-th roots:

$$
\sqrt[n]{5^n+2^n}
=5\left(1+\left(\frac25\right)^n\right)^{1/n}.
$$

### Step 3 — Bound the remaining factor

Because $0<(\frac25)^n<1$,

$$
1\leq 1+\left(\frac25\right)^n\leq2.
$$

Taking $n$-th roots preserves the inequalities:

$$
1\leq\left(1+\left(\frac25\right)^n\right)^{1/n}\leq2^{1/n}.
$$

Both bounds tend to $1$, so the squeeze theorem shows that the remaining factor tends to $1$. Therefore the original expression tends to $5$.

The largest exponential term determines the limit after the common factor is extracted. Unlike a polynomial quotient, the key comparison is between exponential bases.

## Final Answer

$$
\lim_{n\to\infty}\sqrt[n]{5^n+2^n}=5.
$$

## Key Takeaways

- Factor out the term with the largest exponential base.
- The $n$-th root of a factor bounded between positive constants tends to $1$.