# Problem 2. Powers, Roots, and the Domain

## Problem statement

For

$$
f(x)=2\sqrt{x}-\frac3{x^2}+x^{3/2},
$$

rewrite using powers, determine the domain, compute the derivative, and compare the function and derivative domains.

## Named quantities

- $D_f$ is the domain of $f$.
- $D_{f'}$ is the domain of $f'$.

## Step 1 - Rewrite and determine $D_f$

Use $\sqrt{x}=x^{1/2}$ and $1/x^2=x^{-2}$:

$$
f(x)=2x^{1/2}-3x^{-2}+x^{3/2}.
$$

The square-root terms require $x\ge0$, while $-3x^{-2}$ requires $x\neq0$. Combining both restrictions gives

$$
D_f=(0,\infty).
$$

## Step 2 - Differentiate

**Power rule.** For $g(x)=cx^r$, $g'(x)=crx^{r-1}$ because differentiation lowers a power exponent by one and multiplies by the original exponent. This rule applies directly to every rewritten term.

$$
\begin{aligned}
\frac d{dx}(2x^{1/2})&=x^{-1/2}, \\
\frac d{dx}(-3x^{-2})&=6x^{-3}, \\
\frac d{dx}(x^{3/2})&=\frac32x^{1/2}.
\end{aligned}
$$

Thus

$$
f'(x)=x^{-1/2}+6x^{-3}+\frac32x^{1/2}
=\frac1{\sqrt{x}}+\frac6{x^3}+\frac32\sqrt{x}.
$$

## Step 3 - Compare domains

The term $1/\sqrt{x}$ requires $x>0$, and $6/x^3$ also requires $x\neq0$. The term $(3/2)\sqrt{x}$ requires $x\ge0$. Therefore

$$
D_{f'}=(0,\infty)=D_f.
$$

## Verification

At $x=1$, $f'(1)=1+6+3/2=8.5$, agreeing with termwise differentiation. At $x=0$, neither formula is defined.

## Interpretation

The derivative domain cannot include $0$ because $f'(x)$ contains $x^{-1/2}$ and $x^{-3}$, even though $f(0)$ would come from the root terms alone.

## Final answer

$$
D_f=D_{f'}=(0,\infty),
\qquad
f'(x)=\frac1{\sqrt{x}}+\frac6{x^3}+\frac32\sqrt{x}.
$$
