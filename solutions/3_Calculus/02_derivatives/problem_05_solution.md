# Problem 5. The Chain Rule as Working Through Layers

## Problem statement

For

$$
f(x)=(3x^2-2x+1)^5,
$$

identify the inner and outer functions and compute $f'(x)$.

## Named quantities

- $u(x)=3x^2-2x+1$ is the inner function.
- $g(u)=u^5$ is the outer function.

## Step 1 - Differentiate the outer function

**Chain rule.** If $f(x)=g(u(x))$, then

$$
f'(x)=g'(u(x))u'(x).
$$

The factor $u'(x)$ accounts for change in the inner layer.

With $g(u)=u^5$,

$$
g'(u)=5u^4.
$$

Substituting $u=3x^2-2x+1$ gives

$$
5(3x^2-2x+1)^4.
$$

## Step 2 - Differentiate the inner function

$$
u'(x)=6x-2.
$$

## Step 3 - Combine the layers

$$
f'(x)=5(3x^2-2x+1)^4(6x-2).
$$

## Verification

At $x=0$, $u(0)=1$ and $u'(0)=-2$, so $f'(0)=5(1)^4(-2)=-10$. This follows from direct layer-by-layer differentiation.

## Interpretation

The factor $6x-2$ appears because the inner expression changes with $x$. Without it, the derivative would describe only change of the outer power.

## Final answer

$$
f'(x)=5(3x^2-2x+1)^4(6x-2)
$$
