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

