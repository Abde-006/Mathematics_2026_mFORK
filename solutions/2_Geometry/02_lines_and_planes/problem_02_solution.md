# Exercise 2 — A Line in Space

## Problem Statement

Given

$$
L:(x,y,z)=(2,-1,3)+t(1,2,-2),
$$

state a point on the line and its direction vector, determine whether $P=(4,3,-1)$ lies on $L$, and find the point corresponding to $t=-1$.

## Lettered Quantities

- Let $p=(p_1,p_2,p_3)=(2,-1,3)$ be the base point.
- Let $v=(v_1,v_2,v_3)=(1,2,-2)$ be the direction vector.
- Let $P=(x_P,y_P,z_P)=(4,3,-1)$ be the point to test.
- Let $t$ be the real parameter.

## Step 1 — Read the Base Point and Direction

**Parametric point form.** A point $X=p+t v$ lies on $L$ when $X$ is the given base point plus a scalar multiple of the direction. Here $p=(2,-1,3)$ and $v=(1,2,-2)$, so

The given equation is already of the form $p+t v$. Therefore

$$
p=(2,-1,3)
$$

is a point on $L$, and

$$
v=(1,2,-2)
$$

is a direction vector. The coordinate equations are

$$
\begin{aligned}
x&=2+t, \\
y&=-1+2t, \\
z&=3-2t.
\end{aligned}
$$

## Step 2 — Test Whether $P$ Lies on $L$

**Parameter test.** Use the reminder $X=p+t v$: $P$ lies on $L$ exactly when the same real $t$ produces all three coordinates. Compare

Set the $x$-coordinate equal to $4$:

$$
2+t=4,
$$

so

$$
t=4-2=2.
$$

Substitute $t=2$ into the remaining coordinates:

$$
\begin{aligned}
y&=-1+2(2)=3, \\
z&=3-2(2)=-1.
\end{aligned}
$$

Thus $P$ is obtained with the same parameter in all three coordinates.

## Step 3 — Find the Point for $t=-1$

**Evaluate a parameter.** In the parametric formula $X=p+t v$, substituting $t=-1$ gives

Substitute $t=-1$:

$$
\begin{aligned}
(x,y,z)
&=(2,-1,3)+(-1)(1,2,-2) \\
&=(2,-1,3)-(1,2,-2) \\
&=(2-1,-1-2,3-(-2)) \\
&=(1,-3,5).
\end{aligned}
$$

## Verification

At $t=2$,

$$
(2, -1, 3)+2(1,2,-2)
=(2+2,-1+4,3-4)
=(4,3,-1).
$$

At $t=-1$, the calculation gives $(1,-3,5)$ directly. No coordinate conflict occurs.

## Geometric Interpretation

The line passes through $p=(2,-1,3)$ and extends in the direction $v=(1,2,-2)$. The parameter $t=2$ reaches $P$, while $t=-1$ reaches the point in the opposite direction.

## Final Answer

A point on $L$ is $(2,-1,3)$, and a direction vector is $(1,2,-2)$.

The point $P=(4,3,-1)$ lies on $L$ at $t=2$.

The point corresponding to $t=-1$ is $(1,-3,5)$.