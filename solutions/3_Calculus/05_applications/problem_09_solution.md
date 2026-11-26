# Problem 9. Minimizing the Material Used for a Can

A closed cylinder has fixed volume $V$. Find the relation between its height $h$ and radius $r$ that minimizes total surface area.

## Quantities

Let $r>0$ be the radius, $h>0$ the height, $V>0$ the fixed volume, and $S$ the total surface area.

## Step 1 - Write the volume constraint

The volume of a cylinder is base area times height:

$$
V=\pi r^2h.
$$

Solving for $h$ gives

$$
h=\frac{V}{\pi r^2}.
$$

This constraint expresses height in terms of radius so that surface area has only one independent variable.

## Step 2 - Express surface area as a function of radius

The closed cylinder has two circular ends and one curved side:

$$
S=2\pi r^2+2\pi rh.
$$

Substitute $h=V/(\pi r^2)$:

$$
\begin{aligned}
S(r)
&=2\pi r^2+2\pi r\left(\frac{V}{\pi r^2}\right) \\
&=2\pi r^2+\frac{2V}{r}.
\end{aligned}
$$

## Step 3 - Find the minimizing radius

An interior minimum of the differentiable function $S(r)$ can occur where $S'(r)=0$. Differentiating,

$$
S'(r)=4\pi r-\frac{2V}{r^2}.
$$

Solving $S'(r)=0$,

$$
\begin{aligned}
4\pi r-\frac{2V}{r^2}&=0, \\
4\pi r^3-2V&=0, \\
r^3&=\frac{V}{2\pi}.
\end{aligned}
$$

Thus

$$
r=\left(\frac{V}{2\pi}\right)^{1/3}.
$$

## Step 4 - Verify the minimum and find the height

The second derivative tests whether the critical point is concave upward:

$$
S''(r)=4\pi+\frac{4V}{r^3}>0
$$

for $r>0$ and $V>0$. Hence the critical radius gives a strict global minimum on $r>0$.

The second volume relation $V=\pi r^2h$ is reused. From $r^3=V/(2\pi)$,

$$
V=2\pi r^3.
$$

Therefore

$$
\begin{aligned}
h
&=\frac{V}{\pi r^2} \\
&=\frac{2\pi r^3}{\pi r^2} \\
&=2r.
\end{aligned}
$$

## Verification

The optimized height equals the diameter $2r$. Substitution into the volume constraint gives

$$
\pi r^2(2r)=2\pi r^3=V,
$$

which confirms consistency with the fixed volume.

## Geometric interpretation

The minimum-material can has the same height as its diameter. A cross-section through its axis is a square.

## Final answer

The minimizing relation is $h=2r$.
