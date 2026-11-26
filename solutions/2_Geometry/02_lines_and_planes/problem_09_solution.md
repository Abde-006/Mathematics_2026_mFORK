# Exercise 9 — Distances

## Problem Statement

Compute:

1. the distance from $P=(2,3)$ to the line $3x+4y-10=0$;
2. the distance from $Q=(2,-1,3)$ to the plane $2x-2y+z-4=0$.

Compare the formulas and explain their connection with normal directions.

## Lettered Quantities

**Line**

- Let $P=(x_P,y_P)=(2,3)$.
- Let $\ell:a x+b y+c=0$ with $a=3$, $b=4$, $c=-10$.
- Let $n_\ell=(a,b)$ be the line normal.
- Let $d_\ell$ be the distance from $P$ to $\ell$.

**Plane**

- Let $Q=(x_Q,y_Q,z_Q)=(2,-1,3)$.
- Let $\Pi:a x+b y+c z+d=0$ with $a=2$, $b=-2$, $c=1$, $d=-4$.
- Let $n_\Pi=(a,b,c)$ be the plane normal.
- Let $d_\Pi$ be the distance from $Q$ to $\Pi$.

## Step 1 — Compute the Distance to the Line

**Point-to-line distance formula.** For $ax+by+c=0$, the absolute normal residual $|ax_P+by_P+c|$ measures signed displacement; dividing by $\lVert(a,b)\rVert$ converts it to perpendicular distance. Use $P=(2,3)$:

Substitute $P=(2,3)$ and $\ell:3x+4y-10=0$:

$$
\begin{aligned}
a x_P+b y_P+c
&=3(2)+4(3)-10 \\
&=6+12-10 \\
&=8.
\end{aligned}
$$

The normal length is

$$
\sqrt{a^2+b^2}
=\sqrt{3^2+4^2}
=\sqrt{25}
=5.
$$

Therefore

$$
d_\ell=\frac{|8|}{5}=\frac85.
$$

## Step 2 — Compute the Distance to the Plane

**Point-to-plane distance formula.** For $ax+by+cz+d=0$, the formula $|ax_Q+by_Q+cz_Q+d|/\lVert(a,b,c)\rVert$ has the same normal-residual interpretation in three dimensions. Substitute $Q=(2,-1,3)$:

Substitute $Q=(2,-1,3)$ and $2x-2y+z-4=0$:

$$
\begin{aligned}
a x_Q+b y_Q+c z_Q+d
&=2(2)-2(-1)+(1)(3)-4 \\
&=4+2+3-4 \\
&=5.
\end{aligned}
$$

The normal length is

$$
\begin{aligned}
\sqrt{a^2+b^2+c^2}
&=\sqrt{2^2+(-2)^2+1^2} \\
&=\sqrt{4+4+1} \\
&=\sqrt9 \\
&=3.
\end{aligned}
$$

Therefore

$$
d_\Pi=\frac{|5|}{3}=\frac53.
$$

## Verification

Both denominators are positive normal lengths. Absolute values make the distances nonnegative. Each residual measures signed displacement of the point in the normal equation.

## Geometric Interpretation

The shortest segment from a point to a line or plane is perpendicular to the object. The normal vector gives that direction. Dividing the absolute residual by the normal length turns an equation value into a perpendicular Euclidean distance.

## Final Answer

- The distance from $P=(2,3)$ to $3x+4y-10=0$ is $\frac85$.
- The distance from $Q=(2,-1,3)$ to $2x-2y+z-4=0$ is $\frac53$.
