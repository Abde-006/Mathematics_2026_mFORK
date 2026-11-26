# Problem 5. The Classical Limit Leading to the Number $e$

## Problem statement

Compute

$$
\lim_{n\to\infty}\left(1+\frac1n\right)^n.
$$

## Named quantities

- $a_n=(1+1/n)^n$ is the sequence.
- $e$ is the limit.

## Step 1 - Numerical observation

**Classical exponential limit.**

$$
e=\lim_{n\to\infty}\left(1+\frac1n\right)^n.
$$

Numerical values provide evidence only; this named limit supplies the analytical result.

Selected values are

$$
\begin{aligned}
a_1&=2, \\
a_{10}&=2.59374246, \\
a_{100}&=2.704813829, \\
a_{1000}&=2.716923932.
\end{aligned}
$$

The sequence appears to approach $2.71828$.

## Step 2 - Identify the limit

The classical limit gives

$$
\lim_{n\to\infty}\left(1+\frac1n\right)^n
=e\approx2.718281828.
$$

## Verification

At $n=10000$,

$$
\left(1+\frac1{10000}\right)^{10000}\approx2.718145927,
$$

which is consistent with convergence to $e$.

## Interpretation

A finite table cannot prove convergence. It motivates the conjecture that the sequence approaches $e$, while the limit formula identifies the value.

## Final answer

$$
e
$$
