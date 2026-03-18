## Task 6 – Curve Length and Numerical Integration

**Given trajectory:**

$$
x(t) = t, \qquad y(t) = t^2, \qquad t \in [0, 1]
$$

### 1. Velocity vector

$$
\vec{v}(t) = \frac{d\vec{r}}{dt} = (1,\; 2t)
$$

### 2. Speed

$$
|\vec{v}(t)| = \sqrt{1 + 4t^2}
$$

### 3. Arc length integral

$$
s = \int_0^1 \sqrt{1 + 4t^2}\, dt
$$

### 4. Analytical solution

Using the standard formula $\displaystyle\int\sqrt{1 + u^2}\,du = \tfrac{1}{2}\bigl(u\sqrt{1+u^2} + \ln|u + \sqrt{1+u^2}|\bigr)$, substitute $u = 2t$:

$$
s = \int_0^1 \sqrt{1 + 4t^2}\, dt = \frac{1}{2}\left[t\sqrt{1+4t^2} + \frac{1}{2}\ln\!\left(2t + \sqrt{1+4t^2}\right)\right]_0^1
$$

$$
= \frac{1}{2}\left[\sqrt{5} + \frac{1}{2}\ln\!\left(2 + \sqrt{5}\right) - 0 - \frac{1}{2}\ln(1)\right]
$$

$$
s = \frac{\sqrt{5}}{2} + \frac{1}{4}\ln\!\left(2 + \sqrt{5}\right) \approx \frac{2.2361}{2} + \frac{1}{4}\ln(4.2361) \approx 1.1180 + \frac{1.4436}{4} \approx 1.4789
$$
