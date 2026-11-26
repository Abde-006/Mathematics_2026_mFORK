# Problem 13. Fundamental Trigonometric Limit

## Problem statement

Using

$$
\lim_{x\to0}\frac{\sin x}{x}=1,
$$

compute

$$
\lim_{x\to0}\frac{\sin5x}{x},
\qquad
\lim_{x\to0}\frac{\sin2x}{\sin3x}.
$$

## Named quantities

- $L_1$ is the first limit.
- $L_2$ is the second limit.
- $u=5x$, $v=2x$, and $w=3x$ are the arguments used in substitutions.

## Step 1 - First limit

**Fundamental trigonometric limit.**

$$
\lim_{t\to0}\frac{\sin t}{t}=1.
$$

Insert $5$ into both numerator and denominator:

$$
\frac{\sin5x}{x}
=5\frac{\sin5x}{5x}.
$$

As $x\to0$, $5x\to0$, so

$$
L_1=5\cdot1=5.
$$

## Step 2 - Second limit

Write both sine functions relative to their arguments:

$$
\begin{aligned}
\frac{\sin2x}{\sin3x}
&=\frac{\sin2x}{2x}
  \cdot\frac{3x}{\sin3x}
  \cdot\frac23.
\end{aligned}
$$

As $x\to0$, $(\sin2x)/(2x)\to1$ and $(\sin3x)/(3x)\to1$. Therefore

$$
L_2=1\cdot1\cdot\frac23=\frac23.
$$

## Verification

At $x=0.01$, $\sin(0.05)/0.01\approx4.9979$, close to $5$. Also, $\sin(0.02)/\sin(0.03)\approx0.66653$, close to $2/3$.

## Interpretation

For small angles in radians, $\sin t$ is approximately $t$. Thus $\sin5x$ behaves like $5x$, and $\sin2x/\sin3x$ behaves like $2x/(3x)=2/3$.

## Final answers

$$
5,\qquad\frac23
$$
