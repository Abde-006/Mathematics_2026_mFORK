## Exercise 5 — Angle Between Vectors

### Problem statement

For $u=(1,1,0)$ and $v=(1,0,1)$:

1. Use the sign of $u\cdot v$ to predict the angle type.
2. Compute the angle.
3. Compare it with the prediction.

### Formula used

The dot product determines both the sign and cosine of the angle:

$$
u\cdot v=\|u\|\|v\|\cos\theta
$$

Therefore

$$
\cos\theta=\frac{u\cdot v}{\|u\|\|v\|}
$$

The sign of $u\cdot v$ predicts the angle type:

- Positive: acute angle.
- Zero: right angle.
- Negative: obtuse angle.

### Solution

First use the sign for prediction:

$$
u\cdot v=1(1)+1(0)+0(1)=1
$$

Because $u\cdot v>0$, the angle should be acute.

Find the lengths:

$$
\|u\|=\sqrt{1^2+1^2+0^2}=\sqrt{2}
$$

$$
\|v\|=\sqrt{1^2+0^2+1^2}=\sqrt{2}
$$

Substitute them into the angle formula:

$$
\cos\theta
=\frac{1}{\sqrt{2}\sqrt{2}}
=\frac{1}{2}
$$

For $0\leq\theta\leq\pi$,

$$
\theta=\cos^{-1}\left(\frac{1}{2}\right)
=\frac{\pi}{3}
=60^\circ
$$

### Verification

$60^\circ$ is less than $90^\circ$, so it is acute. This agrees with the positive dot product.

### Final answer

$$
\theta=60^\circ=\frac{\pi}{3}
$$
