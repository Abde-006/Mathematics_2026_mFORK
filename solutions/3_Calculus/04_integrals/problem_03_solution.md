# Problem 3. Recognizing Basic Antiderivatives

## Problem

Compute $\int(2e^x+3\cos x-4\sin x)dx$ and verify.

## Solution

Use the basic derivative facts

$$
(e^x)'=e^x,\qquad (\sin x)'=\cos x,\qquad (\cos x)'=-\sin x.
$$

Therefore

$$
\begin{aligned}
\int2e^x dx&=2e^x,\\
\int3\cos x dx&=3\sin x,\\
\int-4\sin x dx&=4\cos x.
\end{aligned}
$$

Combining gives

$$
F(x)=2e^x+3\sin x+4\cos x+C.
$$

### Verification

$$
F'(x)=2e^x+3\cos x-4\sin x,
$$

which equals the integrand.

## Final Answer

$$
2e^x+3\sin x+4\cos x+C.
$$
