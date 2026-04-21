## Problem 8 – Two Coupled Springs

**Setup:** masses $m_1, m_2$ connected by springs $k_1, k_2, k_3$ in series (wall-$k_1$-$m_1$-$k_2$-$m_2$-$k_3$-wall).

### Equations of motion

$$
m_1\ddot{x}_1 = -k_1 x_1 - k_2(x_1 - x_2), \qquad m_2\ddot{x}_2 = -k_2(x_2 - x_1) - k_3 x_2
$$

Matrix form:

$$
\mathbf{M}\ddot{\vec{x}} + \mathbf{K}\vec{x} = 0, \quad \mathbf{M} = \begin{pmatrix}m_1&0\\0&m_2\end{pmatrix}, \quad \mathbf{K} = \begin{pmatrix}k_1+k_2 & -k_2\\-k_2 & k_2+k_3\end{pmatrix}
$$

### Normal mode frequencies

For $m_1 = m_2 = m$, $k_1 = k_3 = k$, $k_2 = k_c$ (coupling spring):

$$
\omega_{\pm}^2 = \frac{(2k + k_c) \pm k_c}{m} \implies \omega_- = \sqrt{\frac{k}{m}},\quad \omega_+ = \sqrt{\frac{k + 2k_c}{m}}
$$

**Mode shapes:**

- $\omega_-$: both masses move **in phase** (symmetric mode)
- $\omega_+$: masses move **out of phase** (antisymmetric mode)

---
