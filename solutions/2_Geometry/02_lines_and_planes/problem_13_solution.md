# Exercise 13 — Closest Point on a Plane

## Problem Statement

Find the point on

$$
\Pi:x+2y+2z=4
$$

closest to $P=(3,0,0)$. Give the distance and check that the segment joining $P$ to the closest point is perpendicular to the plane.

## Lettered Quantities

- Let $P=(p_1,p_2,p_3)=(3,0,0)$.
- Let $n=(1,2,2)$ be the plane normal.
- Let $d=4$ be the plane constant.
- Let $H$ be the closest point.

## Step 1 — Compute the Residual

**Normal residual for closest-point construction.** For $n\cdot X=d$, the signed displacement of $P$ in the normal direction is $(n\cdot P-d)/\lVert n\rVert^2$. It appears in the orthogonal projection formula below. Here

Substitute $P=(3,0,0)$:

$$
\begin{aligned}
n\cdot P-d
&=(1,2,2)\cdot(3,0,0)-4 \\
&=3-4 \\
&=-1.
\end{aligned}
$$

The squared normal length is

$$
\lVert n\rVert^2=1^2+2^2+2^2=9.
$$

## Step 2 — Compute the Closest Point

**Orthogonal projection formula.** The closest point is $H=P-(n\cdot P-d)n/\lVert n\rVert^2$, because subtracting the normal component leaves no perpendicular residual toward the plane. Substitute

Substitute into the projection formula:

$$
\begin{aligned}
H
&=(3,0,0)-\frac{-1}{9}(1,2,2) \\
&=(3,0,0)+\frac19(1,2,2) \\
&=\left(3+\frac19,\frac29,\frac29\right) \\
&=\left(\frac{28}{9},\frac29,\frac29\right).
\end{aligned}
$$

## Step 3 — Compute the Distance

**Point-to-plane distance.** The perpendicular distance is $\mathrm{dist}(P,\Pi)=|n\cdot P-d|/\lVert n\rVert$, the length of the normal residual. Use

Since $\lVert n\rVert=\sqrt9=3$,

$$
$\mathrm{dist}(P,\Pi)=\frac{|-1|}{3}=\frac13$.
$$

## Verification

Check the point's plane membership:

$$
\begin{aligned}
\frac{28}{9}+2\left(\frac29\right)+2\left(\frac29\right)
&=\frac{28+4+4}{9} \\
&=\frac{36}{9} \\
&=4.
\end{aligned}
$$

The displacement from $P$ to $H$ is

$$
\begin{aligned}
H-P
&=\left(\frac{28}{9}-3,\frac29,\frac29\right) \\
&=\left(\frac19,\frac29,\frac29\right) \\
&=\frac19(1,2,2).
\end{aligned}
$$

This is a scalar multiple of $n=(1,2,2)$, so the segment is perpendicular to the plane.

## Geometric Interpretation

The normal segment is the shortest route to the plane. Orthogonal projection produces the unique closest point.

## Final Answer

The closest point is

$$
\left(\frac{28}{9},\frac29,\frac29\right),
$$

and the distance is

$$
\frac13.
$$
