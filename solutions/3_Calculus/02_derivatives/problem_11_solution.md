# Problem 11. Derivative from the Definition

## Problem statement

Using only

$$
f'(x)=\lim_{h\to0}\frac{f(x+h)-f(x)}h,
$$

find the derivative of $f(x)=x^2$ and compare it with the power rule.

## Named quantities

- $x$ is the point of differentiation.
- $h$ is the nonzero increment.
- $D_h$ is the difference quotient.

## Step 1 - Substitute $f(x+h)$ and $f(x)$

**Difference quotient.** The derivative is the limit of the average rate of change over intervals of length $h$:

$$
f'(x)=\lim_{h\to0}\frac{f(x+h)-f(x)}h.
$$

$$
\begin{aligned}
f(x+h)&=(x+h)^2=x^2+2xh+h^2, \\
f(x)&=x^2.
\end{aligned}
$$

## Step 2 - Form the difference quotient

$$
\begin{aligned}
D_h
&=\frac{x^2+2xh+h^2-x^2}{h} \\
&=\frac{2xh+h^2}{h} \\
&=2x+h,\qquad h\neq0.
\end{aligned}
$$

## Step 3 - Take the limit

As $h\to0$,

$$
f'(x)=\lim_{h\to0}(2x+h)=2x.
$$

## Verification

The power rule with $r=2$ gives $2x^{2-1}=2x$, matching the limit calculation.

## Interpretation

The limit removes the increment $h$ from the difference quotient. The resulting number $2x$ is the instantaneous rate of change and tangent slope at $x$.

## Final answer

$$
f'(x)=2x
$$
