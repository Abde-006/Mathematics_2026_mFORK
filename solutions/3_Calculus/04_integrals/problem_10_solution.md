# Problem 10. Definite Integral and Checking the Result

## Problem

Estimate $\int_0^2(x^2+1)dx$ first using $1\le x^2+1\le5$, then compute exactly.

## Solution

On $[0,2]$, the integrand satisfies $1\le x^2+1\le5$.

The bounds property for integrals says that if $m\le f(x)\le M$ on $[a,b]$, then $m(b-a)\le\int_a^b f(x)\,dx\le M(b-a)$; it converts pointwise bounds into a range for accumulated area.
Therefore

$$
2\le I\le10.
$$

### Exact calculation

$$
\begin{aligned}
I
&=\int_0^2(x^2+1)dx\\
&=\left[\frac{x^3}{3}+x\right]_0^2\\
&=\frac83+2=\frac{14}{3}.
\end{aligned}
$$

Since $2<14/3<10$, the result agrees with the estimate. Such an estimate mainly detects gross errors such as a negative answer or an answer outside the predicted range.

## Final Answer

Estimated range $[2,10]$; exact value $14/3$.
