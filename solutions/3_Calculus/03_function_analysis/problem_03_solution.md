# Problem 3. A Rational Function

## Problem

Analyze $f(x)=\frac{x+1}{x-2}$: domain, zeros, asymptotes, monotonicity, and sketch.

## Solution

Let $f(x)=\frac{x+1}{x-2}$.

### Step 1 - Domain and zero

The denominator cannot vanish, so $x
eq2$ and

$$
D_f=(-\infty,2)\cup(2,\infty).
$$

The numerator vanishes at $x=-1$, giving the zero $(-1,0)$.

### Step 2 - Asymptotes

At $x=2$, the denominator tends to zero while the numerator tends to $3$:

$$
\lim_{x\to2^-}f(x)=-\infty,\qquad
\lim_{x\to2^+}f(x)=\infty.
$$

Hence $x=2$ is vertical. Dividing by $x$ or rewriting,

$$
f(x)=1+\frac3{x-2},
$$

shows that $y=1$ is horizontal because $3/(x-2)\to0$ as $|x|\to\infty$.

### Step 3 - Monotonicity

The quotient rule gives

$$
f'(x)=\frac{(x-2)-(x+1)}{(x-2)^2}
=\frac{-3}{(x-2)^2}<0.
$$

Therefore $f$ is decreasing on $(-\infty,2)$ and $(2,\infty)$ and has no local extremum.

## Final Answer

Domain $(-\infty,2)\cup(2,\infty)$; zero $x=-1$; vertical asymptote $x=2$; horizontal asymptote $y=1$; decreasing on both domain intervals.
