# Problem 12. A Function with an Absolute Value

## Problem

Analyze $f(x)=|x^2-4|$, show the effect of the absolute value, and identify points where $f'$ does not exist.

## Solution

Let $g(x)=x^2-4$. The absolute value reflects the negative part of $g$, for $-2<x<2$, above the $x$-axis.

### Piecewise form

$$
f(x)=
\begin{cases}
x^2-4,&|x|\ge2,\\
4-x^2,&|x|<2.
\end{cases}
$$

For $|x|>2$, $f'(x)=2x$. For $|x|<2$, $f'(x)=-2x$. Thus $f$ decreases on $(-\infty,-2)$ and $(0,2)$, and increases on $(-2,0)$ and $(2,\infty)$.

### Nonsmooth points

At $x=-2$, the left-hand derivative of $x^2-4$ is $2x=-4$, and the right-hand derivative of $4-x^2$ is $-2x=4$. At $x=2$, the left-hand derivative is $-4$ and the right-hand derivative is $4$. The one-sided slopes differ, so $f'$ does not exist at $x=-2$ or $x=2$.

Both are minima with value $0$, and $(0,4)$ is a maximum.

## Final Answer

Minima $(\pm2,0)$; maximum $(0,4)$; derivative does not exist at $x=\pm2$ because corners are formed by opposite one-sided slopes.
