# Exercise 10 — Projection of a Point onto a Plane

## Problem Statement

Find the orthogonal projection of $P=(2,1,3)$ onto

$$
x+y+z=3,
$$

and then find the reflection of $P$ across the plane. Check that the midpoint of $P$ and its reflection lies on the plane.

## Lettered Quantities

- Let $P=(p_1,p_2,p_3)=(2,1,3)$.
- Let $n=(1,1,1)$ be the plane normal.
- Let $d=3$ be the plane constant.
- Let $H$ be the orthogonal projection.
- Let $R$ be the reflection of $P$ across the plane.

## Step 1 — Compute the Normal Residual

**Normal residual for a plane.** The signed normal displacement from $P$ to $n\cdot X=d$ is $(n\cdot P-d)/\lVert n\rVert^2$ times $n$; this identifies how far and in which normal direction $P$ lies from the plane. Here

Calculate

$$
\begin{aligned}
n\cdot P-d
&=(1,1,1)\cdot(2,1,3)-3 \\
&=2+1+3-3 \\
&=3.
\end{aligned}
$$

Also,

$$
\lVert n\rVert^2=1^2+1^2+1^2=3.
$$

Thus

$$
\frac{n\cdot P-d}{\lVert n\rVert^2}=\frac33=1.
$$

## Step 2 — Compute the Projection

**Orthogonal projection formula.** The projection is $H=P-(n\cdot P-d)n/\lVert n\rVert^2$, which removes the normal residual from $P$. Substitute $P=(2,1,3)$:

Substitute into the projection formula:

$$
\begin{aligned}
H
&=P-1n \\
&=(2,1,3)-(1,1,1) \\
&=(1,0,2).
\end{aligned}
$$

## Step 3 — Compute the Reflection

**Reflection formula.** The reflected point is $R=P-2(n\cdot P-d)n/\lVert n\rVert^2$, the projection formula twice because $P$ traverses from itself to $H$ and then equally to the opposite side. Compute

Substitute into the reflection formula:

$$
\begin{aligned}
R
&=P-2n \\
&=(2,1,3)-2(1,1,1) \\
&=(2,1,3)-(2,2,2) \\
&=(0,-1,1).
\end{aligned}
$$

## Verification

The projection lies in the plane:

$$
1+0+2=3.
$$

The midpoint is

$$
\begin{aligned}
\frac{P+R}{2}
&=
\begin{pmatrix}
\frac{2+0}{2} \\
\frac{1-1}{2} \\
\frac{3+1}{2} \\
\end{pmatrix} \\
&=(1,0,2).
\end{aligned}
$$

This equals $H$, so the midpoint lies on the plane.

The segment displacement is

$$
H-P=(-1,-1,-1)=-(1,1,1),
$$

which is parallel to $n$.

## Geometric Interpretation

The shortest normal displacement carries $P$ to $H$ on the plane. Reflection carries $P$ the same perpendicular distance again across the plane.

## Final Answer

The orthogonal projection is

$$
H=(1,0,2).
$$

The reflection is

$$
R=(0,-1,1).
$$
