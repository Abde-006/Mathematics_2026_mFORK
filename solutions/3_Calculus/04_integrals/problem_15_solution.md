# Problem 15. Recovering a Function from Its Derivative and a Condition

## Problem

Given $F'(x)=2xe^{x^2}$ and $F(0)=3$, find $F$.

## Solution

The factor $2x$ is the derivative of $x^2$, so substitution is appropriate.

### Step 1 - Substitution

Let

$$
u=x^2,\qquad du=2x dx.
$$

Then

$$
\int2xe^{x^2}dx
=\int e^u du
=e^u+C
=e^{x^2}+C.
$$

Thus the full family is $F(x)=e^{x^2}+C$.

### Step 2 - Initial condition

$$
F(0)=e^0+C=1+C=3,
$$

so $C=2$. Hence

$$
F(x)=e^{x^2}+2.
$$

### Verification

$$
F'(x)=2xe^{x^2},
$$

and

$$
F(0)=e^0+2=3.
$$

## Final Answer

$$
F(x)=e^{x^2}+2.
$$
