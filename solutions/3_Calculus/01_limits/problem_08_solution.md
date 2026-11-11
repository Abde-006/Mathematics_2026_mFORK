# Exercise 8 — A Square Root in a Function Limit

## Problem Statement

Compute

$$
\lim_{x\to4}\frac{\sqrt{x}-2}{x-4}
$$

by rationalizing the numerator.

## Step-by-Step Solution

### Step 1 — Multiply by the conjugate

Multiply the numerator and denominator by $\sqrt{x}+2$:

$$
\frac{\sqrt{x}-2}{x-4}
\cdot\frac{\sqrt{x}+2}{\sqrt{x}+2}
=\frac{(\sqrt{x}-2)(\sqrt{x}+2)}{(x-4)(\sqrt{x}+2)}.
$$

### Step 2 — Use the difference of squares

The numerator is $x-4$, so for $x\ne4$ it cancels with the denominator factor:

$$
\frac{x-4}{(x-4)(\sqrt{x}+2)}
=\frac1{\sqrt{x}+2}.
$$

### Step 3 — Take the limit

The simplified expression is continuous at $x=4$, so substitute:

$$
\lim_{x\to4}\frac1{\sqrt{x}+2}
=\frac1{\sqrt4+2}
=\frac14.
$$

This uses the same conjugate idea as Exercise 3. There, conjugation exposed a factor of $n$ that could be canceled; here, it exposes the factor $x-4$.

## Final Answer

$$
\lim_{x\to4}\frac{\sqrt{x}-2}{x-4}=\frac14.
$$

## Key Takeaways

- Rationalization removes the square root from a difference in the numerator.
- Simplifying away the indeterminate form makes direct substitution possible.