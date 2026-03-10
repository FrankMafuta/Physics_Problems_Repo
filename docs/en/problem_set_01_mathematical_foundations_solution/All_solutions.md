Below is a **Markdown solution format that will render correctly in VS Code** (Markdown preview) because it uses:

* `$$ ... $$` for display math
* `$ ... $` for inline math
* clean Markdown structure

You can **copy this directly into `task_01.md`** inside your repository and it will render properly.

---

# Problem 1 – Vectors and Linear Transformations

## Given vectors

$$
\vec a = (2,-1,3), \qquad
\vec b = (1,4,-2)
$$

---

# 1. Vector lengths

The length of a vector is

$$
|\vec v| = \sqrt{x^2+y^2+z^2}
$$

### Length of $\vec a$

$$
|\vec a|
========

\sqrt{2^2 + (-1)^2 + 3^2}
$$

# $$

\sqrt{4 + 1 + 9}
$$

# $$

\sqrt{14}
$$

---

### Length of $\vec b$

$$
|\vec b|
========

\sqrt{1^2 + 4^2 + (-2)^2}
$$

# $$

\sqrt{1 + 16 + 4}
$$

# $$

\sqrt{21}
$$

---

# 2. Normalized vector

The normalized vector is defined as

$$
\hat a = \frac{\vec a}{|\vec a|}
$$

Substitute the values:

$$
\hat a =
\frac{(2,-1,3)}{\sqrt{14}}
$$

# $$

\left(
\frac{2}{\sqrt{14}},
\frac{-1}{\sqrt{14}},
\frac{3}{\sqrt{14}}
\right)
$$

---

# 3. Dot product and angle between vectors

The dot product is

$$
\vec a \cdot \vec b =
a_x b_x + a_y b_y + a_z b_z
$$

Substitute the components:

$$
\vec a \cdot \vec b =
(2)(1) + (-1)(4) + (3)(-2)
$$

$$
= 2 - 4 - 6
$$

$$
= -8
$$

---

### Angle between vectors

The formula for the angle is

$$
\cos\theta =
\frac{\vec a \cdot \vec b}{|\vec a||\vec b|}
$$

Substitute values:

$$
\cos\theta =
\frac{-8}{\sqrt{14}\sqrt{21}}
$$

# $$

\frac{-8}{\sqrt{294}}
$$

Thus

$$
\theta =
\cos^{-1}
\left(
\frac{-8}{\sqrt{294}}
\right)
$$

---

# 4. Cross product

The cross product is

$$
\vec a \times \vec b =
\begin{vmatrix}
\mathbf i & \mathbf j & \mathbf k \
2 & -1 & 3 \
1 & 4 & -2
\end{vmatrix}
$$

Expanding the determinant:

# $$

\mathbf i
\begin{vmatrix}
-1 & 3 \
4 & -2
\end{vmatrix}
-------------

\mathbf j
\begin{vmatrix}
2 & 3 \
1 & -2
\end{vmatrix}
+
\mathbf k
\begin{vmatrix}
2 & -1 \
1 & 4
\end{vmatrix}
$$

Compute each minor:

$$
\begin{vmatrix}
-1 & 3 \
4 & -2
\end{vmatrix}
= (-1)(-2) - (3)(4) = 2 - 12 = -10
$$

$$
\begin{vmatrix}
2 & 3 \
1 & -2
\end{vmatrix}
= (2)(-2) - (3)(1) = -4 - 3 = -7
$$

$$
\begin{vmatrix}
2 & -1 \
1 & 4
\end{vmatrix}
= (2)(4) - (-1)(1) = 8 + 1 = 9
$$

Thus

$$
\vec a \times \vec b =
(-10, 7, 9)
$$

---

# 5. Area of the parallelogram

The area is the magnitude of the cross product:

$$
A = |\vec a \times \vec b|
$$

# $$

\sqrt{(-10)^2 + 7^2 + 9^2}
$$

# $$

\sqrt{100 + 49 + 81}
$$

# $$

\sqrt{230}
$$

---

# Matrix operations

Matrix:

$$
A =
\begin{pmatrix}
2 & 1 & 0 \
0 & 1 & -1 \
1 & 0 & 1
\end{pmatrix}
$$

---

# 6. Calculate $A\vec a$

Multiply the matrix by vector $\vec a$:

$$
A\vec a =
\begin{pmatrix}
2 & 1 & 0 \
0 & 1 & -1 \
1 & 0 & 1
\end{pmatrix}
\begin{pmatrix}
2\
-1\
3
\end{pmatrix}
$$

First row:

$$
2(2) + 1(-1) + 0(3) = 4 -1 = 3
$$

Second row:

$$
0(2) + 1(-1) + (-1)(3) = -1 -3 = -4
$$

Third row:

$$
1(2) + 0(-1) + 1(3) = 2 +3 = 5
$$

Thus

$$
A\vec a =
\begin{pmatrix}
3\
-4\
5
\end{pmatrix}
$$

---

# 7. Determinant of $A$

$$
\det A =
\begin{vmatrix}
2 & 1 & 0 \
0 & 1 & -1 \
1 & 0 & 1
\end{vmatrix}
$$

Expand along the first row:

# $$

2
\begin{vmatrix}
1 & -1 \
0 & 1
\end{vmatrix}
-------------

1
\begin{vmatrix}
0 & -1 \
1 & 1
\end{vmatrix}
+
0
\begin{vmatrix}
0 & 1 \
1 & 0
\end{vmatrix}
$$

Compute minors:

$$
\begin{vmatrix}
1 & -1 \
0 & 1
\end{vmatrix}
= 1
$$

$$
\begin{vmatrix}
0 & -1 \
1 & 1
\end{vmatrix}
= 1
$$

Thus

$$
\det A = 2(1) - 1(1)
$$

$$
= 1
$$

---

# 8. Orientation preservation

A linear transformation **preserves orientation** if

$$
\det A > 0
$$

Since

$$
\det A = 1 > 0
$$

the transformation **preserves the orientation of space**.

---

✅ This will render **perfectly in VS Code Markdown preview**.

---

If you want, I can also give you:

* **Problem 2–10 fully solved in the same Markdown format**
* **HTML/JS code for Problems 6–9** (since the assignment explicitly requires web visualization)
* a **ready folder structure exactly matching your GitHub repo** so you can just paste everything and push.
