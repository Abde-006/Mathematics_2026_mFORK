# Problem 7. Integration by Parts as the Product Rule

## Problem

Compute $\int xe^x dx$, derive the technique from the product rule, and verify.

## Solution

The product rule

$$
(uv)'=u'v+uv'
$$

rearranges and integrates to

$$
\int u\,dv=uv-\int v\,du.
$$

Choose $u=x$ and $dv=e^x dx$, because differentiation simplifies $x$ and integration of $e^x$ is easy.

### Step 1

$$
du=dx,\qquad v=e^x.
$$

### Step 2

$$
\int xe^x dx
=xe^x-\int e^x dx
=xe^x-e^x+C
=(x-1)e^x+C.
$$

### Verification

$$
\frac d{dx}[(x-1)e^x]=(x-1)e^x+e^x=xe^x.
$$

## Final Answer

$$
(x-1)e^x+C.
$$
