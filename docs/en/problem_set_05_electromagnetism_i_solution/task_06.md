## Problem 6 – 2D Field Map


**Theory — field from $N$ charges:**

$$
\vec{E}(\vec{r}) = \sum_{i=1}^{N} k\frac{q_i(\vec{r}-\vec{r}_i)}{|\vec{r}-\vec{r}_i|^3}
$$

**Equilibrium point:** $\vec{r}^*$ where $\vec{E}(\vec{r}^*)=\vec{0}$, found by grid search minimizing $|\vec{E}|^2$.

**Stability (Earnshaw's theorem):** No stable electrostatic equilibrium exists in free space — the Laplacian of the potential satisfies $\nabla^2 V = 0$ (no charge), so no local minimum of $V$ can exist in free space.
