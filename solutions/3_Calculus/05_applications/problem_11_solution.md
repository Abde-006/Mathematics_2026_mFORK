# Problem 11. Volume of a Solid of Revolution

The region under

$$
y=\sqrt{x},\qquad 0\le x\le4,
$$

is rotated about the $x$-axis. Construct and evaluate the volume integral using the disk method.

## Quantities

Let $x$ be a coordinate in $[0,4]$, $y=\sqrt{x}$ the radius of the circular cross-section at $x$, $A(x)$ the cross-sectional area, $dx$ a small disk thickness, and $V$ the volume.

## Step 1 - Explain and construct the disk integral

At fixed $x$, rotation of the vertical segment creates a circular disk with radius $y$. The area formula for a circle,

$$
A(x)=\pi y^2,
$$

applies because it gives the area of the cross-section. Multiplying this area by the small thickness $dx$ gives the disk volume

$$
dV=A(x)\,dx=\pi y^2\,dx.
$$

Using $y=\sqrt{x}$ and adding these disks from $x=0$ to $x=4$,

$$
\begin{aligned}
V
&=\int_0^4\pi(\sqrt{x})^2\,dx \\
&=\pi\int_0^4x\,dx.
\end{aligned}
$$

## Step 2 - Compute the volume

The power-rule antiderivative of $x$ is $x^2/2$, so

$$
\begin{aligned}
V
&=\pi\left[\frac{x^2}{2}\right]_0^4 \\
&=\pi\left(\frac{16}{2}-0\right) \\
&=8\pi.
\end{aligned}
$$

## Verification

At $x=4$, the radius is $\sqrt4=2$, giving disk area $4\pi$. The integral $\pi\int_0^4x\,dx$ has positive area and evaluates consistently to $8\pi$.

## Interpretation

The factor $\pi y^2$ is not an arbitrary volume formula; it is the area of the circular cross-section, $\pi$ times the square of the radius $y$. The integral sums $\pi y^2\,dx$ over the thicknesses that make up the solid.

## Final answer

The volume is $8\pi$.
