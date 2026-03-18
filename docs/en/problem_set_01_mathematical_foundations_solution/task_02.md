## Task 2 – Parametric Trajectory, Velocity, and Acceleration

**Given:**

$$
\vec{r}(t) = \bigl(t^2,\; \sin t,\; 5\bigr)
$$

### Velocity

$$
\vec{v}(t) = \frac{d\vec{r}}{dt} = (2t,\; \cos t,\; 0)
$$

### Acceleration

$$
\vec{a}(t) = \frac{d^2\vec{r}}{dt^2} = (2,\; -\sin t,\; 0)
$$

### Speed at $t = 1$

$$
|\vec{v}(1)| = \sqrt{(2\cdot1)^2 + \cos^2(1) + 0^2} = \sqrt{4 + \cos^2(1)} \approx \sqrt{4 + 0.2919} \approx \sqrt{4.2919} \approx 2.072
$$

### Dot product $\vec{v} \cdot \vec{a}$

$$
\vec{v}(t) \cdot \vec{a}(t) = 2t \cdot 2 + \cos t \cdot (-\sin t) + 0 = 4t - \frac{1}{2}\sin(2t)
$$

### Cross product $\vec{v} \times \vec{a}$

$$
\vec{v} \times \vec{a} =
\begin{vmatrix}
\vec{i} & \vec{j} & \vec{k} \\
2t & \cos t & 0 \\
2 & -\sin t & 0
\end{vmatrix}
= \vec{i}(0 - 0) - \vec{j}(0 - 0) + \vec{k}\bigl(2t\cdot(-\sin t) - \cos t \cdot 2\bigr)
$$

$$
= \bigl(0,\; 0,\; -2t\sin t - 2\cos t\bigr)
$$

---
