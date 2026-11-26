# Problem 15. Find the Error in the Monotonicity Analysis

## Problem

Diagnose the reversed sign reasoning for $f(x)=x^3-3x$, construct the correct sign chart, and verify with test points.

## Solution

Let $f'(x)=3(x-1)(x+1)$.

### 1. Error

Finding the zeros $-1$ and $1$ does not itself give their signs. The product $(x-1)(x+1)$ is positive outside the roots and negative between them. The student's statement reverses this pattern.

### 2. Correct sign chart

$$
\begin{aligned}
x<-1 &: f'(x)>0,\\
-1<x<1 &: f'(x)<0,\\
x>1 &: f'(x)>0.
\end{aligned}
$$

### 3. Monotonicity and extrema

$f$ is increasing on $(-\infty,-1)\cup(1,\infty)$ and decreasing on $(-1,1)$.

$$
f(-1)=2,\qquad f(1)=-2.
$$

The sign changes positive to negative at $-1$, giving local maximum $(-1,2)$; it changes negative to positive at $1$, giving local minimum $(1,-2)$.

### 4. Test points

Choose $-2,0,2$:

$$
f'(-2)=9>0,\qquad
f'(0)=-3<0,\qquad
f'(2)=9>0.
$$

These signs confirm the classification.

## Final Answer

Maximum $(-1,2)$ and minimum $(1,-2)$; increasing outside $(-1,1)$ and decreasing on $(-1,1)$.
