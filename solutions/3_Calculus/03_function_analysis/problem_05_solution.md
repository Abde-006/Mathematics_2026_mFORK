# Problem 5. An Exponential Function with a Maximum

## Problem

Analyze $f(x)=xe^{-x}$ and examine $x\to\infty$.

## Solution

Let $f(x)=xe^{-x}$.

### Step 1 - Derivative

The product rule $(uv)'=u'v+uv'$ differentiates $f(x)=xe^{-x}$ and is used here because the function is a product of $u=x$ and $v=e^{-x}$.

$$
f'(x)=e^{-x}-xe^{-x}=(1-x)e^{-x}.
$$

Since $e^{-x}>0$, $f'(x)>0$ for $x<1$ and $f'(x)<0$ for $x>1$. Thus $f$ increases on $(-\infty,1)$ and decreases on $(1,\infty)$.

### Step 2 - Maximum

The sign changes positive to negative at $x=1$, giving

$$
f(1)=e^{-1}=1/e.
$$

Hence $(1,1/e)$ is a global maximum.

### Step 3 - Right-hand limit

$$
\lim_{x\to\infty}xe^{-x}
=\lim_{x\to\infty}\frac{x}{e^x}=0.
$$

Exponential growth dominates linear growth, so $y=0$ is approached from above on the right.

## Final Answer

Increasing on $(-\infty,1)$; decreasing on $(1,\infty)$; global maximum $(1,1/e)$; $\lim_{x\to\infty}f(x)=0$.
