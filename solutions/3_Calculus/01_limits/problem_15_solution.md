# Problem 15. Observation Versus Proof

## Problem statement

Choose one sequence and one function from this set. Observe them numerically and compare those observations with analytical results. Explain why finite calculations or a sketch do not prove a limit.

## Named quantities

- $a_n=(4n^2-3n+1)/(2n^2+5n-7)$ is the chosen sequence.
- $g(x)=(x^2-4x+3)/(x-3)$ is the chosen function.
- $L_a$ and $L_g$ are their limits.

## Step 1 - Observe the sequence

**Sequence and function observation.** Examine increasingly large $n$ for a sequence and arguments from the left and right for a function. Numerical evidence can suggest a limit, but it does not replace an exact argument.

| $n$ | $a_n$ |
|---:|---:|
| $10$ | $1.7274$ |
| $100$ | $1.9370$ |
| $1000$ | $1.9937$ |

After division by $n^2$,

$$
a_n=\frac{4-3/n+1/n^2}{2+5/n-7/n^2}\to\frac42=2.
$$

Thus $L_a=2$.

## Step 2 - Observe the function

| $x$ | $g(x)$ | side |
|---:|---:|---|
| $2.99$ | $1.99$ | left |
| $2.999$ | $1.999$ | left |
| $3.001$ | $2.001$ | right |
| $3.01$ | $2.01$ | right |

For $x\neq3$, factorization gives

$$
g(x)=\frac{(x-1)(x-3)}{x-3}=x-1.
$$

Therefore

$$
L_g=\lim_{x\to3}(x-1)=2.
$$

## Sketch interpretation

The sequence terms approach the horizontal level $y=2$. The graph of $g$ is the line $y=x-1$ with a hole at $(3,2)$, approached from both sides.

## Verification

The sequence argument is exact because division identifies every remaining term that tends to zero. The function argument is exact because cancellation is valid for $x\neq3$.

## Observation versus proof

Finite rows and sketches provide evidence and suggest a candidate. They cannot exclude later sequence terms or further nearby function arguments. The exact algebra proves convergence for all relevant terms or arguments.

## Final answer

The sequence limit is $2$, and the function limit is $2$. Finite observations are consistent with these conclusions but do not constitute proofs.
