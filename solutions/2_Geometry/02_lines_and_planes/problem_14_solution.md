# Exercise 14 — Contrast: Intersection and Parallelism

## Problem Statement

From $P=(0,0,1)$, draw lines with direction vectors

$$
v_1=(2,1,-1),\qquad v_2=(2,1,0).
$$

For each line, analyze its position relative to the plane $z=0$. Find the intersection point for the line that intersects the plane. Explain parallelism of the other line without solving an equation.

## Lettered Quantities

- Let $P=(0,0,1)$ be the common base point.
- Let $v_1=(2,1,-1)$ define $L_1$.
- Let $v_2=(2,1,0)$ define $L_2$.
- Let $n=(0,0,1)$ be the normal of $\Pi:z=0$.

## Step 1 — Analyze $L_1$

**Line-plane substitution test.** Substituting $X=P+t v$ into $n\cdot X=0$ gives $n\cdot P+t(n\cdot v)=0$. For $z=0$, $n=(0,0,1)$, so

The first line is

$$
L_1:P+t v_1=(2t,t,1-t).
$$

Compute

$$
n\cdot v_1=(0,0,1)\cdot(2,1,-1)=-1\neq0.
$$

Therefore $L_1$ intersects $z=0$ once.

Set $z=0$:

$$
1-t=0,
$$

so

$$
t=1.
$$

Substitute $t=1$:

$$
(x,y,z)=(2(1),1,1-1)=(2,1,0).
$$

## Step 2 — Analyze $L_2$

**Use the dot-product criterion.** $n\cdot v=0$ means the direction is perpendicular to $n$, hence parallel to the plane. With $n\cdot P=1$, no point is on $z=0$, so apply

The second line is

$$
L_2:P+t v_2=(2t,t,1).
$$

Compute

$$
n\cdot v_2=(0,0,1)\cdot(2,1,0)=0.
$$

Therefore $v_2$ is parallel to $z=0$. In fact, every point on $L_2$ has

$$
z=1.
$$

Since $P=(0,0,1)$ is not on $z=0$, $L_2$ is parallel and disjoint, not contained.

## Verification

At $t=1$, $L_1$ gives $(2,1,0)$, which satisfies $z=0$.

At every $t$, $L_2$ gives $z=1$, so no point satisfies $z=0$.

## Geometric Interpretation

Although $v_1$ and $v_2$ differ only in their $z$ components, that component decides the result. A nonzero normal component allows $z$ to change and cross $z=0$, while a zero normal component keeps $z$ constant.

## Final Answer

- $L_1$ intersects $z=0$ at $(2,1,0)$.
- $L_2$ is parallel to $z=0$ and has no common points.
