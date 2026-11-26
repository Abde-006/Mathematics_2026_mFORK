# Problem 4. A Function with Two Vertical Asymptotes

## Problem

Analyze $f(x)=1/(x^2-1)$: domain, asymptotes, sign, and monotonicity on each interval.

## Solution

Let $f(x)=1/(x^2-1)=1/((x-1)(x+1)).

### Domain and asymptotes

The denominator is zero at $x=-1$ and $x=1$, so

$$
D_f=(-\infty,-1)\cup(-1,1)\cup(1,\infty).
$$

Both excluded points are vertical asymptotes. Since $x^2-1\to\infty$ as $|x|\to\infty$, $y=0$ is horizontal.

### Sign

$x^2-1>0$ outside $[-1,1]$ and $x^2-1<0$ inside $(-1,1)$. Since the numerator is positive, $f(x)>0$ on $(-\infty,-1)\cup(1,\infty)$ and $f(x)<0$ on $(-1,1)$. There is no zero.

### Monotonicity

$$
f'(x)=\frac{-2x}{(x^2-1)^2}.
$$

The denominator is positive on $D_f$, so $f'(x)>0$ for $x<0$ and $f'(x)<0$ for $x>0$. Accounting for the gaps:

$$
\begin{aligned}
&(-\infty,-1):&&\mathrm{increasing},\\
&(-1,0):&&\mathrm{increasing},\\
&(0,1):&&\mathrm{decreasing},\\
&(1,\infty):&&\mathrm{decreasing}.
\end{aligned}
$$

The sign change at $x=0$ gives the local maximum $(0,-1)$. Each interval must be considered separately because the function is undefined at $-1$ and $1$.

## Final Answer

Vertical asymptotes $x=-1,1$; horizontal asymptote $y=0$; positive outside $(-1,1)$ and negative inside; increasing on $(-\infty,-1)$ and $(-1,0)$; decreasing on $(0,1)$ and $(1,\infty)$; maximum $(0,-1)$.
