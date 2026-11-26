# Problem 6. Product Rule and Trigonometry

## Problem statement

For

$$
f(x)=x\sin x+\cos x,
$$

compute $f'(x)$, simplify, and evaluate $f'(0)$.

## Named quantities

- $u=x$ and $v=\sin x$ are the factors in $x\sin x$.
- $m_0=f'(0)$ is the tangent slope at $x=0$.

## Step 1 - Differentiate the product

**Product rule.**

$$
(uv)'=u'v+uv'.
$$

**Trigonometric derivatives.**

$$
\frac d{dx}(\sin x)=\cos x.
$$

$$
\frac d{dx}(x\sin x)
=(1)\sin x+x\cos x.
$$

## Step 2 - Include the cosine term

**Trigonometric derivative reminder.** The remaining term uses $d(\cos x)/dx=-\sin x$, the rule introduced for differentiating cosine.

$$
\begin{aligned}
f'(x)
&=\sin x+x\cos x-\sin x \\
&=x\cos x.
\end{aligned}
$$

## Step 3 - Evaluate at $x=0$

$$
m_0=f'(0)=0\cdot\cos0=0.
$$

## Verification

At $x=0$, $f(0)=0+\cos0=1$. For small negative $x$, $x\cos x<0$, and for small positive $x$, $x\cos x>0$, which confirms the transition of the function's slope through $0$.

## Interpretation

The tangent at $x=0$ is horizontal because the tangent slope is $0$.

## Final answer

$$
f'(x)=x\cos x,\qquad f'(0)=0.
$$
