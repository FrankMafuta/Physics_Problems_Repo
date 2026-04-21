## Problem 9 – Chain of $N$ Springs

**Equations of motion** for mass $i$ ($1 \le i \le N$):

$$
m\ddot{x}_i = k(x_{i+1} - x_i) - k(x_i - x_{i-1}) = k(x_{i+1} - 2x_i + x_{i-1})
$$

This is the **discrete wave equation**. In the long-wavelength limit ($\lambda \gg a$, lattice spacing):

$$
\frac{\partial^2 x}{\partial t^2} = \frac{ka^2}{m}\frac{\partial^2 x}{\partial s^2} \implies v_{\text{wave}} = a\sqrt{\frac{k}{m}}
$$

The dispersion relation is: $\omega(q) = 2\sqrt{k/m}\,\left|\sin\!\left(\frac{qa}{2}\right)\right|$

For small $q$: $\omega \approx v_{\text{wave}}\,q$ (linear, non-dispersive).

---
