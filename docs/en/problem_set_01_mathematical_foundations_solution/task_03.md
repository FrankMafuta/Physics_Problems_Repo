## Task 3 – Integration of Motion

### Part A

**Given:**

$$
\vec{v}(t) = (2t,\; 3,\; -e^{-t}), \qquad \vec{r}(0) = (0, 1, 2)
$$

**Position:**

$$
\vec{r}(t) = \vec{r}(0) + \int_0^t \vec{v}(\tau)\, d\tau = (0,1,2) + \left(\int_0^t 2\tau\, d\tau,\; \int_0^t 3\, d\tau,\; \int_0^t -e^{-\tau}\, d\tau\right)
$$

$$
= (0,1,2) + \bigl(t^2,\; 3t,\; e^{-t} - 1\bigr) = \bigl(t^2,\; 1 + 3t,\; 1 + e^{-t}\bigr)
$$

**Acceleration:**

$$
\vec{a}(t) = \frac{d\vec{v}}{dt} = (2,\; 0,\; e^{-t})
$$

---

### Part B

**Given:**

$$
\vec{a}(t) = (4,\; -\sin t,\; 0), \qquad \vec{v}(0) = (1, 0, 2), \qquad \vec{r}(0) = (0, 0, 0)
$$

**Velocity:**

$$
\vec{v}(t) = \vec{v}(0) + \int_0^t \vec{a}(\tau)\, d\tau = (1,0,2) + \bigl(4t,\; \cos t - 1,\; 0\bigr) = \bigl(1 + 4t,\; \cos t - 1,\; 2\bigr)
$$

**Position:**

$$
\vec{r}(t) = \vec{r}(0) + \int_0^t \vec{v}(\tau)\, d\tau = (0,0,0) + \left(\int_0^t(1+4\tau)\,d\tau,\; \int_0^t(\cos\tau-1)\,d\tau,\; \int_0^t 2\, d\tau\right)
$$

$$
= \bigl(t + 2t^2,\; \sin t - t,\; 2t\bigr)
$$

---
