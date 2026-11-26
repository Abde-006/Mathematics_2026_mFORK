# Problem 11. A Parameter and the Number of Extrema

## Problem

For $f_a(x)=x^3-3ax$, determine critical points and extrema for each real parameter $a$.

## Solution

Let $f_a(x)=x^3-3ax$, with $a$ fixed.

### Critical points

$$
f_a'(x)=3x^2-3a=3(x^2-a).
$$

- If $a<0$, $x^2=a$ has no real solution.
- If $a=0$, $x=0$ is the only critical point.
- If $a>0$, critical points are $x=\pm\sqrt a$.

### Character

For $a>0$,

$$
f_a'(x)=3(x+\sqrt a)(x-\sqrt a).
$$

The derivative is positive outside $[-\sqrt a,\sqrt a]$ and negative inside. Hence $-\sqrt a$ is a local maximum and $\sqrt a$ is a local minimum:

$$
f_a(-\sqrt a)=2a\sqrt a,\qquad
f_a(\sqrt a)=-2a\sqrt a.
$$

For $a=0$, $f_0(x)=x^3$, which is strictly increasing and has no extremum. For $a<0$, $f_a'(x)>0$ everywhere, so again there is no extremum.

## Final Answer

$a<0$: no critical points or extrema. $a=0$: stationary point $x=0$, no extremum. $a>0$: maximum $(-\sqrt a,2a\sqrt a)$ and minimum $(\sqrt a,-2a\sqrt a)$.
