# Ch 3: Linear Transformations - Practice & Solutions

> **Note:** Click the toggle below each question to reveal the solution.

---

### Q1. Geometric Conditions for Linearity
Which two geometric conditions must a transformation satisfy to be considered **'Linear'**?

(A) Only vector addition needs to be defined.
(B) Lengths of vectors must be preserved.
(C) Grid lines must become curves.
(D) The origin must remain fixed, and grid lines must remain parallel and evenly spaced.

<details>
<summary><strong>💡 Answer</strong></summary>

<br>

**Answer: (D)**

Linearity preserves the structure of the coordinate system by keeping the **origin at (0,0)** and ensuring grid lines remain **straight, parallel, and evenly spaced**.

</details>

---

### Q2. Geometric Significance of Matrix Columns
In a matrix $A$, what is the geometric significance of the **first column**?

<div align="left">
  <img src="https://latex.codecogs.com/svg.image?A=\begin{bmatrix}a&c\\b&d\end{bmatrix},\quad\text{First Column}=\begin{bmatrix}a\\b\end{bmatrix}" />
</div>

(A) It represents the change in area.
(B) It indicates the new position of the origin.
(C) It represents where $\hat{j}$ lands.
(D) It represents the coordinates where the basis vector $\hat{i}$ lands after the transformation.

<details>
<summary><strong>💡 Answer</strong></summary>

<br>

**Answer: (D)**

A matrix is essentially a map where:
* **Column 1:** Records the landing spot of $\hat{i}$ (x-axis basis).
* **Column 2:** Records the landing spot of $\hat{j}$ (y-axis basis).

</details>

---

### Q3. Reflection Matrix
Consider a reflection across the x-axis.
* $\hat{i}$ stays at <img src="https://latex.codecogs.com/svg.image?\begin{bmatrix}1\\0\end{bmatrix}" align="center" height="25"/>
* $\hat{j}$ moves to <img src="https://latex.codecogs.com/svg.image?\begin{bmatrix}0\\-1\end{bmatrix}" align="center" height="25"/>

What is the matrix for this transformation?

(A) <img src="https://latex.codecogs.com/svg.image?\begin{bmatrix}1&0\\0&-1\end{bmatrix}" align="center" height="25"/>
(B) <img src="https://latex.codecogs.com/svg.image?\begin{bmatrix}0&1\\-1&0\end{bmatrix}" align="center" height="25"/>
(C) <img src="https://latex.codecogs.com/svg.image?\begin{bmatrix}-1&0\\0&1\end{bmatrix}" align="center" height="25"/>
(D) <img src="https://latex.codecogs.com/svg.image?\begin{bmatrix}0&0\\0&0\end{bmatrix}" align="center" height="25"/>

<details>
<summary><strong>💡 Answer</strong></summary>

<br>

**Answer: (A)** <img src="https://latex.codecogs.com/svg.image?\begin{bmatrix}1&0\\0&-1\end{bmatrix}" align="center" height="25"/>

The first column is the destination of $\hat{i}$, and the second column is the destination of $\hat{j}$.

</details>

---

### Q4. Matrix-Vector Multiplication Interpretation
How can the following matrix-vector multiplication be interpreted in terms of basis vectors?

<div align="left">
  <img src="https://latex.codecogs.com/svg.image?\begin{bmatrix}1&2\\3&4\end{bmatrix}\begin{bmatrix}5\\6\end{bmatrix}" />
</div>

(A) <img src="https://latex.codecogs.com/svg.image?\begin{bmatrix}1\cdot5\\4\cdot6\end{bmatrix}" align="center" height="25"/>
(B) <img src="https://latex.codecogs.com/svg.image?5\cdot\begin{bmatrix}1\\2\end{bmatrix}+6\cdot\begin{bmatrix}3\\4\end{bmatrix}" align="center" height="25"/>
(C) <img src="https://latex.codecogs.com/svg.image?\begin{bmatrix}5\\6\end{bmatrix}\cdot(1+2+3+4)" align="center" height="25"/>
(D) <img src="https://latex.codecogs.com/svg.image?5\cdot\begin{bmatrix}1\\3\end{bmatrix}+6\cdot\begin{bmatrix}2\\4\end{bmatrix}" align="center" height="25"/>

<details>
<summary><strong>💡 Answer</strong></summary>

<br>

**Answer: (D)**

The result is a **linear combination** of the transformed basis vectors (the columns), scaled by the input vector's components.
* 5 times the new $\hat{i}$ + 6 times the new $\hat{j}$.

</details>

---

### Q5. Non-Linear Transformation
Which of the following is an example of a **non-linear** transformation?

(A) Applying a 'Shear' transformation along the x-axis.
(B) Rotating the entire space 45 degrees.
(C) Scaling every vector by a factor of 2.
(D) Mapping all coordinates $(x, y)$ to $(x^2, y)$.

<details>
<summary><strong>💡 Answer</strong></summary>

<br>

**Answer: (D)**

Mapping to <img src="https://latex.codecogs.com/svg.image?(x^2,y)" align="center"/> introduces squared terms, which cause grid lines to **curve**. Curving violates the definition of linearity.

</details>

---

### Q6. [Advanced] Rotation Matrix
What is the matrix for a 45-degree **counter-clockwise rotation**?
(Given $\cos 45^\circ = \sin 45^\circ = \frac{\sqrt{2}}{2}$)

(A) <img src="https://latex.codecogs.com/svg.image?\begin{bmatrix}1&-1\\1&1\end{bmatrix}" align="center" height="25"/>
(B) <img src="https://latex.codecogs.com/svg.image?\begin{bmatrix}0&-1\\1&0\end{bmatrix}" align="center" height="25"/>
(C) <img src="https://latex.codecogs.com/svg.image?\begin{bmatrix}\frac{\sqrt{2}}{2}&\frac{\sqrt{2}}{2}\\-\frac{\sqrt{2}}{2}&\frac{\sqrt{2}}{2}\end{bmatrix}" align="center" height="35"/>
(D) <img src="https://latex.codecogs.com/svg.image?\begin{bmatrix}\frac{\sqrt{2}}{2}&-\frac{\sqrt{2}}{2}\\\frac{\sqrt{2}}{2}&\frac{\sqrt{2}}{2}\end{bmatrix}" align="center" height="35"/>

<details>
<summary><strong>💡 Answer</strong></summary>

<br>

**Answer: (D)**

* $\hat{i}$ lands at $(\cos 45, \sin 45)$.
* $\hat{j}$ lands at $(-\sin 45, \cos 45)$.

</details>

---

### Q7. [Advanced] Linear Dependence & Dimension
If the two column vectors of a 2x2 matrix are **linearly dependent**, what happens to the 2D plane under this transformation?

(A) The grid becomes a series of perfect rectangles.
(B) The entire plane collapses into a single line or a point.
(C) Nothing happens; the plane remains unchanged.
(D) The plane expands into a 3D volume.

<details>
<summary><strong>💡 Answer</strong></summary>

<br>

**Answer: (B)**

Since the basis vectors land on the same line (redundant direction), the **Span** of the output is reduced (squished) from 2D to 1D (line) or 0D (point).

</details>

---

### Q8. Identity Matrix
What is the name of the matrix $I$ which leaves vectors unchanged?

<div align="left">
  <img src="https://latex.codecogs.com/svg.image?I=\begin{bmatrix}1&0\\0&1\end{bmatrix}" />
</div>

(A) Zero Matrix
(B) Identity Matrix
(C) Transpose Matrix
(D) Inverse Matrix

<details>
<summary><strong>💡 Answer</strong></summary>

<br>

**Answer: (B) Identity Matrix**

It is the "do-nothing" transformation that keeps every vector in its original place.

</details>

---

### Q9. [Spatial Audio App] Scaling
To double the amplitude of a sound source in 3D space using scaling, what should the values of the **diagonal elements** ($a_{11}, a_{22}, a_{33}$) be?

(A) 0
(B) 0.5
(C) 2
(D) 1

<details>
<summary><strong>💡 Answer</strong></summary>

<br>

**Answer: (C) 2**

Diagonal scaling by 2 stretches the position vector of the sound source by a factor of 2 in all directions (x, y, z).

</details>

---

### Q10. [Advanced] Shear Transformation
What kind of geometric transformation does the matrix $A$ represent?

<div align="left">
  <img src="https://latex.codecogs.com/svg.image?A=\begin{bmatrix}1&1\\0&1\end{bmatrix}" />
</div>

(A) Shear: The x-axis remains fixed, and the top slides right.
(B) Scaling: Expands diagonally.
(C) Rotation: Turns counter-clockwise.
(D) Projection: Flattens onto the y-axis.

<details>
<summary><strong>💡 Answer</strong></summary>

<br>

**Answer: (A) Shear**

* $\hat{i}$ stays at $(1, 0)$ (Fixed base).
* $\hat{j}$ moves to $(1, 1)$ (Pushed right).
This causes a slanted distortion known as a **Shear**.

</details>

---

## 📝 Review Note: Matrix Types & Transformations

> **Context:** Deep dive after missing Q8 (Identity Matrix).

<details>
<summary><strong>📚 Core Concepts (Click to Expand)</strong></summary>

<br>

Matrices are not just grids of numbers; they are **"commands"** acting on space. Understanding the "intent" of each matrix is crucial.

### 1. Identity Matrix ($I$)
* **Definition:** A square matrix with 1s on the main diagonal and 0s elsewhere.
* **Intuition:** Equivalent to **'1'** in arithmetic. Multiplying by $I$ changes nothing.
* **Geometry:** **"State Preservation"**. The basis vectors $\hat{i}, \hat{j}$ remain exactly where they are.
    <div align="left">
      <img src="https://latex.codecogs.com/svg.image?AI=A,\quad\begin{bmatrix}1&0\\0&1\end{bmatrix}" />
    </div>

### 2. Zero Matrix ($O$)
* **Definition:** A matrix where every entry is 0.
* **Intuition:** Equivalent to **'0'** in arithmetic.
* **Geometry:** **"Dimensional Collapse"**. It crushes every vector into the origin $(0,0)$. All spatial information is lost.
    <div align="left">
      <img src="https://latex.codecogs.com/svg.image?AO=O,\quad\begin{bmatrix}0&0\\0&0\end{bmatrix}" />
    </div>

### 3. Transpose Matrix ($A^T$)
* **Definition:** Flipping a matrix over its main diagonal ($a_{ij} \to a_{ji}$).
* **Intuition:** **"Mirroring"** the grid structure.

### 4. Inverse Matrix ($A^{-1}$)
* **Definition:** A matrix that yields the Identity Matrix when multiplied by $A$.
* **Intuition:** **"Ctrl + Z" (Undo)**. It restores the transformed space back to its original state.
    <div align="left">
      <img src="https://latex.codecogs.com/svg.image?AA^{-1}=I" />
    </div>
* **Reality Check:** If the space was squished into a lower dimension (Determinant = 0), you cannot undo it. (No inverse exists).

### 5. Shear Transformation
* **Definition:** Fixing one axis and pushing the other.
* **Intuition:** Sliding the side of a deck of cards. The area (Determinant) remains unchanged.

</details>

---

### 🎧 Spatial Audio Insight (Reality Check)

> **"The Efficiency of Rotation Matrices"**

In Spatial Audio, the **Rotation Matrix ($R$)** used for Head Tracking has a special property called **Orthogonality**.

<div align="center">
  <img src="https://latex.codecogs.com/svg.image?R^{-1}=R^T" />
</div>

This means if you want to **undo a rotation** (e.g., converting world coordinates back to local head coordinates), you **do not** need to calculate a complex inverse. **You simply Transpose the matrix.** This mathematical shortcut is the secret to efficient real-time audio rendering.
