# Problem 8. Choosing Factors in Integration by Parts

## Problem

Compute $\int x\cos x dx$ and justify the choice of factors.

## Solution

Integration by parts is

$$
\int u\,dv=uv-\int v\,du.
$$

Choose

$$
u=x,\qquad dv=\cos x dx.
$$

This is convenient because $du=dx$ simplifies the polynomial factor and $v=\sin x$ is immediate. Reversing the roles would introduce $x^2/2$ and $-\sin x$, making the remaining product no simpler.

### Computation

$$
du=dx,\qquad v=\sin x,
$$

$$
\int x\cos x dx
=x\sin x-\int\sin x dx
=x\sin x+\cos x+C.
$$

### Verification

$$
\frac d{dx}(x\sin x+\cos x)
=\sin x+x\cos x-\sin x
=x\cos x.
$$

## Final Answer

$$
x\sin x+\cos x+C.
$$
