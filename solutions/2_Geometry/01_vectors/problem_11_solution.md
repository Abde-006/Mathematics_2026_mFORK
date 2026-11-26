## Exercise 11 — Decomposition into Parallel and Perpendicular Components

### Problem statement

Decompose $u=(3,4)$ into components parallel and perpendicular to $v=(1,2)$. Check

$$
u=u_{\parallel}+u_{\perp}
$$

and

$$
u_{\perp}\cdot v=0
$$

Explain why these are independent checks.

### Formula used

The parallel component is the projection onto $v$:

$$
u_{\parallel}
=\frac{u\cdot v}{v\cdot v}v
$$

The perpendicular component is

$$
u_{\perp}=u-u_{\parallel}
$$

The first formula selects the part of $u$ along $v$. Subtraction leaves the remainder perpendicular to $v$.

### Solution

Compute the required dot products:

$$
u\cdot v=3(1)+4(2)=11
$$

$$
v\cdot v=1^2+2^2=5
$$

Therefore

$$
u_{\parallel}
=\frac{11}{5}(1,2)
=\left(\frac{11}{5},\frac{22}{5}\right)
$$

Subtract this from $u$:

$$
\begin{aligned}
u_{\perp}
&=(3,4)-\left(\frac{11}{5},\frac{22}{5}\right) \\
&=\left(3-\frac{11}{5},4-\frac{22}{5}\right) \\
&=\left(\frac{4}{5},-\frac{2}{5}\right)
\end{aligned}
$$

### Verification

Check that the components add back to $u$:

$$
\begin{aligned}
u_{\parallel}+u_{\perp}
&=\left(\frac{11}{5},\frac{22}{5}\right)
+\left(\frac{4}{5},-\frac{2}{5}\right) \\
&=\left(3,4\right)
\end{aligned}
$$

Check perpendicularity:

$$
u_{\perp}\cdot v
=\left(\frac{4}{5},-\frac{2}{5}\right)\cdot(1,2)
=\frac{4}{5}-\frac{4}{5}
=0
$$

The reconstruction check confirms that no part of $u$ was lost or added incorrectly. The dot-product check confirms that $u_{\perp}$ is genuinely perpendicular to $v$. A single answer could satisfy only one of these conditions accidentally.

### Final answer

$$
u_{\parallel}=\left(\frac{11}{5},\frac{22}{5}\right)
$$

$$
u_{\perp}=\left(\frac{4}{5},-\frac{2}{5}\right)
$$
