# Problem 6. From a Sequence to a Function — Limit at Infinity

## Problem statement

Compute

$$
\lim_{x\to\infty}\frac{3x^2-x+1}{5x^2+4x-2}.
$$

## Named quantities

- $x$ is a real variable.
- $L$ is the requested limit.

## Step 1 - Divide by $x^2$

**Leading-term rule.** For $x\to\pm\infty$, divide numerator and denominator by the highest power of $x$ in the denominator. Lower-degree terms then vanish.

$$
\frac{3x^2-x+1}{5x^2+4x-2}
=\frac{3-\frac1x+\frac1{x^2}}
       {5+\frac4x-\frac2{x^2}}.
$$

## Step 2 - Take the limit

As $x\to\infty$, $1/x\to0$ and $1/x^2\to0$. Therefore

$$
L=\frac{3-0+0}{5+0-0}=\frac35.
$$

## Verification

At $x=100$,

$$
\frac{30000-100+1}{50000+400-2}\approx0.5933,
$$

close to $3/5$.

## Interpretation

The algebra is the same as for the sequence in Problem 1. The variable changes from integer $n$ to continuous real $x$; degree comparison remains unchanged.

## Final answer

$$
\frac35
$$
