# Problem 1. Motion — from Position to Velocity

The position of a point is described by

$$
s(t)=t^3-6t^2+9t+2,\qquad t\ge 0.
$$

Determine its velocity and acceleration, the stopping times, and the intervals on which it moves in the positive and negative directions.

## Quantities

Let $t$ be time in seconds, $s(t)$ the position on the axis in distance units, $v(t)$ the velocity in distance units per second, and $a(t)$ the acceleration.

## Step 1 - Determine velocity and acceleration

Velocity is the instantaneous rate of change of position, so the derivative $v(t)=s'(t)$ is appropriate. Applying the power rule term by term gives

$$
\begin{aligned}
v(t)
&=s'(t) \\
&=\frac{d}{dt}(t^3-6t^2+9t+2) \\
&=3t^2-12t+9.
\end{aligned}
$$

Acceleration is the rate of change of velocity, so $a(t)=v'(t)=s''(t)$:

$$
\begin{aligned}
a(t)
&=v'(t) \\
&=\frac{d}{dt}(3t^2-12t+9) \\
&=6t-12.
\end{aligned}
$$

## Step 2 - Find the stopping times

A moving point stops when its velocity is zero, because zero velocity means that its instantaneous rate of change of position vanishes. Factor the velocity:

$$
\begin{aligned}
v(t)
&=3t^2-12t+9 \\
&=3(t^2-4t+3) \\
&=3(t-1)(t-3).
\end{aligned}
$$

For $t\ge0$, solving $v(t)=0$ gives $t=1$ or $t=3$.

## Step 3 - Determine direction of motion

The sign of velocity indicates direction: positive velocity is motion in the positive axis direction and negative velocity is motion in the negative direction. The factors $(t-1)$ and $(t-3)$ change sign at $1$ and $3$, respectively:

| Interval | Sign of $(t-1)$ | Sign of $(t-3)$ | Sign of $v(t)$ | Motion |
|---|---|---|---|---|
| $0\le t<1$ | negative | negative | positive | positive direction |
| $1<t<3$ | positive | negative | negative | negative direction |
| $t>3$ | positive | positive | positive | positive direction |

## Verification

The stopping times are genuine reversals, not merely zeros at isolated points. Using the acceleration found in Step 1,

$$
a(1)=6(1)-12=-6<0,
$$

so velocity changes from positive to negative at $t=1$, and

$$
a(3)=6(3)-12=6>0,
$$

so velocity changes from negative to positive at $t=3$.

## Interpretation

The point initially moves away in the positive direction, reverses at $t=1$, moves backward until $t=3$, and then reverses again.

## Final answer

The velocity is $v(t)=3t^2-12t+9$, and the acceleration is $a(t)=6t-12$.

and the point stops at $t=1$ and $t=3$ seconds. It moves in the positive direction for $0\le t<1$ and $t>3$, and in the negative direction for $1<t<3$.
