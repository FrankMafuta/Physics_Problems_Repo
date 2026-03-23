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
