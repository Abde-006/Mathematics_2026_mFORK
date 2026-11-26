# Problem 13. A Logarithm and an Asymptote

## Problem

Complete the analysis of $f(x)=\ln x/x$ for $x>0$.

## Solution

Let $f(x)=\ln x/x$, with $D_f=(0,\infty)$.

### Derivative

By the quotient rule,

$$
f'(x)=\frac{(1/x)x-\ln x}{x^2}
=\frac{1-\ln x}{x^2}.
$$

Since $x^2>0$, $f'(x)>0$ for $x<e$ and $f'(x)<0$ for $x>e$. Thus $f$ is increasing on $(0,e)$ and decreasing on $(e,\infty)$.

### Maximum

$$
f(e)=\ln e/e=1/e.
$$

### End behavior

$$
\lim_{x\to0^+}\frac{\ln x}{x}=-\infty,
$$

and

$$
\lim_{x\to\infty}\frac{\ln x}{x}=0.
$$

At the left boundary the graph decreases to $-\infty$; at infinity it approaches $y=0$ from above.

## Final Answer

Maximum $(e,1/e)$; increasing on $(0,e)$; decreasing on $(e,\infty)$; end limits $-\infty$ and $0$.
