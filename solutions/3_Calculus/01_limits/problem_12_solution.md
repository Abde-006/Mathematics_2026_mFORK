# Problem 12. Exponential Function Limit

## Problem statement

Compute

$$
\lim_{x\to0}(1+3x)^{1/x}.
$$

## Named quantities

- $u=3x$ is the increment in the base.
- $L$ is the requested limit.

## Step 1 - Substitute $u=3x$

**Classical exponential limit.**

$$
\lim_{u\to0}(1+u)^{1/u}=e.
$$

As $x\to0$, $u=3x\to0$. Also,

$$
\frac1x=\frac3u.
$$

Thus

$$
(1+3x)^{1/x}
=(1+u)^{3/u}
=\left((1+u)^{1/u}\right)^3.
$$

## Step 2 - Apply the limit

By continuity of exponentiation,

$$
L=\left(\lim_{u\to0}(1+u)^{1/u}\right)^3=e^3.
$$

## Verification

At $x=0.001$, $(1.003)^{1000}\approx20.073$, close to $e^3\approx20.0855$. At $x=-0.001$, $(0.997)^{-1000}\approx20.079$. Both sides approach $e^3$.

## Interpretation

The factor $3$ in $3x$ becomes a triple exponent in the limit, giving $e^3$.

## Final answer

$$
e^3
$$
