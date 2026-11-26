# Problem 7. A Trigonometric Composition

## Problem statement

For

$$
f(x)=\sin(x^2+1),
$$

compute $f'(x)$ and determine the sign of $f'(0)$.

## Named quantities

- $u(x)=x^2+1$ is the inner function.
- $g(u)=\sin u$ is the outer function.

## Step 1 - Differentiate the inner function

**Chain rule.**

$$
f'(x)=g'(u(x))u'(x).
$$

Here $d(\sin u)/du=\cos u$.

$$
u'(x)=2x.
$$

## Step 2 - Differentiate the outer function

$$
g'(u)=\cos u.
$$

Substituting $u=x^2+1$ gives

$$
g'(u(x))=\cos(x^2+1).
$$

## Step 3 - Apply the chain rule

$$
f'(x)=\cos(x^2+1)\cdot2x=2x\cos(x^2+1).
$$

## Step 4 - Determine the sign at zero

$$
f'(0)=2(0)\cos(1)=0.
$$

## Verification

For small positive $x$, $2x>0$ and $\cos(x^2+1)$ is close to $\cos1>0$, so $f'(x)>0$ for sufficiently small positive $x$. For small negative $x$, $f'(x)<0$.

## Interpretation

The sign changes from negative to positive through $x=0$, consistent with $f'(0)=0$ and a local minimum of $f$ near $x=0$.

## Final answer

$$
f'(x)=2x\cos(x^2+1),
\qquad
f'(0)=0.
$$
