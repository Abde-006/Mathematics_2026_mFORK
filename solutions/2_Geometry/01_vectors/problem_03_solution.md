## Exercise 3 — Vector Normalization

### Problem statement

For $v=(3,4)$, find a unit vector $e$ in the same direction and with the same orientation. Check $\|e\|=1$, reconstruct $v=\|v\|e$, and explain what normalization changes.

### Formula used

For a nonzero vector $v$, a unit vector in the same direction is

$$
e=\frac{v}{\|v\|}
$$

The length formula in $\mathbb R^2$ is

$$
\|(x,y)\|=\sqrt{x^2+y^2}
$$

Dividing by $\|v\|$ changes the magnitude to $1$ while preserving the ratios of the coordinates, and therefore preserves direction and orientation.

### Solution

Calculate the length of $v$:

$$
\|v\|=\sqrt{3^2+4^2}=\sqrt{25}=5
$$

Divide each coordinate by $5$:

$$
e=\frac{(3,4)}{5}
=\left(\frac{3}{5},\frac{4}{5}\right)
$$

Check the unit length:

$$
\|e\|
=\sqrt{\left(\frac{3}{5}\right)^2+\left(\frac{4}{5}\right)^2}
=\sqrt{\frac{9}{25}+\frac{16}{25}}
=1
$$

Reconstruct $v$:

$$
\|v\|e
=5\left(\frac{3}{5},\frac{4}{5}\right)
=(3,4)
=v
$$

### Interpretation

Normalization removes the magnitude while keeping the direction. Multiplication by $\|v\|=5$ restores the original length. The vector becomes $v=5e$, where $e$ describes only direction and $5$ describes magnitude.

### Final answer

$$
e=\left(\frac{3}{5},\frac{4}{5}\right)
$$

$$
\|e\|=1,\qquad v=5e
$$
