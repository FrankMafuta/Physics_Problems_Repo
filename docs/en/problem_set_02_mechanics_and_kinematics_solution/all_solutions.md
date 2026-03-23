# Task Set 2 – Solutions
## Mechanics I: Kinematics

---

## Task 1 – Uniform and Uniformly Accelerated Motion

**Given equation of motion:**

$$
x(t) = x_0 + v_0 t + \frac{1}{2} a t^2
$$

### 1. Velocity and acceleration by differentiation

$$
v(t) = \frac{dx}{dt} = v_0 + at
$$

$$
a(t) = \frac{dv}{dt} = a = \text{const}
$$

### 2. Numerical case: $x_0 = 0$, $v_0 = 5\ \text{m/s}$, $a = -2\ \text{m/s}^2$

**Stopping time** — body stops when $v(t_s) = 0$:

$$
v_0 + a t_s = 0 \implies t_s = -\frac{v_0}{a} = -\frac{5}{-2} = 2.5\ \text{s}
$$

**Maximum displacement** — since $a < 0$, the body decelerates and reaches maximum $x$ at $t = t_s$:

$$
x_{\max} = x(t_s) = v_0 t_s + \frac{1}{2}a t_s^2 = 5 \cdot 2.5 + \frac{1}{2}(-2)(2.5)^2 = 12.5 - 6.25 = 6.25\ \text{m}
$$

**Maximum velocity:**

- If $a > 0$: velocity grows without bound; maximum is reached as $t \to \infty$.
- If $a < 0$: velocity is maximum at $t = 0$, i.e., $v_{\max} = v_0 = 5\ \text{m/s}$.
- If $a = 0$: velocity is constant, $v(t) = v_0$.

### 3. Graphs

The three graphs $x(t)$, $v(t)$, $a(t)$ for the numerical case:

- $x(t) = 5t - t^2$ — upward parabola with vertex at $t = 2.5\ \text{s}$
- $v(t) = 5 - 2t$ — linear, crosses zero at $t = 2.5\ \text{s}$
- $a(t) = -2\ \text{m/s}^2$ — horizontal line

---

## Task 2 – Projectile Motion

**Setup:** initial velocity $v_0$, launch angle $\alpha$ from horizontal, no air resistance.

### Equations of motion

Decomposing the initial velocity:

$$
v_{0x} = v_0 \cos\alpha, \qquad v_{0y} = v_0 \sin\alpha
$$

Equations of motion (with $g$ acting downward):

$$
x(t) = v_0 \cos\alpha \cdot t
$$

$$
y(t) = v_0 \sin\alpha \cdot t - \frac{1}{2}g t^2
$$

### Time of flight

The body returns to the ground when $y(t_f) = 0$:

$$
v_0 \sin\alpha \cdot t_f - \frac{1}{2}g t_f^2 = 0
\implies t_f \left(v_0 \sin\alpha - \frac{1}{2}g t_f\right) = 0
$$

$$
\boxed{t_f = \frac{2 v_0 \sin\alpha}{g}}
$$

### Maximum height

Vertical velocity is zero at the peak:

$$
v_y = v_0 \sin\alpha - g t_H = 0 \implies t_H = \frac{v_0 \sin\alpha}{g}
$$

$$
\boxed{H = y(t_H) = \frac{v_0^2 \sin^2\alpha}{2g}}
$$

### Range

$$
\boxed{R = x(t_f) = v_0 \cos\alpha \cdot \frac{2 v_0 \sin\alpha}{g} = \frac{v_0^2 \sin(2\alpha)}{g}}
$$

### Angle for maximum range

$R$ is maximized when $\sin(2\alpha) = 1$, i.e.:

$$
\boxed{\alpha = 45°}
$$

---

## Task 3 – Elimination of Time and Interpretation of Acceleration

**Parametric path:**

$$
x(t) = 2t^2, \qquad y(t) = 3t^3
$$

### Eliminating $t$

From the first equation:

$$
t^2 = \frac{x}{2} \implies t = \sqrt{\frac{x}{2}}
$$

Substituting into $y$:

$$
y = 3t^3 = 3t \cdot t^2 = 3\sqrt{\frac{x}{2}} \cdot \frac{x}{2} = \frac{3x}{2}\sqrt{\frac{x}{2}}
$$

$$
\boxed{y = \frac{3x}{2} \cdot \sqrt{\frac{x}{2}}}
$$

This is a semicubical parabola (defined for $x \geq 0$).

### Velocity vector

$$
\vec{v}(t) = \left(\frac{dx}{dt},\ \frac{dy}{dt}\right) = (4t,\ 9t^2)
$$

$$
|\vec{v}(t)| = \sqrt{(4t)^2 + (9t^2)^2} = \sqrt{16t^2 + 81t^4} = |t|\sqrt{16 + 81t^2}
$$

### Acceleration vector

$$
\vec{a}(t) = \left(\frac{d^2x}{dt^2},\ \frac{d^2y}{dt^2}\right) = (4,\ 18t)
$$

$$
|\vec{a}(t)| = \sqrt{16 + 324t^2}
$$

### Is the acceleration constant?

No. While the $x$-component of acceleration is constant ($a_x = 4$), the $y$-component changes with time ($a_y = 18t$). Therefore:

$$
\vec{a}(t) = (4,\ 18t) \neq \text{const}
$$

---

## Task 4 – Circular Motion

**Setup:** radius $R$, angular velocity $\omega$.

### Position, velocity, acceleration vectors

$$
\vec{r}(t) = \bigl(R\cos(\omega t),\ R\sin(\omega t)\bigr)
$$

$$
\vec{v}(t) = \frac{d\vec{r}}{dt} = \bigl(-R\omega\sin(\omega t),\ R\omega\cos(\omega t)\bigr)
$$

$$
\vec{a}(t) = \frac{d\vec{v}}{dt} = \bigl(-R\omega^2\cos(\omega t),\ -R\omega^2\sin(\omega t)\bigr) = -\omega^2\,\vec{r}(t)
$$

### Magnitudes

$$
|\vec{r}(t)| = R
$$

$$
|\vec{v}(t)| = R\omega
$$

$$
|\vec{a}(t)| = R\omega^2
$$

### Centripetal nature of acceleration

Since $\vec{a}(t) = -\omega^2 \vec{r}(t)$, the acceleration vector always points **opposite to $\vec{r}$**, i.e., toward the center. This confirms it is centripetal (center-seeking).

Furthermore, $\vec{v} \cdot \vec{a} = 0$, confirming that velocity and acceleration are perpendicular at all times.

---

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

## Task 7 – 2D Motion with Given Acceleration

**Given:** $\vec{a} = (2,\ -3)$, $\vec{v}(0) = (1,\ 0)$, $\vec{r}(0) = (0,\ 0)$

### Velocity

$$
\vec{v}(t) = \vec{v}(0) + \vec{a}\,t = (1 + 2t,\ -3t)
$$

### Position

$$
\vec{r}(t) = \vec{r}(0) + \vec{v}(0)\,t + \frac{1}{2}\vec{a}\,t^2 = \left(t + t^2,\ -\frac{3}{2}t^2\right)
$$

### Trajectory (eliminating $t$)

From the $x$-component: $x = t + t^2$. This is a quadratic in $t$, so expressing $t$ in terms of $x$ and substituting into $y$ yields a parabola-like curve. The trajectory is a **parabola** in the $xy$-plane.

---

## Task 8 – Relative Motion

**Given:** $\vec{v}_A = (3,\ 1)$, $\vec{v}_B = (1,\ -2)$

### 1. Relative velocity of A with respect to B

$$
\vec{v}_{A/B} = \vec{v}_A - \vec{v}_B = (3-1,\ 1-(-2)) = (2,\ 3)
$$

### 2. Direction of relative motion

$$
\theta = \arctan\!\left(\frac{3}{2}\right) \approx 56.3°
$$

measured from the positive $x$-axis.

### 3. Reference frames

- **Lab frame (origin fixed):** both bodies move along straight lines — A along direction $(3,1)$, B along $(1,-2)$.
- **Frame of A:** body B appears to move with velocity $\vec{v}_{B/A} = \vec{v}_B - \vec{v}_A = (-2,\ -3)$.
- **Frame of B:** body A appears to move with velocity $\vec{v}_{A/B} = (2,\ 3)$.

---

## Task 9 – Change of Reference Frame (Heliocentric → Geocentric)

**Heliocentric positions:**

$$
\vec{r}_E(t) = R_E\,\bigl(\cos(\omega_E t),\ \sin(\omega_E t)\bigr)
$$

$$
\vec{r}_M(t) = R_M\,\bigl(\cos(\omega_M t),\ \sin(\omega_M t)\bigr)
$$

### Position of Mars relative to Earth

$$
\vec{r}_{M/E}(t) = \vec{r}_M(t) - \vec{r}_E(t)
$$

**Components:**

$$
x_{M/E}(t) = R_M\cos(\omega_M t) - R_E\cos(\omega_E t)
$$

$$
y_{M/E}(t) = R_M\sin(\omega_M t) - R_E\sin(\omega_E t)
$$

### Physical interpretation

Since $\omega_E > \omega_M$ (Earth orbits faster than Mars), Earth periodically "laps" Mars. In the geocentric frame, Mars traces a **retrograde loop** — it appears to move backward on the sky for a period. This is the purely kinematic origin of retrograde motion, known since antiquity and explained geometrically by the Copernican model.

---

## Task 10 – Analysis of Motion from Numerical Data

**Given:** $x(t) = t + \frac{1}{20}t^2$, $t \in [0, 10]$, $\Delta t = 0.1$

### 1. Finite difference approximation of velocity

Central difference formula:

$$
v_i \approx \frac{x_{i+1} - x_{i-1}}{2\,\Delta t}
$$

Forward/backward difference at the endpoints:

$$
v_0 \approx \frac{x_1 - x_0}{\Delta t}, \qquad v_N \approx \frac{x_N - x_{N-1}}{\Delta t}
$$

### 2. Finite difference approximation of acceleration

$$
a_i \approx \frac{x_{i+1} - 2x_i + x_{i-1}}{(\Delta t)^2}
$$

### 3. Analytical solution

$$
v(t) = \frac{dx}{dt} = 1 + \frac{t}{10}
$$

$$
a(t) = \frac{dv}{dt} = \frac{1}{10} = 0.1\ \text{m/s}^2 = \text{const}
$$

### 4. Effect of time step on accuracy

The central difference approximation has **second-order accuracy** in $\Delta t$, meaning the error scales as $O(\Delta t^2)$. Since the exact solution is a polynomial of degree 2, the finite difference approximation for acceleration is **exact** (the second finite difference of a quadratic is exact regardless of $\Delta t$). For velocity, the error is proportional to $\Delta t^2$, so halving the step size reduces the error by a factor of 4.
