# Problem 14. A Piecewise-Defined Function

## Problem

Given the piecewise function $f(x)=x+1$ on $[-1,1)$ and $f(x)=2$ on $[1,3]$, sketch it and compute $\int_{-1}^{3}f(x)dx$.

## Solution

The definition changes at $x=1$, so the integral must split there.

### Step 1 - First interval

The additivity property $\int_a^c f=\int_a^b f+\int_b^c f$ is used because $a=-1$, $b=1$, and $c=3$ place the piecewise switch inside the interval.

$$
\begin{aligned}
\int_{-1}^{1}(x+1)dx
&=\left[\frac{x^2}{2}+x\right]_{-1}^{1}\\
&=\left(\frac12+1\right)-\left(\frac12-1\right)=2.
\end{aligned}
$$

### Step 2 - Second interval

$$
\int_1^32dx=[2x]_1^3=6-2=4.
$$

### Step 3 - Add

$$
\int_{-1}^{3}f(x)dx=2+4=6.
$$

Geometrically, the first interval is a trapezoid of area $2$, and the second is a rectangle of area $4$. The isolated value at $x=1$ does not affect the integral.

## Final Answer

$$
\int_{-1}^{3}f(x)dx=6.
$$
