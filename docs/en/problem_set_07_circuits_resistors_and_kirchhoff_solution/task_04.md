## Problem 4 – Voltage across $R_3$ and current through $R_3$

*(circ_1: Two parallel branches, upper branch $R_1=6\ \Omega + R_2=4\ \Omega$, lower branch $R_3=3\ \Omega + R_4=12\ \Omega$, supply $U=3\ \mathrm{V}$, points A and B at mid-nodes)*

### Step 1 — Equivalent resistance of each branch

**Upper branch** (series):

$$
R_{12} = R_1 + R_2 = 6 + 4 = 10\ \Omega
$$

**Lower branch** (series):

$$
R_{34} = R_3 + R_4 = 3 + 12 = 15\ \Omega
$$

### Step 2 — Parallel combination (total resistance)

$$
\frac{1}{R_{eq}} = \frac{1}{R_{12}} + \frac{1}{R_{34}} = \frac{1}{10} + \frac{1}{15} = \frac{3}{30} + \frac{2}{30} = \frac{5}{30}
$$

$$
\boxed{R_{eq} = 6\ \Omega}
$$

### Step 3 — Branch currents

$$
I_{12} = \frac{U}{R_{12}} = \frac{3}{10} = 0.3\ \mathrm{A}
$$

$$
I_{34} = \frac{U}{R_{34}} = \frac{3}{15} = 0.2\ \mathrm{A}
$$

### Step 4 — Voltage across $R_3$ (voltage divider in lower branch)

$$
\boxed{U_{R_3} = I_{34} \cdot R_3 = 0.2 \cdot 3 = 0.6\ \mathrm{V}}
$$

$$
\boxed{I_{R_3} = I_{34} = 0.2\ \mathrm{A}}
$$

### Step 5 — Potential difference $U_{AB}$

Taking the left node as reference (0 V), the right node is at $+U = 3\ \mathrm{V}$.

Potential at A (from the left, through $R_1$):

$$
V_A = U - I_{12} \cdot R_1 = 3 - 0.3 \cdot 6 = 3 - 1.8 = 1.2\ \mathrm{V}
$$

Potential at B (from the left, through $R_3$):

$$
V_B = U - I_{34} \cdot R_3 = 3 - 0.2 \cdot 3 = 3 - 0.6 = 2.4\ \mathrm{V}
$$

$$
\boxed{U_{AB} = V_A - V_B = 1.2 - 2.4 = -1.2\ \mathrm{V}}
$$

The negative sign means B is at higher potential than A.

---
