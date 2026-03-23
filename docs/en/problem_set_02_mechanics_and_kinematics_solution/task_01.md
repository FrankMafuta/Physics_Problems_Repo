## Task 1 – Uniform and Uniformly Accelerated Motion

**Given equation of motion:**

$$
x(t) = x_0 + v_0 t + \frac{1}{2} a t^2
$$

### 1. Velocity and acceleration by differentiation

$$
v(t) = \frac{dx}{dt} = v_0 + at
$$

$$
a(t) = \frac{dv}{dt} = a = \text{const}
$$

### 2. Numerical case: $x_0 = 0$, $v_0 = 5\ \text{m/s}$, $a = -2\ \text{m/s}^2$

**Stopping time** — body stops when $v(t_s) = 0$:

$$
v_0 + a t_s = 0 \implies t_s = -\frac{v_0}{a} = -\frac{5}{-2} = 2.5\ \text{s}
$$

**Maximum displacement** — since $a < 0$, the body decelerates and reaches maximum $x$ at $t = t_s$:

$$
x_{\max} = x(t_s) = v_0 t_s + \frac{1}{2}a t_s^2 = 5 \cdot 2.5 + \frac{1}{2}(-2)(2.5)^2 = 12.5 - 6.25 = 6.25\ \text{m}
$$

**Maximum velocity:**

- If $a > 0$: velocity grows without bound; maximum is reached as $t \to \infty$.
- If $a < 0$: velocity is maximum at $t = 0$, i.e., $v_{\max} = v_0 = 5\ \text{m/s}$.
- If $a = 0$: velocity is constant, $v(t) = v_0$.

### 3. Graphs

The three graphs $x(t)$, $v(t)$, $a(t)$ for the numerical case:

- $x(t) = 5t - t^2$ — upward parabola with vertex at $t = 2.5\ \text{s}$
- $v(t) = 5 - 2t$ — linear, crosses zero at $t = 2.5\ \text{s}$
- $a(t) = -2\ \text{m/s}^2$ — horizontal line

---
