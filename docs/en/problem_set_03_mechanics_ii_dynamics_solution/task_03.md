## Task 3 – Work of a Variable Force

**Given:** $F(x) = -kx$

### Equation of motion and solution

$$
m\ddot{x} = -kx \implies \ddot{x} + \omega_0^2 x = 0, \quad \omega_0 = \sqrt{\frac{k}{m}}
$$

General solution:

$$
x(t) = A\cos(\omega_0 t) + B\sin(\omega_0 t)
$$

This is **simple harmonic motion**.

### Work from $0$ to $x_0$

$$
W = \int_0^{x_0} F(x)\,dx = \int_0^{x_0} (-kx)\,dx = -\frac{1}{2}kx_0^2
$$

### Potential energy

The work done against the force equals the stored potential energy:

$$
\boxed{U(x) = \frac{1}{2}kx^2}
$$

### Verification: $F = -dU/dx$

$$
-\frac{dU}{dx} = -\frac{d}{dx}\left(\frac{1}{2}kx^2\right) = -kx = F(x) \checkmark
$$

---