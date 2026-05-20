## Problem 7 – Equivalent resistance and potential difference A–B

*(circ_5: Bridge network with nodes A, B, C, D; $R_1=r$ (A→C), $R_2=2r$ (C→B), $R_3=r$ (A→D), $R_4=r$ (D→B), $R_5=6r$ (C→D))*

### Step 1 — Is this a balanced Wheatstone bridge?

For balance: $\dfrac{R_1}{R_2} = \dfrac{R_3}{R_4}$

$$
\frac{r}{2r} = \frac{1}{2}, \qquad \frac{r}{r} = 1 \qquad \Rightarrow \frac{1}{2} \neq 1
$$

**Not balanced** — $R_5$ carries current. Apply Kirchhoff's laws.

### Step 2 — Node voltage method (set $V_A = 0$, $V_B = V$)

KCL at node C:

$$
\frac{V_A - V_C}{R_1} = \frac{V_C - V_B}{R_2} + \frac{V_C - V_D}{R_5}
$$

$$
\frac{-V_C}{r} = \frac{V_C - V}{2r} + \frac{V_C - V_D}{6r}
$$

Multiply through by $6r$:

$$
-6V_C = 3(V_C - V) + (V_C - V_D)
$$

$$
-6V_C = 3V_C - 3V + V_C - V_D
$$

$$
\boxed{-10V_C + V_D = -3V} \quad \text{(Eq. 1)}
$$

KCL at node D:

$$
\frac{V_A - V_D}{R_3} + \frac{V_C - V_D}{R_5} = \frac{V_D - V_B}{R_4}
$$

$$
\frac{-V_D}{r} + \frac{V_C - V_D}{6r} = \frac{V_D - V}{r}
$$

Multiply through by $6r$:

$$
-6V_D + V_C - V_D = 6V_D - 6V
$$

$$
V_C - 13V_D = -6V
$$

$$
\boxed{V_C - 13V_D = -6V} \quad \text{(Eq. 2)}
$$

### Step 3 — Solve the system

From Eq. 1: $V_D = 10V_C - 3V$

Substitute into Eq. 2:

$$
V_C - 13(10V_C - 3V) = -6V
$$

$$
V_C - 130V_C + 39V = -6V
$$

$$
-129V_C = -45V \implies V_C = \frac{45}{129}V = \frac{15}{43}V
$$

$$
V_D = 10 \cdot \frac{15}{43}V - 3V = \frac{150}{43}V - \frac{129}{43}V = \frac{21}{43}V
$$

### Step 4 — Equivalent resistance $R_{AB}$

Total current from A:

$$
I_{total} = I_{R_1} + I_{R_3} = \frac{V_C}{r} + \frac{V_D}{r} = \frac{1}{r}\left(\frac{15}{43}V + \frac{21}{43}V\right) = \frac{36}{43}\cdot\frac{V}{r}
$$

$$
R_{AB} = \frac{V}{I_{total}} = \frac{V}{\frac{36}{43}\cdot\frac{V}{r}} = \frac{43r}{36}
$$

$$
\boxed{R_{AB} = \frac{43}{36}r \approx 1.194\,r}
$$

### Step 5 — Individual branch currents

$$
I_1 = \frac{V_C}{r} = \frac{15V}{43r}, \quad I_2 = \frac{V-V_C}{2r} = \frac{28V}{86r} = \frac{14V}{43r}
$$

$$
I_3 = \frac{V_D}{r} = \frac{21V}{43r}, \quad I_4 = \frac{V-V_D}{r} = \frac{22V}{43r}
$$

$$
I_5 = \frac{V_C - V_D}{6r} = \frac{(15-21)V}{43\cdot6r} = \frac{-6V}{258r} = \frac{-V}{43r}
$$

The negative sign means current in $R_5$ flows from D to C (opposite to assumed direction).

---
