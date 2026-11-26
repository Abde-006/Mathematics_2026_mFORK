# Problem 5. Distance from Velocity

The velocity of a car during the first five seconds is

$$
v(t)=4t+2\qquad [\mathrm{m/s}],\qquad 0\le t\le5.
$$

Compute the displacement and explain the integral interpretation and the change needed if velocity may be negative.

## Quantities

Let $t$ be time in seconds, $v(t)$ velocity in meters per second, $s(t)$ position in meters, and $\Delta s=s(5)-s(0)$ displacement.

## Step 1 - Compute displacement

Velocity is the derivative of position, $v(t)=s'(t)$. The Fundamental Theorem of Calculus therefore gives displacement as the signed integral of velocity:

$$
\Delta s=\int_0^5v(t)\,dt.
$$

Substituting $v(t)=4t+2$,

$$
\begin{aligned}
\Delta s
&=\int_0^5(4t+2)\,dt \\
&=\left[2t^2+2t\right]_0^5 \\
&=\left(2(25)+2(5)\right)-0 \\
&=60\ \mathrm{m}.
\end{aligned}
$$

This theorem applies because integrating the position rate $s'(t)$ over time reconstructs the change $s(5)-s(0)$.

## Step 2 - State the negative-velocity modification

The integral of velocity remains displacement regardless of sign. If velocity is negative on part of the interval, those parts reduce displacement rather than contribute positively to total distance.

The signed calculation is

$$
\Delta s=\int_0^5v(t)\,dt,
$$

whereas actual distance is the integral of speed:

$$
D=\int_0^5|v(t)|\,dt.
$$

The absolute value makes motion in the negative direction contribute a positive length.

## Verification

Here $v(t)=4t+2\ge2$ for $0\le t\le5$, so velocity never becomes negative. Consequently $|v(t)|=v(t)$ and

$$
D=\int_0^5(4t+2)\,dt=60\ \mathrm{m}.
$$

## Interpretation

On the given interval, displacement and actual distance coincide. If negative velocity occurs, the two quantities differ.

## Final answer

The displacement is $60\,\mathrm{m}$, and the actual distance is also $60\,\mathrm{m}$ for the stated positive velocity. For negative velocities, use $\int |v(t)|\,dt$ for distance.
