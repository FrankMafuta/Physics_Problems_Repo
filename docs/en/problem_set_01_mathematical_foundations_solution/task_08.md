## Task 8 – First-Order Differential Equation

$$
\frac{dy}{dt} = -k y
$$

### 1. Solution

This is a separable ODE. Separating variables:

$$
\frac{dy}{y} = -k\, dt
$$

Integrating both sides:

$$
\ln|y| = -kt + C_1 \;\Rightarrow\; y(t) = Ce^{-kt}, \quad C = y(0)
$$

$$
\boxed{y(t) = y_0\, e^{-kt}}
$$

For $k > 0$: exponential decay. For $k < 0$: exponential growth.
