## Task 7 – Work of a Force Along a Trajectory

**Given:**

$$
\vec{F}(x,y) = (y,\; 2x), \qquad x = t,\; y = t^2,\; t \in [0,1]
$$

### 1. Velocity vector

$$
\vec{v}(t) = \frac{d\vec{r}}{dt} = (1,\; 2t)
$$

### 2. Work as a line integral

$$
W = \int_C \vec{F} \cdot d\vec{r} = \int_0^1 \vec{F}(x(t), y(t)) \cdot \vec{v}(t)\, dt
$$

Substituting $x = t,\; y = t^2$:

$$
\vec{F}(t^2, t) = (t^2,\; 2t)
$$

$$
W = \int_0^1 (t^2,\; 2t) \cdot (1,\; 2t)\, dt = \int_0^1 \bigl(t^2 + 4t^2\bigr)\, dt = \int_0^1 5t^2\, dt
$$

$$
W = 5 \cdot \frac{t^3}{3}\Bigg|_0^1 = \frac{5}{3}
$$

