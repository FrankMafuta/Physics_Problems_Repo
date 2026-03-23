## Task 3 – Elimination of Time and Interpretation of Acceleration

**Parametric path:**

$$
x(t) = 2t^2, \qquad y(t) = 3t^3
$$

### Eliminating $t$

From the first equation:

$$
t^2 = \frac{x}{2} \implies t = \sqrt{\frac{x}{2}}
$$

Substituting into $y$:

$$
y = 3t^3 = 3t \cdot t^2 = 3\sqrt{\frac{x}{2}} \cdot \frac{x}{2} = \frac{3x}{2}\sqrt{\frac{x}{2}}
$$

$$
\boxed{y = \frac{3x}{2} \cdot \sqrt{\frac{x}{2}}}
$$

This is a semicubical parabola (defined for $x \geq 0$).

### Velocity vector

$$
\vec{v}(t) = \left(\frac{dx}{dt},\ \frac{dy}{dt}\right) = (4t,\ 9t^2)
$$

$$
|\vec{v}(t)| = \sqrt{(4t)^2 + (9t^2)^2} = \sqrt{16t^2 + 81t^4} = |t|\sqrt{16 + 81t^2}
$$

### Acceleration vector

$$
\vec{a}(t) = \left(\frac{d^2x}{dt^2},\ \frac{d^2y}{dt^2}\right) = (4,\ 18t)
$$

$$
|\vec{a}(t)| = \sqrt{16 + 324t^2}
$$

### Is the acceleration constant?

No. While the $x$-component of acceleration is constant ($a_x = 4$), the $y$-component changes with time ($a_y = 18t$). Therefore:

$$
\vec{a}(t) = (4,\ 18t) \neq \text{const}
$$

---
