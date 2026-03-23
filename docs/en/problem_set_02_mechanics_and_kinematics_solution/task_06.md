## Task 6 – Cycloid

**Equations:**

$$
x(t) = R\bigl(\omega t - \sin(\omega t)\bigr), \qquad y(t) = R\bigl(1 - \cos(\omega t)\bigr)
$$

### 1. Velocity and acceleration

$$
\vec{v}(t) = \bigl(R\omega(1 - \cos(\omega t)),\ R\omega\sin(\omega t)\bigr)
$$

$$
\vec{a}(t) = \bigl(R\omega^2\sin(\omega t),\ R\omega^2\cos(\omega t)\bigr)
$$

### 2. Speed and stopping moments

$$
|\vec{v}(t)|^2 = R^2\omega^2\bigl[(1-\cos(\omega t))^2 + \sin^2(\omega t)\bigr]
= R^2\omega^2 \cdot 2(1-\cos(\omega t))
$$

$$
|\vec{v}(t)| = R\omega\sqrt{2(1-\cos(\omega t))} = 2R\omega\left|\sin\!\left(\frac{\omega t}{2}\right)\right|
$$

The point **stops** (touches the ground) when $\cos(\omega t) = 1$, i.e.:

$$
\omega t = 2\pi k, \quad k \in \mathbb{Z} \implies t_k = \frac{2\pi k}{\omega}
$$

### 3. Maximum values

$$
|\vec{v}|_{\max} = 2R\omega \quad \text{(at } \omega t = \pi + 2\pi k \text{, top of the arc)}
$$

$$
|\vec{a}(t)| = R\omega^2\sqrt{\sin^2(\omega t)+\cos^2(\omega t)} = R\omega^2 = \text{const}
$$

The magnitude of acceleration is **constant** and equals the centripetal acceleration of the rolling circle.

### 4–5. Animation & reference frame comparison

The cycloid can be understood as circular motion in the frame of the rolling circle, transformed to the lab frame. In the frame of the circle's center, the point moves in a circle of radius $R$ with angular velocity $\omega$. Adding the translational velocity $R\omega$ of the center gives the lab-frame cycloid.

---
