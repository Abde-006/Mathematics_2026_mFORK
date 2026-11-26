## Exercise 14 — Closest Point on a Line

### Problem statement

Given point $P=(4,1)$ and the line through the origin with direction $v=(1,2)$:

1. Use projection to find the closest point $Q$ on the line.
2. Find the distance from $P$ to the line.
3. Verify that $P-Q$ is perpendicular to $v$.

### Formula used

The line is

$$
\ell=\{tv:t\in\mathbb R\}
$$

The closest point is the orthogonal projection

$$
Q=\mathrm{proj}_v P
=\frac{P\cdot v}{v\cdot v}v
$$

The distance is the length of the perpendicular displacement:

$$
d(P,\ell)=\|P-Q\|
$$

Finally, the residual should satisfy

$$
(P-Q)\cdot v=0
$$

### Solution

Compute the dot products:

$$
P\cdot v=4(1)+1(2)=6
$$

$$
v\cdot v=1^2+2^2=5
$$

Then

$$
Q
=\frac{6}{5}(1,2)
=\left(\frac{6}{5},\frac{12}{5}\right)
$$

Construct $P-Q$:

$$
\begin{aligned}
P-Q
&=\left(4-\frac{6}{5},1-\frac{12}{5}\right) \\
&=\left(\frac{20-6}{5},\frac{5-12}{5}\right) \\
&=\left(\frac{14}{5},-\frac{7}{5}\right)
\end{aligned}
$$

Compute the distance:

$$
\begin{aligned}
d(P,\ell)
&=\|P-Q\| \\
&=\sqrt{\left(\frac{14}{5}\right)^2+
\left(-\frac{7}{5}\right)^2} \\
&=\sqrt{\frac{196+49}{25}} \\
&=\sqrt{\frac{245}{25}} \\
&=\frac{7\sqrt{5}}{5}
\end{aligned}
$$

### Verification

Check perpendicularity:

$$
(P-Q)\cdot v
=\left(\frac{14}{5},-\frac{7}{5}\right)\cdot(1,2)
=\frac{14}{5}-\frac{14}{5}
=0
$$

A displacement perpendicular to the line cannot be reduced by moving along the line, so $Q$ is the closest point.

### Final answer

$$
Q=\left(\frac{6}{5},\frac{12}{5}\right)
$$

$$
d(P,\ell)=\frac{7\sqrt{5}}{5}
$$
