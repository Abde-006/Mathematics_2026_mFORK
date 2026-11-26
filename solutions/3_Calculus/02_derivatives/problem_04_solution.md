# Problem 4. A Quotient and Domain Control

## Problem statement

For

$$
f(x)=\frac{x^2+1}{x-1},
$$

determine the domain and simplify $f'(x)$.

## Named quantities

- $u=x^2+1$ is the numerator.
- $v=x-1$ is the denominator.
- $D_f$ is the domain.

## Step 1 - Determine the domain

The denominator $x-1$ vanishes at $x=1$, so

$$
D_f=\mathbb R\setminus\{1\}.
$$

## Step 2 - Differentiate

**Quotient rule.** If $f=u/v$, then $f'=(u'v-uv')/v^2$ because the numerator and denominator both change. It applies here because $f$ is explicitly a quotient of differentiable expressions.

Here $u'=2x$ and $v'=1$. Therefore

$$
\begin{aligned}
f'(x)
&=\frac{(2x)(x-1)-(x^2+1)(1)}{(x-1)^2} \\
&=\frac{2x^2-2x-x^2-1}{(x-1)^2} \\
&=\frac{x^2-2x-1}{(x-1)^2}.
\end{aligned}
$$

## Step 3 - State the derivative domain

The simplified derivative is undefined at $x=1$ because its denominator vanishes:

$$
D_{f'}=\mathbb R\setminus\{1\}.
$$

## Verification

At $x=2$, $f'(2)=(4-4-1)/(1)^2=-1$. A direct local estimate or termwise quotient calculation gives the same sign.

## Interpretation

The quotient rule differentiates the numerator and denominator separately. The restriction $x\neq1$ remains important because the original function and derivative are not defined there.

## Final answer

$$
D_f=D_{f'}=\mathbb R\setminus\{1\},
\qquad
f'(x)=\frac{x^2-2x-1}{(x-1)^2}.
$$
