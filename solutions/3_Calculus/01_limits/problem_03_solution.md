# Problem 3. A Square Root and Removing an Indeterminate Form

## Problem statement

Compute

$$
\lim_{n\to\infty}\left(\sqrt{n^2+5n}-n\right).
$$

## Named quantities

- $n$ is a positive integer.
- $L$ is the requested limit.

## Step 1 - Conjugate

**Conjugate identity.**

$$
(\sqrt a-\sqrt b)(\sqrt a+\sqrt b)=a-b.
$$

Multiplication by $(\sqrt a+\sqrt b)/(\sqrt a+\sqrt b)$ can remove an apparent $\infty-\infty$ form.

Because $n>0$, $\sqrt{n^2}=n$. Thus

$$
\begin{aligned}
\sqrt{n^2+5n}-n
&=\frac{(\sqrt{n^2+5n}-n)(\sqrt{n^2+5n}+n)}
        {\sqrt{n^2+5n}+n} \\
&=\frac{n^2+5n-n^2}{\sqrt{n^2+5n}+n} \\
&=\frac{5n}{\sqrt{n^2+5n}+n}.
\end{aligned}
$$

## Step 2 - Divide by $n$

For $n>0$,

$$
\frac{5n}{\sqrt{n^2+5n}+n}
=\frac5{\sqrt{1+5/n}+1}.
$$

As $n\to\infty$, $5/n\to0$, so

$$
L=\frac5{\sqrt1+1}=\frac52.
$$

## Verification

At $n=100$, $\sqrt{10500}-100\approx2.4695$, and at $n=1000$ it is approximately $2.4969$. Both approach $2.5$.

## Interpretation

The conjugate reveals the difference $5n$ explicitly. The numerator grows like $5n$, while the denominator grows like $2n$, giving $5/2$.

## Final answer

$$
\frac52
$$
