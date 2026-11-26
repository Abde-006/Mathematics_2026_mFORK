# Problem 3. The Product Rule — Why Is It Needed?

## Problem statement

For

$$
f(x)=(x^2+1)e^x,
$$

compute $f'(x)$ and explain why $(2x)e^x$ is incomplete.

## Named quantities

- $u(x)=x^2+1$ is the first factor.
- $v(x)=e^x$ is the second factor.

## Step 1 - Identify and differentiate the factors

**Product rule.** If $f=uv$, then

$$
f'=u'v+uv'.
$$

Both factors vary, so neither factor may be treated as constant.

$$
u'(x)=2x,
\qquad
v'(x)=e^x.
$$

## Step 2 - Apply the product rule

$$
\begin{aligned}
f'(x)
&=(2x)e^x+(x^2+1)e^x \\
&=(x^2+2x+1)e^x \\
&=(x+1)^2e^x.
\end{aligned}
$$

## Verification

The incorrect formula $(2x)e^x$ omits $uv'=(x^2+1)e^x$. Direct substitution at $x=0$ gives $f'(0)=1$, while $(2x)e^x$ incorrectly gives $0$.

## Interpretation

Differentiation of a product accounts for the change in each factor. The derivative of $x^2+1$ times $e^x$ and the first factor times the derivative of $e^x$ must both appear.

## Final answer

$$
f'(x)=(x+1)^2e^x
$$
