# Exercise 5 — Relative Position of Two Lines

## Problem Statement

Analyze

$$
L_1:(x,y,z)=(1,1,0)+t(1,2,1),
$$

$$
L_2:(x,y,z)=(2,0,1)+s(0,1,-1).
$$

If they intersect, give the intersection point. Otherwise determine whether they are parallel or skew.

## Lettered Quantities

- Let $p_1=(1,1,0)$ and $v_1=(1,2,1)$ define $L_1$.
- Let $p_2=(2,0,1)$ and $v_2=(0,1,-1)$ define $L_2$.
- Let $w=p_2-p_1$.
- Let $t,s\in\mathbb R$ be the line parameters.

## Step 1 — Compare the Directions

**Parallel-direction test.** Lines are parallel exactly when their direction vectors are scalar multiples. Compare $v_1=(1,2,1)$ and $v_2=(0,1,-1)$:

The directions are

$$
v_1=(1,2,1),\qquad v_2=(0,1,-1).
$$

They are not scalar multiples because $v_2$ has first component $0$ while $v_1$ has first component $1$. Therefore $L_1$ and $L_2$ are not parallel.

## Step 2 — Test for an Intersection

**Intersection condition.** A common point exists when $p_1+t v_1=p_2+s v_2$ has a real solution. Write this vector equation in coordinates:

Equating coordinates gives

$$
\begin{aligned}
1+t&=2, \\
1+2t&=s, \\
t&=1-s.
\end{aligned}
$$

The first equation gives

$$
t=1.
$$

The third equation then gives

$$
1=1-s,
$$

so

$$
s=0.
$$

The second equation requires

$$
s=1+2t=1+2(1)=3,
$$

which contradicts $s=0$. Thus no pair $(t,s)$ satisfies all three equations.

## Step 3 — Confirm the Skew Classification

**Skew test.** For nonparallel lines, let $w=p_2-p_1$. If $w\cdot(v_1\times v_2)$ is nonzero, no plane contains both lines, so they are skew. Here

Compute

$$
w=p_2-p_1=(1,-1,1).
$$

Compute the cross product:

$$
\begin{aligned}
v_1\times v_2
&=
\begin{pmatrix}
(2)(-1)-(1)(1) \\
(1)(0)-(1)(-1) \\
(1)(1)-(2)(0) \\
\end{pmatrix} \\
&=(-3,1,1).
\end{aligned}
$$

The scalar triple product is

$$
\begin{aligned}
w\cdot(v_1\times v_2)
&=(1,-1,1)\cdot(-3,1,1) \\
&=-3-1+1 \\
&=-3.
\end{aligned}
$$

Since $-3\neq0$, the lines are not coplanar.

## Verification

The coordinate equations are inconsistent, and the independent scalar-triple-product test is nonzero. Both checks agree that the lines do not meet.

## Geometric Interpretation

The two lines have different directions and occupy noncoplanar positions. They are skew rather than intersecting or parallel.

## Final Answer

$L_1$ and $L_2$ are skew lines. They are not parallel and have no intersection point.
