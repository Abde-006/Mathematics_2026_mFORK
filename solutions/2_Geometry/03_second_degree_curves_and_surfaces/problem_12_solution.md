# Solution 12 — Recognizing a Surface from Cross-Sections

## Problem Statement

A surface has a point as its section at $z=0$, circular sections of increasing radius for $z>0$, and parabolas in vertical planes through the $Oz$ axis. Propose and justify an equation.

## Objective

Construct a surface equation from its horizontal and vertical cross-sections.

## Concepts and Formulas

The equation $x^2+y^2=r^2$ describes a circle of radius $r$ in a horizontal plane. A vertical section through the $z$-axis can be studied by fixing a vertical plane through that axis.

## Step-by-Step Solution

Choose the simplest increasing radius relation $r^2=z$. Since $r^2=x^2+y^2$, the proposed surface is

$$
x^2+y^2=z.
$$

At $z=0$, this requires $x^2+y^2=0$, so the section is just $(0,0,0)$. At each $z=c>0$, the section is

$$
x^2+y^2=c,
$$

a circle of radius $\sqrt c$. These radii increase as $c$ increases.

In the vertical plane $y=0$, the equation becomes $z=x^2$, a parabola. In the vertical plane $x=0$, it becomes $z=y^2$, also a parabola. More generally, a vertical plane through the $Oz$ axis has a horizontal coordinate $s$ measured from that axis, and its section is $z=s^2$. The surface is therefore a bowl opening upward, with its vertex at the origin.

## Verification

The proposed equation produces exactly the stated point at height zero, circles with increasing radii at positive heights, and parabolic vertical sections through the axis.

## Final Answer

One suitable equation is

$$
z=x^2+y^2.
$$

## Key Takeaways

- The squared radius of a horizontal circle can be set equal to its height.
- Checking both horizontal and vertical sections verifies that a proposed equation matches the description.