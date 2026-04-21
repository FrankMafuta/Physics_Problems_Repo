## Problem 4 – Wave Equation

**Given:** $y(x,t) = A\cos(kx - \omega t)$

### 1. Verification

$$
\frac{\partial^2 y}{\partial t^2} = -\omega^2 A\cos(kx - \omega t)
$$

$$
\frac{\partial^2 y}{\partial x^2} = -k^2 A\cos(kx - \omega t)
$$

Substituting into the wave equation $\partial^2 y/\partial t^2 = v^2\,\partial^2 y/\partial x^2$:

$$
-\omega^2 A\cos(\cdots) = v^2 \cdot (-k^2 A\cos(\cdots))
$$

This is satisfied if and only if:

$$
\boxed{v = \frac{\omega}{k}}
$$

### 2. Dispersion relation

The wave equation implies a **linear dispersion relation** $\omega = vk$, meaning the phase velocity is independent of frequency — the medium is **non-dispersive**.

---

