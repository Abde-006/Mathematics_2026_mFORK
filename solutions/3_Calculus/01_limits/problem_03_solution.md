# Exercise 3 — A Square Root and Removing an Indeterminate Form

## Problem Statement

Compute

$$
\lim_{n\to\infty}\left(\sqrt{n^2+5n}-n\right)
$$

using the conjugate expression.

## Step-by-Step Solution

### Step 1 — Multiply by the conjugate

The two terms inside the parentheses both grow like $n$, so their difference is not easy to read directly. Multiply by the conjugate and divide by the same expression:

$$
\sqrt{n^2+5n}-n
=\frac{(\sqrt{n^2+5n}-n)(\sqrt{n^2+5n}+n)}
{\sqrt{n^2+5n}+n}.
$$

### Step 2 — Simplify using the difference of squares

The numerator becomes $(n^2+5n)-n^2=5n$:

$$
\frac{(n^2+5n)-n^2}{\sqrt{n^2+5n}+n}
=\frac{5n}{\sqrt{n^2+5n}+n}.
$$

Since $n>0$, factor $n$ from the denominator and cancel:

$$
\frac{5n}{n\sqrt{1+\frac5n}+n}
=\frac{5}{\sqrt{1+\frac5n}+1}.
$$

### Step 3 — Take the limit

As $n\to\infty$, $\frac5n\to0$. Therefore

$$
\lim_{n\to\infty}\frac{5}{\sqrt{1+\frac5n}+1}
=\frac5{\sqrt{1}+1}=\frac52.
$$

Conjugation replaces a difference of two large, nearly equal quantities with a quotient whose behavior is direct.

## Final Answer

$$
\lim_{n\to\infty}\left(\sqrt{n^2+5n}-n\right)=\frac52.
$$

## Key Takeaways

- Multiply by the conjugate to use the difference-of-squares identity.
- Factor the dominant power before taking the limit.