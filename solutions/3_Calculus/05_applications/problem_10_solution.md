# Problem 10. A Cable Through Water and Land

Point $A$ lies on one bank of a river of width $100$ m, while point $B$ lies on the other bank $500$ m along the bank from the point directly opposite $A$. Cable costs twice as much per meter underwater as on land. Find the cable exit point that minimizes cost.

## Quantities

Let $k>0$ be the land cost in currency units per meter, $P$ the point where the cable comes out of the water, and $x$ the horizontal distance from the point directly opposite $A$ to $P$, measured in meters.

The underwater length forms a right triangle with legs $x$ and $100$. The remaining land distance is $500-x$.

## Step 1 - Build the cost function

The Pythagorean theorem gives the underwater length

$$
d_w=\sqrt{x^2+100^2}.
$$

It applies because the river crossing has perpendicular components $100$ and $x$. Underwater cost is twice land cost, so

$$
C(x)=2k\sqrt{x^2+10000}+k(500-x).
$$

## Step 2 - Determine the domain

The exit point can range from the point directly opposite $A$ to the shore position opposite $B$:

$$
0\le x\le500.
$$

The positive factor $k$ scales cost but does not change the minimizing location.

## Step 3 - Find the critical point

At an interior minimum, the derivative of $C(x)$ is zero. Factoring $k$ and differentiating,

$$
C'(x)
=k\left(\frac{2x}{\sqrt{x^2+10000}}-1\right).
$$

Setting $C'(x)=0$ gives

$$
\frac{2x}{\sqrt{x^2+10000}}=1.
$$

For $x\ge0$, both sides are nonnegative, so squaring preserves this condition:

$$
\begin{aligned}
4x^2&=x^2+10000, \\
3x^2&=10000, \\
x&=\frac{100}{\sqrt3}\approx57.735.
\end{aligned}
$$

The negative solution is outside the domain.

## Step 4 - Verify the minimum

The second derivative is

$$
C''(x)
=k\frac{20000}{(x^2+10000)^{3/2}}>0
$$

for $0\le x\le500$. A positive second derivative proves strict convexity, so the critical point is the minimum.

For an independent endpoint comparison,

$$
C(0)=k(200+500)=700k,
$$

and

$$
C(500)=k(2\sqrt{260000})\approx1019.804k.
$$

At $x=100/\sqrt3$,

$$
\begin{aligned}
C\left(\frac{100}{\sqrt3}\right)
&=k\left(2\sqrt{\frac{10000}{3}+10000}+500-\frac{100}{\sqrt3}\right) \\
&\approx673.205k,
\end{aligned}
$$

which is below both endpoint costs.

## Interpretation

The cable exits the water about $57.735$ m along the bank from the point directly opposite $A$, so it uses less expensive land for the remaining

$$
500-\frac{100}{\sqrt3}\approx442.265\ \mathrm{m}.
$$

## Final answer

The minimizing exit distance is

$$
\frac{100}{\sqrt3}\,\mathrm{m}\approx57.735\,\mathrm{m}.
$$
