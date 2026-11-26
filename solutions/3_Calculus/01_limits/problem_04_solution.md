# Problem 4. Powers and Oscillation

## Problem statement

Analyze

$$
\left(\frac23\right)^n,\qquad
\left(\frac32\right)^n,\qquad
(-1)^n,\qquad
\frac{(-1)^n}{n}.
$$

## Named quantities

- $r$ is the base of a geometric sequence $r^n$.
- $a_n$ denotes a term of a generic sequence.

## Step 1 - Positive bases

**Geometric sequence behavior.** For $r^n$:

- $|r|<1$ gives limit $0$;
- $r>1$ gives limit $+\infty$;
- $r=-1$ gives alternation between $-1$ and $1$.

Since $|2/3|<1$,

$$
\left(\frac23\right)^n\to0.
$$

Since $3/2>1$,

$$
\left(\frac32\right)^n\to+\infty.
$$

## Step 2 - Alternating sequences

The sequence $(-1)^n$ is $1,-1,1,-1,\ldots$. Even terms have limit $1$ and odd terms have limit $-1$, so the sequence has no limit.

For $(-1)^n/n$, the squeeze bounds are

$$
-\frac1n\le\frac{(-1)^n}{n}\le\frac1n.
$$

Both bounds tend to $0$, hence

$$
\frac{(-1)^n}{n}\to0.
$$

## Verification

The terms $(-1)^n/n$ begin $-1,1/2,-1/3,1/4,\ldots$, and their absolute values $1/n$ tend to zero.

## Interpretation

Oscillation does not always prevent convergence. Alternating signs accompanied by decreasing magnitude can still give limit $0$.

## Final answer

- $\left(\frac23\right)^n\to0$.
- $\left(\frac32\right)^n\to+\infty$.
- $(-1)^n$ has no limit.
- $\frac{(-1)^n}{n}\to0$.
