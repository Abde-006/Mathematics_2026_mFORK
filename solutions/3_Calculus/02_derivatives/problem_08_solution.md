# Problem 8. Two Exponential Functions

## Problem statement

For

$$
f(x)=e^{2x-3}+5^x,
$$

compute $f'(x)$ and explain both additional factors.

## Named quantities

- $u=2x-3$ is the exponent of the natural exponential.
- $a=5$ is the base of the exponential $a^x$.

## Step 1 - Differentiate $e^{2x-3}$

**Natural-exponential chain rule.** The formula $d(e^u)/dx=e^u(du/dx)$ applies because $e^u$ is composed with the linear exponent $u=2x-3$.

The inner exponent has derivative

$$
\frac d{dx}(2x-3)=2.
$$

Therefore

$$
\frac d{dx}(e^{2x-3})=2e^{2x-3}.
$$

## Step 2 - Differentiate $5^x$

**General exponential rule.** For a constant base $a>0$, $d(a^x)/dx=a^x\ln a$; the logarithmic factor appears because $a^x=e^{x\ln a}$.

Using $a=5$,

$$
\frac d{dx}(5^x)=5^x\ln5.
$$

## Step 3 - Add the derivatives

$$
f'(x)=2e^{2x-3}+5^x\ln5.
$$

## Verification

At $x=0$, $f'(0)=2e^{-3}+\ln5\approx0.0996+1.6094=1.7090$. Direct application of the two formulas gives the same result.

## Interpretation

The factor $2$ comes from the chain rule in $e^{2x-3}$. The factor $\ln5$ comes from the general exponential formula $d(a^x)/dx=a^x\ln a$.

## Final answer

$$
f'(x)=2e^{2x-3}+5^x\ln5
$$
