# Problem 2. Maximum Area of a Rectangle

A rectangle has perimeter $40$. Find the side lengths that maximize its area and justify the maximum.

## Quantities

Let $x$ be the length of one side, $y$ the length of an adjacent side, and $A$ the area. All lengths are in the same unspecified units.

## Step 1 - Build the area function

The perimeter is the sum of the four side lengths, so $2x+2y=40$. Solving this constraint for $y$ gives

$$
\begin{aligned}
2y&=40-2x, \\
y&=20-x.
\end{aligned}
$$

Area is length times width, $A=xy$. Substituting $y=20-x$ eliminates $y$ and produces the objective function

$$
A(x)=x(20-x)=20x-x^2.
$$

## Step 2 - Determine the domain

Geometrically, both side lengths must be positive:

$$
x>0,\qquad y=20-x>0.
$$

Therefore $0<x<20$. For maximizing over the closed geometric limit, $x=0$ and $x=20$ are degenerate endpoint cases where no positive rectangle remains.

## Step 3 - Find the critical point

For a differentiable objective function on an interval, an interior maximum can occur where the derivative is zero. Differentiating $A(x)$ gives

$$
A'(x)=20-2x.
$$

Solving $A'(x)=0$,

$$
\begin{aligned}
20-2x&=0, \\
x&=10.
\end{aligned}
$$

The reminder $y=20-x$ gives

$$
y=20-10=10.
$$

## Step 4 - Verify the maximum

The second derivative tests whether a critical point is concave downward. Thus

$$
A''(x)=\frac{d}{dx}(20-2x)=-2<0.
$$

Because $A''(10)<0$, $x=10$ is a strict local maximum. At the degenerate endpoints,

$$
A(0)=0,\qquad A(20)=20(20-20)=0,
$$

while

$$
A(10)=10(20-10)=100.
$$

The concave parabola therefore attains its greatest area at $x=10$.

## Interpretation

Among rectangles with perimeter $40$, the maximizing shape is a square. Its area is $100$ square units.

## Final answer

The dimensions are $x=y=10$, and the maximum area is $100$ square units.
