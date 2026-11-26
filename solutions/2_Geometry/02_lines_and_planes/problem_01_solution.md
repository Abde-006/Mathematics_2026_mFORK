# Exercise 1 — Line Through Two Points

## Problem Statement

Find the line through $A=(1,2)$ and $B=(4,-1)$ in parametric and general form. Identify a direction vector and a normal vector, and check that both points satisfy the general equation.

## Lettered Quantities

- Let $A=(a_1,a_2)=(1,2)$ and $B=(b_1,b_2)=(4,-1)$.
- Let $\vec v=(v_1,v_2)$ denote a direction vector.
- Let $\vec n=(n_1,n_2)$ denote a normal vector.
- Let $X=(x,y)$ denote an arbitrary point in the plane.

## Step 1 — Compute a Direction Vector

**Vector difference for the direction.** Subtracting the starting point $A$ from the endpoint $B$ gives the displacement $\vec v=B-A=(b_1-a_1,b_2-a_2)$, parallel to the line. Substitution gives

Substitute $A=(1,2)$ and $B=(4,-1)$:

$$
\begin{aligned}
\vec v
&=B-A \\
&=(4-1,-1-2) \\
&=(3,-3).
\end{aligned}
$$

The vector $(3,-3)$ is a valid direction vector. Dividing by $3$ gives the simpler direction

$$
\vec v=(1,-1).
$$

## Step 2 — Construct the Parametric Equation

**Parametric line form.** A point $X$ on the line through $A$ in direction $\vec v$ is $X=A+t\vec v$, $t\in\mathbb R$. Substituting $A$ and $\vec v$ gives

Using $A=(1,2)$ and $\vec v=(1,-1)$,

$$
(x,y)=(1,2)+t(1,-1),
$$

or, in coordinate form,

$$
\begin{aligned}
x&=1+t, \\
y&=2-t.
\end{aligned}
$$

## Step 3 — Construct a Normal Vector and General Equation

**Point-normal form.** A normal $\vec n=(n_1,n_2)$ is perpendicular to every direction on the line, so a point $X=(x,y)$ satisfies $\vec n\cdot(X-A)=0$. Using $A$ and $\vec n=(1,1)$ gives

Choose $\vec n=(1,1)$. It is perpendicular to $\vec v$ because

$$
\vec n\cdot\vec v=(1)(1)+(1)(-1)=0.
$$

The normal equation through $A=(1,2)$ is

$$
\begin{aligned}
(1)(x-1)+(1)(y-2)&=0, \\
x-1+y-2&=0, \\
x+y-3&=0.
\end{aligned}
$$

## Verification

Substitute $A=(1,2)$:

$$
1+2-3=0.
$$

Substitute $B=(4,-1)$:

$$
4+(-1)-3=0.
$$

Both points satisfy the general equation. Also, $t=0$ in the parametric equation gives $A$, while $t=3$ gives

$$
(1,2)+3(1,-1)=(4,-1)=B.
$$

## Geometric Interpretation

The line is an affine line in $\mathbb R^2$ directed by $(1,-1)$. Its normal $(1,1)$ is perpendicular to every direction on the line, so $x+y=3$ is the collection of all points reached by moving from $A$ in directions perpendicular to $(1,-1)$.

## Final Answer

Parametric form:

$$
(x,y)=(1,2)+t(1,-1),\qquad t\in\mathbb R.
$$

General form:

$$
x+y-3=0.
$$

A direction vector is $(1,-1)$, and a normal vector is $(1,1)$.