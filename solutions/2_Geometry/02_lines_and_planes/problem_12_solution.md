# Exercise 12 — Intersection Line of Two Planes

## Problem Statement

Find a parametric equation of the intersection of

$$
x+y+z=3,\qquad x-y+z=1.
$$

Find the direction vector in two ways: from the system and from the cross product of the normals. Compare the results.

## Lettered Quantities

- Let $\Pi_1:x+y+z=3$ with normal $n_1=(1,1,1)$.
- Let $\Pi_2:x-y+z=1$ with normal $n_2=(1,-1,1)$.
- Let $X=(x,y,z)$ be a point on the intersection.
- Let $p$ be a known point on the intersection and $v$ its direction.

## Step 1 — Solve the System Algebraically

**Algebraic plane intersection.** A point of the intersection must satisfy both plane equations. Solving the system gives the line in parametric form. Write

Subtract the second equation from the first:

$$
\begin{aligned}
(x+y+z)-(x-y+z)&=3-1, \\
2y&=2.
\end{aligned}
$$

Hence

$$
y=1.
$$

Substitute $y=1$ into $x+y+z=3$:

$$
x+1+z=3,
$$

so

$$
x+z=2.
$$

Set $x=t$. Then

$$
z=2-t.
$$

Thus the intersection line is

$$
\begin{aligned}
(x,y,z)
&=(t,1,2-t) \\
&=(0,1,2)+t(1,0,-1).
\end{aligned}
$$

Its direction from the system is

$$
v_{\mathrm{system}}=(1,0,-1).
$$

## Step 2 — Compute the Direction by Cross Product

**Cross-product direction.** The intersection line is perpendicular to both plane normals, so $v=n_1\times n_2$ is its direction. The normals are $n_1=(1,1,1)$ and $n_2=(1,-1,1)$:

Compute

$$
\begin{aligned}
n_1\times n_2
&=
\begin{pmatrix}
(1)(1)-(1)(-1) \\
(1)(1)-(1)(1) \\
(1)(-1)-(1)(1) \\
\end{pmatrix} \\
&=(2,0,-2).
\end{aligned}
$$

Thus

$$
v_{\mathrm{cross}}=(2,0,-2)=2(1,0,-1).
$$

## Verification

At $p=(0,1,2)$,

$$
0+1+2=3,
$$

and

$$
0-1+2=1.
$$

Therefore $p$ lies on both planes.

The system-derived direction satisfies

$$
\begin{aligned}
n_1\cdot v_{\mathrm{system}}&=(1,1,1)\cdot(1,0,-1)=1-1=0, \\
n_2\cdot v_{\mathrm{system}}&=(1,-1,1)\cdot(1,0,-1)=1-1=0.
\end{aligned}
$$

Hence it is perpendicular to both normals.

For every $t$,

$$
\begin{aligned}
t+(1)+(2-t)&=3, \\
t-1+(2-t)&=1.
\end{aligned}
$$

## Geometric Interpretation

Two nonparallel planes intersect along a line. That line is perpendicular to both plane normals, so its direction is parallel to their cross product.

## Final Answer

The intersection line is

$$
(x,y,z)=(0,1,2)+t(1,0,-1),\qquad t\in\mathbb R.
$$

The cross product gives $(2,0,-2)$, which is the scalar multiple $2(1,0,-1)$ and therefore the same direction.
