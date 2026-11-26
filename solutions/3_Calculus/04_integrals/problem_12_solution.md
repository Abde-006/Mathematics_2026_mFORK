# Problem 12. Symmetry, Sign, and Absolute Value

## Problem

Compare $\int_{-2}^{2}x dx$ and $\int_{-2}^{2}|x|dx$ using symmetry and sketching.

## Solution

The function $x$ is odd, so equal positive and negative signed regions cancel on $[-2,2]$.

### Signed integral

For odd $g$, $g(-x)=-g(x)$, so positive and negative signed areas cancel: $\int_{-a}^{a}g(x)\,dx=0$. This symmetry condition applies to $g(x)=x$.

$$
\int_{-2}^{2}x dx
=\left[\frac{x^2}{2}\right]_{-2}^{2}
=0.
$$

### Absolute-value integral

Since $|x|$ is even,

$$
\int_{-2}^{2}|x|dx
=2\int_0^2x dx
=2[x^2/2]_0^2
=4.
$$

Geometrically, the $x$ integral consists of two opposite triangles whose areas cancel. The absolute-value integral consists of two positive triangles, each of area $2$, whose total area is $4$.

## Final Answer

$$
\int_{-2}^{2}x dx=0,\qquad
\int_{-2}^{2}|x|dx=4.
$$
