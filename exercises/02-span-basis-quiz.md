# Ch 2: Span and Basis - Practice & Solutions

> **Note:** Click the toggle below each question to reveal the solution.

---

### Q1. Definition of Basis Vectors
What do we call $\hat{i}$ and $\hat{j}$ when they serve as the fundamental building blocks for all vectors in a coordinate system?

(A) Basis Vectors
(B) Scalar Vectors
(C) Dependent Vectors
(D) Virtual Vectors

<details>
<summary><strong>💡 Answer</strong></summary>

<br>

**Answer: (A) Basis Vectors**

They form the "Basis" because any vector can be represented as a unique sum of scaled $\hat{i}$ and $\hat{j}$.

</details>

---

### Q2. Vector Decomposition
Which is the correct expression of the vector below using basis vectors $\hat{i}$ and $\hat{j}$?

<div align="left">
  <img src="https://latex.codecogs.com/svg.image?\vec{v}=\begin{bmatrix}5\\-3\end{bmatrix}" />
</div>

<br>

(A) <img src="https://latex.codecogs.com/svg.image?5\hat{i}-3\hat{j}" align="center"/>
<br>
(B) <img src="https://latex.codecogs.com/svg.image?5\hat{i}+3\hat{j}" align="center"/>
<br>
(C) <img src="https://latex.codecogs.com/svg.image?-3\hat{i}+5\hat{j}" align="center"/>
<br>
(D) <img src="https://latex.codecogs.com/svg.image?2\hat{i}\hat{j}" align="center"/>

<details>
<summary><strong>💡 Answer</strong></summary>

<br>

**Answer: (A)** <img src="https://latex.codecogs.com/svg.image?5\hat{i}-3\hat{j}" align="center"/>

The top component scales $\hat{i}$ (x-axis), and the bottom component scales $\hat{j}$ (y-axis).

</details>

---

### Q3. Linear Combination
What is the operation of scaling two vectors and adding them together called?

<div align="left">
  <img src="https://latex.codecogs.com/svg.image?a\vec{v}+b\vec{w}" />
</div>

(A) Linear Combination
(B) Linear Decomposition
(C) Scalar Projection
(D) Vector Determinant

<details>
<summary><strong>💡 Answer</strong></summary>

<br>

**Answer: (A) Linear Combination**

This is the most fundamental operation in linear algebra.

</details>

---

### Q4. Definition of Span
What do we call the set of **all possible** linear combinations of two vectors $\vec{v}$ and $\vec{w}$?

(A) Span
(B) Vector Space
(C) Dimension
(D) Matrix

<details>
<summary><strong>💡 Answer</strong></summary>

<br>

**Answer: (A) Span**

The Span represents everywhere you can possibly reach using only those two vectors.

</details>

---

### Q5. Span of Collinear Vectors
In a 2D plane, if two vectors lie on the same line (are collinear), what is their Span?

(A) A single line passing through the origin
(B) The entire 2D plane
(C) Just the origin point
(D) A single quadrant

<details>
<summary><strong>💡 Answer</strong></summary>

<br>

**Answer: (A) A single line passing through the origin**

Since the second vector doesn't point in a new direction, you are stuck moving back and forth on one line. (Linearly Dependent).

</details>

---

### Q6. Span in 3D Space
What geometric shape does the Span of two distinct vectors generally form in a 3D space?

(A) A flat plane passing through the origin
(B) The entire 3D space
(C) A Sphere
(D) A single point

<details>
<summary><strong>💡 Answer</strong></summary>

<br>

**Answer: (A) A flat plane passing through the origin**

Two vectors create a 2D sheet (plane) cutting through the 3D space. You need a 3rd vector to fill the 3D space.

</details>

---

### Q7. Linear Dependence
If adding a new vector to an existing set **does not** increase the Span at all, what is this state called?

(A) Linearly Dependent
(B) Linearly Independent
(C) Orthogonal
(D) Normalized

<details>
<summary><strong>💡 Answer</strong></summary>

<br>

**Answer: (A) Linearly Dependent**

The new vector is redundant because it can already be made by combining the previous vectors.

</details>

---

### Q8. Basis Requirements
What do we call a set of vectors that "Spans" a specific space and is also "Linearly Independent"?

(A) Basis
(B) Normal
(C) Solution Set
(D) Subspace

<details>
<summary><strong>💡 Answer</strong></summary>

<br>

**Answer: (A) Basis**

A Basis is the most efficient way to describe a space (Spanning everything without any redundancy).

</details>

---

### Q9. Dimensions and Basis
What is the minimum number of vectors required to form a basis for 3D space ($\mathbb{R}^3$)?

(A) 3
(B) 2
(C) 4
(D) Infinite

<details>
<summary><strong>💡 Answer</strong></summary>

<br>

**Answer: (A) 3**

You need one for width, one for height, and one for depth. (e.g., x, y, z axes).

</details>

---

### Q10. Relationship between Vectors
If $\vec{u}$ and $\vec{v}$ are linearly independent, but $\vec{w} = 2\vec{u} + 3\vec{v}$, what is the relationship of the set $\{ \vec{u}, \vec{v}, \vec{w} \}$?

(A) Linearly Dependent
(B) Linearly Independent
(C) Orthogonal
(D) Basis of the space

<details>
<summary><strong>💡 Answer</strong></summary>

<br>

**Answer: (A) Linearly Dependent**

Since $\vec{w}$ is made from $\vec{u}$ and $\vec{v}$, it doesn't add anything new. It falls inside the span of the first two.

</details>
