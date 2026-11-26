# Exercise 7 — A Line Relative to a Plane

## Problem Statement

For

$$
L:(x,y,z)=(1,1,0)+t(1,-1,0),
\qquad
\Pi:x+y+z=2,
$$

determine whether $L$ intersects $\Pi$ at one point, is parallel to $\Pi$, or lies in $\Pi$. Explain the role of $v\cdot n$.

## Lettered Quantities

- Let $p=(1,1,0)$ be a point on $L$.
- Let $v=(1,-1,0)$ be the direction vector of $L$.
- Let $n=(1,1,1)$ be the normal of $\Pi$.
- Let $d=2$ be the plane constant.

## Step 1 — Test the Direction-Normal Dot Product

**Line-plane dot-product test.** Substituting $X=p+t v$ into $n\cdot X=d$ gives $n\cdot p+t(n\cdot v)=d$. The coefficient $n\cdot v$ tells whether $t$ can change the signed position in the normal direction. Thus use $v=(1,-1,0)$ and $n=(1,1,1)$:

Compute

$$
\begin{aligned}
n\cdot v
&=(1,1,1)\cdot(1,-1,0) \\
&=(1)(1)+(1)(-1)+(1)(0) \\
&=1-1+0 \\
&=0.
\end{aligned}
$$

A zero dot product means $v$ is parallel to $\Pi$. It does not yet distinguish containment from a disjoint parallel line.

## Step 2 — Test a Point on the Line

**Point membership test.** When $n\cdot v=0$, choose a point $X=p$ on $L$ and test $n\cdot p=d$: membership of one point plus parallelism determines whether the line lies in the plane. Substitute

For $p=(1,1,0)$,

$$
n\cdot p=(1,1,1)\cdot(1,1,0)=1+1+0=2=d.
$$

Therefore $p$ lies in $\Pi$.

## Step 3 — Check Every Point

**Criterion reminder.** If $n\cdot v=0$ and $n\cdot p=d$, every point $p+t v$ satisfies the plane equation. This is the containment case;

Since $n\cdot v=0$,

$$
n\cdot(p+t v)=n\cdot p+t(n\cdot v)=2+t(0)=2
$$

for every $t$. Thus every point on $L$ satisfies the plane equation.

## Verification

In coordinates,

$$
x=1+t,\qquad y=1-t,\qquad z=0.
$$

Therefore

$$
x+y+z=(1+t)+(1-t)+0=2.
$$

## Geometric Interpretation

The line direction $(1,-1,0)$ has no normal component, so movement along $L$ leaves the plane equation unchanged. Since $p$ is on the plane, the entire line lies in it.

## Final Answer

The line lies in the plane $x+y+z=2$.
