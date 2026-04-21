## Problem 3 – Harmonic Wave

**Given:** $y(x,t) = A\sin(kx - \omega t)$

### 1. Wavelength

$$
\lambda = \frac{2\pi}{k}
$$

### 2. Phase velocity

A point of constant phase satisfies $kx - \omega t = \text{const}$, so:

$$
\boxed{v_{\text{ph}} = \frac{\omega}{k} = \lambda f}
$$

### 3. Numerical: $k = 4\pi\ \text{rad/m}$, $\omega = 20\pi\ \text{rad/s}$

$$
v_{\text{ph}} = \frac{20\pi}{4\pi} = 5\ \text{m/s}, \qquad \lambda = \frac{2\pi}{4\pi} = 0.5\ \text{m}
$$

### 4. Phase comparison of $x = \lambda$ vs $x = 0$

$$
y(0, t) = A\sin(-\omega t), \quad y(\lambda, t) = A\sin(k\lambda - \omega t) = A\sin(2\pi - \omega t) = A\sin(-\omega t)
$$

Yes — the two points oscillate **in phase** (differ by exactly $2\pi$). This is the definition of wavelength.

---
