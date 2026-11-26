# Problem 6. Average Value of a Function

Compute the average value of $f(x)=x^2$ on $[0,3]$, find $c\in[0,3]$ with $f(c)$ equal to that average, and interpret the result.

## Quantities

Let $f(x)=x^2$, $a=0$, $b=3$, $f_{\mathrm{avg}}$ the average value, and $c$ a point whose function value is $f_{\mathrm{avg}}$.

## Step 1 - Compute the average value

The average value of an integrable function $f$ on $[a,b]$ is its integral divided by the interval length:

$$
f_{\mathrm{avg}}=\frac1{b-a}\int_a^b f(x)\,dx.
$$

This tests what constant height would produce the same signed area over $[a,b]$. Substituting $f(x)=x^2$, $a=0$, and $b=3$,

$$
\begin{aligned}
\int_0^3x^2\,dx
&=\left[\frac{x^3}{3}\right]_0^3 \\
&=\frac{27}{3}-0 \\
&=9.
\end{aligned}
$$

The interval length is $b-a=3$, so

$$
f_{\mathrm{avg}}=\frac93=3.
$$

## Step 2 - Find $c$

For $f(c)$ to equal the average, solve $c^2=3$:

$$
c=\pm\sqrt3.
$$

Only $c=\sqrt3$ belongs to $[0,3]$.

## Verification

Direct substitution gives

$$
f(\sqrt3)=(\sqrt3)^2=3,
$$

which confirms the Mean Value Theorem for Integrals result.

## Geometric interpretation

The area under $y=x^2$ is $9$, and a rectangle of width $3$ and height $3$ has area

$$
3\cdot3=9.
$$

Thus $y=3$ is the constant height having the same area. At $x=\sqrt3$, the graph reaches that height.

## Final answer

The average value is $3$, attained in the interval at $c=\sqrt3$.
