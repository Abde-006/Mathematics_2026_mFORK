# Problem 9. One-Sided Limits and an Asymptote

## Problem statement

For

$$
f(x)=\frac1{x-2},
$$

analyze the left-hand and right-hand limits as $x\to2$, determine whether the two-sided limit exists, and identify the vertical asymptote.

## Named quantities

- $d=x-2$ is the signed distance from $2$.
- $L^-$ is the left-hand limit.
- $L^+$ is the right-hand limit.

## Step 1 - Left-hand limit

**One-sided sign rule.** As $x\to2^-$, $d<0$ and $d\to0$, so $1/d\to-\infty$. As $x\to2^+$, $d>0$ and $d\to0$, so $1/d\to+\infty$.

For $x<2$ sufficiently close to $2$, $x-2$ is negative with magnitude approaching zero:

$$
L^-=\lim_{x\to2^-}\frac1{x-2}=-\infty.
$$

## Step 2 - Right-hand limit

For $x>2$, $x-2$ is positive and approaches zero:

$$
L^+=\lim_{x\to2^+}\frac1{x-2}=+\infty.
$$

## Step 3 - Compare the one-sided limits

Because $L^-\neq L^+$, the two-sided limit does not exist.

## Verification

At $x=1.999$, $f(x)=1/(-0.001)=-1000$. At $x=2.001$, $f(x)=1/0.001=1000$. The signs confirm the upward and downward behavior.

## Interpretation

The line $x=2$ is a vertical asymptote. The left branch decreases without bound, while the right branch increases without bound.

## Final answer

$$
\lim_{x\to2^-}f(x)=-\infty,
\qquad
\lim_{x\to2^+}f(x)=+\infty.
$$

The two-sided limit does not exist, and the vertical asymptote is $x=2$.
