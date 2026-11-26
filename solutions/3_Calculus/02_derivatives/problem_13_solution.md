# Problem 13. A Multi-Layer Composition

## Problem statement

For

$$
f(x)=e^{\sin(x^2)},
$$

identify all layers and compute $f'(x)$.

## Named quantities

- $u_1=x^2$ is the innermost expression.
- $u_2=\sin(x^2)$ is the middle expression.
- $u_3=e^{\sin(x^2)}$ is the outer result.

## Step 1 - Write the layers

**Chain rule through three layers.** Differentiate in reverse order of composition:

$$
\frac d{dx}e^{u}=e^u\frac{du}{dx},
\qquad
\frac d{dx}\sin v=\cos v\frac{dv}{dx}.
$$

$$
x\longrightarrow x^2\longrightarrow\sin(x^2)\longrightarrow e^{\sin(x^2)}.
$$

Differentiation moves backward:

$$
e^{\sin(x^2)}\longrightarrow\sin(x^2)\longrightarrow x^2\longrightarrow x.
$$

## Step 2 - Differentiate each layer

Starting from the outer exponential,

$$
\frac d{dx}e^{\sin(x^2)}
=e^{\sin(x^2)}\cos(x^2)\frac d{dx}(x^2).
$$

Then

$$
\frac d{dx}(x^2)=2x.
$$

Therefore

$$
f'(x)=e^{\sin(x^2)}\cos(x^2)(2x).
$$

## Step 3 - Simplify

$$
f'(x)=2x e^{\sin(x^2)}\cos(x^2).
$$

## Verification

At $x=0$, $f'(0)=2(0)e^{0}\cos0=0$. The derivative factor is also $0$, matching the chain rule.

## Interpretation

Differentiation moves in reverse order because each outer layer is waiting for the derivative of the inner layer on which it depends.

## Final answer

$$
f'(x)=2x e^{\sin(x^2)}\cos(x^2)
$$
