## Problem 7 – Forced Oscillator and Resonance

**Equation:** $m\ddot{x} + b\dot{x} + kx = F_0\cos(\Omega t)$

### Steady-state amplitude

The particular solution is $x_p(t) = C(\Omega)\cos(\Omega t - \delta)$ where:

$$
\boxed{C(\Omega) = \frac{F_0/m}{\sqrt{(\omega_0^2 - \Omega^2)^2 + (2\gamma\Omega)^2}}}
$$

### Phase shift

$$
\tan\delta = \frac{2\gamma\Omega}{\omega_0^2 - \Omega^2}
$$

### Resonance

Amplitude is maximized when $\frac{dC}{d\Omega} = 0$, giving:

$$
\Omega_{\text{res}} = \sqrt{\omega_0^2 - 2\gamma^2}
$$

For small damping $\gamma \ll \omega_0$: $\Omega_{\text{res}} \approx \omega_0$, and $C_{\max} \approx \frac{F_0}{2m\gamma\omega_0} = \frac{F_0 Q}{k}$ where $Q = \omega_0/(2\gamma)$ is the quality factor.

---
