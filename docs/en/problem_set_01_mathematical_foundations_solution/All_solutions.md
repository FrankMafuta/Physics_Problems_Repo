Task 01 – Vectors and Linear Transformations
 
Problem Statement
 
Given the vectors  
$\vec a = (2,-1,3)$ and $\vec b = (1,4,-2)$, compute magnitudes, normalized vectors, dot and cross products, and the angle between them.  
For the matrix
 
$$
A =
\begin{pmatrix}
2 & 1 & 0 \\
0 & 1 & -1 \\
1 & 0 & 1
\end{pmatrix}
$$
 
compute $A\vec a$, $\det A$, and determine whether the transformation preserves orientation.
 
Theory
 
For a vector $\vec v = (v1,v2,v3)$:
 
• Magnitude: $|\vec v| = \sqrt{v1^2+v2^2+v3^2}$
• Normalized vector: $\hat v = \vec v / |\vec v|$
• Dot product:
 
  $$
  \vec a\cdot\vec b = a1 b1 + a2 b2 + a3 b3
  $$
• Angle:
 
  $$
  \cos\theta = \frac{\vec a\cdot\vec b}{|\vec a||\vec b|}
  $$
• Cross product:
 
  $$
  \vec a\times\vec b =
  \begin{pmatrix}
  a2 b3 - a3 b2 \\
  a3 b1 - a1 b3 \\
  a1 b2 - a2 b1
  \end{pmatrix}
  $$
• Parallelogram area: $|\vec a\times\vec b|$
• Orientation preserved if $\det A > 0$
 
Step-by-Step Solution
Vector magnitudes
 
$$
|\vec a| = \sqrt{2^2 + (-1)^2 + 3^2}
$$
 
$$
|\vec a| = \sqrt{4 + 1 + 9}
$$
 
$$
|\vec a| = \sqrt{14}
$$
 
$$
|\vec b| = \sqrt{1^2 + 4^2 + (-2)^2}
$$
 
$$
|\vec b| = \sqrt{1 + 16 + 4}
$$
 
$$
|\vec b| = \sqrt{21}
$$
 
Normalized vector
 
$$
\hat a = \frac{1}{\sqrt{14}}(2,-1,3)
$$
 
Dot product
 
$$
\vec a\cdot\vec b = 2\cdot 1 + (-1)\cdot 4 + 3\cdot(-2)
$$
 
$$
\vec a\cdot\vec b = -8
$$
 
Angle between vectors
 
$$
\cos\theta = \frac{-8}{\sqrt{14}\sqrt{21}}
$$
 
Cross product
 
$$
\vec a\times\vec b =
\begin{pmatrix}
2 - 12 \\
3 + 4 \\
8 + 1
\end{pmatrix}
$$
 
$$
\vec a\times\vec b = (-10,7,9)
$$
 
Area:
 
$$
|\vec a\times\vec b| = \sqrt{230}
$$
 
Matrix–vector multiplication
 
$$
A\vec a = (3,-4,5)
$$
 
Determinant
 
Expanding:
 
$$
\det A = 1
$$
 
Since $\det A>0$, orientation is preserved.
 
Final Result
• $|\vec a|=\sqrt{14}$  
• $|\vec b|=\sqrt{21}$  
• $\hat a = \frac{1}{\sqrt{14}}(2,-1,3)$  
• $\vec a\cdot\vec b=-8$  
• $\vec a\times\vec b=(-10,7,9)$  
• Area $=\sqrt{230}$  
• $A\vec a=(3,-4,5)$  
• $\det A = 1 > 0$
 
Interpretation
 
The vectors enclose an obtuse angle (negative dot product).  
The cross product describes the oriented area.  
The transformation preserves orientation.
 
Task 02 – Parametric Trajectory, Velocity, and Acceleration
Problem Statement
 
Given:
 
$$
\vec r(t) = (t^2,\sin t,5)
$$
 
Compute velocity, acceleration, $|\vec v(1)|$, dot and cross product of $\vec v$ and $\vec a$.
 
Theory
• Velocity: $\vec v = d\vec r/dt$
• Acceleration: $\vec a = d^2\vec r/dt^2$
 
Step-by-Step Solution
Velocity
 
$$
\vec v(t) = (2t,\cos t,0)
$$
 
Acceleration
 
$$
\vec a(t) = (2,-\sin t,0)
$$
 
Speed at \( t=1 \)
 
$$
|\vec v(1)| = \sqrt{4+\cos^2 1}
$$
 
Dot product
 
$$
\vec v\cdot\vec a = 4t - \cos t\sin t
$$
 
Cross product
 
$$
\vec v\times\vec a = (0,0,-2t\sin t -2\cos t)
$$
 
Final Result
• $\vec v(t)=(2t,\cos t,0)$  
• $\vec a(t)=(2,-\sin t,0)$  
• $|\vec v(1)|=\sqrt{4+\cos^2 1}$  
• $\vec v\cdot\vec a=4t-\cos t\sin t$  
• $\vec v\times\vec a=(0,0,-2t\sin t -2\cos t)$
 
Interpretation
 
The motion stays in the $xy$-plane. The cross product is perpendicular to it.
 
Task 03 – Integration of Motion
Problem Statement
 
A) Given velocity  
$\vec v(t)=(2t,3,-e^{-t})$, with $\vec r(0)=(0,1,2)$.
 
B) Given acceleration  
$\vec a(t)=(4,-\sin t,0)$, with $\vec v(0)=(1,0,2)$ and $\vec r(0)=(0,0,0)$.
 
Theory
 
Integration of velocity gives position.  
Integration of acceleration gives velocity.
 
Step-by-Step Solution
Part A1: Position
 
Integrate each component:
 
$$
\int0^t (2\tau)\,d\tau = t^2
$$
 
$$
\int0^t 3\,d\tau = 3t
$$
 
$$
\int0^t -e^{-\tau}\,d\tau = e^{-t}-1
$$
 
Thus
 
$$
\vec r(t)=(t^2,\,1+3t,\,2+e^{-t}-1)
$$
 
$$
\vec r(t) = (t^2,\,1+3t,\,1+e^{-t})
$$
 
Part A2: Acceleration
 
Differentiate $\vec v$:
 
$$
\vec a(t)=(2,0,e^{-t})
$$
 
Part B1: Velocity
 
Integrate:
 
$$
\int0^t 4\,d\tau = 4t
$$
 
$$
\int0^t -\sin\tau\,d\tau = \cos t - 1
$$
 
$$
\int0^t 0\,d\tau = 0
$$
 
Thus
 
$$
\vec v(t)=(1+4t,\;\cos t -1,\;2)
$$
 
Part B2: Position
 
Integrate:
 
$$
\int0^t (1+4\tau)\,d\tau = t + 2t^2
$$
 
$$
\int0^t (\cos\tau -1)d\tau = \sin t - t
$$
 
$$
\int0^t 2\,d\tau = 2t
$$
 
Thus
 
$$
\vec r(t) = (t+2t^2,\;\sin t - t,\;2t)
$$
 
Final Result
 
Part A:  
$\vec r(t)=(t^2,1+3t,1+e^{-t})$  
$\vec a(t)=(2,0,e^{-t})$
 
Part B:  
$\vec v(t)=(1+4t,\cos t -1,2)$  
$\vec r(t)=(t+2t^2,\sin t - t,2t)$
 
Task 04 – Geometry of Parametric Curves
 
For each curve: eliminate parameter (if possible), identify, compute $\vec v$ and $\vec a$, and check constancy of speed/acceleration.
 
A) Circle
 
$x=R\cos t$, $y=R\sin t$.
 
Eliminate parameter
 
$$
x^2+y^2=R^2
$$
 
Circle.
 
Velocity
 
$$
\vec v=(-R\sin t, R\cos t)
$$
 
Acceleration
 
$$
\vec a=(-R\cos t,-R\sin t)
$$
 
Speed magnitude
 
$$
|\vec v|=R
$$
 
Constant.
 
B) Ellipse
 
$x=a\cos t$, $y=b\sin t$.
 
Eliminate parameter
 
$$
\frac{x^2}{a^2}+\frac{y^2}{b^2}=1
$$
 
Ellipse.
 
Velocity
 
$$
\vec v=(-a\sin t, b\cos t)
$$
 
Acceleration
 
$$
\vec a=(-a\cos t,-b\sin t)
$$
 
Speed magnitude
 
$$
|\vec v|=\sqrt{a^2\sin^2 t + b^2\cos^2 t}
$$
 
Not constant unless $a=b$.
 
C) Parabola
 
$x=t$, $y=t^2$.
 
Eliminate
 
$t=x$, thus $y=x^2$.
 
Velocity
 
$$
\vec v=(1,2t)
$$
 
Acceleration
 
$$
\vec a=(0,2)
$$
 
Speed
 
$$
|\vec v|=\sqrt{1+4t^2}
$$
 
Not constant.
 
D) Hyperbolic curve
 
$x=\cosh t$, $y=\sinh t$.
 
Eliminate
 
$$
x^2-y^2=1
$$
 
Hyperbola.
 
Velocity
 
$$
\vec v=(\sinh t,\cosh t)
$$
 
Acceleration
 
$$
\vec a=(\cosh t,\sinh t)
$$
 
Speed
 
$$
|\vec v|=\sqrt{\sinh^2 t+\cosh^2 t}
$$
 
Not constant.
 
Task 05 – Trajectory Curvature and Normal Acceleration
 
Given ellipse:
 
$$
x=a\cos t,\qquad y=b\sin t
$$
 
Theory
• Tangent unit vector: $\hat T = \vec v/|\vec v|$
• Decomposition: $\vec a=\vec at+\vec an$
• Normal acceleration magnitude:
 
$$
an=\frac{v^2}{R}
$$
 
Step-by-Step Solution
Velocity
 
$$
\vec v=(-a\sin t,b\cos t)
$$
 
Acceleration
 
$$
\vec a=(-a\cos t,-b\sin t)
$$
 
Speed squared
 
$$
v^2 = a^2 \sin^2 t + b^2 \cos^2 t
$$
 
Unit tangent
 
$$
\hat T = \frac{\vec v}{\sqrt{a^2\sin^2 t + b^2\cos^2 t}}
$$
 
Normal acceleration
 
Compute projection:
 
$$
an = \frac{v^2}{R}
$$
 
At \(t=0\):
 
$$
v^2(0) = b^2
$$
 
Radius of curvature for ellipse at \(t=0\):
 
$$
R(0)=\frac{a^2}{b}
$$
 
Thus
 
$$
an(0)=\frac{b^2}{a^2/b} = \frac{b^3}{a^2}
$$
 
Circle comparison
 
If $a=b=R$:
 
$$
R(0)=R
$$
 
Normal acceleration equals $v^2/R$.
 
Interpretation
• Larger curvature → larger normal acceleration.  
• Ellipse curvature is largest at ends of minor axis.  
• Normal acceleration changes the direction of velocity.
 
Task 06 – Curve Length and Numerical Integration
 
Given $x=t$, $y=t^2$, $t\in[0,1]$.
 
Step-by-Step Solution
Velocity
 
$$
\vec v = (1,2t)
$$
 
Speed magnitude
 
$$
|\vec v|=\sqrt{1+4t^2}
$$
 
Arc length integral
 
$$
s=\int0^1 \sqrt{1+4t^2}\,dt
$$
 
This integral has the closed form:
 
$$
\frac{1}{4}\left(2t\sqrt{1+4t^2}+\sinh^{-1}(2t)\right)\Big|0^1
$$
 
Numerical method: trapezoidal rule
 
HTML/JS implementation would evaluate subintervals and compute convergence.
 
Task 07 – Work of a Force Along a Trajectory
 
Force:
 
$$
\vec F=(y,2x)
$$
 
Trajectory:
 
$$
x=t,\qquad y=t^2
$$
 
Step-by-Step Solution
Velocity
 
$$
\vec v=(1,2t)
$$
 
Work integral
 
Compute:
 
$$
\vec F(t)=(t^2,2t)
$$
 
Dot product:
 
$$
\vec F\cdot\vec v = t^2\cdot 1 + 2t\cdot 2t = t^2 + 4t^2 = 5t^2
$$
 
Thus
 
$$
W=\int0^1 5t^2\,dt = \frac{5}{3}
$$
 
Task 08 – First-Order Differential Equation
 
Equation:
 
$$
\frac{dy}{dt}=-ky
$$
 
Solution
 
Separate variables:
 
$$
\frac{dy}{y}=-k\,dt
$$
 
Integrate:
 
$$
\ln y = -kt + C
$$
 
Exponentiate:
 
$$
y(t)=y_0 e^{-kt}
$$
 
Task 09 – Harmonic Oscillator
 
Equation:
 
$$
x''+\omega^2 x=0
$$
 
General solution
 
$$
x(t)=A\cos(\omega t)+B\sin(\omega t)
$$
 
Initial conditions determine \(A\) and \(B\).
 
Task 10 – Angular Momentum in Circular Motion
 
Trajectory:
 
$$
\vec r=(R\cos\omega t,\;R\sin\omega t,\;0)
$$
 
Velocity
 
$$
\vec v=(-R\omega\sin\omega t,\;R\omega\cos\omega t,\;0)
$$
 
Angular momentum
 
$$
\vec L=m(\vec r\times\vec v)
$$
 
Compute cross product:
 
$$
\vec L = (0,0,mR^2\omega)
$$
 
Magnitude:
 
$$
|\vec L|=mR^2\omega
$$
 
Constant.
 
Vector is perpendicular to the plane.