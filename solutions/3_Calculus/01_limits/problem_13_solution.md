# Exercise 13 — Fundamental Trigonometric Limit

## Problem Statement

Using

$$
\lim_{x\to0}\frac{\sin x}{x}=1,
$$

compute

$$
\lim_{x\to0}\frac{\sin5x}{x},
\qquad
\lim_{x\to0}\frac{\sin2x}{\sin3x}.
$$

## Step-by-Step Solution

### Step 1 — Reduce the first limit to the fundamental limit

Multiply and divide by $5$:

$$
\frac{\sin5x}{x}
=5\frac{\sin5x}{5x}.
$$

As $x\to0$, the angle $5x\to0$. Therefore

$$
\lim_{x\to0}\frac{\sin5x}{x}
=5\lim_{x\to0}\frac{\sin5x}{5x}
=5.
$$

### Step 2 — Reduce the second limit

Rewrite both sine terms using their respective angles in the denominator:

$$
\frac{\sin2x}{\sin3x}
=\frac23
\frac{\frac{\sin2x}{2x}}{\frac{\sin3x}{3x}}.
$$

As $x\to0$, both fractions approach the fundamental limit $1$. The denominator limit is nonzero, so

$$
\lim_{x\to0}\frac{\sin2x}{\sin3x}
=\frac23\frac{1}{1}
=\frac23.
$$

## Final Answer

$$
\lim_{x\to0}\frac{\sin5x}{x}=5,
\qquad
\lim_{x\to0}\frac{\sin2x}{\sin3x}=\frac23.
$$

## Key Takeaways

- Rescale the denominator to match the sine's angle.
- Apply the fundamental limit to each factor after rewriting.