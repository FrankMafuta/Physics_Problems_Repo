## Task 5 – Elliptical Motion

**Parametric equations:**

$$
x(t) = a\cos(\omega t), \qquad y(t) = b\sin(\omega t)
$$

### Trajectory

Eliminating $t$:

$$
\frac{x^2}{a^2} + \frac{y^2}{b^2} = \cos^2(\omega t) + \sin^2(\omega t) = 1
$$

This is an **ellipse** with semi-axes $a$ and $b$.

### Velocity vector

$$
\vec{v}(t) = \bigl(-a\omega\sin(\omega t),\ b\omega\cos(\omega t)\bigr)
$$

$$
|\vec{v}(t)| = \omega\sqrt{a^2\sin^2(\omega t) + b^2\cos^2(\omega t)}
$$

### Is the speed constant?

No — unless $a = b$ (circular motion). In general $|\vec{v}|$ varies with time.

### Where is the velocity maximum/minimum?

$$
|\vec{v}|^2 = \omega^2\bigl(a^2\sin^2(\omega t) + b^2\cos^2(\omega t)\bigr)
$$

Assuming $a > b$:

- **Maximum speed** at the ends of the minor axis ($\omega t = \pi/2,\ 3\pi/2$): $\quad |\vec{v}|_{\max} = a\omega$
- **Minimum speed** at the ends of the major axis ($\omega t = 0,\ \pi$): $\quad |\vec{v}|_{\min} = b\omega$

### Acceleration

$$
\vec{a}(t) = \bigl(-a\omega^2\cos(\omega t),\ -b\omega^2\sin(\omega t)\bigr) = -\omega^2\,(x(t),\, y(t))
$$

$$
|\vec{a}(t)| = \omega^2\sqrt{a^2\cos^2(\omega t) + b^2\sin^2(\omega t)}
$$

---
