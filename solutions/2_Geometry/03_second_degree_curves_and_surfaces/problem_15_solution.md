# Solution 15 — Recognition and Sketch Without a Given Name

## Problem Statement

For

$$
4x^2+9y^2-8x+36y+4=0,
$$

reduce the equation to canonical form and give the curve's main features and sketch. For

$$
4x^2+y^2=z^2,
$$

first describe the sections $z=c$, $x=0$, and $y=0$, including the relative scales along the axes, and then identify and sketch the surface.

## Objective

Apply completing the square to a shifted conic and use coordinate sections to recognize a three-dimensional surface.

## Concepts and Formulas

Completing the square reveals the center and semiaxes of an ellipse. For a surface, substituting a fixed coordinate gives a cross-section; comparing the dimensions of those sections reveals its orientation and scale.

## Step-by-Step Solution

### First equation: reduce to canonical form

Group the $x$- and $y$-terms and complete each square:

$$
4(x^2-2x)+9(y^2+4y)+4=0,
$$

$$
4\bigl((x-1)^2-1\bigr)+9\bigl((y+2)^2-4\bigr)+4=0.
$$

Collect constants:

$$
4(x-1)^2+9(y+2)^2=36.
$$

Divide by $36$:

$$
\frac{(x-1)^2}{9}+\frac{(y+2)^2}{4}=1.
$$

The curve is an ellipse centered at $(1,-2)$. Its horizontal semiaxis is $3$ and vertical semiaxis is $2$, so its major axis is horizontal. The vertices are $(4,-2)$ and $(-2,-2)$; the endpoints of the shorter axis are $(1,0)$ and $(1,-4)$. Its $y$-axis intersections satisfy $x=0$:

$$
4+9(y+2)^2=36,
\qquad
y=-2\pm\frac{4\sqrt2}{3}.
$$

It touches the $x$-axis at $(1,0)$, its top endpoint. Sketch a horizontally elongated oval centered two units below the origin and one unit to its right.

### Second equation: analyze the sections first

At a fixed height $z=c$:

$$
4x^2+y^2=c^2.
$$

For $c\ne0$, divide by $c^2$:

$$
\frac{x^2}{c^2/4}+\frac{y^2}{c^2}=1.
$$

This is an ellipse with semiaxis $|c|/2$ along the $x$-direction and $|c|$ along the $y$-direction. The section at $c=0$ is only the origin. As $|c|$ grows, the ellipses expand, and the $y$-semiaxis is twice the $x$-semiaxis.

At $x=0$, the vertical section is $y^2=z^2$, giving the lines $y=z$ and $y=-z$. At $y=0$, it is $4x^2=z^2$, giving $z=2x$ and $z=-2x$. Thus the sections are pairs of lines, with the second pair steeper in the $xz$-plane than the first pair in the $yz$-plane.

Together these sections describe an elliptic double cone with vertex at the origin and axis the $z$-axis. Its horizontal cross-sections are wider in the $y$-direction than in the $x$-direction. Sketch two symmetric cone nappes meeting at the origin, expanding upward and downward with the stated unequal scales.

## Verification

Expanding $4(x-1)^2+9(y+2)^2=36$ gives $4x^2+9y^2-8x+36y+4=0$, confirming the first conversion. For the second surface, every fixed-height ellipse and both vertical line-pairs satisfy $4x^2+y^2=z^2$ by substitution.

## Final Answer

The first equation is the ellipse

$$
\frac{(x-1)^2}{9}+\frac{(y+2)^2}{4}=1,
$$

centered at $(1,-2)$ with horizontal and vertical semiaxes $3$ and $2$. The second equation describes an elliptic double cone: its sections $z=c$ have semiaxes $|c|/2$ in $x$ and $|c|$ in $y$, while its coordinate vertical sections are the line pairs $y=\pm z$ and $z=\pm2x$.

## Key Takeaways

- Completing the square exposes both the shift and the orientation of a conic.
- Cross-section scales matter: equal circular sections are not the only possibility for a cone.
- A zero-height section that is a point, together with expanding ellipses, identifies a cone with vertex at that point.