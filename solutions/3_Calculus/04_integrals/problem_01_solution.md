# Problem 1. Antiderivative and Verification

## Problem

For $f(x)=3x^2-4x+5$, find one antiderivative $F(x)$ and the entire family, verify, and explain $C$.

## Solution

Let $f(x)=3x^2-4x+5$. Integration is the inverse of differentiation.

### Step 1 - Integrate term by term

The power rule $\int x^n\,dx=\frac{x^{n+1}}{n+1}+C$, for $n\neq-1$, reverses differentiation. It applies to $3x^2$, $-4x$, and $5$ because their exponents are $2$, $1$, and $0$.

$$
F(x)=x^3-2x^2+5x.
$$

### Step 2 - Entire family

$$
F(x)=x^3-2x^2+5x+C,\qquad C\in\mathbb R.
$$

### Verification

$$
F'(x)=3x^2-4x+5=f(x).
$$

$C$ represents all vertical translations of the same antiderivative, since constants differentiate to zero.

## Final Answer

One antiderivative is $x^3-2x^2+5x$; the family is $x^3-2x^2+5x+C$.
