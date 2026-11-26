# Problem 3. A Box Made from Cardboard

From a $30\,\mathrm{cm}\times40\,\mathrm{cm}$ sheet, squares of side length $x$ are cut from the corners and the edges are folded up to form an open box. Find the value of $x$ that maximizes the volume.

## Quantities

Let $x$ be the side length of each cutout and the resulting height, $L$ the folded length, $W$ the folded width, and $V$ the volume. These quantities are measured in centimeters or cubic centimeters.

## Step 1 - Build the volume function

Cutting $x$ from each end reduces the original length and width:

$$
L=40-2x,\qquad W=30-2x,\qquad H=x.
$$

Volume is length times width times height, $V=LWH$. Substitution gives

$$
\begin{aligned}
V(x)
&=x(40-2x)(30-2x) \\
&=x(1200-140x+4x^2) \\
&=1200x-140x^2+4x^3.
\end{aligned}
$$

## Step 2 - Determine the physical domain

The dimensions must remain positive. Thus

$$
40-2x>0,\qquad 30-2x>0,\qquad x>0.
$$

The most restrictive inequality is $30-2x>0$, so

$$
0<x<15.
$$

## Step 3 - Find the critical points

For an interior maximum of a differentiable function, solve $V'(x)=0$. Differentiating gives

$$
\begin{aligned}
V'(x)
&=1200-280x+12x^2 \\
&=4(3x^2-70x+300).
\end{aligned}
$$

The quadratic formula determines $V'(x)=0$:

$$
\begin{aligned}
x
&=\frac{70\pm\sqrt{70^2-4(3)(300)}}{2(3)} \\
&=\frac{70\pm\sqrt{1300}}{6} \\
&=\frac{35\pm5\sqrt{13}}{3}.
\end{aligned}
$$

The two numerical values are approximately

$$
x_1\approx5.657,\qquad x_2\approx17.676.
$$

Only $x_1$ belongs to $(0,15)$.

## Step 4 - Verify the maximum

The second derivative classifies the interior critical point:

$$
\begin{aligned}
V''(x)&=24x-280, \\
V''(x_1)&\approx24(5.657)-280\approx-144.2<0.
\end{aligned}
$$

Therefore $x_1$ is a strict local maximum. At the domain endpoints,

$$
V(0)=0,\qquad V(15)=0,
$$

so the remaining interior critical point gives the greatest volume.

## Verification and interpretation

The maximizing dimensions are approximately

$$
L=40-2(5.657)\approx28.686\,\mathrm{cm},
$$

$$
W=30-2(5.657)\approx18.686\,\mathrm{cm},
$$

and

$$
H=5.657\,\mathrm{cm}.
$$

## Final answer

The maximum-volume cutout is

$$
x=\frac{35-5\sqrt{13}}{3}\,\mathrm{cm}\approx5.657\,\mathrm{cm}.
$$
