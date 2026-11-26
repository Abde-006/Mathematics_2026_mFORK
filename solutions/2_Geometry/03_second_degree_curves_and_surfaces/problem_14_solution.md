# Solution 14 - Cone and Cylinder

## Problem statement

Compare

$$
x^2+y^2=z^2
$$

and

$$
x^2+y^2=4.
$$

For each surface, describe the cross-sections $z=c$, $x=0$, and $y=0$, and explain the difference in horizontal radii.

## Lettered quantities

- Let $c$ denote a fixed height and $r$ the radius of a horizontal section.

## Surface 1 - $x^2+y^2=z^2$

**Horizontal-section rule.** Substitute $z=c$; the radius is real when $c^2\ge0$ and equals $|c|$ because $x^2+y^2=c^2$. Apply:
 - $x^2+y^2=z^2$

### Section $z=c$

Substitute $z=c$:

$$
x^2+y^2=c^2.
$$

At $c\ne0$, the section is a circle of radius $|c|$. At $c=0$, the section is only $(0,0,0)$. The radius grows linearly with the distance from $z=0$.

### Section $x=0$

Substitute $x=0$:

$$
y^2=z^2.
$$

Factoring,

$$
(y-z)(y+z)=0,
$$

gives the lines

$$
y=z,\qquad y=-z
$$

in the $yz$-plane.

### Section $y=0$

Substitute $y=0$:

$$
x^2=z^2,
$$

so

$$
x=z,\qquad x=-z
$$

are the two lines in the $xz$-plane.

The surface is a double cone with vertex $(0,0,0)$ and axis $Oz$. Its upper and lower nappes widen linearly away from the vertex.

## Surface 2 - $x^2+y^2=4$

**Constant-cylinder section rule.** The equation contains no $z$, so every horizontal plane $z=c$ has the same circular trace of radius $2$:
 - $x^2+y^2=4$

### Section $z=c$

Because $z$ does not occur in the equation, substitution of $z=c$ leaves

$$
x^2+y^2=4
$$

for every $c$. The radius is therefore always $r=2$, independent of height.

### Section $x=0$

Substitute $x=0$:

$$
y^2=4,
$$

so

$$
y=2,\qquad y=-2.
$$

These are two vertical lines parallel to the $Oz$ axis.

### Section $y=0$

Substitute $y=0$:

$$
x^2=4,
$$

so

$$
x=2,\qquad x=-2.
$$

These are another pair of vertical lines parallel to the $Oz$ axis.

The surface is a circular cylinder of radius $2$, extending along the $z$ direction.

## Verification

For the cone, the squared horizontal radius is $c^2$, so $r=|c|$. For the cylinder, the squared horizontal radius remains $4$, so $r=2$ at every height.

## Geometric interpretation

The cone's radius varies because $z$ appears in the radial equation. The cylinder's radius is constant because $z$ does not appear at all.

## Final answer

- $x^2+y^2=z^2$ is a double cone. Its horizontal radius is $|z|$, and the $x=0$ and $y=0$ sections are pairs of lines.
- $x^2+y^2=4$ is a circular cylinder of radius $2$. Every horizontal section is the same circle, and the coordinate vertical sections are vertical line pairs.
