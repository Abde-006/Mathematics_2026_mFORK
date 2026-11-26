# Solution 11 - Two Similar Surfaces

## Problem statement

Compare

$$
x^2+y^2-z^2=1
$$

and

$$
x^2+y^2-z^2=-1.
$$

For several heights $z=c$, determine whether the section exists and find its radius. Describe the difference and give qualitative sketches.

## Lettered quantities

- Let $c$ denote a fixed height and $r(c)\ge0$ the radius of a horizontal cross-section.

## Surface 1 - $x^2+y^2-z^2=1$

**Horizontal-section rule.** A fixed height $z=c$ is found by substitution. The remaining equation $x^2+y^2=r^2$ is a circle of radius $r$ when $r^2>0$. Apply:
 - $x^2+y^2-z^2=1$

Substitute $z=c$:

$$
x^2+y^2-c^2=1,
$$

so

$$
x^2+y^2=1+c^2.
$$

Because $1+c^2>0$ for every real $c$, a section exists at every height. Its radius is

$$
r(c)=\sqrt{1+c^2}.
$$

Examples:

$$
r(0)=1,\qquad r(1)=r(-1)=\sqrt2,\qquad r(2)=r(-2)=\sqrt5.
$$

The radius is smallest at $c=0$ and increases as $|c|$ increases. The surface is one connected surface around the $z$-axis, with a circular waist of radius $1$.

## Surface 2 - $x^2+y^2-z^2=-1$

**Reminder for horizontal sections.** At $z=c$, solve $x^2+y^2=c^2-1$ and classify according to whether $c^2-1$ is positive, zero, or negative:
 - $x^2+y^2-z^2=-1$

Substitute $z=c$:

$$
x^2+y^2-c^2=-1,
$$

so

$$
x^2+y^2=c^2-1.
$$

If $|c|<1$, then $c^2-1<0$, so no real section exists.

If $|c|=1$, the equation becomes

$$
x^2+y^2=0,
$$

so the section consists of the single point $(0,0,c)$.

If $|c|>1$, the section is a circle with radius

$$
r(c)=\sqrt{c^2-1}.
$$

Examples:

$$
r(1)=r(-1)=0,\qquad r(2)=r(-2)=\sqrt3.
$$

Thus the surface has two separated portions above and below $z=1$ and $z=-1$, respectively.

## Verification

For the first surface, $x=y=0$ at $z=0$ gives $-0^2=1$, which is false, so the waist is not a point. It has radius $1$.

For the second surface, substituting $c=0$ requires $x^2+y^2=-1$, an impossible real equation. At $c=\pm1$, direct substitution gives $x^2+y^2=0$, confirming the two tips.

## Geometric interpretation

The first equation describes a one-sheet hyperboloid: every horizontal plane cuts it, and the horizontal radius first decreases to a minimum then increases. The second equation describes a two-sheet hyperboloid: the origin plane and nearby planes miss it entirely, while planes farther out cut circular sections.

## Final answer

For $x^2+y^2-z^2=1$, the section radius is $\sqrt{1+c^2}$ for every $c$.

For $x^2+y^2-z^2=-1$, no section exists for $|c|<1$, the section is a point at $c=\pm1$, and the radius is $\sqrt{c^2-1}$ for $|c|>1$.
