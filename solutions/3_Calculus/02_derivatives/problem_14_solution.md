# Problem 14. Continuity and Differentiability of a Piecewise Function

## Problem statement

Investigate at $x=0$

$$
f(x)=
\begin{cases}
x^2,&x\ge0, \\
ax,&x<0.
\end{cases}
$$

Determine values of $a$ for continuity and for agreement of one-sided derivatives.

## Named quantities

- $a$ is the slope of the left branch.
- $L^-=f(0^-)$ is the left-hand limit.
- $L^+=f(0^+)$ is the right-hand limit.
- $D^-f(0)$ and $D^+f(0)$ are left and right derivatives.

## Step 1 - Continuity

**Continuity.** The function is continuous at $0$ when

$$
\lim_{x\to0^-}f(x)=\lim_{x\to0^+}f(x)=f(0).
$$

The right-hand limit and function value are

$$
L^+=\lim_{x\to0^+}x^2=0,
\qquad
f(0)=0.
$$

The left-hand limit is

$$
L^-=\lim_{x\to0^-}ax=0
$$

for every real $a$. Therefore the function is continuous for every real $a$.

## Step 2 - Left-hand derivative

**Left one-sided derivative.** The left derivative is $f'_-(0)=\lim_{h\to0^-}(f(h)-f(0))/h$ because $h$ approaches zero only through negative values.

For $h<0$, $f(h)=ah$ and $f(0)=0$. Thus

$$
D^-f(0)=\lim_{h\to0^-}\frac{ah-0}{h}=a.
$$

## Step 3 - Right-hand derivative

**Right one-sided derivative.** The corresponding right-hand test is $f'_+(0)=\lim_{h\to0^+}(f(h)-f(0))/h$, where $h$ approaches zero only through positive values.

For $h>0$, $f(h)=h^2$ and $f(0)=0$. Thus

$$
D^+f(0)=\lim_{h\to0^+}\frac{h^2-0}{h}
=\lim_{h\to0^+}h=0.
$$

## Step 4 - Compare derivatives

The one-sided derivatives exist for every real $a$ and agree only when

$$
a=0.
$$

Therefore the function is differentiable at $0$ exactly for $a=0$.

## Verification

When $a=1$, the function is continuous because both sides approach $(0,0)$, but the left derivative is $1$ and the right derivative is $0$. This shows that continuity alone does not guarantee differentiability.

## Interpretation

At $a=0$, the left and right tangents both become horizontal, forming a smooth common tangent.

## Final answer

Continuous for every real $a$. The one-sided derivatives exist for every real $a$ and agree only at $a=0$. The function is differentiable at $0$ exactly for $a=0$.
