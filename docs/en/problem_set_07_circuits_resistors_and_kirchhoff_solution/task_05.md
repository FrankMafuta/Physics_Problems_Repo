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
