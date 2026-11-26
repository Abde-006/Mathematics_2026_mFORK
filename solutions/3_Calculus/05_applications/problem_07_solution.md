# Problem 7. Exponential Growth

Assume the population model

$$
N(t)=N_0e^{kt},\qquad k>0.
$$

Verify its differential relation, find the doubling time, and explain why that time is independent of $N_0$.

## Quantities

Let $N_0$ be the initial population, $N(t)$ the population at time $t$, $k>0$ the relative growth rate, and $T$ the doubling time.

## Step 1 - Verify the differential relation

The exponential differentiation rule

$$
\frac{d}{dt}e^{kt}=ke^{kt}
$$

applies because $k$ is a constant multiplying $t$. It gives the instantaneous growth rate of $e^{kt}$. Differentiating the model,

$$
\begin{aligned}
N'(t)
&=\frac{d}{dt}(N_0e^{kt}) \\
&=N_0(ke^{kt}) \\
&=k(N_0e^{kt}) \\
&=kN(t).
\end{aligned}
$$

Thus the growth rate is proportional to the current population.

## Step 2 - Find the doubling time

The doubling time is the time $T>0$ for which $N(T)=2N_0$. Substituting $N(T)=N_0e^{kT}$ gives

$$
N_0e^{kT}=2N_0.
$$

For $N_0>0$, dividing by $N_0$ removes the initial population:

$$
e^{kT}=2.
$$

Taking natural logarithms is the inverse operation to exponentiation:

$$
\begin{aligned}
kT&=\ln2, \\
T&=\frac{\ln2}{k}.
\end{aligned}
$$

## Verification

Substituting $T=\ln2/k$ gives

$$
\begin{aligned}
N(T)
&=N_0e^{k(\ln2/k)} \\
&=N_0e^{\ln2} \\
&=2N_0.
\end{aligned}
$$

## Interpretation

The cancellation of $N_0$ occurs because the model measures relative growth. Whether the population starts at $N_0$ or $3N_0$, the same fixed percentage growth occurs in the same elapsed time.

## Final answer

The model satisfies $N'(t)=kN(t)$, and the doubling time is $T=\frac{\ln2}{k}$, which does not depend on $N_0$.
