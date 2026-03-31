## Task 5 – Elastic Collision (1D)

**Conservation laws:**

$$
m_1 v_1 + m_2 v_2 = m_1 v_1' + m_2 v_2' \quad \text{(momentum)}
$$

$$
\frac{1}{2}m_1 v_1^2 + \frac{1}{2}m_2 v_2^2 = \frac{1}{2}m_1 v_1'^2 + \frac{1}{2}m_2 v_2'^2 \quad \text{(energy)}
$$

### General solution

$$
\boxed{v_1' = \frac{m_1 - m_2}{m_1 + m_2}v_1 + \frac{2m_2}{m_1 + m_2}v_2}
$$

$$
\boxed{v_2' = \frac{2m_1}{m_1 + m_2}v_1 + \frac{m_2 - m_1}{m_1 + m_2}v_2}
$$

### Case $m_1 = m_2$

$$
v_1' = v_2, \quad v_2' = v_1
$$

The bodies **exchange velocities** — a well-known billiard-ball result.

### Limit $m_2 \gg m_1$ (with $v_2 = 0$)

$$
v_1' \approx -v_1, \quad v_2' \approx 0
$$

The light body **bounces back** with the same speed; the heavy body barely moves (e.g., ball hitting a wall).

---
