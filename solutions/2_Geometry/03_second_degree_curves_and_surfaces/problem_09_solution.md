# Solution 9 — Ellipsoid and Its Cross-Sections

## Problem Statement

For

$$
\frac{x^2}{9}+\frac{y^2}{4}+\frac{z^2}{16}=1,
$$

give the semiaxis lengths, describe the section $z=0$, and explain how the sections $z=c$ vary for $|c|<4$.

## Objective

Understand an ellipsoid by studying its coordinate-plane slices.

## Concepts and Formulas

An ellipsoid in standard form has semiaxis lengths equal to the square roots of the denominators. Substituting a fixed coordinate gives the equation of the corresponding planar cross-section.

## Step-by-Step Solution

The semiaxis lengths are $3$ along the $x$-axis, $2$ along the $y$-axis, and $4$ along the $z$-axis.

At $z=0$, the equation becomes

$$
\frac{x^2}{9}+\frac{y^2}{4}=1,
$$

an ellipse in the $xy$-plane with semiaxes $3$ and $2$.

For a fixed $z=c$:

$$
\frac{x^2}{9}+\frac{y^2}{4}=1-\frac{c^2}{16}.
$$

When $|c|<4$, the right side is positive. Dividing by it puts the section in canonical ellipse form:

$$
\frac{x^2}{9(1-c^2/16)}+\frac{y^2}{4(1-c^2/16)}=1.
$$

Its semiaxes are $3\sqrt{1-c^2/16}$ and $2\sqrt{1-c^2/16}$. The sections are largest at $c=0$ and shrink uniformly in both planar directions as $|c|$ approaches $4$. At $c=\pm4$ each section degenerates to one point; for $|c|>4$ there is no section.

## Verification

At $c=0$ the semiaxes reduce to $3$ and $2$. At $c=\pm4$ the right side of the substituted equation is zero, requiring $x=y=0$, consistent with the two endpoints of the ellipsoid.

## Final Answer

The semiaxes are $3,2,4$. The section at $z=0$ is an ellipse with semiaxes $3$ and $2$. For $|c|<4$, the section is an ellipse whose semiaxes are $3\sqrt{1-c^2/16}$ and $2\sqrt{1-c^2/16}$.

## Key Takeaways

- A horizontal slice of an ellipsoid is an ellipse except at the extreme top and bottom points.
- Slices shrink as their fixed coordinate approaches the endpoint of the corresponding semiaxis.