# Problem 15. The Difference Quotient as a Check of the Derivative

## Problem statement

Choose a function and a point $x_0$ where the derivative exists. Compute $f'(x_0)$ exactly, then evaluate the difference quotient for $h=1$, $0.1$, and $0.01$. Compare the values with $f'(x_0)$.

## Named quantities

- $f(x)=x^2$ is the chosen function.
- $x_0=2$ is the chosen point.
- $D(h)=\frac{f(x_0+h)-f(x_0)}h$ is the difference quotient.

## Step 1 - Compute the exact derivative

**Power-rule check.**

$$
\frac d{dx}(x^2)=2x.
$$

At $x_0=2$,

$$
f'(2)=2(2)=4.
$$

## Step 2 - Simplify the difference quotient

**Derivative definition.** The difference quotient $D(h)=[f(x_0+h)-f(x_0)]/h$ computes the secant slope and tends to $f'(x_0)$ as $h\to0$.

$$
\begin{aligned}
D(h)
&=\frac{(2+h)^2-2^2}{h} \\
&=\frac{4+4h+h^2-4}{h} \\
&=\frac{4h+h^2}{h} \\
&=4+h,\qquad h\neq0.
\end{aligned}
$$

## Step 3 - Substitute the three values

$$
\begin{aligned}
D(1)&=4+1=5, \\
D(0.1)&=4.1, \\
D(0.01)&=4.01.
\end{aligned}
$$

## Verification

The values approach $4$, exactly matching $f'(2)$. Algebraically,

$$
\lim_{h\to0}(4+h)=4.
$$

## Interpretation

The difference quotient represents the secant slope. As $h$ shrinks, the secant slope approaches the tangent slope $4$. Three numerical values suggest this behavior but do not replace the limit argument.

## Final answer

$$
f'(2)=4,
\qquad
D(1)=5,\ D(0.1)=4.1,\ D(0.01)=4.01.
$$
