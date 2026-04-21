## Problem 10 – Double Pendulum and Deterministic Chaos

### Coordinates

$$
x_1 = l_1\sin\theta_1, \quad y_1 = -l_1\cos\theta_1
$$

$$
x_2 = x_1 + l_2\sin\theta_2, \quad y_2 = y_1 - l_2\cos\theta_2
$$

### Equations of motion (standard Lagrangian derivation)

Let $M = m_1 + m_2$. The coupled ODEs for $(\theta_1, \theta_2)$ are:

$$
\ddot{\theta}_1 = \frac{-m_2 l_2\dot\theta_2^2\sin(\theta_1-\theta_2) - (m_1+m_2)g\sin\theta_1 - m_2 l_1\dot\theta_1^2\sin(\theta_1-\theta_2)\cos(\theta_1-\theta_2) + m_2 g\sin\theta_2\cos(\theta_1-\theta_2)}{l_1(m_1+m_2) - m_2 l_1\cos^2(\theta_1-\theta_2)}
$$

(and similarly for $\ddot\theta_2$ — see code for the full RK4 implementation.)

### Chaos and sensitivity to initial conditions

- For small angles: nearly integrable, predictable.
- For large angles: the Lyapunov exponent $\lambda > 0$ means trajectories diverge exponentially as $\delta\theta \sim e^{\lambda t}$.
- With 50 copies perturbed by $\delta\theta_2 \sim 10^{-4}$–$10^{-2}$: at first all trajectories are indistinguishable; after a finite time they spread into fully independent orbits — this is the hallmark of **deterministic chaos**.
