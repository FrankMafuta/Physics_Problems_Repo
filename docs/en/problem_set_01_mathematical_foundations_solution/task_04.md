## Task 4 – Geometry of Parametric Curves

### A) Circle: $x(t) = R\cos t,\quad y(t) = R\sin t$

**Elimination of parameter:**

$$
x^2 + y^2 = R^2\cos^2 t + R^2\sin^2 t = R^2 \quad \Rightarrow \quad \text{circle of radius } R
$$

**Velocity and acceleration:**

$$
\vec{v}(t) = (-R\sin t,\; R\cos t), \qquad \vec{a}(t) = (-R\cos t,\; -R\sin t)
$$

**Magnitudes:**

$$
|\vec{v}| = \sqrt{R^2\sin^2 t + R^2\cos^2 t} = R = \text{const}
$$

$$
|\vec{a}| = R = \text{const}
$$

---

### B) Ellipse: $x(t) = a\cos t,\quad y(t) = b\sin t$

**Elimination of parameter:**

$$
\frac{x^2}{a^2} + \frac{y^2}{b^2} = \cos^2 t + \sin^2 t = 1 \quad \Rightarrow \quad \text{ellipse with semi-axes } a, b
$$

**Velocity and acceleration:**

$$
\vec{v}(t) = (-a\sin t,\; b\cos t), \qquad \vec{a}(t) = (-a\cos t,\; -b\sin t)
$$

**Magnitudes:**

$$
|\vec{v}| = \sqrt{a^2\sin^2 t + b^2\cos^2 t} \neq \text{const (unless } a = b\text{)}
$$

$$
|\vec{a}| = \sqrt{a^2\cos^2 t + b^2\sin^2 t} \neq \text{const (unless } a = b\text{)}
$$

---

### C) Parabola: $x(t) = t,\quad y(t) = t^2$

**Elimination of parameter:**

$$
x = t \;\Rightarrow\; y = x^2 \quad \Rightarrow \quad \text{upward-opening parabola}
$$

**Velocity and acceleration:**

$$
\vec{v}(t) = (1,\; 2t), \qquad \vec{a}(t) = (0,\; 2)
$$

**Magnitudes:**

$$
|\vec{v}| = \sqrt{1 + 4t^2} \neq \text{const}, \qquad |\vec{a}| = 2 = \text{const}
$$

---

### D) Hyperbola: $x(t) = \cosh t,\quad y(t) = \sinh t$

**Elimination of parameter** (using the identity $\cosh^2 t - \sinh^2 t = 1$):

$$
x^2 - y^2 = 1 \quad \Rightarrow \quad \text{right branch of unit hyperbola}
$$

**Velocity and acceleration:**

$$
\vec{v}(t) = (\sinh t,\; \cosh t), \qquad \vec{a}(t) = (\cosh t,\; \sinh t)
$$

**Magnitudes:**

$$
|\vec{v}| = \sqrt{\sinh^2 t + \cosh^2 t} = \sqrt{\cosh(2t)} \neq \text{const}
$$

$$
|\vec{a}| = \sqrt{\cosh^2 t + \sinh^2 t} = \sqrt{\cosh(2t)} \neq \text{const}
$$

---
