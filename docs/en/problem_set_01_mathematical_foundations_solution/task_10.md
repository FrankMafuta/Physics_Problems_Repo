## Task 10 – Angular Momentum in Circular Motion

**Given:**

$$
\vec{r}(t) = \bigl(R\cos(\omega t),\; R\sin(\omega t),\; 0\bigr)
$$

### 1. Velocity

$$
\vec{v}(t) = \dot{\vec{r}}(t) = \bigl(-R\omega\sin(\omega t),\; R\omega\cos(\omega t),\; 0\bigr)
$$

### 2. Angular momentum

$$
\vec{L}(t) = m\,\vec{r}(t) \times \vec{v}(t)
$$

$$
\vec{r} \times \vec{v} =
\begin{vmatrix}
\vec{i} & \vec{j} & \vec{k} \\
R\cos(\omega t) & R\sin(\omega t) & 0 \\
-R\omega\sin(\omega t) & R\omega\cos(\omega t) & 0
\end{vmatrix}
$$

$$
= \vec{k}\bigl(R\cos(\omega t)\cdot R\omega\cos(\omega t) - R\sin(\omega t)\cdot(-R\omega\sin(\omega t))\bigr)
$$

$$
= \vec{k}\bigl(R^2\omega\cos^2(\omega t) + R^2\omega\sin^2(\omega t)\bigr) = R^2\omega\,\vec{k}
$$

$$
\boxed{\vec{L}(t) = mR^2\omega\,\hat{k}}
$$

### 3. Constant magnitude and perpendicularity

$$
|\vec{L}| = mR^2\omega = \text{const}
$$

The vector $\vec{L} = mR^2\omega\,\hat{k}$ points along the $z$-axis, which is **perpendicular to the $xy$-plane** of motion. $\checkmark$

### 4. Right-hand rule

Curl the fingers of the right hand in the direction of rotation (counterclockwise for $\omega > 0$). The thumb points in the $+z$ direction — consistent with $\vec{L} = mR^2\omega\,\hat{k}$ for $\omega > 0$.

### 5. (Optional) Torque and verification

For uniform circular motion, the centripetal force is:

$$
\vec{F} = -m\omega^2\vec{r} = \bigl(-m\omega^2 R\cos(\omega t),\; -m\omega^2 R\sin(\omega t),\; 0\bigr)
$$

**Torque:**

$$
\vec{\tau} = \vec{r} \times \vec{F} = \vec{r} \times (-m\omega^2\vec{r}) = -m\omega^2(\vec{r} \times \vec{r}) = \vec{0}
$$

**Verification:**

$$
\frac{d\vec{L}}{dt} = \frac{d}{dt}(mR^2\omega\,\hat{k}) = \vec{0} = \vec{\tau} \;\checkmark
$$

The angular momentum is constant because the centripetal force produces zero torque (it is parallel to $\vec{r}$).
