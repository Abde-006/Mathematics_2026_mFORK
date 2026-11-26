# Problem 11. An $n$-th Root

## Problem statement

Compute

$$
\lim_{n\to\infty}\sqrt[n]{5^n+2^n}.
$$

## Named quantities

- $n$ is a positive integer.
- $a_n=5^n+2^n$ is the radicand.
- $L$ is the requested limit.

## Step 1 - Factor out $5^n$

**Factor the dominant exponential.** Factor out the exponential with the largest base. For $C>0$,

$$
\sqrt[n]{C^n}=C.
$$

$$
\begin{aligned}
\sqrt[n]{5^n+2^n}
&=\sqrt[n]{5^n\left(1+\left(\frac25\right)^n\right)} \\
&=5\sqrt[n]{1+\left(\frac25\right)^n}.
\end{aligned}
$$

## Step 2 - Evaluate the correction

Since $0<2/5<1$,

$$
\left(\frac25\right)^n\to0.
$$

Therefore $1+(2/5)^n\to1$, and

$$
L=5\cdot1=5.
$$

## Verification

At $n=10$, $\sqrt[10]{5^{10}+2^{10}}\approx5.000051$. The correction shrinks rapidly as $n$ grows.

## Interpretation

Unlike polynomial quotients, exponential bases determine dominance. Since $5>2$, $5^n$ overwhelms $2^n$, and the $n$-th root returns the larger base.

## Final answer

$$
5
$$
