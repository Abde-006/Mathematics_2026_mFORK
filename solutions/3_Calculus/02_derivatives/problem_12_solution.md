# Problem 12. Several Rules at Once

## Problem statement

For

$$
f(x)=(x^2+1)^3e^x,
$$

compute $f'(x)$ and factor the result.

## Named quantities

- $u(x)=(x^2+1)^3$ is the first factor.
- $v(x)=e^x$ is the second factor.

## Step 1 - Plan the differentiation

The whole expression is a product, so apply the product rule. One factor requires the chain rule.

## Step 2 - Differentiate the factors

**Chain rule.** For $u(x)=(x^2+1)^3$, the outer power $u^3$ and inner expression $x^2+1$ give $u'=3(x^2+1)^2(2x)$.

$$
u'=6x(x^2+1)^2,
\qquad
v'=e^x.
$$

## Step 3 - Apply the product rule

**Product rule.** The whole expression is $uv$, so $(uv)'=u'v+uv'$; this accounts for variation in both factors.

$$
\begin{aligned}
f'(x)
&=u'v+uv' \\
&=6x(x^2+1)^2e^x+(x^2+1)^3e^x.
\end{aligned}
$$

## Step 4 - Factor common terms

The common factors are $(x^2+1)^2$ and $e^x$. Thus

$$
\begin{aligned}
f'(x)
&=(x^2+1)^2e^x\left(6x+(x^2+1)\right) \\
&=(x^2+1)^2e^x(x^2+6x+1).
\end{aligned}
$$

## Verification

At $x=0$, the result gives $(1)^2(1)(1)=1$. Direct product-rule substitution at $x=0$ gives $0+1=1$.

## Interpretation

Factoring exposes the common structure and makes zeros and signs easier to analyze.

## Final answer

$$
f'(x)=(x^2+1)^2e^x(x^2+6x+1)
$$
