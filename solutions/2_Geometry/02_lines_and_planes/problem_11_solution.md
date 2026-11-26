# Exercise 11 — Plane Containing a Line and a Point

## Problem Statement

Find the plane containing

$$
L:(x,y,z)=(1,0,2)+t(1,1,-1)
$$

and the point $P=(0,2,1)$. Check that the entire line and $P$ lie in the plane.

## Lettered Quantities

- Let $A=(1,0,2)$ be a point on $L$.
- Let $v=(1,1,-1)$ be the direction of $L$.
- Let $P=(0,2,1)$ be the additional point.
- Let $w=P-A$ be a second direction in the plane.
- Let $n=v\times w$ be a normal vector.

## Step 1 — Find Two Independent Directions

**Two independent directions.** One direction is $v=(1,1,-1)$ along the given line. A second is $w=P-A$ from a point $A$ on the line to $P$; it is independent of $v$ for a plane not already containing $P$.

The line supplies $v=(1,1,-1)$. The additional direction is

$$
\begin{aligned}
w
&=P-A \\
&=(0-1,2-0,1-2) \\
&=(-1,2,-1).
\end{aligned}
$$

The vectors $v$ and $w$ are not scalar multiples, so they span a plane.

## Step 2 — Compute a Normal Vector

**Cross product as normal reminder.** $n=v\times w$ is perpendicular to both independent plane directions, so it is a normal to the plane. Compute

Compute

$$
\begin{aligned}
n
&=v\times w \\
&=
\begin{pmatrix}
(1)(-1)-(-1)(2) \\
(-1)(-1)-(1)(-1) \\
(1)(2)-(1)(-1) \\
\end{pmatrix} \\
&=(1,2,3).
\end{aligned}
$$

## Step 3 — Write the Plane Equation

**Point-normal equation reminder.** With normal $n$ and base point $A$, a plane point $X$ satisfies $n\cdot(X-A)=0$. Substitute

Using $n=(1,2,3)$ and $A=(1,0,2)$,

$$
(1,2,3)\cdot(x-1,y,z-2)=0.
$$

Expand:

$$
(x-1)+2y+3(z-2)=0.
$$

Thus

$$
x-1+2y+3z-6=0,
$$

and hence

$$
x+2y+3z=7.
$$

## Verification

Substitute $P=(0,2,1)$:

$$
0+2(2)+3(1)=0+4+3=7.
$$

Substitute $A=(1,0,2)$:

$$
1+2(0)+3(2)=1+6=7.
$$

The line direction is perpendicular to $n$:

$$
n\cdot v=(1,2,3)\cdot(1,1,-1)=1+2-3=0.
$$

Therefore, for every $t$,

$$
n\cdot(A+t v)=n\cdot A+t(n\cdot v)=7+0=7.
$$

## Geometric Interpretation

The cross product of $v$ and $w=P-A$ is normal to the plane. Consequently $L$ and $P$ determine a unique plane if $P$ is not on $L$, which is the case here.

## Final Answer

The plane is

$$
x+2y+3z=7.
$$
