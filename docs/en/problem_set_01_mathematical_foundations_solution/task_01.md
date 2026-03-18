# Task1 – Mathematical Foundations – Solutions

---

## Task 1 – Vectors and Linear Transformations

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
