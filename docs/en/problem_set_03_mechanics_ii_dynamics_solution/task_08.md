## Task 8 – Harmonic Oscillator

**Equation of motion:** $m\ddot{x} + kx = 0$

### Solution

$$
\boxed{x(t) = A\cos(\omega_0 t + \varphi)}, \quad \omega_0 = \sqrt{\frac{k}{m}}
$$

where $A$ and $\varphi$ are determined by initial conditions.

### Natural frequency

$$
f_0 = \frac{\omega_0}{2\pi} = \frac{1}{2\pi}\sqrt{\frac{k}{m}}
$$

### Energy as a function of time

$$
T(t) = \frac{1}{2}m\dot{x}^2 = \frac{1}{2}m\omega_0^2 A^2\sin^2(\omega_0 t + \varphi) = \frac{1}{2}kA^2\sin^2(\omega_0 t + \varphi)
$$

$$
U(t) = \frac{1}{2}kx^2 = \frac{1}{2}kA^2\cos^2(\omega_0 t + \varphi)
$$

$$
E = T + U = \frac{1}{2}kA^2\bigl[\sin^2 + \cos^2\bigr] = \frac{1}{2}kA^2 = \text{const} \checkmark
$$

### Phase space

In the $(x, v)$ plane, the trajectory is an **ellipse**:

$$
\frac{x^2}{A^2} + \frac{v^2}{(A\omega_0)^2} = 1
$$

Energy is constant along this ellipse — each orbit corresponds to a fixed $E = \frac{1}{2}kA^2$.

---
