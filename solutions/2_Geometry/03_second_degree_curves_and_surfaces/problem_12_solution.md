# Solution 12 - Recognizing a Surface from Cross-Sections

## Problem statement

A surface has the following properties:

- the cross-section $z=0$ is a point;
- for $z>0$, the cross-section $z=c$ is a circle with increasing radius;
- vertical cross-sections through the $Oz$ axis are parabolas.

Propose a simple equation for such a surface and justify the choice.

## Lettered quantities

- Let $c>0$ denote height and $r(c)$ the radius of the horizontal section.

## Step 1 - Choose

**Geometry-to-equation rule.** A horizontal section of radius $r(c)$ has equation $x^2+y^2=r(c)^2$. The condition $r(0)=0$ and increasing positive radius for $z>0$ is matched by $r(c)^2=z$ for $z\ge0$. Use:
 the radius-height relation

The simplest relation making the radius increase with height and give a point at $z=0$ is

$$
r(c)^2=c.
$$

Consequently, the proposed surface equation is

$$
x^2+y^2=z.
$$

Equivalently,

$$
z=x^2+y^2.
$$

## Step 2 - Verify

**Section substitution.** Put $z=c$ into the proposed equation and compare with $x^2+y^2=r(c)^2$:
 the horizontal sections

At $z=c$, the equation becomes

$$
x^2+y^2=c.
$$

At $c=0$, the only real solution is $x=y=0$, so the section is the point $(0,0,0)$.

For $c>0$, the section is a circle of radius

$$
r(c)=\sqrt c.
$$

As $c$ increases, $\sqrt c$ increases, exactly matching the description.

## Step 3 - Verify

**Vertical-section rule.** A plane through the $Oz$ axis uses a radial coordinate $s$ and leaves $z$ as $z=s^2$, a parabola:
 the vertical sections

In the plane $y=0$, substitute $y=0$:

$$
z=x^2.
$$

This is an upward-opening parabola in the $xz$-plane.

In the plane $x=0$, substitute $x=0$:

$$
z=y^2.
$$

This is an upward-opening parabola in the $yz$-plane.

More generally, a vertical plane through the $Oz$ axis uses a radial coordinate $s$ and gives $z=s^2$, so every such principal section is parabolic.

## Verification

The proposed equation gives a point at height zero, expanding circles for positive heights, and parabolas through the axis. For negative height $z=c<0$, $x^2+y^2=c$ has no real section, which is also geometrically consistent with an upward-opening surface.

## Geometric interpretation

The surface is a circular paraboloid. Its vertex is $(0,0,0)$, and its axis is $Oz$.

## Final answer

One simple equation satisfying all the stated conditions is

$$
z=x^2+y^2.
$$
