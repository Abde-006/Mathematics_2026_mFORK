# Exercise 14 — A $0/0$ Limit with Trigonometry

## Problem Statement

Compute, without l'Hôpital's rule,

$$
\lim_{x\to0}\frac{1-\cos x}{x^2}.
$$

## Step-by-Step Solution

### Step 1 — Apply a trigonometric identity

Use the half-angle identity

$$
1-\cos x=2\sin^2\left(\frac{x}{2}\right).
$$

Substitute it into the quotient:

$$
\frac{1-\cos x}{x^2}
=\frac{2\sin^2(\frac{x}{2})}{x^2}.
$$

### Step 2 — Rewrite using the fundamental limit

Since $x^2=4(\frac{x}{2})^2$, rearrange the expression as

$$
\frac{2\sin^2(\frac{x}{2})}{x^2}
=\frac12\left(\frac{\sin(\frac{x}{2})}{\frac{x}{2}}\right)^2.
$$

### Step 3 — Take the limit

As $x\to0$, $\frac{x}{2}\to0$, so the fraction in parentheses tends to $1$:

$$
\lim_{x\to0}\frac12\left(\frac{\sin(\frac{x}{2})}{\frac{x}{2}}\right)^2
=\frac12(1)^2
=\frac12.
$$

## Final Answer

$$
\lim_{x\to0}\frac{1-\cos x}{x^2}=\frac12.
$$

## Key Takeaways

- The half-angle identity converts $1-\cos x$ into a squared sine.
- Rescaling by $x/2$ reduces the expression to the fundamental trigonometric limit.