# Solution 14 — Cone and Cylinder

## Problem Statement

Compare

$$
x^2+y^2=z^2,
\qquad
x^2+y^2=4.
$$

For each surface, describe the sections $z=c$, $x=0$, and $y=0$, and give a qualitative sketch.

## Objective

Distinguish a cone from a cylinder by tracking how horizontal sections change with height.

## Concepts and Formulas

An equation $x^2+y^2=R^2$ at fixed $z$ describes a circle of radius $R$. In a vertical coordinate plane, setting one horizontal coordinate to zero reveals the section curve.

## Step-by-Step Solution

### Surface 1: $x^2+y^2=z^2$

At $z=c$, the equation is $x^2+y^2=c^2$, a circle of radius $|c|$. At $c=0$ it is only the origin; the radius grows linearly with distance above or below that height.

At $x=0$, the section is $y^2=z^2$, which factors as $(y-z)(y+z)=0$ and gives the two lines $y=z$ and $y=-z$ in the $yz$-plane. At $y=0$, the section is $x^2=z^2$, giving $x=z$ and $x=-z$ in the $xz$-plane.

The sketch is a double cone with vertex at the origin and axis the $z$-axis. Its two nappes widen as $|z|$ increases.

### Surface 2: $x^2+y^2=4$

At every height $z=c$, the section is the same circle $x^2+y^2=4$, of radius $2$. At $x=0$, the equation gives $y=2$ or $y=-2$, with $z$ free; these are two vertical lines. At $y=0$, it gives $x=2$ or $x=-2$, again with $z$ free.

The sketch is a circular cylinder of radius $2$ extending indefinitely in both directions along the $z$-axis. Its horizontal radius does not depend on $z$ because $z$ does not appear in its equation.

## Verification

For the first surface, substituting $z=c$ gives squared radius $c^2$. For the second, substituting any $c$ leaves squared radius $4$. The vertical sections also follow by direct substitution.

## Final Answer

The first surface is a double cone whose horizontal radius is $|z|$. The second is a cylinder whose horizontal radius is always $2$.

## Key Takeaways

- A variable radius in horizontal sections signals a cone-like surface.
- If the axis variable is absent from the equation, the same cross-section repeats along that axis.