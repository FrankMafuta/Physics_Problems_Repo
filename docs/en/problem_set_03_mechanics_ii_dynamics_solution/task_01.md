## Task 1 – Newton's Second Law (Constant Force)

**Given:** $m = 2\ \text{kg}$, $\vec{F} = (6, 2)\ \text{N}$, $\vec{v}(0) = (1, -1)\ \text{m/s}$, $\vec{r}(0) = (0, 0)$

### Acceleration

By Newton's second law $\vec{F} = m\vec{a}$:

$$
\vec{a} = \frac{\vec{F}}{m} = \frac{(6,\ 2)}{2} = (3,\ 1)\ \text{m/s}^2
$$

### Velocity

$$
\vec{v}(t) = \vec{v}(0) + \vec{a}\,t = (1 + 3t,\ -1 + t)
$$

### Position

$$
\vec{r}(t) = \vec{r}(0) + \vec{v}(0)\,t + \tfrac{1}{2}\vec{a}\,t^2 = \left(t + \tfrac{3}{2}t^2,\ -t + \tfrac{1}{2}t^2\right)
$$

### Work done at $t = 3\ \text{s}$

Using the work-energy theorem $W = \Delta E_k$:

$$
\vec{v}(3) = (1+9,\ -1+3) = (10,\ 2)\ \text{m/s}
$$

$$
E_k(0) = \tfrac{1}{2} \cdot 2 \cdot (1^2 + 1^2) = 2\ \text{J}
$$

$$
E_k(3) = \tfrac{1}{2} \cdot 2 \cdot (100 + 4) = 104\ \text{J}
$$

$$
\boxed{W = \Delta E_k = 104 - 2 = 102\ \text{J}}
$$

**Verification via direct calculation:**

$$
\vec{r}(3) = (3 + 13.5,\ -3 + 4.5) = (16.5,\ 1.5)\ \text{m}
$$

$$
W = \vec{F} \cdot \vec{r}(3) = 6 \cdot 16.5 + 2 \cdot 1.5 = 99 + 3 = 102\ \text{J} \checkmark
$$

---