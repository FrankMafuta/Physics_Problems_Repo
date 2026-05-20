# Problem Set 7 – Linear Circuit Analysis: Solutions

---

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

## Problem 5 – Equivalent resistance and ammeter current

*(circ_2: Single loop, $\mathcal{E}_1=4.5\ \mathrm{V}$, $r_{w1}=1\ \Omega$, $R_1=20\ \Omega$ in top branch; $R_3=60\ \Omega$ on left, $R_2=40\ \Omega$ on right; $\mathcal{E}_2=1.5\ \mathrm{V}$, $r_{w2}=1\ \Omega$, ammeter in bottom branch — all in one single loop)*

### Circuit topology

All elements are in **one single series loop**:

$$
\mathcal{E}_1 \to r_{w1} \to R_1 \to R_2 \to \text{A} \to r_{w2} \to \mathcal{E}_2 \to R_3 \to \text{back}
$$

The two EMFs are in **series-aiding** configuration (both drive current in the same direction around the loop).

### Step 1 — Total EMF

$$
\mathcal{E}_{total} = \mathcal{E}_1 + \mathcal{E}_2 = 4.5 + 1.5 = 6\ \mathrm{V}
$$

### Step 2 — Total resistance

$$
R_{total} = r_{w1} + R_1 + R_2 + r_{w2} + R_3 = 1 + 20 + 40 + 1 + 60 = 122\ \Omega
$$

$$
\boxed{R_{eq} = 122\ \Omega}
$$

### Step 3 — Ammeter current (series circuit → same current everywhere)

$$
\boxed{I_A = \frac{\mathcal{E}_{total}}{R_{total}} = \frac{6}{122} = \frac{3}{61} \approx 0.049\ \mathrm{A} \approx 49\ \mathrm{mA}}
$$

---

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

## Problem 8 – Ammeter current (circ_4)

*(circ_4: Top branch 10 Ω; middle branch 5 Ω + 10 Ω in series; bottom branch 10 Ω; ammeter on the right side — supply voltage U)*

### Step 1 — Topology

The three horizontal paths between the left and right nodes are:
- **Top:** $10\ \Omega$
- **Middle:** $5\ \Omega + 10\ \Omega = 15\ \Omega$ in series
- **Bottom:** $10\ \Omega$

The ammeter (ideal, zero resistance) is in the **right vertical branch** connecting the middle-right node to the right main node.

### Step 2 — Identify the node structure

Let the left main node be L, right main node be R, middle-left node be M (between the 5 Ω and 10 Ω resistors).

The right side of the 10 Ω middle resistor connects to M'. The ammeter connects M' to R.

Since the ammeter is ideal: $V_{M'} = V_R$.

So the 10 Ω middle-right resistor has both ends at $V_R$ — **no current flows through it**.

### Step 3 — Effective circuit

With no current through the middle 10 Ω, the middle branch only carries current through the 5 Ω resistor from L to M', but M' = R, so the 5 Ω connects L directly to R.

Parallel combination: $10\ \Omega \parallel 5\ \Omega \parallel 10\ \Omega$

$$
\frac{1}{R_{eq}} = \frac{1}{10} + \frac{1}{5} + \frac{1}{10} = \frac{1}{10}+\frac{2}{10}+\frac{1}{10} = \frac{4}{10}
$$

$$
\boxed{R_{eq} = 2.5\ \Omega}
$$

### Step 4 — Ammeter current

The ammeter carries the current from the 5 Ω branch only (the middle 10 Ω carries zero):

$$
I_{5\Omega} = \frac{U}{5}
$$

By KCL at node M': the ammeter current equals the current arriving from the 5 Ω minus the current continuing through the middle 10 Ω. Since the middle 10 Ω current is zero:

$$
\boxed{I_A = \frac{U}{5}}
$$

For example, if $U = 10\ \mathrm{V}$: $I_A = 2\ \mathrm{A}$.

