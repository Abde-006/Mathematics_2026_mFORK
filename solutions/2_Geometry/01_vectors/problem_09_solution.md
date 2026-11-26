## Exercise 9 — Cross Product as a Perpendicular Direction

### Problem statement

For $u=(1,2,0)$ and $v=(0,1,3)$:

1. Compute $u\times v$.
2. Use dot products to check that it is perpendicular to both vectors.
3. Compute $v\times u$ and compare the results.

### Formula used

For $u=(u_1,u_2,u_3)$ and $v=(v_1,v_2,v_3)$,

$$
u\times v
=
(u_2v_3-u_3v_2,\,
u_3v_1-u_1v_3,\,
u_1v_2-u_2v_1)
$$

The result is perpendicular to both inputs. Reversing the order gives

$$
v\times u=-u\times v
$$

so changing the order reverses the direction of the cross product.

### Solution

Apply the formula:

$$
\begin{aligned}
u\times v
&=(2(3)-0(1),\,0(0)-1(3),\,1(1)-2(0)) \\
&=(6,-3,1)
\end{aligned}
$$

Check perpendicularity to $u$:

$$
(u\times v)\cdot u=(6,-3,1)\cdot(1,2,0)=6-6+0=0
$$

Check perpendicularity to $v$:

$$
(u\times v)\cdot v=(6,-3,1)\cdot(0,1,3)=0-3+3=0
$$

Both dot products are zero, so $(6,-3,1)$ is perpendicular to both input vectors.

Now reverse the order:

$$
v\times u
=(-6,3,-1)
=-(6,-3,1)
=-(u\times v)
$$

### Geometric interpretation

The cross product selects a perpendicular direction determined by the right-hand rule. Reversing $u$ and $v$ reverses that direction.

### Final answer

$$
u\times v=(6,-3,1)
$$

$$
v\times u=(-6,3,-1)
$$
