## Task 5 – Trajectory Curvature and Normal Acceleration

**Given ellipse:**

$$
x = a\cos t, \qquad y = b\sin t
$$

### 1. Velocity and acceleration

$$
\vec{v}(t) = (-a\sin t,\; b\cos t), \qquad \vec{a}(t) = (-a\cos t,\; -b\sin t)
$$

$$
|\vec{v}(t)| = \sqrt{a^2\sin^2 t + b^2\cos^2 t}
$$

### 2. Unit tangent vector

$$
\hat{T}(t) = \frac{\vec{v}(t)}{|\vec{v}(t)|} = \frac{(-a\sin t,\; b\cos t)}{\sqrt{a^2\sin^2 t + b^2\cos^2 t}}
$$

### 3. Decomposition of acceleration

**Tangential component:**

$$
a_t = \frac{\vec{v} \cdot \vec{a}}{|\vec{v}|} = \frac{(-a\sin t)(-a\cos t) + (b\cos t)(-b\sin t)}{|\vec{v}|} = \frac{a^2\sin t\cos t - b^2\sin t\cos t}{|\vec{v}|}
$$

$$
a_t = \frac{(a^2 - b^2)\sin t\cos t}{|\vec{v}|} = \frac{\frac{1}{2}(a^2 - b^2)\sin(2t)}{|\vec{v}|}
$$

$$
\vec{a}_t = a_t\,\hat{T}
$$

**Normal component:**

$$
\vec{a}_n = \vec{a} - \vec{a}_t
$$

$$
a_n = |\vec{a}_n| = \sqrt{|\vec{a}|^2 - a_t^2}
$$

where $|\vec{a}|^2 = a^2\cos^2 t + b^2\sin^2 t$.

### 4. Radius of curvature at $t = 0$

At $t = 0$: $\;x = a,\; y = 0$

$$
\vec{v}(0) = (0,\; b), \quad |\vec{v}(0)| = b
$$

$$
\vec{a}(0) = (-a,\; 0), \quad |\vec{a}(0)| = a
$$

At $t = 0$, $\sin t = 0$, so $a_t = 0$. Hence $\vec{a}_n = \vec{a}(0) = (-a, 0)$ and $a_n = a$.

$$
a_n = \frac{v^2}{R} \;\Rightarrow\; R = \frac{v^2}{a_n} = \frac{b^2}{a}
$$

### 5. Comparison with circle ($a = b$)

$$
R = \frac{b^2}{a} \xrightarrow{a=b} R = \frac{a^2}{a} = a \checkmark
$$

This is consistent — for a circle of radius $a$, the radius of curvature equals $a$ everywhere.

### Physical interpretation

- **Greater curvature $\Rightarrow$ greater normal acceleration**: Yes, since $a_n = v^2/R$, a smaller $R$ means larger $a_n$ (for fixed speed).
- **Where is the ellipse more curved?** At the end of the **minor semi-axis** ($t = \pi/2$, point $(0, b)$), where $R = a^2/b < b$ (assuming $a > b$). The curve is most curved where the semi-axis is shortest.
- **Physical meaning of normal acceleration**: Normal acceleration does not change the speed, only the direction of $\vec{v}$. It is the centripetal cause of changing direction, always pointing toward the center of curvature.

---
