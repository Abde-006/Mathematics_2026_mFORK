# Solution 11 — Two Similar Surfaces

## Problem Statement

Compare

$$
x^2+y^2-z^2=1,
\qquad
x^2+y^2-z^2=-1.
$$

For several values $z=c$, determine whether each section exists and its radius, then describe and sketch the surfaces.

## Objective

Use horizontal sections to distinguish two surfaces with similar equations.

## Concepts and Formulas

At $z=c$, each equation becomes a relation between $x$ and $y$. An equation $x^2+y^2=R^2$ describes a real circle when $R^2>0$, a point when $R^2=0$, and no real points when $R^2<0$.

## Step-by-Step Solution

### First equation

At $z=c$:

$$
x^2+y^2=1+c^2.
$$

This section exists for every real $c$, with radius $\sqrt{1+c^2}$. For example, at $c=0$ the radius is $1$; at $c=1$ or $c=-1$ it is $\sqrt2$; at $c=2$ or $c=-2$ it is $\sqrt5$. The sections are smallest at the middle plane and expand in both directions. The sketch is a connected, hourglass-like surface with a circular waist of radius $1$ at $z=0$.

### Second equation

At $z=c$:

$$
x^2+y^2=c^2-1.
$$

There is no real section when $|c|<1$. At $c=1$ and $c=-1$, the section is a single point of radius $0$. For $|c|>1$, it is a circle of radius $\sqrt{c^2-1}$. For example, at $c=2$ or $c=-2$, the radius is $\sqrt3$. The sketch consists of two separated parts, one above and one below the plane, beginning at $z=1$ and $z=-1$ and widening away from those tips.

## Verification

The right sides $1+c^2$ and $c^2-1$ give the stated existence conditions and radii. In particular, the second section at $c=0$ would require $x^2+y^2=-1$, which has no real solutions.

## Final Answer

The first surface has circular sections at every height, with radius $\sqrt{1+c^2}$ and a minimum waist at $z=0$. The second has no sections for $|c|<1$, point sections at $c=\pm1$, and growing circles for $|c|>1$, producing two disconnected portions.

## Key Takeaways

- The sign of the fixed-height radius squared determines whether a section exists.
- A minimum-radius waist and two separated tips yield qualitatively different global shapes.