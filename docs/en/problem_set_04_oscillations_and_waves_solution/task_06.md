## Problem 5 – Superposition of Waves, Beats, and Group Velocity

**Given:** $y_1 = A\sin(kx - \omega t)$, $y_2 = A\sin(kx - (\omega + \Delta\omega)t)$

### 1. Resultant wave (product form)

Using sum-to-product: $\sin\alpha + \sin\beta = 2\cos\!\left(\frac{\alpha-\beta}{2}\right)\sin\!\left(\frac{\alpha+\beta}{2}\right)$

$$
y = y_1 + y_2 = 2A\cos\!\left(\frac{\Delta\omega}{2}\,t\right)\sin\!\left(kx - \left(\omega + \frac{\Delta\omega}{2}\right)t\right)
$$

$$
\boxed{y = \underbrace{2A\cos\!\left(\frac{\Delta\omega}{2}\,t\right)}_{\text{envelope (slow)}}\cdot\underbrace{\sin\!\left(kx - \left(\omega + \tfrac{\Delta\omega}{2}\right)t\right)}_{\text{carrier (fast)}}}
$$

### 2. Beat frequency and period (at $x = 0$)

The envelope oscillates at $\Delta\omega/2$, but the amplitude repeats at twice that rate (absolute value):

$$
f_{\text{beat}} = \frac{\Delta\omega}{2\pi} = \Delta f, \qquad T_{\text{beat}} = \frac{1}{\Delta f} = \frac{2\pi}{\Delta\omega}
$$

### 3. Physical interpretation

- **Carrier wave:** oscillates at the average frequency $\bar{\omega} = \omega + \Delta\omega/2$ — this is what you "hear" as the tone.
- **Envelope:** modulates amplitude slowly at frequency $\Delta\omega/(2\pi)$ — this is the periodic "wah-wah" loudness variation heard as beats.
- **Group velocity:** $v_g = d\omega/dk$ (the speed at which the envelope — and thus energy — travels).

---
