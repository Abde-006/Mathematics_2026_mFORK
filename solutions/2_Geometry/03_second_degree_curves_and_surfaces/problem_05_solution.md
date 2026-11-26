# Solution 5 - Hyperbola and Asymptotes

## Problem statement

For

$$
\frac{x^2}{16}-\frac{y^2}{9}=1,
$$

find the $x$-axis intercepts and asymptotes, and describe a sketch.

## Lettered quantities

- Let $a>0$ and $b>0$ denote the hyperbola semiaxis and asymptote parameter.

## Step 1 - Read

**Hyperbola form.** In $x^2/a^2-y^2/b^2=1$, $a^2$ and $b^2$ are denominators of the positive and negative squared terms. Read:
 $a$ and $b$

Because $16=4^2$ and $9=3^2$,

$$
a=4,\qquad b=3.
$$

## Step 2 - Find

**Intercept condition.** Set $y=0$ to find real $x$-axis intersections:
 the $x$-axis intercepts

Set $y=0$:

$$
\frac{x^2}{16}=1.
$$

Thus

$$
x^2=16,\qquad x=\pm4.
$$

The intercepts, also called vertices, are $(4,0)$ and $(-4,0)$.

## Step 3 - Find

**Asymptote property.** The right-left hyperbola $x^2/a^2-y^2/b^2=1$ has asymptotes $y=\pm(b/a)x$, obtained from balancing the two leading squared terms. Substitute:
 the asymptotes

Substitute $a=4$ and $b=3$ into the asymptote formula:

$$
y=\pm\frac{3}{4}x.
$$

## Step 4 - Explain the far-field behavior

For $|x|$ and $|y|$ large, the constant $1$ is insignificant compared with $x^2/16$ and $y^2/9$. The limiting equation is therefore

$$
\frac{x^2}{16}-\frac{y^2}{9}=0.
$$

Multiplying by $144$ gives

$$
9x^2-16y^2=0.
$$

This factors as

$$
(3x-4y)(3x+4y)=0,
$$

so $y=3x/4$ or $y=-3x/4$, exactly the asymptotes.

## Verification

At $(4,0)$,

$$
\frac{16}{16}-\frac0{9}=1.
$$

At $(-4,0)$, the same calculation is obtained. No $y$-axis point satisfies the equation because $x=0$ would give $-y^2/9=1$, which is impossible.

## Geometric interpretation

The two branches open left and right. They meet no $y$-axis point and approach the diagonal lines as their distance from the center becomes large.

## Final answer

The vertices are $(\pm4,0)$ and the asymptotes are

$$
y=\pm\frac34x.
$$
