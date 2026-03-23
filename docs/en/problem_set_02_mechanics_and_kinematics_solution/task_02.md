## Task 2 – Projectile Motion

**Setup:** initial velocity $v_0$, launch angle $\alpha$ from horizontal, no air resistance.

### Equations of motion

Decomposing the initial velocity:

$$
v_{0x} = v_0 \cos\alpha, \qquad v_{0y} = v_0 \sin\alpha
$$

Equations of motion (with $g$ acting downward):

$$
x(t) = v_0 \cos\alpha \cdot t
$$

$$
y(t) = v_0 \sin\alpha \cdot t - \frac{1}{2}g t^2
$$

### Time of flight

The body returns to the ground when $y(t_f) = 0$:

$$
v_0 \sin\alpha \cdot t_f - \frac{1}{2}g t_f^2 = 0
\implies t_f \left(v_0 \sin\alpha - \frac{1}{2}g t_f\right) = 0
$$

$$
\boxed{t_f = \frac{2 v_0 \sin\alpha}{g}}
$$

### Maximum height

Vertical velocity is zero at the peak:

$$
v_y = v_0 \sin\alpha - g t_H = 0 \implies t_H = \frac{v_0 \sin\alpha}{g}
$$

$$
\boxed{H = y(t_H) = \frac{v_0^2 \sin^2\alpha}{2g}}
$$

### Range

$$
\boxed{R = x(t_f) = v_0 \cos\alpha \cdot \frac{2 v_0 \sin\alpha}{g} = \frac{v_0^2 \sin(2\alpha)}{g}}
$$

### Angle for maximum range

$R$ is maximized when $\sin(2\alpha) = 1$, i.e.:

$$
\boxed{\alpha = 45°}
$$

---
