# Exercise 15 — Complete Classification of a Line Relative to a Plane

## Problem Statement

Let

$$
L:p+t v,\qquad \Pi:n\cdot X=d.
$$

State the conditions for one intersection point, a parallel disjoint line, and containment. Illustrate each case with a numerical example.

## Lettered Quantities

- Let $p=(p_1,p_2,p_3)$ be a point on $L$.
- Let $v=(v_1,v_2,v_3)$ be the direction of $L$.
- Let $n=(n_1,n_2,n_3)$ be the plane normal.
- Let $d$ be the plane constant.
- Let $t\in\mathbb R$ be the line parameter.

## Step 1 — State the Three Cases

**Substitution criterion.** Substituting $X=p+t v$ in $n\cdot X=d$ gives $n\cdot p+t(n\cdot v)=d$, equivalently $t(n\cdot v)=d-n\cdot p$. This linear equation determines the number of intersections. State the cases:

**One intersection point**

If

$$
n\cdot v\neq0,
$$

the equation has the unique solution

$$
t=\frac{d-n\cdot p}{n\cdot v}.
$$

The unique point is $p+t v$.

**Parallel with no common point**

If

$$
n\cdot v=0
$$

and

$$
n\cdot p\neq d,
$$

the substituted equation becomes

$$
n\cdot p=d,
$$

but $n\cdot p\neq d$, so it is impossible for any $t$. The line is parallel and disjoint.

**Line contained in the plane**

If

$$
n\cdot v=0
$$

and

$$
n\cdot p=d,
$$

the equation holds for every $t$. The base point and every point reached from it by $v$ lie in the plane.

## Step 2 — Give a Numerical Example of One Intersection

**One-intersection example.** This case requires $n\cdot v\neq0$, so the equation has the unique solution $t=(d-n\cdot p)/(n\cdot v)$. Use

Use

$$
\Pi:z=0,\qquad n=(0,0,1),\qquad d=0.
$$

Take

$$
p=(0,0,1),\qquad v=(1,0,-1).
$$

Then

$$
n\cdot v=-1\neq0.
$$

Compute $n\cdot p=(0,0,1)\cdot(0,0,1)=1$. The parameter is therefore

$$
t=\frac{d-n\cdot p}{n\cdot v}
=\frac{0-1}{-1}
=1.
$$

At $t=1$, the intersection is $(1,0,0)$.

## Step 3 — Give a Parallel Disjoint Example

**Parallel-disjoint example.** This case uses $n\cdot v=0$ and $n\cdot p\neq d$, making $0=d-n\cdot p$ impossible. Use

Use $\Pi:z=0$, $n=(0,0,1)$, $d=0$. Take

$$
p=(0,0,1),\qquad v=(1,2,0).
$$

Then

$$
n\cdot v=0,\qquad n\cdot p=1\neq0.
$$

Every point has $z=1$, so $L$ is parallel and has no point in $z=0$.

## Step 4 — Give a Contained-Line Example

**Contained-line example.** Here $n\cdot v=0$ and $n\cdot p=d$, so every real $t$ satisfies the substitution equation. Use

Use $\Pi:z=0$, $n=(0,0,1)$, $d=0$. Take

$$
p=(1,0,0),\qquad v=(1,1,0).
$$

Then

$$
n\cdot v=0,\qquad n\cdot p=0=d.
$$

The line is

$$
(x,y,z)=(1+t,t,0),
$$

and every point has $z=0$.

## Verification

In the intersection example, $z=1-t$, so $z=0$ at exactly $t=1$. In the disjoint example, $z=1$ for every $t$. In the contained example, $z=0$ for every $t$. These checks correspond exactly to the classification conditions.

## Geometric Interpretation

The dot product $n\cdot v$ measures whether the line direction has a component perpendicular to the plane. A nonzero component crosses the plane once. A zero component keeps the signed plane residual constant, giving either no points or every point.

## Final Answer

- $n\cdot v\neq0$: exactly one intersection at

$$
t=\frac{d-n\cdot p}{n\cdot v}.
$$

- $n\cdot v=0$ and $n\cdot p\neq d$: parallel with no common points.
- $n\cdot v=0$ and $n\cdot p=d$: the line is contained in the plane.
