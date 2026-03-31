## Task 9 – Potential and Conservative Field

**Given:** $U(x,y) = \frac{k}{2}(x^2 + y^2)$

### Force from gradient

$$
\vec{F} = -\nabla U = -\left(\frac{\partial U}{\partial x},\ \frac{\partial U}{\partial y}\right) = (-kx,\ -ky) = -k\vec{r}
$$

This is a **central restoring force** (2D harmonic oscillator).

### Equations of motion

$$
m\ddot{x} = -kx, \qquad m\ddot{y} = -ky
$$

### Type of motion

Both coordinates oscillate independently at the same frequency $\omega_0 = \sqrt{k/m}$:

$$
x(t) = A\cos(\omega_0 t + \varphi_x), \qquad y(t) = B\cos(\omega_0 t + \varphi_y)
$$

The trajectory is in general an **ellipse** (or circle if $A = B$, $\Delta\varphi = \pi/2$) — a **Lissajous figure** with equal frequencies.

### Total energy

$$
E = \frac{1}{2}m(\dot{x}^2 + \dot{y}^2) + \frac{k}{2}(x^2 + y^2) = \frac{1}{2}kA^2 + \frac{1}{2}kB^2 = \text{const}
$$

---
