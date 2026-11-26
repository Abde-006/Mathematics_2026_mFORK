# Problem 7. Limit at a Point and Canceling a Factor

## Problem statement

Compute

$$
\lim_{x\to3}\frac{x^2-4x+3}{x-3}.
$$

## Named quantities

- $x$ is the independent variable.
- $P(x)=x^2-4x+3=(x-1)(x-3)$ is the numerator.
- $D(x)=x-3$ is the denominator.
- $L$ is the limit.

## Step 1 - Factor and cancel

**Limit after cancellation.** For $x\neq c$, an algebraic factor common to numerator and denominator may be canceled. The limit concerns values arbitrarily close to $c$, not necessarily the value at $c$.

$$
\frac{x^2-4x+3}{x-3}
=\frac{(x-1)(x-3)}{x-3}
=x-1,\qquad x\neq3.
$$

## Step 2 - Take the limit

The original and simplified expressions agree for every $x\neq3$, so

$$
L=\lim_{x\to3}(x-1)=3-1=2.
$$

## Verification

At $x=3.01$, the quotient equals $2.01$, and at $x=2.99$ it equals $1.99$. Both sides approach $2$.

## Interpretation

The original function is undefined at $x=3$, but nearby values determine the limit. The graph is the line $y=x-1$ with a hole at $(3,2)$.

## Final answer

$$
2
$$
