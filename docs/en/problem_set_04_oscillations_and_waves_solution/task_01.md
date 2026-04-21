## Problem 1 – Harmonic Motion: Motion Parameters

**Given:** $x(t) = A\cos(\omega t + \varphi)$

### 1. Period and frequency

$$
T = \frac{2\pi}{\omega}, \qquad f = \frac{1}{T} = \frac{\omega}{2\pi}
$$

### 2. Maximum velocity and acceleration

Differentiating:

$$
v(t) = \dot{x}(t) = -A\omega\sin(\omega t + \varphi) \implies v_{\max} = A\omega
$$

$$
a(t) = \ddot{x}(t) = -A\omega^2\cos(\omega t + \varphi) \implies a_{\max} = A\omega^2
$$

### 3. Numerical case: $A = 0.2\ \text{m}$, $f = 2\ \text{Hz}$

$$
\omega = 2\pi f = 2\pi \cdot 2 = 4\pi \approx 12.57\ \text{rad/s}
$$

$$
v_{\max} = A\omega = 0.2 \cdot 4\pi \approx 2.51\ \text{m/s}
$$

$$
a_{\max} = A\omega^2 = 0.2 \cdot (4\pi)^2 \approx 31.6\ \text{m/s}^2
$$

**Interpretation:** The velocity is 90° ahead of position in phase. The acceleration is always directed toward the equilibrium and proportional to displacement, which is the defining property of SHM.

---
