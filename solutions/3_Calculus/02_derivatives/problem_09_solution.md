# Problem 9. A Logarithm and the Chain Rule

## Problem statement

For

$$
f(x)=\ln(x^2+1),
$$

compute $f'(x)$ and determine its sign for $x<0$, $x=0$, and $x>0$.

## Named quantities

- $u=x^2+1$ is the inner expression.
- $m=f'(x)$ is the derivative.

## Step 1 - Apply the chain rule

**Logarithmic chain rule.**

$$
\frac d{dx}\ln u=\frac1u\frac{du}{dx}.
$$

The inner derivative is $du/dx=2x$.

$$
f'(x)=\frac1{x^2+1}(2x)
=\frac{2x}{x^2+1}.
$$

## Step 2 - Determine the sign

The denominator $x^2+1$ is positive for every real $x$. Thus the sign is the sign of $2x$:

$$
\begin{aligned}
x<0 &: f'(x)<0, \\
x=0 &: f'(0)=0, \\
x>0 &: f'(x)>0.
\end{aligned}
$$

## Verification

At $x=1$, $f'(1)=1$. At $x=-1$, $f'(-1)=-1$. The derivatives agree by symmetry with the even function $f(x)$.

## Interpretation

The function decreases for $x<0$, has horizontal tangent at $x=0$, and increases for $x>0$. Its minimum is $f(0)=\ln1=0$.

## Final answer

$$
f'(x)=\frac{2x}{x^2+1}.
$$

It is negative for $x<0$, zero at $x=0$, and positive for $x>0$.
