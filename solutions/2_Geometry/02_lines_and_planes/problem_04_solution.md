# Exercise 4 — Plane Through Three Points

## Problem Statement

Find the plane through

$$
A=(1,0,0),\qquad B=(0,1,0),\qquad C=(0,0,1).
$$

Construct two vectors in the plane, use their cross product, and check the equation at all three points.

## Lettered Quantities

- Let $A=(1,0,0)$, $B=(0,1,0)$, and $C=(0,0,1)$.
- Let $\vec u=\overrightarrow{AB}$ and $\vec w=\overrightarrow{AC}$.
- Let $n=\vec u\times\vec w$ be a normal vector.
- Let $X=(x,y,z)$ be a general point.

## Step 1 — Construct Two Plane Directions

**In-plane displacement vectors.** The differences $B-A$ and $C-A$ point from $A$ to two other points in the plane, so they are two directions of the plane. Use $A=(1,0,0)$, $B=(0,1,0)$, and $C=(0,0,1)$:

Using $A=(1,0,0)$,

$$
\begin{aligned}
\vec u&=B-A=(-1,1,0), \\
\vec w&=C-A=(-1,0,1).
\end{aligned}
$$

They are not scalar multiples, so they determine two independent directions.

## Step 2 — Compute a Normal Vector

**Cross product as normal.** A cross product $u\times w$ is perpendicular to both $u$ and $w$, so it supplies a normal to their plane. With $u=(-1,1,0)$ and $w=(-1,0,1)$, compute

Substitute $\vec u=(-1,1,0)$ and $\vec w=(-1,0,1)$:

$$
\begin{aligned}
n
&=\vec u\times\vec w \\
&=
\begin{pmatrix}
(1)(1)-(0)(0) \\
(0)(-1)-(-1)(1) \\
(-1)(0)-(1)(-1) \\
\end{pmatrix} \\
&=(1,1,1).
\end{aligned}
$$

## Step 3 — Form the Plane Equation

**Point-normal plane equation.** A normal $n$ gives $n\cdot(X-A)=0$, because $X-A$ lies in the plane exactly when it is perpendicular to $n$. Substitute $n$ and $A$:

Using $n=(1,1,1)$ and $A=(1,0,0)$,

$$
(1,1,1)\cdot(x-1,y,z)=0.
$$

Hence

$$
x-1+y+z=0,
$$

and therefore

$$
x+y+z=1.
$$

## Verification

For $A=(1,0,0)$:

$$
1+0+0=1.
$$

For $B=(0,1,0)$:

$$
0+1+0=1.
$$

For $C=(0,0,1)$:

$$
0+0+1=1.
$$

The normal is also perpendicular to both plane directions:

$$
\begin{aligned}
n\cdot\vec u&=(1,1,1)\cdot(-1,1,0)=-1+1+0=0, \\
n\cdot\vec w&=(1,1,1)\cdot(-1,0,1)=-1+0+1=0.
\end{aligned}
$$

## Geometric Interpretation

The plane intercepts each coordinate axis at unit distance. Its normal $(1,1,1)$ is perpendicular to both $\overrightarrow{AB}$ and $\overrightarrow{AC}$.

## Final Answer

$$
x+y+z=1.
$$
