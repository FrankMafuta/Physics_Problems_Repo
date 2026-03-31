## Task 2 – Inclined Plane with Friction

**Setup:** mass $m$, angle $\alpha$, kinetic friction $\mu$, height $h$.

### Forces acting on the body

- Gravity component along slope: $F_{\parallel} = mg\sin\alpha$ (down the slope)
- Normal force: $N = mg\cos\alpha$
- Friction force: $F_f = \mu N = \mu mg\cos\alpha$ (up the slope, opposing motion)

### Acceleration

Applying Newton's second law along the slope:

$$
ma = mg\sin\alpha - \mu mg\cos\alpha
$$

$$
\boxed{a = g(\sin\alpha - \mu\cos\alpha)}
$$

For motion to occur we need $\tan\alpha > \mu$.

### Time of descent from height $h$

The length of the slope: $L = h/\sin\alpha$. Starting from rest ($v_0 = 0$):

$$
L = \tfrac{1}{2}at^2 \implies t = \sqrt{\frac{2L}{a}} = \sqrt{\frac{2h}{a\sin\alpha}}
$$

$$
\boxed{t = \sqrt{\frac{2h}{g\sin\alpha(\sin\alpha - \mu\cos\alpha)}}}
$$

### Final velocity

$$
\boxed{v = at = \sqrt{2aL} = \sqrt{2gh\,\frac{\sin\alpha - \mu\cos\alpha}{\sin\alpha}}}
$$

### Energy balance check

Work by gravity: $W_g = mgh$

Work by friction: $W_f = -\mu mg\cos\alpha \cdot L = -\mu mgh\cot\alpha \cdot \sin\alpha = -\mu mgh\cos\alpha/\sin\alpha \cdot \sin\alpha= -\mu mg h \frac{\cos\alpha}{\sin\alpha}\cdot \sin\alpha$

$$
W_f = -\mu mgh \frac{\cos\alpha}{\sin\alpha}
$$

Kinetic energy gained:

$$
\tfrac{1}{2}mv^2 = mgh\left(1 - \frac{\mu\cos\alpha}{\sin\alpha}\right) = W_g + W_f \checkmark
$$

---
