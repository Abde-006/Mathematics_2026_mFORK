# Problem 8. Number of Requests Handled by a Server

The arrival rate during the first five minutes is

$$
r(t)=100+20t\qquad [\mathrm{requests/min}],\qquad 0\le t\le5.
$$

Compute the total requests, average rate, and compare the average with the endpoint rates.

## Quantities

Let $t$ be elapsed time in minutes, $r(t)$ the arrival rate in requests per minute, $R$ the accumulated requests, and $r_{\mathrm{avg}}$ the average rate.

## Step 1 - Compute the total requests

A varying rate is accumulated by integration. Thus the total over $[a,b]$ is

$$
R=\int_a^b r(t)\,dt.
$$

Substituting $r(t)=100+20t$, $a=0$, and $b=5$,

$$
\begin{aligned}
R
&=\int_0^5(100+20t)\,dt \\
&=\left[100t+10t^2\right]_0^5 \\
&=(500+250)-0 \\
&=750\ \mathrm{requests}.
\end{aligned}
$$

## Step 2 - Compute the average arrival rate

The average value of a rate over $[a,b]$ is total accumulation divided by elapsed time:

$$
r_{\mathrm{avg}}=\frac1{b-a}\int_a^b r(t)\,dt.
$$

Using $R=750$ and $b-a=5-0=5$,

$$
r_{\mathrm{avg}}=\frac{750}{5}=150\ \mathrm{requests/min}.
$$

## Step 3 - Compare with endpoint rates

The endpoint rates are

$$
r(0)=100+20(0)=100\ \mathrm{requests/min},
$$

and

$$
r(5)=100+20(5)=200\ \mathrm{requests/min}.
$$

Therefore

$$
100<150<200.
$$

## Verification

The function $r(t)$ is linear, so its average over an interval equals the arithmetic mean of its endpoint values:

$$
\frac{r(0)+r(5)}2=\frac{100+200}{2}=150\ \mathrm{requests/min}.
$$

This independent check agrees with the integral result.

## Final answer

The server handled $750$ requests at an average rate of $150\,\mathrm{requests/min}$, which lies strictly between $100$ and $200$ requests per minute.
