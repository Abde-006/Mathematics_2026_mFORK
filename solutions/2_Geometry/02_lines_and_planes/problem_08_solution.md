# Exercise 8 — Intersection Point of a Line and a Plane

## Problem Statement

Find the intersection of

$$
(x,y,z)=(1,0,2)+t(1,2,-1)
$$

with the plane

$$
x+y+z=4.
$$

Check the resulting point in both descriptions.

## Lettered Quantities

- Let $p=(1,0,2)$ be a point on $L$.
- Let $v=(1,2,-1)$ be the direction of $L$.
- Let $n=(1,1,1)$ be the normal of $\Pi$.
- Let $d=4$ be the plane constant.
- Let $t$ be the parameter at the intersection.

## Step 1 — Write the Parametric Coordinates

**Parametric coordinates.** Write $X=p+t v$ coordinatewise before imposing the plane equation. For $p=(1,0,2)$ and $v=(1,2,-1)$,

For $p=(1,0,2)$ and $v=(1,2,-1)$,

$$
\begin{aligned}
x&=1+t, \\
y&=2t, \\
z&=2-t.
\end{aligned}
$$

## Step 2 — Solve for the Parameter

**Substitution into a plane.** The condition $X$ lies in $x+y+z=4$ is $n\cdot X=d$, with $n=(1,1,1)$ and $d=4$. Substituting $X(p+t v)$ gives

Substitute the coordinates into $x+y+z=4$:

$$
(1+t)+(2t)+(2-t)=4.
$$

Collect like terms:

$$
\begin{aligned}
1+2+ t+2t-t &=4, \\
3+2t&=4.
\end{aligned}
$$

Therefore

$$
2t=1,
$$

and

$$
t=\frac12.
$$

This is unique because

$$
n\cdot v=(1,1,1)\cdot(1,2,-1)=1+2-1=2\neq0.
$$

## Step 3 — Compute the Intersection Point

**Evaluate the parameter.** Using the solved parameter in $X=p+t v$ returns the intersection point:

Substitute $t=\frac12$:

$$
\begin{aligned}
x&=1+\frac12=\frac32, \\
y&=2\left(\frac12\right)=1, \\
z&=2-\frac12=\frac32.
\end{aligned}
$$

Thus

$$
I=\left(\frac32,1,\frac32\right).
$$

## Verification

Substitute $I$ into the plane equation:

$$
\frac32+1+\frac32
=\frac32+\frac32+1
=3+1
=4.
$$

The line also produces $I$ at $t=\frac12$:

$$
(1,0,2)+\frac12(1,2,-1)
=\left(\frac32,1,\frac32\right).
$$

## Geometric Interpretation

The line has a nonzero normal component $n\cdot v=2$, so it crosses the plane rather than being parallel or contained in it. The unique parameter $t=\frac12$ gives the crossing point.

## Final Answer

$$
I=\left(\frac32,1,\frac32\right).
$$
