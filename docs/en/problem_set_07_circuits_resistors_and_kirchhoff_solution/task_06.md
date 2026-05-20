## Problem 6 – Equivalent resistance and currents through all resistors

*(circ_3: $R_1=20\ \Omega$ left branch, $R_2=60\ \Omega$ top branch, $R_3=30\ \Omega$ + ammeter middle branch, $R_4=10\ \Omega$ right branch, $U=200\ \mathrm{V}$)*

### Step 1 — Identify the topology

From the diagram: $R_2$ (60 Ω) and $R_3$ (30 Ω) are in **parallel** between the inner nodes. This parallel combination is then in **series** with $R_1$ (20 Ω) on the left and $R_4$ (10 Ω) on the right.

$$
R_{23} = \frac{R_2 \cdot R_3}{R_2 + R_3} = \frac{60 \cdot 30}{60 + 30} = \frac{1800}{90} = 20\ \Omega
$$

### Step 2 — Total equivalent resistance

$$
R_{eq} = R_1 + R_{23} + R_4 = 20 + 20 + 10 = \boxed{50\ \Omega}
$$

### Step 3 — Total current from supply

$$
I_{total} = \frac{U}{R_{eq}} = \frac{200}{50} = 4\ \mathrm{A}
$$

This current flows through $R_1$ and $R_4$:

$$
\boxed{I_1 = I_4 = 4\ \mathrm{A}}
$$

### Step 4 — Voltage across the parallel section

$$
U_{23} = I_{total} \cdot R_{23} = 4 \cdot 20 = 80\ \mathrm{V}
$$

### Step 5 — Currents through $R_2$ and $R_3$

$$
\boxed{I_2 = \frac{U_{23}}{R_2} = \frac{80}{60} = \frac{4}{3} \approx 1.33\ \mathrm{A}}
$$

$$
\boxed{I_3 = \frac{U_{23}}{R_3} = \frac{80}{30} = \frac{8}{3} \approx 2.67\ \mathrm{A}}
$$

**Check (KCL):** $I_2 + I_3 = \frac{4}{3} + \frac{8}{3} = \frac{12}{3} = 4\ \mathrm{A} = I_{total}\ \checkmark$

**Ammeter reads:** $I_A = I_3 \approx 2.67\ \mathrm{A}$

---
