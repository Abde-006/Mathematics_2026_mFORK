# Problem 1. Derivative of a Polynomial and the Tangent Slope

## Problem statement

For

$$
f(x)=3x^5-2x^3+7x-4,
$$

find $f'(x)$, then compute $f'(0)$ and $f'(1)$ and interpret their signs.

## Named quantities

- $f(x)$ is the given polynomial.
- $m_0=f'(0)$ is the tangent slope at $x=0$.
- $m_1=f'(1)$ is the tangent slope at $x=1$.

## Step 1 - Differentiate each term

**Power rule.** If $g(x)=cx^r$, then $g'(x)=crx^{r-1}$. The derivative of a sum is the sum of the derivatives.

$$
\begin{aligned}
\frac d{dx}(3x^5)&=15x^4, \\
\frac d{dx}(-2x^3)&=-6x^2, \\
\frac d{dx}(7x)&=7, \\
\frac d{dx}(-4)&=0.
\end{aligned}
$$

Therefore

$$
f'(x)=15x^4-6x^2+7.
$$

## Step 2 - Evaluate the tangent slopes

At $x=0$,

$$
m_0=f'(0)=15(0)^4-6(0)^2+7=7.
$$

At $x=1$,

$$
m_1=f'(1)=15-6+7=16.
$$

## Verification

Both values are positive, and direct differentiation gives the same terms with no missing constant term. The constant $-4$ disappears because constants have derivative zero.

## Interpretation

At $(0,f(0))$, the tangent rises with slope $7$. At $(1,f(1))$, it rises more steeply with slope $16$.

## Final answer

$$
f'(x)=15x^4-6x^2+7,\qquad f'(0)=7,\qquad f'(1)=16.
$$
