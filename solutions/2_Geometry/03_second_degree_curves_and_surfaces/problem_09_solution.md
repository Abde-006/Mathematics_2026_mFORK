# Solution 9 - Ellipsoid and Its Cross-Sections

## Problem statement

Consider

$$
\frac{x^2}{9}+\frac{y^2}{4}+\frac{z^2}{16}=1.
$$

Give the semiaxis lengths, describe the cross-section $z=0$, and explain how the cross-sections $z=c$ change for $|c|<4$.

## Lettered quantities

- Let $a,b,d>0$ denote semiaxes along $x,y,z$, respectively.

## Step 1 - Read

**Ellipsoid form.** In $x^2/a^2+y^2/b^2+z^2/d^2=1$, $a,b,d$ are the semiaxes along $x,y,z$. Read:
 the semiaxis lengths

The denominators give

$$
a^2=9,\qquad b^2=4,\qquad d^2=16.
$$

Therefore

$$
a=3,\qquad b=2,\qquad d=4.
$$

The semiaxes point along the $x$, $y$, and $z$ directions, respectively.

## Step 2 - Describe

**Cross-section rule.** Substitute the fixed coordinate $z=0$ and keep the $x,y$ equation:
 $z=0$

Substitute $z=0$:

$$
\frac{x^2}{9}+\frac{y^2}{4}=1.
$$

This is an ellipse in the $xy$-plane centered at the origin, with horizontal semiaxis $3$ and vertical semiaxis $2$.

## Step 3 - Describe

**Fixed-height ellipse.** Substitution of $z=c$ gives $x^2/a^2+y^2/b^2=1-c^2/d^2$; this is real only when the right side is nonnegative. Apply:

For $z=c$,

$$
\frac{x^2}{9}+\frac{y^2}{4}=1-\frac{c^2}{16}.
$$

When $|c|<4$, let

$$
A=1-\frac{c^2}{16}>0.
$$

Divide the equation by $A$:

$$
\frac{x^2}{9A}+\frac{y^2}{4A}=1.
$$

The two semiaxes of the section are $3\sqrt A$ and $2\sqrt A$, equivalently $3\sqrt{1-c^2/16}$ and $2\sqrt{1-c^2/16}$.

## Step 4 - Compare

**Section comparison.** As $|c|$ grows toward $d$, the common scale $1-c^2/d^2$ decreases, so both semiaxes shrink:
 the sections

At $c=0$, $A=1$, and the section is the original ellipse with semiaxes $3$ and $2$. As $|c|$ increases toward $4$, the factor $\sqrt A$ decreases to $0$, so both semiaxes shrink. At $c=\pm4$, the section is $(x,y)=(0,0)$, that is, a single point. For $|c|>4$, $A<0$, so no real cross-section exists.

## Verification

For $c=4$,

$$
\frac{x^2}{9}+\frac{y^2}{4}=0.
$$

The sum of two nonnegative terms can equal zero only at $x=y=0$. The same result occurs at $c=-4$. This agrees with the endpoints of the ellipsoid on the $z$-axis.

## Geometric interpretation

Horizontal slices are ellipses whose shape stays fixed and whose scale decreases uniformly toward the top and bottom. The fixed ratio $3:2$ of the two in-plane semiaxes is preserved.

## Final answer

The semiaxes are $3$, $2$, and $4$. The section $z=0$ is

$$
\frac{x^2}{9}+\frac{y^2}{4}=1.
$$

For $|c|<4$, the section $z=c$ is an ellipse with semiaxes $3\sqrt{1-c^2/16}$ and $2\sqrt{1-c^2/16}$.
