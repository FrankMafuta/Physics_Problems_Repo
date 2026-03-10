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