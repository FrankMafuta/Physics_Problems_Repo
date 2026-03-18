# Problem Set 1 – Mathematical Foundations – Solutions

---

## Problem 1 – Vectors and Linear Transformations

**Given:**

$$
\vec{a} = (2, -1, 3), \qquad \vec{b} = (1, 4, -2)
$$

### Lengths of the vectors

$$
|\vec{a}| = \sqrt{2^2 + (-1)^2 + 3^2} = \sqrt{4 + 1 + 9} = \sqrt{14}
$$

$$
|\vec{b}| = \sqrt{1^2 + 4^2 + (-2)^2} = \sqrt{1 + 16 + 4} = \sqrt{21}
$$

### Normalized vector $\hat{a}$

$$
\hat{a} = \frac{\vec{a}}{|\vec{a}|} = \frac{1}{\sqrt{14}}(2, -1, 3) = \left(\frac{2}{\sqrt{14}},\; \frac{-1}{\sqrt{14}},\; \frac{3}{\sqrt{14}}\right)
$$

### Dot product and angle

$$
\vec{a} \cdot \vec{b} = 2 \cdot 1 + (-1) \cdot 4 + 3 \cdot (-2) = 2 - 4 - 6 = -8
$$

$$
\cos\theta = \frac{\vec{a} \cdot \vec{b}}{|\vec{a}||\vec{b}|} = \frac{-8}{\sqrt{14}\cdot\sqrt{21}} = \frac{-8}{\sqrt{294}}
$$

$$
\theta = \arccos\!\left(\frac{-8}{\sqrt{294}}\right) \approx \arccos(-0.4664) \approx 117.8°
$$

### Cross product and area of the parallelogram

$$
\vec{a} \times \vec{b} =
\begin{vmatrix}
\vec{i} & \vec{j} & \vec{k} \\
2 & -1 & 3 \\
1 & 4 & -2
\end{vmatrix}
= \vec{i}\bigl((-1)(-2) - 3\cdot4\bigr) - \vec{j}\bigl(2(-2) - 3\cdot1\bigr) + \vec{k}\bigl(2\cdot4 - (-1)\cdot1\bigr)
$$

$$
= \vec{i}(2 - 12) - \vec{j}(-4 - 3) + \vec{k}(8 + 1) = (-10,\; 7,\; 9)
$$

$$
S = |\vec{a} \times \vec{b}| = \sqrt{(-10)^2 + 7^2 + 9^2} = \sqrt{100 + 49 + 81} = \sqrt{230}
$$

### Matrix operations

$$
A = \begin{pmatrix} 2 & 1 & 0 \\ 0 & 1 & -1 \\ 1 & 0 & 1 \end{pmatrix}
$$

**Product $A\vec{a}$:**

$$
A\vec{a} = \begin{pmatrix} 2 & 1 & 0 \\ 0 & 1 & -1 \\ 1 & 0 & 1 \end{pmatrix} \begin{pmatrix} 2 \\ -1 \\ 3 \end{pmatrix} = \begin{pmatrix} 2\cdot2 + 1\cdot(-1) + 0\cdot3 \\ 0\cdot2 + 1\cdot(-1) + (-1)\cdot3 \\ 1\cdot2 + 0\cdot(-1) + 1\cdot3 \end{pmatrix} = \begin{pmatrix} 3 \\ -4 \\ 5 \end{pmatrix}
$$

**Determinant** (expansion along first row):

$$
\det A = 2\begin{vmatrix}1 & -1 \\ 0 & 1\end{vmatrix} - 1\begin{vmatrix}0 & -1 \\ 1 & 1\end{vmatrix} + 0
= 2(1\cdot1 - (-1)\cdot0) - 1(0\cdot1 - (-1)\cdot1)
$$

$$
= 2(1) - 1(1) = 2 - 1 = 1
$$

**Orientation:** Since $\det A = 1 > 0$, the transformation **preserves** the orientation of space.

---

## Problem 2 – Parametric Trajectory, Velocity, and Acceleration

**Given:**

$$
\vec{r}(t) = \bigl(t^2,\; \sin t,\; 5\bigr)
$$

### Velocity

$$
\vec{v}(t) = \frac{d\vec{r}}{dt} = (2t,\; \cos t,\; 0)
$$

### Acceleration

$$
\vec{a}(t) = \frac{d^2\vec{r}}{dt^2} = (2,\; -\sin t,\; 0)
$$

### Speed at $t = 1$

$$
|\vec{v}(1)| = \sqrt{(2\cdot1)^2 + \cos^2(1) + 0^2} = \sqrt{4 + \cos^2(1)} \approx \sqrt{4 + 0.2919} \approx \sqrt{4.2919} \approx 2.072
$$

### Dot product $\vec{v} \cdot \vec{a}$

$$
\vec{v}(t) \cdot \vec{a}(t) = 2t \cdot 2 + \cos t \cdot (-\sin t) + 0 = 4t - \frac{1}{2}\sin(2t)
$$

### Cross product $\vec{v} \times \vec{a}$

$$
\vec{v} \times \vec{a} =
\begin{vmatrix}
\vec{i} & \vec{j} & \vec{k} \\
2t & \cos t & 0 \\
2 & -\sin t & 0
\end{vmatrix}
= \vec{i}(0 - 0) - \vec{j}(0 - 0) + \vec{k}\bigl(2t\cdot(-\sin t) - \cos t \cdot 2\bigr)
$$

$$
= \bigl(0,\; 0,\; -2t\sin t - 2\cos t\bigr)
$$

---

## Problem 3 – Integration of Motion

### Part A

**Given:**

$$
\vec{v}(t) = (2t,\; 3,\; -e^{-t}), \qquad \vec{r}(0) = (0, 1, 2)
$$

**Position:**

$$
\vec{r}(t) = \vec{r}(0) + \int_0^t \vec{v}(\tau)\, d\tau = (0,1,2) + \left(\int_0^t 2\tau\, d\tau,\; \int_0^t 3\, d\tau,\; \int_0^t -e^{-\tau}\, d\tau\right)
$$

$$
= (0,1,2) + \bigl(t^2,\; 3t,\; e^{-t} - 1\bigr) = \bigl(t^2,\; 1 + 3t,\; 1 + e^{-t}\bigr)
$$

**Acceleration:**

$$
\vec{a}(t) = \frac{d\vec{v}}{dt} = (2,\; 0,\; e^{-t})
$$

---

### Part B

**Given:**

$$
\vec{a}(t) = (4,\; -\sin t,\; 0), \qquad \vec{v}(0) = (1, 0, 2), \qquad \vec{r}(0) = (0, 0, 0)
$$

**Velocity:**

$$
\vec{v}(t) = \vec{v}(0) + \int_0^t \vec{a}(\tau)\, d\tau = (1,0,2) + \bigl(4t,\; \cos t - 1,\; 0\bigr) = \bigl(1 + 4t,\; \cos t - 1,\; 2\bigr)
$$

**Position:**

$$
\vec{r}(t) = \vec{r}(0) + \int_0^t \vec{v}(\tau)\, d\tau = (0,0,0) + \left(\int_0^t(1+4\tau)\,d\tau,\; \int_0^t(\cos\tau-1)\,d\tau,\; \int_0^t 2\, d\tau\right)
$$

$$
= \bigl(t + 2t^2,\; \sin t - t,\; 2t\bigr)
$$

---

## Problem 4 – Geometry of Parametric Curves

### A) Circle: $x(t) = R\cos t,\quad y(t) = R\sin t$

**Elimination of parameter:**

$$
x^2 + y^2 = R^2\cos^2 t + R^2\sin^2 t = R^2 \quad \Rightarrow \quad \text{circle of radius } R
$$

**Velocity and acceleration:**

$$
\vec{v}(t) = (-R\sin t,\; R\cos t), \qquad \vec{a}(t) = (-R\cos t,\; -R\sin t)
$$

**Magnitudes:**

$$
|\vec{v}| = \sqrt{R^2\sin^2 t + R^2\cos^2 t} = R = \text{const}
$$

$$
|\vec{a}| = R = \text{const}
$$

---

### B) Ellipse: $x(t) = a\cos t,\quad y(t) = b\sin t$

**Elimination of parameter:**

$$
\frac{x^2}{a^2} + \frac{y^2}{b^2} = \cos^2 t + \sin^2 t = 1 \quad \Rightarrow \quad \text{ellipse with semi-axes } a, b
$$

**Velocity and acceleration:**

$$
\vec{v}(t) = (-a\sin t,\; b\cos t), \qquad \vec{a}(t) = (-a\cos t,\; -b\sin t)
$$

**Magnitudes:**

$$
|\vec{v}| = \sqrt{a^2\sin^2 t + b^2\cos^2 t} \neq \text{const (unless } a = b\text{)}
$$

$$
|\vec{a}| = \sqrt{a^2\cos^2 t + b^2\sin^2 t} \neq \text{const (unless } a = b\text{)}
$$

---

### C) Parabola: $x(t) = t,\quad y(t) = t^2$

**Elimination of parameter:**

$$
x = t \;\Rightarrow\; y = x^2 \quad \Rightarrow \quad \text{upward-opening parabola}
$$

**Velocity and acceleration:**

$$
\vec{v}(t) = (1,\; 2t), \qquad \vec{a}(t) = (0,\; 2)
$$

**Magnitudes:**

$$
|\vec{v}| = \sqrt{1 + 4t^2} \neq \text{const}, \qquad |\vec{a}| = 2 = \text{const}
$$

---

### D) Hyperbola: $x(t) = \cosh t,\quad y(t) = \sinh t$

**Elimination of parameter** (using the identity $\cosh^2 t - \sinh^2 t = 1$):

$$
x^2 - y^2 = 1 \quad \Rightarrow \quad \text{right branch of unit hyperbola}
$$

**Velocity and acceleration:**

$$
\vec{v}(t) = (\sinh t,\; \cosh t), \qquad \vec{a}(t) = (\cosh t,\; \sinh t)
$$

**Magnitudes:**

$$
|\vec{v}| = \sqrt{\sinh^2 t + \cosh^2 t} = \sqrt{\cosh(2t)} \neq \text{const}
$$

$$
|\vec{a}| = \sqrt{\cosh^2 t + \sinh^2 t} = \sqrt{\cosh(2t)} \neq \text{const}
$$

---

## Problem 5 – Trajectory Curvature and Normal Acceleration

**Given ellipse:**

$$
x = a\cos t, \qquad y = b\sin t
$$

### 1. Velocity and acceleration

$$
\vec{v}(t) = (-a\sin t,\; b\cos t), \qquad \vec{a}(t) = (-a\cos t,\; -b\sin t)
$$

$$
|\vec{v}(t)| = \sqrt{a^2\sin^2 t + b^2\cos^2 t}
$$

### 2. Unit tangent vector

$$
\hat{T}(t) = \frac{\vec{v}(t)}{|\vec{v}(t)|} = \frac{(-a\sin t,\; b\cos t)}{\sqrt{a^2\sin^2 t + b^2\cos^2 t}}
$$

### 3. Decomposition of acceleration

**Tangential component:**

$$
a_t = \frac{\vec{v} \cdot \vec{a}}{|\vec{v}|} = \frac{(-a\sin t)(-a\cos t) + (b\cos t)(-b\sin t)}{|\vec{v}|} = \frac{a^2\sin t\cos t - b^2\sin t\cos t}{|\vec{v}|}
$$

$$
a_t = \frac{(a^2 - b^2)\sin t\cos t}{|\vec{v}|} = \frac{\frac{1}{2}(a^2 - b^2)\sin(2t)}{|\vec{v}|}
$$

$$
\vec{a}_t = a_t\,\hat{T}
$$

**Normal component:**

$$
\vec{a}_n = \vec{a} - \vec{a}_t
$$

$$
a_n = |\vec{a}_n| = \sqrt{|\vec{a}|^2 - a_t^2}
$$

where $|\vec{a}|^2 = a^2\cos^2 t + b^2\sin^2 t$.

### 4. Radius of curvature at $t = 0$

At $t = 0$: $\;x = a,\; y = 0$

$$
\vec{v}(0) = (0,\; b), \quad |\vec{v}(0)| = b
$$

$$
\vec{a}(0) = (-a,\; 0), \quad |\vec{a}(0)| = a
$$

At $t = 0$, $\sin t = 0$, so $a_t = 0$. Hence $\vec{a}_n = \vec{a}(0) = (-a, 0)$ and $a_n = a$.

$$
a_n = \frac{v^2}{R} \;\Rightarrow\; R = \frac{v^2}{a_n} = \frac{b^2}{a}
$$

### 5. Comparison with circle ($a = b$)

$$
R = \frac{b^2}{a} \xrightarrow{a=b} R = \frac{a^2}{a} = a \checkmark
$$

This is consistent — for a circle of radius $a$, the radius of curvature equals $a$ everywhere.

### Physical interpretation

- **Greater curvature $\Rightarrow$ greater normal acceleration**: Yes, since $a_n = v^2/R$, a smaller $R$ means larger $a_n$ (for fixed speed).
- **Where is the ellipse more curved?** At the end of the **minor semi-axis** ($t = \pi/2$, point $(0, b)$), where $R = a^2/b < b$ (assuming $a > b$). The curve is most curved where the semi-axis is shortest.
- **Physical meaning of normal acceleration**: Normal acceleration does not change the speed, only the direction of $\vec{v}$. It is the centripetal cause of changing direction, always pointing toward the center of curvature.

---

## Problem 6 – Curve Length and Numerical Integration

**Given trajectory:**

$$
x(t) = t, \qquad y(t) = t^2, \qquad t \in [0, 1]
$$

### 1. Velocity vector

$$
\vec{v}(t) = \frac{d\vec{r}}{dt} = (1,\; 2t)
$$

### 2. Speed

$$
|\vec{v}(t)| = \sqrt{1 + 4t^2}
$$

### 3. Arc length integral

$$
s = \int_0^1 \sqrt{1 + 4t^2}\, dt
$$

### 4. Analytical solution

Using the standard formula $\displaystyle\int\sqrt{1 + u^2}\,du = \tfrac{1}{2}\bigl(u\sqrt{1+u^2} + \ln|u + \sqrt{1+u^2}|\bigr)$, substitute $u = 2t$:

$$
s = \int_0^1 \sqrt{1 + 4t^2}\, dt = \frac{1}{2}\left[t\sqrt{1+4t^2} + \frac{1}{2}\ln\!\left(2t + \sqrt{1+4t^2}\right)\right]_0^1
$$

$$
= \frac{1}{2}\left[\sqrt{5} + \frac{1}{2}\ln\!\left(2 + \sqrt{5}\right) - 0 - \frac{1}{2}\ln(1)\right]
$$

$$
s = \frac{\sqrt{5}}{2} + \frac{1}{4}\ln\!\left(2 + \sqrt{5}\right) \approx \frac{2.2361}{2} + \frac{1}{4}\ln(4.2361) \approx 1.1180 + \frac{1.4436}{4} \approx 1.4789
$$

### 5. Trapezoidal rule (HTML/JS)

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Arc Length – Trapezoidal Rule</title>
  <style>
    body { font-family: Arial, sans-serif; max-width: 700px; margin: 2rem auto; }
    canvas { border: 1px solid #ccc; display: block; margin: 1rem 0; }
    label { font-weight: bold; }
  </style>
</head>
<body>
  <h2>Arc Length of y = x² on [0,1]</h2>
  <label>N (divisions): <input type="range" id="N" min="2" max="500" value="10" oninput="update()"></label>
  <span id="Nval">10</span>
  <p>Trapezoidal approximation: <strong id="approx">–</strong></p>
  <p>Analytical value: <strong>≈ 1.47894</strong></p>
  <p>Error: <strong id="err">–</strong></p>
  <canvas id="traj" width="300" height="300"></canvas>
  <canvas id="errplot" width="500" height="200"></canvas>

  <script>
    const analytical = Math.sqrt(5)/2 + Math.log(2 + Math.sqrt(5))/4;

    function f(t) { return Math.sqrt(1 + 4*t*t); }

    function trapezoid(N) {
      const h = 1/N;
      let s = (f(0) + f(1)) / 2;
      for (let i = 1; i < N; i++) s += f(i*h);
      return s * h;
    }

    function update() {
      const N = parseInt(document.getElementById('N').value);
      document.getElementById('Nval').textContent = N;
      const approx = trapezoid(N);
      document.getElementById('approx').textContent = approx.toFixed(8);
      document.getElementById('err').textContent = Math.abs(approx - analytical).toExponential(4);
      drawTrajectory(N);
      drawError();
    }

    function drawTrajectory(N) {
      const canvas = document.getElementById('traj');
      const ctx = canvas.getContext('2d');
      const W = canvas.width, H = canvas.height;
      ctx.clearRect(0, 0, W, H);
      // Draw parabola
      ctx.beginPath();
      ctx.strokeStyle = '#2196F3'; ctx.lineWidth = 2;
      for (let i = 0; i <= 100; i++) {
        const t = i/100, px = t*W*0.9 + 20, py = H - t*t*H*0.9 - 10;
        i === 0 ? ctx.moveTo(px,py) : ctx.lineTo(px,py);
      }
      ctx.stroke();
      // Draw trapezoid segments
      ctx.strokeStyle = '#F44336'; ctx.lineWidth = 1;
      for (let i = 0; i <= N; i++) {
        const t = i/N, px = t*W*0.9 + 20, py = H - t*t*H*0.9 - 10;
        i === 0 ? ctx.moveTo(px,py) : ctx.lineTo(px,py);
      }
      ctx.stroke();
    }

    function drawError() {
      const canvas = document.getElementById('errplot');
      const ctx = canvas.getContext('2d');
      const W = canvas.width, H = canvas.height;
      ctx.clearRect(0, 0, W, H);
      const Nmax = 100;
      const errors = [];
      for (let n = 2; n <= Nmax; n++) errors.push({n, e: Math.abs(trapezoid(n) - analytical)});
      const maxE = Math.max(...errors.map(d=>d.e));
      ctx.beginPath(); ctx.strokeStyle = '#4CAF50'; ctx.lineWidth = 2;
      errors.forEach(({n, e}, i) => {
        const x = (n-2)/(Nmax-2) * (W-40) + 20;
        const y = H - (e/maxE)*(H-20) - 10;
        i === 0 ? ctx.moveTo(x,y) : ctx.lineTo(x,y);
      });
      ctx.stroke();
      ctx.fillStyle = '#333'; ctx.font = '12px Arial';
      ctx.fillText('Error vs N (N=2..100)', 20, 15);
    }

    update();
  </script>
</body>
</html>
```

---

## Problem 7 – Work of a Force Along a Trajectory

**Given:**

$$
\vec{F}(x,y) = (y,\; 2x), \qquad x = t,\; y = t^2,\; t \in [0,1]
$$

### 1. Velocity vector

$$
\vec{v}(t) = \frac{d\vec{r}}{dt} = (1,\; 2t)
$$

### 2. Work as a line integral

$$
W = \int_C \vec{F} \cdot d\vec{r} = \int_0^1 \vec{F}(x(t), y(t)) \cdot \vec{v}(t)\, dt
$$

Substituting $x = t,\; y = t^2$:

$$
\vec{F}(t^2, t) = (t^2,\; 2t)
$$

$$
W = \int_0^1 (t^2,\; 2t) \cdot (1,\; 2t)\, dt = \int_0^1 \bigl(t^2 + 4t^2\bigr)\, dt = \int_0^1 5t^2\, dt
$$

$$
W = 5 \cdot \frac{t^3}{3}\Bigg|_0^1 = \frac{5}{3}
$$

### 3. Numerical Riemann sum (HTML/JS)

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Work – Riemann Sum</title>
  <style>body { font-family: Arial, sans-serif; max-width: 500px; margin: 2rem auto; }</style>
</head>
<body>
  <h2>Work of F = (y, 2x) along y = x²</h2>
  <label>N: <input type="range" id="N" min="1" max="1000" value="10" oninput="update()"></label>
  <span id="Nval">10</span>
  <p>Numerical W ≈ <strong id="num">–</strong></p>
  <p>Analytical W = 5/3 ≈ <strong>1.66667</strong></p>
  <p>Error: <strong id="err">–</strong></p>
  <script>
    const analytical = 5/3;
    function update() {
      const N = parseInt(document.getElementById('N').value);
      document.getElementById('Nval').textContent = N;
      const h = 1/N;
      let W = 0;
      for (let i = 0; i < N; i++) {
        const t = (i + 0.5) * h; // midpoint rule
        const Fx = t*t, Fy = 2*t;
        const vx = 1, vy = 2*t;
        W += (Fx*vx + Fy*vy) * h;
      }
      document.getElementById('num').textContent = W.toFixed(8);
      document.getElementById('err').textContent = Math.abs(W - analytical).toExponential(4);
    }
    update();
  </script>
</body>
</html>
```

---

## Problem 8 – First-Order Differential Equation

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

### 2. Visualization (HTML/JS)

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Exponential Decay/Growth</title>
  <style>
    body { font-family: Arial, sans-serif; max-width: 650px; margin: 2rem auto; }
    canvas { border: 1px solid #ccc; }
  </style>
</head>
<body>
  <h2>y(t) = y₀ · e^(−kt)</h2>
  <label>k: <input type="range" id="k" min="-3" max="3" step="0.1" value="1" oninput="update()"></label>
  <span id="kval">1.0</span><br><br>
  <label>y₀: <input type="range" id="y0" min="-5" max="5" step="0.5" value="1" oninput="update()"></label>
  <span id="y0val">1.0</span><br><br>
  <canvas id="c" width="600" height="300"></canvas>
  <script>
    function update() {
      const k = parseFloat(document.getElementById('k').value);
      const y0 = parseFloat(document.getElementById('y0').value);
      document.getElementById('kval').textContent = k.toFixed(1);
      document.getElementById('y0val').textContent = y0.toFixed(1);
      const canvas = document.getElementById('c');
      const ctx = canvas.getContext('2d');
      const W = canvas.width, H = canvas.height;
      ctx.clearRect(0, 0, W, H);
      // Axes
      ctx.strokeStyle = '#999';
      ctx.beginPath(); ctx.moveTo(40,H/2); ctx.lineTo(W-10,H/2); ctx.stroke();
      ctx.beginPath(); ctx.moveTo(40,10); ctx.lineTo(40,H-10); ctx.stroke();
      // Curve
      ctx.strokeStyle = '#2196F3'; ctx.lineWidth = 2;
      ctx.beginPath();
      const T = 5, scaleX = (W-50)/T, scaleY = (H-20)/12;
      for (let i = 0; i <= 500; i++) {
        const t = i/500*T;
        const y = y0 * Math.exp(-k*t);
        const px = 40 + t*scaleX;
        const py = H/2 - y*scaleY;
        i === 0 ? ctx.moveTo(px,py) : ctx.lineTo(px,py);
      }
      ctx.stroke();
      ctx.fillStyle='#333'; ctx.font='13px Arial';
      ctx.fillText(`k=${k.toFixed(1)}, y₀=${y0.toFixed(1)}`, 50, 25);
    }
    update();
  </script>
</body>
</html>
```

---

## Problem 9 – Harmonic Oscillator

$$
\frac{d^2x}{dt^2} + \omega^2 x = 0
$$

### 1. General solution

The characteristic equation: $\lambda^2 + \omega^2 = 0 \;\Rightarrow\; \lambda = \pm i\omega$

$$
\boxed{x(t) = A\cos(\omega t) + B\sin(\omega t)}
$$

Equivalently: $x(t) = C\cos(\omega t + \phi)$, where $C = \sqrt{A^2 + B^2}$ and $\tan\phi = -B/A$.

### 2. Solution with initial conditions

For $x(0) = x_0$ and $x'(0) = v_0$:

$$
x(0) = A = x_0
$$

$$
x'(t) = -A\omega\sin(\omega t) + B\omega\cos(\omega t) \;\Rightarrow\; x'(0) = B\omega = v_0 \;\Rightarrow\; B = \frac{v_0}{\omega}
$$

$$
\boxed{x(t) = x_0\cos(\omega t) + \frac{v_0}{\omega}\sin(\omega t)}
$$

$$
x'(t) = -x_0\omega\sin(\omega t) + v_0\cos(\omega t)
$$

$$
x''(t) = -x_0\omega^2\cos(\omega t) - v_0\omega\sin(\omega t) = -\omega^2 x(t) \checkmark
$$

### 3. Visualization (HTML/JS)

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Harmonic Oscillator</title>
  <style>
    body { font-family: Arial, sans-serif; max-width: 700px; margin: 2rem auto; }
    canvas { border: 1px solid #ccc; display: block; margin: 0.5rem 0; }
  </style>
</head>
<body>
  <h2>Harmonic Oscillator: x'' + ω²x = 0</h2>
  <label>ω: <input type="range" id="omega" min="0.5" max="5" step="0.1" value="1" oninput="update()"></label>
  <span id="wval">1.0</span><br>
  <label>x₀: <input type="range" id="x0" min="-3" max="3" step="0.1" value="1" oninput="update()"></label>
  <span id="x0val">1.0</span><br>
  <label>v₀: <input type="range" id="v0" min="-5" max="5" step="0.1" value="0" oninput="update()"></label>
  <span id="v0val">0.0</span><br><br>
  <canvas id="c" width="660" height="250"></canvas>
  <script>
    function update() {
      const omega = parseFloat(document.getElementById('omega').value);
      const x0 = parseFloat(document.getElementById('x0').value);
      const v0 = parseFloat(document.getElementById('v0').value);
      document.getElementById('wval').textContent = omega.toFixed(1);
      document.getElementById('x0val').textContent = x0.toFixed(1);
      document.getElementById('v0val').textContent = v0.toFixed(1);

      const canvas = document.getElementById('c');
      const ctx = canvas.getContext('2d');
      const W = canvas.width, H = canvas.height;
      ctx.clearRect(0, 0, W, H);

      const T = 4 * Math.PI / omega; // two full periods
      const N = 800;
      const scaleX = (W - 60) / T;
      const amp = Math.max(Math.abs(x0), Math.abs(v0/omega), 0.5);
      const scaleY = (H/2 - 20) / (2 * amp);

      ctx.strokeStyle='#ccc';
      ctx.beginPath(); ctx.moveTo(50,H/2); ctx.lineTo(W-10,H/2); ctx.stroke();

      const colors = ['#2196F3','#4CAF50','#F44336'];
      const labels = ['x(t)','x\'(t)','x\'\'(t)'];
      const funcs = [
        t =>  x0*Math.cos(omega*t) + (v0/omega)*Math.sin(omega*t),
        t => -x0*omega*Math.sin(omega*t) + v0*Math.cos(omega*t),
        t => -(x0*omega**2*Math.cos(omega*t) + v0*omega*Math.sin(omega*t))
      ];

      funcs.forEach((fn, idx) => {
        ctx.strokeStyle = colors[idx]; ctx.lineWidth = 2;
        ctx.beginPath();
        for (let i = 0; i <= N; i++) {
          const t = i/N * T;
          const px = 50 + t * scaleX;
          const py = H/2 - fn(t) * scaleY;
          i === 0 ? ctx.moveTo(px,py) : ctx.lineTo(px,py);
        }
        ctx.stroke();
        ctx.fillStyle = colors[idx]; ctx.font='13px Arial';
        ctx.fillText(labels[idx], W - 80, 20 + idx*20);
      });
    }
    update();
  </script>
</body>
</html>
```

---

## Problem 10 – Angular Momentum in Circular Motion

**Given:**

$$
\vec{r}(t) = \bigl(R\cos(\omega t),\; R\sin(\omega t),\; 0\bigr)
$$

### 1. Velocity

$$
\vec{v}(t) = \dot{\vec{r}}(t) = \bigl(-R\omega\sin(\omega t),\; R\omega\cos(\omega t),\; 0\bigr)
$$

### 2. Angular momentum

$$
\vec{L}(t) = m\,\vec{r}(t) \times \vec{v}(t)
$$

$$
\vec{r} \times \vec{v} =
\begin{vmatrix}
\vec{i} & \vec{j} & \vec{k} \\
R\cos(\omega t) & R\sin(\omega t) & 0 \\
-R\omega\sin(\omega t) & R\omega\cos(\omega t) & 0
\end{vmatrix}
$$

$$
= \vec{k}\bigl(R\cos(\omega t)\cdot R\omega\cos(\omega t) - R\sin(\omega t)\cdot(-R\omega\sin(\omega t))\bigr)
$$

$$
= \vec{k}\bigl(R^2\omega\cos^2(\omega t) + R^2\omega\sin^2(\omega t)\bigr) = R^2\omega\,\vec{k}
$$

$$
\boxed{\vec{L}(t) = mR^2\omega\,\hat{k}}
$$

### 3. Constant magnitude and perpendicularity

$$
|\vec{L}| = mR^2\omega = \text{const}
$$

The vector $\vec{L} = mR^2\omega\,\hat{k}$ points along the $z$-axis, which is **perpendicular to the $xy$-plane** of motion. $\checkmark$

### 4. Right-hand rule

Curl the fingers of the right hand in the direction of rotation (counterclockwise for $\omega > 0$). The thumb points in the $+z$ direction — consistent with $\vec{L} = mR^2\omega\,\hat{k}$ for $\omega > 0$.

### 5. (Optional) Torque and verification

For uniform circular motion, the centripetal force is:

$$
\vec{F} = -m\omega^2\vec{r} = \bigl(-m\omega^2 R\cos(\omega t),\; -m\omega^2 R\sin(\omega t),\; 0\bigr)
$$

**Torque:**

$$
\vec{\tau} = \vec{r} \times \vec{F} = \vec{r} \times (-m\omega^2\vec{r}) = -m\omega^2(\vec{r} \times \vec{r}) = \vec{0}
$$

**Verification:**

$$
\frac{d\vec{L}}{dt} = \frac{d}{dt}(mR^2\omega\,\hat{k}) = \vec{0} = \vec{\tau} \;\checkmark
$$

The angular momentum is constant because the centripetal force produces zero torque (it is parallel to $\vec{r}$).
