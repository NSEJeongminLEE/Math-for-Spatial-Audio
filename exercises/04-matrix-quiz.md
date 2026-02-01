# Ch 4: Matrix Multiplication - Practice & Solutions

> **Note:** Click the toggle below each question to reveal the solution.

---

### Q1. Geometric Interpretation of Multiplication
What is the most accurate geometric interpretation of matrix multiplication $AB$?

(A) Multiplying corresponding elements individually.
(B) The 'Composition' of applying two linear transformations sequentially.
(C) Dot product to find the angle between two vectors.
(D) Scaling the area of the space by a factor of 2.

<details>
<summary><strong>💡 Answer</strong></summary>

<br>

**Answer: (B)**

Matrix multiplication represents applying transformation $B$ first, and then applying transformation $A$ to the result. It combines two movements into one.

</details>

---

### Q2. Order of Operations
In the calculation <img src="https://latex.codecogs.com/svg.image?A(B\vec{v})" align="center" height="20"/>, which transformation happens **first** geometrically?

(A) Transformation $B$
(B) $A$ and $B$ happen simultaneously
(C) Impossible to know
(D) Transformation $A$

<details>
<summary><strong>💡 Answer</strong></summary>

<br>

**Answer: (A) Transformation $B$**

Functions and linear transformations are read from **Right to Left**. $\vec{v}$ gets hit by $B$ first, and the result is then hit by $A$.

</details>

---

### Q3. Columns of the Product Matrix
In the product <img src="https://latex.codecogs.com/svg.image?M=AB" align="center" height="15"/>, what is the geometric meaning of the **first column** of $M$?

(A) The location where basis vector $\hat{j}$ lands after $A$.
(B) The total area increased by the two transformations.
(C) The original standard basis vector $\hat{i}$ itself.
(D) The final location where basis vector $\hat{i}$ lands after passing through $B$ and then $A$.

<details>
<summary><strong>💡 Answer</strong></summary>

<br>

**Answer: (D)**

The columns of any matrix record the destination of basis vectors. Since $M$ is the combined effect of $B$ then $A$, the first column tracks $\hat{i}$ through that entire journey.

</details>

---

### Q4. Non-Commutativity
Generally, why is <img src="https://latex.codecogs.com/svg.image?AB\neq&space;BA" align="center" height="15"/> in matrix multiplication?

(A) Because changing the order of transformations changes the final destination of the basis vectors.
(B) Because matrix elements might not be integers.
(C) $AB=BA$ is always true, exceptions are rare.
(D) Because linear transformations are only defined in one direction.

<details>
<summary><strong>💡 Answer</strong></summary>

<br>

**Answer: (A)**

Example: "Rotate then Shear" yields a different geometric shape than "Shear then Rotate". Order matters in geometry.

</details>

---

### Q5. [Application] Rotation & Uniform Scaling
If $A$ is a 90-degree counter-clockwise rotation and $B$ scales all vectors by 2 (Uniform Scaling), what is the relationship between $AB$ and $BA$?

(A) <img src="https://latex.codecogs.com/svg.image?AB=-BA" align="center" height="15"/>
(B) <img src="https://latex.codecogs.com/svg.image?AB=BA" align="center" height="15"/>
(C) <img src="https://latex.codecogs.com/svg.image?AB\neq&space;BA" align="center" height="15"/>
(D) One becomes a Zero Matrix.

<details>
<summary><strong>💡 Answer</strong></summary>

<br>

**Answer: (B)** <img src="https://latex.codecogs.com/svg.image?AB=BA" align="center" height="15"/>

**Uniform** scaling stretches space evenly in all directions. It doesn't matter if you rotate first then stretch, or stretch first then rotate. The result is identical.

</details>

---

### Q6. Associativity
What is the geometric reason why Associativity <img src="https://latex.codecogs.com/svg.image?(AB)C=A(BC)" align="center" height="15"/> holds true?

(A) Only holds for square matrices.
(B) Because basis vectors always return to the origin.
(C) Because regardless of how you group them, the sequence of transformations ($C \to B \to A$) remains the same.
(D) Because matrix multiplication satisfies the distributive property with addition.

<details>
<summary><strong>💡 Answer</strong></summary>

<br>

**Answer: (C)**

Parentheses only indicate calculation convenience. The physical reality is that vector $\vec{v}$ travels through $C$, then $B$, then $A$ in that exact order.

</details>

---

### Q7. [Advanced] Inverse Relationship
If multiplying matrices $A$ and $B$ yields the Identity Matrix (<img src="https://latex.codecogs.com/svg.image?AB=I" align="center" height="15"/>), what is the relationship between $A$ and $B$?

(A) Projection transformation lowering dimensions.
(B) They are "Inverse" to each other; one undoes the effect of the other.
(C) They push space in perpendicular directions.
(D) They are both Identity transformations.

<details>
<summary><strong>💡 Answer</strong></summary>

<br>

**Answer: (B)**

Returning to the Identity Matrix ($I$) means the space has been restored to its original state (basis vectors are back at $[1,0]$ and $[0,1]$). Thus, $B$ undoes $A$ (or vice versa).

</details>

---

### Q8. [Application] Powers of Matrix
Let $A$ be a 90-degree rotation matrix <img src="https://latex.codecogs.com/svg.image?\begin{bmatrix}0&-1\\1&0\end{bmatrix}" align="center" height="25"/>. What is the geometric result of <img src="https://latex.codecogs.com/svg.image?A^2" align="center" height="18"/> (applying $A$ twice)?

(A) Shear 45 degrees.
(B) 360-degree rotation (back to start).
(C) Space collapses to origin.
(D) 180-degree rotation (<img src="https://latex.codecogs.com/svg.image?\hat{i}\to-\hat{i},\hat{j}\to-\hat{j}" align="center" height="18"/>).

<details>
<summary><strong>💡 Answer</strong></summary>

<br>

**Answer: (D)**

Rotating 90 degrees twice equals a total of $90 + 90 = 180$ degrees.
<img src="https://latex.codecogs.com/svg.image?\begin{bmatrix}0&-1\\1&0\end{bmatrix}\begin{bmatrix}0&-1\\1&0\end{bmatrix}=\begin{bmatrix}-1&0\\0&-1\end{bmatrix}" align="center" height="25"/>

</details>

---

### Q9. [Spatial Audio App] Commutativity Check
You have a matrix $R$ (90-degree rotation) and matrix $S$ (Scale distance by 2x). An engineer calculated $RS$ instead of $SR$. What happens to the result?

(A) Rotation works, but distance doesn't change.
(B) The result is identical.
(C) The audio signal is destroyed.
(D) Distance doubles, but rotation is reversed.

<details>
<summary><strong>💡 Answer</strong></summary>

<br>

**Answer: (B) The result is identical.**

Since $S$ is a **Uniform Scaling** (stretching x and y equally), it commutes with rotation.
> **Note:** If $S$ were a non-uniform scale (e.g., stretch only x-axis), the order would matter significantly!

</details>

---

### Q10. [Advanced] The "Row dot Column" Method
What is the fundamental reason we use the "Row $\cdot$ Column" method to calculate elements <img src="https://latex.codecogs.com/svg.image?c_{ij}" align="center" height="15"/> of a matrix product?

(A) Computers process multiplication faster than addition.
(B) It is a required step to find the area.
(C) It efficiently summarizes the linear combination where rows of the first matrix meet columns of the second to determine final coordinates.
(D) Because Newton defined it that way.

<details>
<summary><strong>💡 Answer</strong></summary>

<br>

**Answer: (C)**

The numerical method is a shortcut. It calculates the component-wise contribution of the transformed basis vectors to the final position.

</details>
