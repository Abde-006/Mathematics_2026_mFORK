# Problem 1. Dominant Terms in a Sequence

## Problem statement

Compute

$$
\lim_{n\to\infty}\frac{4n^2-3n+1}{2n^2+5n-7}.
$$

## Named quantities

- $n$ is a positive integer.
- $L$ is the requested limit.

## Step 1 - Divide out $n^2$

**Division by the dominant power.** Divide every term in the numerator and denominator by the highest power of $n$ in the denominator. This makes lower-degree terms tend to zero.

The numerator and denominator both have degree $2$, so

$$
\begin{aligned}
\frac{4n^2-3n+1}{2n^2+5n-7}
&=\frac{\frac{4n^2}{n^2}-\frac{3n}{n^2}+\frac1{n^2}}
        {\frac{2n^2}{n^2}+\frac{5n}{n^2}-\frac7{n^2}} \\
&=\frac{4-\frac3n+\frac1{n^2}}
        {2+\frac5n-\frac7{n^2}}.
\end{aligned}
$$

## Step 2 - Take the limit

As $n\to\infty$, $1/n\to0$ and $1/n^2\to0$. Therefore

$$
L=\frac{4-0+0}{2+0-0}=2.
$$

## Verification

At $n=100$,

$$
\frac{40000-300+1}{20000+500-7}\approx1.9370,
$$

and at $n=1000$ the quotient is approximately $1.9937$. These values approach $2$.

## Interpretation

For large $n$, terms of degree $2$ determine both growth rates; lower-degree terms become negligible relative to $n^2$.

## Final answer

$$
2
$$
