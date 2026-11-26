# Solution 1 - Recognizing Curves from Canonical Form

## Problem statement

Recognize the curves

$$
x^2+y^2=9,
$$

$$
\frac{x^2}{16}+\frac{y^2}{9}=1,
$$

$$
y^2=8x,
$$

$$
\frac{x^2}{9}-\frac{y^2}{4}=1.
$$

For each equation, identify the curve and its principal features.

## Lettered quantities

- Let $(h,k)$ denote center or vertex coordinates, and let $a,b,r,p>0$ denote semiaxes, radius, or focal parameter.

## Step 1 - Circle

**Circle property.** A circle with center $(h,k)$ and radius $r$ has $(x-h)^2+(y-k)^2=r^2$ because every point is $r$ units from $(h,k)$. Rewrite and compare:


Write $x^2+y^2=9$ as

$$
(x-0)^2+(y-0)^2=3^2.
$$

Comparing with the circle formula gives center $(0,0)$ and radius $r=3$. The coordinate-axis intercepts are $(\pm3,0)$ and $(0,\pm3)$.

The sketch is a circle centered at the origin passing through all four intercepts.

## Step 2 - Ellipse

**Ellipse property.** A centered ellipse is $(x-h)^2/a^2+(y-k)^2/b^2=1$; $a$ and $b$ are the semiaxis lengths. Compare coefficients:


Compare

$$
\frac{x^2}{16}+\frac{y^2}{9}=1
$$

with the ellipse formula. Thus $a^2=16$ and $b^2=9$, so

$$
a=4,\qquad b=3.
$$

The center is $(0,0)$, the horizontal vertices are $(\pm4,0)$, and the vertical vertices are $(0,\pm3)$. The ellipse is more stretched along the $x$-axis because $4>3$.

## Step 3 - Parabola

**Parabola property.** The standard form $(y-k)^2=4p(x-h)$ opens in the positive $x$ direction and has vertex $(h,k)$. Here $k=h=0$, so compare:


Set $y^2=8x$ equal to $y^2=4px$. Therefore

$$
4p=8,\qquad p=2.
$$

The vertex is $(0,0)$, the axis of symmetry is $y=0$, and the opening direction is positive $x$. The focus is $(p,0)=(2,0)$, and the directrix is $x=-p=-2$.

## Step 4 - Hyperbola

**Hyperbola property.** $(x-h)^2/a^2-(y-k)^2/b^2=1$ has vertices $(h\pm a,k)$ and asymptotes $y-k=\pm(b/a)(x-h)$. Compare:


Compare

$$
\frac{x^2}{9}-\frac{y^2}{4}=1
$$

with the hyperbola formula. Hence $a^2=9$ and $b^2=4$, so $a=3$ and $b=2$. The center is $(0,0)$, and the vertices are $(\pm3,0)$.

Substitute these values into the asymptote formula:

$$
y=\pm\frac{2}{3}x.
$$

## Verification

Substituting $(3,0)$ into the hyperbola gives $9/9-0/4=1$. Substituting $(4,0)$ into the ellipse gives $16/16+0/9=1$. Substituting $(2,4)$ into $y^2=8x$ gives $16=16$. These checks confirm the principal points and scales.

## Geometric interpretation

The equal positive squared terms describe a circle, unequal positive squared terms describe an ellipse, one squared coordinate equal to a linear coordinate describes a parabola, and a difference of positive squared terms describes a hyperbola.

## Final answer

- $x^2+y^2=9$: circle centered at $(0,0)$ with radius $3$.
- $x^2/16+y^2/9=1$: ellipse centered at $(0,0)$ with semiaxes $4$ and $3$.
- $y^2=8x$: right-opening parabola with vertex $(0,0)$ and $p=2$.
- $x^2/9-y^2/4=1$: left-right-opening hyperbola with vertices $(\pm3,0)$ and asymptotes $y=\pm2x/3$.
