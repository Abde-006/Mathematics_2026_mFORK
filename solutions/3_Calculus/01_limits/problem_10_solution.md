# Problem 10. Continuity of a Piecewise Function

## Problem statement

Find $a$ so that

$$
f(x)=
\begin{cases}
ax+1,&x<2, \\
x^2-1,&x\ge2
\end{cases}
$$

is continuous at $x=2$.

## Named quantities

- $a$ is the unknown slope of the left branch.
- $L^-$ is the left-hand limit.
- $L^+$ is the right-hand limit.
- $f(2)$ is the function value.

## Step 1 - Compute $L^-$

**Continuity test.** A function is continuous at $x=c$ when

$$
\lim_{x\to c^-}f(x)
=\lim_{x\to c^+}f(x)
=f(c).
$$

For $x<2$, $f(x)=ax+1$, so

$$
L^-=\lim_{x\to2^-}(ax+1)=2a+1.
$$

## Step 2 - Compute $L^+$ and $f(2)$

For $x\ge2$, $f(x)=x^2-1$, so

$$
L^+=\lim_{x\to2^+}(x^2-1)=4-1=3
$$

and

$$
f(2)=2^2-1=3.
$$

## Step 3 - Match the quantities

Continuity requires

$$
2a+1=3.
$$

Subtracting $1$ and dividing by $2$ gives

$$
a=1.
$$

## Verification

With $a=1$,

$$
L^-=2(1)+1=3=L^+=f(2).
$$

## Interpretation

The left and right branches meet at $(2,3)$, so the graph has no jump at $x=2$.

## Final answer

$$
a=1
$$
