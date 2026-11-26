# Solution 10 - Paraboloids

## Problem statement

Compare

$$
z=x^2+y^2
$$

and

$$
z=x^2-y^2.
$$

For each surface, describe the cross-sections $x=0$, $y=0$, and $z=c$, and provide a qualitative sketch.

## Lettered quantities and method

Let $c$ be a fixed height and let $r$ denote the radius of a horizontal cross-section. To obtain a cross-section, substitute the fixed coordinate into the surface equation and retain the remaining variables.

## Surface 1 - $z=x^2+y^2$

### Vertical section $x=0$

Substitution gives

$$
z=y^2.
$$

This is an upward-opening parabola in the $yz$-plane.

### Vertical section $y=0$

Substitution gives

$$
z=x^2.
$$

This is also an upward-opening parabola in the $xz$-plane.

### Horizontal section $z=c$

Substitution gives

$$
x^2+y^2=c.
$$

If $c>0$, the section is a circle of radius

$$
r=\sqrt c.
$$

If $c=0$, the section is only $(0,0)$. If $c<0$, no real section exists.

The surface is a circular paraboloid, or upward-opening bowl, with vertex $(0,0,0)$ and axis $Oz$.

## Surface 2 - $z=x^2-y^2$

### Vertical section $x=0$

Substitute $x=0$:

$$
z=-y^2.
$$

This is a downward-opening parabola in the $yz$-plane.

### Vertical section $y=0$

Substitute $y=0$:

$$
z=x^2.
$$

This is an upward-opening parabola in the $xz$-plane.

### Horizontal section $z=c$

Substitution gives

$$
x^2-y^2=c.
$$

If $c>0$, this is a hyperbola opening along the $x$-axis. If $c<0$, it is a hyperbola opening along the $y$-axis. If $c=0$, factor:

$$
x^2-y^2=(x-y)(x+y)=0,
$$

so the section is the pair of lines $y=x$ and $y=-x$.

The surface is a hyperbolic paraboloid, or saddle. It rises in the positive $x$ direction and falls in the positive $y$ direction.

## Verification

The first surface has horizontal radius $\sqrt c$, while the second surface has no circular horizontal sections. At $c=0$ in the second surface, the factorization confirms the two intersecting lines.

## Geometric interpretation

For $z=x^2+y^2$, both vertical sections bend upward, so the surface curves the same way in every radial direction. For $z=x^2-y^2$, the two principal vertical sections bend in opposite directions, creating the saddle.

## Final answer

- $z=x^2+y^2$ is a circular bowl with vertex $(0,0,0)$ and circular horizontal sections.
- $z=x^2-y^2$ is a saddle with opposite-facing parabolic vertical sections and hyperbolic horizontal sections.
