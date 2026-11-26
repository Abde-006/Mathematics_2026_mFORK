# Problem 12. Complete Model and Computer Verification

A museum wants to create a rectangular exhibition room next to an existing straight wall. The side along the wall does not need to be built. The remaining sides have unequal costs: the two sides perpendicular to the wall cost $300\,\mathrm{PLN/m}$ each, while the side parallel to the wall costs $500\,\mathrm{PLN/m}$. The budget is $30\,000\,\mathrm{PLN}$.

Build a model that maximizes room area, complete the mathematical analysis, provide a graph, and numerically verify values near the optimum.

## Quantities and units

Let $x$ be the length of each perpendicular side, in meters. Let $y$ be the length of the parallel side, in meters. Let $C$ be construction cost in Polish zloty and $A$ the room area in square meters.

## Step 1 - Build the cost constraint

The two perpendicular sides cost $300x$ each, for a combined cost of $600x$. The parallel side costs $500y$. Since the full budget is available,

$$
600x+500y=30000.
$$

This constraint is the budget model, not merely a formula for $C$, because it relates the two dimensions that determine area.

## Step 2 - Eliminate $y$

Solving $600x+500y=30000$ for $y$ gives

$$
\begin{aligned}
500y&=30000-600x, \\
y&=60-\frac65x.
\end{aligned}
$$

## Step 3 - Build the objective function

The area of a rectangle is length times width:

$$
A=xy.
$$

Substitution of $y=60-\frac65x$ yields

$$
\begin{aligned}
A(x)
&=x\left(60-\frac65x\right) \\
&=60x-\frac65x^2.
\end{aligned}
$$

## Step 4 - Determine the domain

The dimensions must be nonnegative:

$$
x\ge0,\qquad y=60-\frac65x\ge0.
$$

The second inequality gives

$$
x\le50.
$$

Thus the closed physical domain is

$$
0\le x\le50.
$$

## Step 5 - Compute the derivative

For an interior maximum of the differentiable objective function, the derivative is zero. Differentiating,

$$
\begin{aligned}
A'(x)
&=\frac{d}{dx}\left(60x-\frac65x^2\right) \\
&=60-\frac{12}{5}x.
\end{aligned}
$$

Solving $A'(x)=0$,

$$
\begin{aligned}
60-\frac{12}{5}x&=0, \\
300-12x&=0, \\
x&=25.
\end{aligned}
$$

The corresponding parallel length is

$$
y=60-\frac65(25)=60-30=30.
$$

## Step 6 - Verify the optimum

The second derivative tests concavity:

$$
A''(x)=-\frac{12}{5}<0.
$$

Therefore $A(x)$ is concave downward and $x=25$ is a strict maximum.

The endpoint areas provide an independent comparison:

$$
A(0)=0,\qquad A(50)=50(60-60)=0.
$$

At $x=25$,

$$
A(25)=25(30)=750\ \mathrm{m^2}.
$$

The budget is checked by substitution:

$$
600(25)+500(30)=15000+15000=30000\ \mathrm{PLN}.
$$

## Step 7 - Graph the objective function

The graph of

$$
A(x)=60x-\frac65x^2,\qquad 0\le x\le50,
$$

is a downward-opening parabola with roots $x=0$ and $x=50$ and vertex $(25,750)$:

```text
A (m^2)
750 |                         *
    |                       *   *
    |                     *       *
    |                   *           *
    |                 *               *
  0 +----------------*-------*-------*-------*-- x (m)
                     12.5    25      37.5    50
```

The sketch is visualization only; the derivative and endpoint tests establish the maximum.

## Step 8 - Numerically verify nearby values

Using $A(x)=60x-1.2x^2$ and $y=60-1.2x$, every row uses the full $30\,000\,\mathrm{PLN}$ budget:

| $x$ (m) | $y$ (m) | Cost (PLN) | Area (m$^2$) |
|---:|---:|---:|---:|
| 24.0 | 31.2 | 30,000 | 748.8 |
| 24.5 | 30.6 | 30,000 | 749.7 |
| 25.0 | 30.0 | 30,000 | 750.0 |
| 25.5 | 29.4 | 30,000 | 749.7 |
| 26.0 | 28.8 | 30,000 | 748.8 |

The values decrease symmetrically around $x=25$, independently supporting the analytical maximum.

## Modeling versus calculation

The modeling portion is the conversion of the physical description into the budget constraint

$$
600x+500y=30000
$$

and the one-variable objective

$$
A(x)=60x-\frac65x^2.
$$

Differentiation, endpoint comparison, graph sketching, and the numerical table execute and verify that model.

## Interpretation

The room should have two sides perpendicular to the wall of $25$ m each and one side parallel to the wall of $30$ m. It uses the full budget and encloses $750\,\mathrm{m^2}$.

## Final answer

The maximizing dimensions are $x=25\,\mathrm{m}$ and $y=30\,\mathrm{m}$, and the maximum area is $750\,\mathrm{m^2}$.
