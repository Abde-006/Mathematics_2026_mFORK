# Problem 9. An Oblique Asymptote

## Problem

Analyze the asymptotes of $f(x)= (x^2+1)/(x-1)$ using polynomial division.

## Solution

Let $f(x)=(x^2+1)/(x-1)$.

### Polynomial division

$$
x^2+1=(x-1)(x+1)+2,
$$

so

$$
f(x)=x+1+\frac2{x-1}.
$$

### Asymptotes

The remainder term tends to zero as $|x|\to\infty$, so $y=x+1$ is oblique. At $x=1$, the original denominator vanishes and the numerator is $2$, so

$$
\lim_{x\to1^-}f(x)=-\infty,\qquad
\lim_{x\to1^+}f(x)=\infty.
$$

Thus $x=1$ is vertical.

### Verification

For $x=3$, $f(3)=5$ and $x+1=4$, with difference $1=2/(3-1)$. The difference exactly equals the remainder term and tends to zero for large $|x|$.

## Final Answer

Vertical asymptote $x=1$; oblique asymptote $y=x+1$.
