# Exercise 6 — Angle Between Planes

## Problem Statement

Given

$$
\Pi_1:x+y+z=1,\qquad \Pi_2:x-y=2,
$$

use the normal vectors to determine whether the planes are parallel. If they are not parallel, compute the angle between them and explain why normals are sufficient.

## Lettered Quantities

- Let $n_1=(1,1,1)$ be the normal of $\Pi_1$.
- Let $n_2=(1,-1,0)$ be the normal of $\Pi_2$.
- Let $\theta$ be the acute angle between the planes.

## Step 1 — Compare the Normal Vectors

**Normal-vector test.** For $ax+by+cz=d$, $(a,b,c)$ is a normal vector. A normal points perpendicular to the plane, so parallel normals mean parallel planes. Read

The normals are

$$
n_1=(1,1,1),\qquad n_2=(1,-1,0).
$$

The vector $n_2$ is not a scalar multiple of $n_1$: for example, their third components are $0$ and $1$. Therefore the planes are not parallel.

## Step 2 — Compute the Dot Product

**Reminded dot-product test.** The dot product $n_1\cdot n_2$ measures whether the normals share a direction; its numerator magnitude is used below. Compute

$$
\begin{aligned}
n_1\cdot n_2
&=(1)(1)+(1)(-1)+(1)(0) \\
&=1-1+0 \\
&=0.
\end{aligned}
$$

Thus the normal vectors are perpendicular.

## Step 3 — Compute the Plane Angle

**Acute plane angle.** The angle between planes equals the acute angle between their normals: $\cos\theta=|n_1\cdot n_2|/(\lVert n_1\rVert\lVert n_2\rVert)$. This why the normals determine the angle. Substitute

The lengths are

$$
\begin{aligned}
\lVert n_1\rVert&=\sqrt{1^2+1^2+1^2}=\sqrt3, \\
\lVert n_2\rVert&=\sqrt{1^2+(-1)^2+0^2}=\sqrt2.
\end{aligned}
$$

Substitution gives

$$
\cos\theta
=\frac{|0|}{\sqrt3\sqrt2}
=0.
$$

Therefore

$$
\theta=\arccos(0)=90^\circ.
$$

## Verification

The normals are perpendicular by $n_1\cdot n_2=0$, so the planes are perpendicular as well. This agrees with the angle formula.

## Geometric Interpretation

Each plane has the orientation of all vectors perpendicular to its normal. Rotating a plane and rotating the plane of its normal have the same angle, so the angle between two normals equals the angle between the planes. The absolute value selects the acute angle.

## Final Answer

The planes are not parallel. They intersect at a right angle, so

$$
\theta=90^\circ.
$$
