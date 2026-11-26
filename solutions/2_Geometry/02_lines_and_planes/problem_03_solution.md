# Exercise 3 — Plane Through a Point with a Given Normal Vector

## Problem Statement

Find the equation of the plane through $P=(1,-2,3)$ and perpendicular to $n=(2,1,-1)$. Check the result by substituting $P$, and explain the role of the normal vector.

## Lettered Quantities

- Let $P=(p_1,p_2,p_3)=(1,-2,3)$.
- Let $n=(n_1,n_2,n_3)=(2,1,-1)$.
- Let $X=(x,y,z)$ be a general point on the plane.
- Let $d=n\cdot P$ be the plane constant.

## Step 1 — Compute the Plane Constant

**Point-normal plane property.** The plane through $P$ with normal $n$ consists of points $X$ for which $X-P$ is perpendicular to $n$, so $n\cdot(X-P)=0$. Using $P=(1,-2,3)$ and $n=(2,1,-1)$ gives

Substitute $n=(2,1,-1)$ and $P=(1,-2,3)$:

$$
\begin{aligned}
d
&=n\cdot P \\
&=(2)(1)+(1)(-2)+(-1)(3) \\
&=2-2-3 \\
&=-3.
\end{aligned}
$$

## Step 2 — Write and Expand the Plane Equation

**Expand the point-normal equation.** The scalar product is computed componentwise; this form identifies the plane constant while preserving $P$. Expand

Using $n\cdot X=d$,

$$
(2,1,-1)\cdot(x,y,z)=-3.
$$

Therefore

$$
2x+y-z=-3,
$$

or

$$
2x+y-z+3=0.
$$

## Verification

Substitute $P=(1,-2,3)$:

$$
\begin{aligned}
2(1)+(-2)-3+3
&=2-2-3+3 \\
&=0.
\end{aligned}
$$

Thus $P$ lies on the plane.

## Geometric Interpretation

The normal vector $n=(2,1,-1)$ is perpendicular to every direction in the plane. It fixes the plane's orientation, while $P$ fixes its location.

## Final Answer

$$
2x+y-z+3=0.
$$
