# Ch 6: The Determinant - Practice & Solutions

> **Note:** Click the toggle below each question to reveal the solution.

---

## 🧠 Part 1: Conceptual Understanding

### Q1. Geometric Meaning
What is the most fundamental geometric interpretation of the **Determinant** in linear algebra?

(A) The sum of diagonal elements (Trace).
(B) The scaling factor of the area or volume caused by the linear transformation.
(C) The sum of angles between basis vectors after transformation.
(D) The computational complexity required to perform the transformation.

<details>
<summary><strong>💡 Answer</strong></summary>

<br>

**Answer: (B)**

The determinant measures how much a given region of space is **scaled** (stretched or squished) during the transformation.

</details>

---

### Q2. Negative Determinant
In a 2D plane, what does a **Negative Determinant** imply geometrically?

(A) The orientation of space has been flipped.
(B) The area of the space has decreased.
(C) All coordinates became negative numbers.
(D) The space moved to the imaginary axis.

<details>
<summary><strong>💡 Answer</strong></summary>

<br>

**Answer: (A)**

A negative sign indicates that the orientation is inverted, similar to flipping a sheet of paper. The relative order of basis vectors ($\hat{i}$ to $\hat{j}$) is reversed.

</details>

---

### Q3. Zero Determinant
If the determinant of matrix $A$ is 0 ($\det(A) = 0$), what has happened to the transformed space?

(A) The space is perfectly symmetric around the origin.
(B) No transformation occurred (Identity matrix).
(C) Dimension Collapse: The volume (or area) has become 0.
(D) The space expanded infinitely.

<details>
<summary><strong>💡 Answer</strong></summary>

<br>

**Answer: (C)**

A zero determinant means the space has been squished into a lower dimension (e.g., 3D $\to$ 2D plane or line), resulting in zero volume. In this state, the transformation is **irreversible**.

</details>

---

### Q4. Determinant in 3D
What does the determinant represent in **3D space**?

(A) The volume of the parallelepiped formed by the unit cube after transformation.
(B) The surface area of the transformed space.
(C) The length of the longest diagonal.
(D) The area of the triangle formed by three basis vectors.

<details>
<summary><strong>💡 Answer</strong></summary>

<br>

**Answer: (A)**

It represents the scaling factor of the **Volume**. If the original cube had a volume of 1, the transformed shape (parallelepiped) has a volume of $\det(A)$.

</details>

---

### Q5. Shear Transformation
What is the determinant of the following **Shear** matrix, and why?

<div align="left">
  <img src="https://latex.codecogs.com/svg.image?\begin{bmatrix}1&1\\0&1\end{bmatrix}" />
</div>

(A) 1, because the base and height remain unchanged, preserving the area.
(B) 2, because the width increased.
(C) 0, because the shape is distorted.
(D) -1, because the direction changed.

<details>
<summary><strong>💡 Answer</strong></summary>

<br>

**Answer: (A)**

Even though the shape tilts, the total area (Base $\times$ Height) remains exactly the same. Therefore, the determinant of any shear transformation is **1**.

</details>

---

## 🚀 Part 2: Advanced Application

### Q6. Scaling in 3D
If you multiply every element of a $3 \times 3$ matrix $A$ by 2 (creating matrix $2A$), how does the determinant change?

(A) 2 times ($2$)
(B) 6 times ($3 \times 2$)
(C) 8 times ($2^3$)
(D) Same ($1$)

<details>
<summary><strong>💡 Answer</strong></summary>

<br>

**Answer: (C) 8 times**

In 3D space, scaling $x, y, z$ axes by 2 increases volume by $2 \times 2 \times 2 = 8$.
<div align="left">
  <img src="https://latex.codecogs.com/svg.image?\det(kA)=k^n\det(A)\quad(n=\text{dimension})" />
</div>

</details>

---

### Q7. Determinant of a Product
Which property is true for the determinant of the product of two matrices $A$ and $B$?

(A) <img src="https://latex.codecogs.com/svg.image?\det(AB)=\det(A)+\det(B)" align="center" height="15"/>
(B) <img src="https://latex.codecogs.com/svg.image?\det(AB)=\det(A)\cdot\det(B)" align="center" height="15"/>
(C) <img src="https://latex.codecogs.com/svg.image?\det(AB)=\det(A)" align="center" height="15"/>
(D) <img src="https://latex.codecogs.com/svg.image?\det(AB)=0" align="center" height="15"/>

<details>
<summary><strong>💡 Answer</strong></summary>

<br>

**Answer: (B)**

Applying two transformations sequentially multiplies their scaling factors.
* "Scale by 2" then "Scale by 3" results in "Scale by 6".

</details>

---

### Q8. Determinant of Inverse
What is the relationship between the determinant of an inverse matrix $A^{-1}$ and the original matrix $A$?

(A) <img src="https://latex.codecogs.com/svg.image?\det(A^{-1})=\det(A)" align="center" height="15"/>
(B) <img src="https://latex.codecogs.com/svg.image?\det(A^{-1})=-\det(A)" align="center" height="15"/>
(C) <img src="https://latex.codecogs.com/svg.image?\det(A^{-1})=\frac{1}{\det(A)}" align="center" height="20"/>
(D) <img src="https://latex.codecogs.com/svg.image?\det(A^{-1})=0" align="center" height="15"/>

<details>
<summary><strong>💡 Answer</strong></summary>

<br>

**Answer: (C)**

If transformation $A$ scales space by $k$, the inverse transformation (undoing it) must scale space by $1/k$ to return to the original size.

</details>

---

### Q9. Linear Dependence
If the columns of a matrix are **Linearly Dependent**, what must the determinant be?

(A) 1
(B) 0
(C) Negative
(D) Unknown

<details>
<summary><strong>💡 Answer</strong></summary>

<br>

**Answer: (B) 0**

Linear dependence means redundancy. The vectors do not span the full dimension (e.g., 3 vectors lie on a 2D plane), causing the volume to collapse to **0**.

</details>

---

### Q10. Area Calculation
To find the area of a parallelogram defined by vectors $\vec{v}$ and $\vec{w}$, we calculate the determinant. If the result is negative, what is the area?

(A) The square of the determinant $\det(A)^2$
(B) The determinant as is
(C) The absolute value $|\det(A)|$
(D) 0

<details>
<summary><strong>💡 Answer</strong></summary>

<br>

**Answer: (C)**

Geometric area must always be positive. The negative sign only indicates orientation (flipping), so we take the **absolute value**.

</details>
