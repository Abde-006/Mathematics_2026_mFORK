# Problem 14. Reconstructing Information from the Derivative

## Problem

Given $f'(x)=(x-1)(x+2)$, determine monotonicity and extrema, then verify $g(x)=x^3/3+x^2/2-2x$.

## Solution

Suppose

$$
f'(x)=(x-1)(x+2).
$$

### Sign chart

The derivative zeros are $-2$ and $1$. The quadratic opens upward:

$$
\begin{aligned}
x<-2 &: f'(x)>0,\\
-2<x<1 &: f'(x)<0,\\
x>1 &: f'(x)>0.
\end{aligned}
$$

Thus $f$ increases on $(-\infty,-2)$, decreases on $(-2,1)$, and increases on $(1,\infty)$. There is a local maximum at $x=-2$ and a local minimum at $x=1$. $f'$ does not determine a vertical shift.

### Verification with $g$

$$
g'(x)=x^2+x-2=(x-1)(x+2),
$$

so $g$ has the same qualitative derivative behavior. Its values are

$$
g(-2)=10/3,\qquad g(1)=-7/6.
$$

Therefore its specific maximum and minimum are $(-2,10/3)$ and $(1,-7/6)$.

## Final Answer

Increasing on $(-\infty,-2)$ and $(1,\infty)$; decreasing on $(-2,1)$; maximum position $x=-2$; minimum position $x=1$.
