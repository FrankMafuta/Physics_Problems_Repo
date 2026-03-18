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
 