# Ch 5: 3D Linear Transformations - Practice & Solutions

> **Note:** Click the toggle below each question to reveal the solution.

---

### Q1. Describing 3D Transformations
What information is strictly required to perfectly describe a linear transformation in 3D space?

(A) The length of the x, y, z axes before transformation.
(B) The new coordinates of where the three basis vectors $\hat{i}, \hat{j}, \hat{k}$ land.
(C) The new location of the origin.
(D) The coordinates of every single point in space.

<details>
<summary><strong>💡 Answer</strong></summary>

<br>

**Answer: (B)**

The core principle of linear transformations is that the destination of the basis vectors determines the transformation of the entire space.

</details>

---

### Q2. Columns of a 3x3 Matrix
In a $3 \times 3$ matrix, what is the geometric significance of the **third column**?

<div align="left">
  <img src="https://latex.codecogs.com/svg.image?A=\begin{bmatrix}c_1\\c_2\\c_3\end{bmatrix}" />
</div>

(A) The transformed coordinates of the basis vector $\hat{i}$.
(B) The transformed coordinates of the basis vector $\hat{k}$ (z-axis unit vector).
(C) The transformed coordinates of the basis vector $\hat{j}$.
(D) The diagonal direction vector of the space.

<details>
<summary><strong>💡 Answer</strong></summary>

<br>

**Answer: (B)**

* Col 1: Destination of $\hat{i}$
* Col 2: Destination of $\hat{j}$
* Col 3: Destination of $\hat{k}$

</details>

---

### Q3. Rotation around an Axis
When rotating 3D space 90 degrees around the **x-axis**, what happens to the basis vector $\hat{i}$?

(A) It stays at <img src="https://latex.codecogs.com/svg.image?(1,0,0)" align="center" height="15"/> without changing.
(B) It moves to the origin <img src="https://latex.codecogs.com/svg.image?(0,0,0)" align="center" height="15"/>.
(C) It moves to the y-axis <img src="https://latex.codecogs.com/svg.image?(0,1,0)" align="center" height="15"/>.
(D) It moves to the z-axis <img src="https://latex.codecogs.com/svg.image?(0,0,1)" align="center" height="15"/>.

<details>
<summary><strong>💡 Answer</strong></summary>

<br>

**Answer: (A)**

Any vector lying **on the axis of rotation** is unaffected by the rotation. Since we rotate around the x-axis, $\hat{i}$ (which is the x-axis) stays put.

</details>

---

### Q4. Linearity Violation
Which of the following operations is **NOT** a linear transformation?

(A) Translating the entire space so the origin moves to <img src="https://latex.codecogs.com/svg.image?(1,2,3)" align="center" height="15"/>.
(B) Flattening all z-components to 0 (Projection).
(C) Rotating the space 45 degrees around the y-axis.
(D) Stretching the space diagonally (Scaling).

<details>
<summary><strong>💡 Answer</strong></summary>

<br>

**Answer: (A)**

A fundamental rule of linear transformations is **"The Origin must remain fixed."** Translation moves the origin, so it is an *Affine Transformation*, not Linear.

</details>

---

### Q5. 3D Rotation Order
If $A$ is a 90-degree rotation around the x-axis, and $B$ is a 90-degree rotation around the y-axis, is the result of $AB$ and $BA$ the same?

(A) Yes, $AB = BA$.
(B) Same direction, different length.
(C) No, $AB \neq BA$.
(D) They both return to the origin.

<details>
<summary><strong>💡 Answer</strong></summary>

<br>

**Answer: (C) Different ($AB \neq BA$)**

In 3D space, changing the order of rotations results in a completely different final orientation. (Think of rotating a Rubik's cube).

</details>

---

### Q6. Uniform Scaling Matrix
How does the following matrix transform 3D space?

<div align="left">
  <img src="https://latex.codecogs.com/svg.image?A=\begin{bmatrix}2&0&0\\0&2&0\\0&0&2\end{bmatrix}" />
</div>

(A) Stretches only the x-axis by 2.
(B) Projects space onto $x=y=z$.
(C) Rotates the space by 2 radians.
(D) Uniform Scaling: Expands everything by 2 in all directions.

<details>
<summary><strong>💡 Answer</strong></summary>

<br>

**Answer: (D)**

Since the diagonal elements are all 2 and off-diagonals are 0, it scales x, y, and z axes equally.

</details>

---

### Q7. Dimensional Collapse
If, after a 3D transformation, all three basis vectors $\hat{i}, \hat{j}, \hat{k}$ land on the **same single plane**, what happens to the 3D space?

(A) Expands to 4D space.
(B) Becomes a single line.
(C) Maintains 3D volume.
(D) Collapses into a flat 2D plane.

<details>
<summary><strong>💡 Answer</strong></summary>

<br>

**Answer: (D)**

If the three pillars holding up the space fall onto a flat surface, every point inside that space is trapped on that surface. The volume becomes zero.

</details>

---

### Q8. [Application] 3D Shear
Imagine a "Shear" transformation where the x-coordinate is pushed in the x-direction proportional to its **z-value** (z stays fixed). Which basis vector changes its orientation?

(A) $\hat{k}$ (z-axis unit vector)
(B) $\hat{i}$ (x-axis unit vector)
(C) All basis vectors
(D) $\hat{j}$ (y-axis unit vector)

<details>
<summary><strong>💡 Answer</strong></summary>

<br>

**Answer: (A) $\hat{k}$**

* $\hat{i}$ (at z=0) stays.
* $\hat{j}$ (at z=0) stays.
* $\hat{k}$ (at z=1) gets pushed sideways because it has a non-zero z-value. Thus, the vertical $\hat{k}$ tilts.

</details>

---

### Q9. Axis Swapping Matrix
What is the geometric effect of the following matrix?

<div align="left">
  <img src="https://latex.codecogs.com/svg.image?\begin{bmatrix}0&0&1\\0&1&0\\1&0&0\end{bmatrix}" />
</div>

(A) Identity Matrix (No change).
(B) Projecting space onto a plane.
(C) Rotation 90 degrees around y-axis.
(D) Swapping the x-axis and z-axis.

<details>
<summary><strong>💡 Answer</strong></summary>

<br>

**Answer: (D)**

* Column 1 (New $\hat{i}$) is $(0,0,1)$ $\rightarrow$ x-axis became z-axis.
* Column 3 (New $\hat{k}$) is $(1,0,0)$ $\rightarrow$ z-axis became x-axis.

</details>

---

### Q10. Interpretation of Matrix-Vector Product
What is the most accurate geometric interpretation of multiplying a $3 \times 3$ matrix $A$ by a vector $\vec{v}$?

(A) Sending the vector to 9D space.
(B) Stretching the vector length by the matrix size.
(C) Simply adding rows to the vector.
(D) A linear combination of the transformed basis vectors (columns) scaled by $\vec{v}$'s components $(x,y,z)$.

<details>
<summary><strong>💡 Answer</strong></summary>

<br>

**Answer: (D)**

<div align="left">
  <img src="https://latex.codecogs.com/svg.image?A%5Cvec%7Bv%7D%3Dx%28%5Ctext%7BNew%20%7D%5Chat%7Bi%7D%29%2By%28%5Ctext%7BNew%20%7D%5Chat%7Bj%7D%29%2Bz%28%5Ctext%7BNew%20%7D%5Chat%7Bk%7D%29" alt="Linear Combination of Basis Vectors"/>
</div>

It means constructing the vector using the new coordinate system defined by the matrix.

</details>
