# Solution 15 - Recognition and Sketch Without a Given Name

## Problem statement

Consider

$$
4x^2+9y^2-8x+36y+4=0
$$

and

$$
4x^2+y^2=z^2.
$$

For the first equation, reduce it to canonical form and give the curve's principal features and a sketch. For the second equation, analyze the cross-sections $z=c$, $x=0$, and $y=0$, using the different scales along the axes, and then identify and sketch the surface.

## Part 1 - Shifted ellipse

### Lettered quantities

- Let $(h,k)$ be the ellipse center, $a,b>0$ its semiaxes, and $c$ a fixed height for the surface section.

## Step 1 - Group and factor

**Completing-square ellipse form.** Factor quadratic coefficients, complete $(x-h)^2$ and $(y-k)^2$, and normalize to $(x-h)^2/a^2+(y-k)^2/b^2=1$. Apply:

Group the terms:

$$
4(x^2-2x)+9(y^2+4y)+4=0.
$$

### Step 2 - Complete both squares

**Square-completion reminder.** $u^2+bu=(u+b/2)^2-(b/2)^2$. Apply to $x$ and $y$:

For $x^2-2x$, add and subtract $1=(-2/2)^2$. For $y^2+4y$, add and subtract $4=(4/2)^2$:

$$
4\bigl((x-1)^2-1\bigr)
+
9\bigl((y+2)^2-4\bigr)
+4=0.
$$

Expand the constant terms:

$$
4(x-1)^2-4+9(y+2)^2-36+4=0.
$$

Combining constants gives

$$
4(x-1)^2+9(y+2)^2=36.
$$

### Step 3 - Normalize

**Canonical comparison reminder.** Compare the normalized equation with $(x-h)^2/a^2+(y-k)^2/b^2=1$:


Divide by $36$:

$$
\frac{(x-1)^2}{9}+\frac{(y+2)^2}{4}=1.
$$

This is an ellipse with

$$
(h,k)=(1,-2),\qquad a=3,\qquad b=2.
$$

The horizontal vertices are $(h\pm a,k)$:

$$
(4,-2),\qquad (-2,-2).
$$

The vertical vertices are $(h,k\pm b)$:

$$
(1,0),\qquad (1,-4).
$$

The major axis is horizontal because $a>b$. The ellipse also intersects the $y$-axis at $x=0$, where

$$
\frac{(-1)^2}{9}+\frac{(y+2)^2}{4}=1,
$$

so

$$
\frac{(y+2)^2}{4}=\frac89,
\qquad (y+2)^2=\frac{32}{9},
\qquad y=-2\pm\frac{4\sqrt2}{3}.
$$

### Verification for the ellipse

Expanding

$$
4(x-1)^2+9(y+2)^2=36
$$

gives

$$
4x^2-8x+4+9y^2+36y+36=36,
$$

which simplifies to

$$
4x^2+9y^2-8x+36y+4=0.
$$

The point $(1,-2)$ gives $4(0)+9(0)=36-36=0$ in the unnormalized completed equation, confirming the center.

## Part 2 - Surface $4x^2+y^2=z^2$

### Step 1 - Section $z=c$

**Fixed-height section rule.** Substitute $z=c$ and normalize the resulting quadratic equation:


Substitute $z=c$:

$$
4x^2+y^2=c^2.
$$

For $c\ne0$, divide by $c^2$:

$$
\frac{x^2}{c^2/4}+\frac{y^2}{c^2}=1.
$$

This section is an ellipse with semiaxis

$$
a_x=\frac{|c|}{2}
$$

along $x$ and semiaxis

$$
a_y=|c|
$$

along $y$. The $y$-semiaxis is twice the $x$-semiaxis. At $c=0$, the section is only $(0,0,0)$. As $|c|$ increases, every horizontal ellipse expands in both directions.

### Step 2 - Section $x=0$

**Coordinate-plane section reminder.** Substitute $x=0$ and factor the resulting difference of squares:


Substitute $x=0$:

$$
y^2=z^2.
$$

Factoring gives

$$
(y-z)(y+z)=0,
$$

so the section is the pair of lines

$$
y=z,\qquad y=-z
$$

in the $yz$-plane.

### Step 3 - Section $y=0$

**Coordinate-plane section reminder.** Substitute $y=0$ and solve for $z$ in terms of $x$:


Substitute $y=0$:

$$
4x^2=z^2.
$$

Taking square roots gives $z=\pm2x$, or equivalently

$$
z=2x,\qquad z=-2x
$$

in the $xz$-plane.

### Identification and verification

The point at $c=0$, expanding elliptical sections, and paired lines in the coordinate vertical planes describe an elliptic double cone with vertex $(0,0,0)$ and axis $Oz$. The unequal horizontal semiaxes are the different scales: $a_x=|c|/2$ and $a_y=|c|$.

Substituting the vertical section equations back into $4x^2+y^2=z^2$ gives an identity:

- if $y=\pm z$, then $4x^2+y^2=z^2$ becomes $4x^2+z^2=z^2$, hence $x=0$, which is the factored $x=0$ plane, while the section is the pair of lines;
- if $z=\pm2x$, then $4x^2+y^2=4x^2$, hence $y=0$, describing the corresponding $y=0$ section.

The horizontal-section formula directly satisfies $4x^2+y^2=c^2$.

## Geometric interpretation

The first equation is a horizontally stretched ellipse shifted one unit right and two units down. The second is a vertically oriented cone with elliptical rather than circular horizontal sections: it is wider along $y$ than along $x$ at every height.

## Final answer

The first equation reduces to

$$
\frac{(x-1)^2}{9}+\frac{(y+2)^2}{4}=1.
$$

It is an ellipse centered at $(1,-2)$ with horizontal semiaxis $3$ and vertical semiaxis $2$.

The second equation describes an elliptic double cone. For $z=c$, its semiaxes are $|c|/2$ along $x$ and $|c|$ along $y$; at $c=0$ it is a point. Its coordinate vertical sections are $y=\pm z$ and $z=\pm2x$.
