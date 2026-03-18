## Task 9 – Harmonic Oscillator

$$
\frac{d^2x}{dt^2} + \omega^2 x = 0
$$

### 1. General solution

The characteristic equation: $\lambda^2 + \omega^2 = 0 \;\Rightarrow\; \lambda = \pm i\omega$

$$
\boxed{x(t) = A\cos(\omega t) + B\sin(\omega t)}
$$

Equivalently: $x(t) = C\cos(\omega t + \phi)$, where $C = \sqrt{A^2 + B^2}$ and $\tan\phi = -B/A$.

### 2. Solution with initial conditions

For $x(0) = x_0$ and $x'(0) = v_0$:

$$
x(0) = A = x_0
$$

$$
x'(t) = -A\omega\sin(\omega t) + B\omega\cos(\omega t) \;\Rightarrow\; x'(0) = B\omega = v_0 \;\Rightarrow\; B = \frac{v_0}{\omega}
$$

$$
\boxed{x(t) = x_0\cos(\omega t) + \frac{v_0}{\omega}\sin(\omega t)}
$$

$$
x'(t) = -x_0\omega\sin(\omega t) + v_0\cos(\omega t)
$$

$$
x''(t) = -x_0\omega^2\cos(\omega t) - v_0\omega\sin(\omega t) = -\omega^2 x(t) \checkmark
$$
