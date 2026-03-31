## Task 10 – Numerical Model: Anharmonic Oscillator

**Potential:** $U(x) = \frac{k}{2}x^2 + \lambda x^4$

### Force

$$
F(x) = -\frac{dU}{dx} = -kx - 4\lambda x^3
$$

### Equation of motion

$$
m\ddot{x} = -kx - 4\lambda x^3
$$

This is a **nonlinear ODE** — no closed-form solution in general.

### Key observations

- For $\lambda = 0$: reduces to simple harmonic oscillator.
- For $\lambda > 0$: the restoring force is stronger than linear → **stiffer** potential, higher frequency for larger amplitudes.
- For $\lambda < 0$ (with $k > 0$): double-well potential if $\lambda < -k^2/(8|x_0|^2)$; can exhibit bounded or unbounded motion depending on energy.

### Phase portrait interpretation

The phase portrait $(x, \dot{x})$ shows:
- **Closed orbits** (ellipses for $\lambda=0$, deformed for $\lambda \neq 0$) for bounded motion.
- **Separatrix** (saddle-point orbit) for the double-well case separating libration from rotation.
- The period of oscillation **increases with amplitude** for $\lambda > 0$.
