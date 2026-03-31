## Task 6 – Motion with Linear Drag

**Equation of motion:** $m\dot{v} = -kv$

### Solution

Separable ODE:

$$
\frac{dv}{v} = -\frac{k}{m}\,dt \implies \ln v = -\frac{k}{m}t + C
$$

$$
\boxed{v(t) = v_0\,e^{-k t/m}}
$$

Position (integrating):

$$
\boxed{x(t) = \frac{mv_0}{k}\left(1 - e^{-kt/m}\right)}
$$

### Limit $t \to \infty$

$$
\lim_{t\to\infty} v(t) = 0, \qquad \lim_{t\to\infty} x(t) = \frac{mv_0}{k}
$$

The body **stops at a finite distance** $x_\infty = mv_0/k$.

### Comparison with drag-free motion

Without drag: $v(t) = v_0$ (constant), $x(t) = v_0 t$ (unbounded).

With drag: exponential decay, finite stopping distance.

---
