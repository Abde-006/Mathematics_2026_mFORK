# Problem 2. Different Growth Rates

## Problem statement

Compute

$$
\lim_{n\to\infty}\frac{3n+1}{n^2+4},
\qquad
\lim_{n\to\infty}\frac{2n^3-n}{5n^2+1}.
$$

## Named quantities

- $L_1$ is the first limit.
- $L_2$ is the second limit.

## Step 1 - First sequence

**Degree comparison.** For rational sequences:

- denominator degree higher gives $0$;
- numerator degree higher gives unbounded magnitude;
- equal degrees give the ratio of leading coefficients.

Divide numerator and denominator by $n^2$:

$$
\frac{3n+1}{n^2+4}
=\frac{\frac3n+\frac1{n^2}}
       {1+\frac4{n^2}}.
$$

Every fraction in the numerator tends to zero, while the denominator tends to $1$. Thus

$$
L_1=0.
$$

## Step 2 - Second sequence

Divide numerator and denominator by $n^2$:

$$
\frac{2n^3-n}{5n^2+1}
=\frac{2n-\frac1n}{5+\frac1{n^2}}.
$$

The numerator grows like $2n$, while the denominator approaches $5$. Hence

$$
L_2=+\infty.
$$

## Verification

At $n=100$, the first quotient is approximately $0.0297$, and the second is $(2000000-100)/(50000+1)>39$, consistent with $2n/5$ growth.

## Interpretation

The denominator grows faster in the first case. The numerator grows faster in the second case.

## Final answers

$$
0,\qquad+\infty
$$
