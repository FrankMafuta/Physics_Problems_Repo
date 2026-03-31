## Task 7 – Vertical Throw with Drag

**Equation of motion:** $m\dot{v} = -mg - kv$, $v(0) = v_0 > 0$

### Solution

Define the terminal velocity $v_t = mg/k$. The equation becomes:

$$
m\dot{v} = -k(v + v_t)
$$

Separating variables:

$$
\frac{dv}{v + v_t} = -\frac{k}{m}\,dt
$$

$$
\boxed{v(t) = (v_0 + v_t)\,e^{-kt/m} - v_t}
$$

Position:

$$
\boxed{x(t) = \frac{m}{k}(v_0 + v_t)\left(1 - e^{-kt/m}\right) - v_t\,t}
$$

### Maximum height

At $v(t_{\max}) = 0$:

$$
t_{\max} = \frac{m}{k}\ln\!\left(1 + \frac{v_0}{v_t}\right)
$$

$$
x_{\max} = \frac{m}{k}\left[v_0 - v_t\ln\!\left(1 + \frac{v_0}{v_t}\right)\right]
$$

### Comparison without drag

Without drag: $x_{\max} = v_0^2/(2g)$. With drag: always smaller, since energy is dissipated by friction.

---
