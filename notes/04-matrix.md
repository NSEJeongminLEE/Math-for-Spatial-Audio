# Ch 4: Matrix Multiplication as Composition

> **Source:** [3Blue1Brown - Essence of Linear Algebra (Chapter 4)](https://www.youtube.com/watch?v=XkY2DOUCWMU)  
> **Date:** 2026-01-25

## 1. Composition of Transformations (합성 변환)

We often want to apply one transformation, and then another. For example, "Rotate first, then Shear."
In mathematics, applying two functions sequentially is called **Composition**.

* **Notation:** If we apply transformation $M_1$ first, and then $M_2$, we write it from **Right to Left**.

<div align="center">
  <img src="https://latex.codecogs.com/svg.image?M_2M_1\vec{v}" alt="Composition Notation" />
</div>

<br>

* **Reason:** This comes from function notation $g(f(x))$, where $f$ happens first inside, and $g$ wraps around it.

---

## 2. Computing Matrix Multiplication

How do we find the single matrix that represents the combined effect of two transformations?
We track where $\hat{i}$ and $\hat{j}$ land after **both** transformations.

<div align="center">
  <img src="https://latex.codecogs.com/svg.image?\begin{bmatrix}a&b\\c&d\end{bmatrix}\begin{bmatrix}e&f\\g&h\end{bmatrix}=\begin{bmatrix}ae+bg&af+bh\\ce+dg&cf+dh\end{bmatrix}" alt="Matrix Multiplication Formula" />
</div>

<br>

* **Left Column:** Where $\hat{i}$ lands after passing through $M_1$ then $M_2$.
* **Right Column:** Where $\hat{j}$ lands after passing through $M_1$ then $M_2$.

It is **NOT** just multiplying number by number. It is the geometric composition of space.

---

## 3. Non-Commutativity (순서의 중요성)

Order matters significantly in Matrix Multiplication.

<div align="center">
  <img src="https://latex.codecogs.com/svg.image?M_1M_2\neq&space;M_2M_1" alt="Non-commutativity" />
</div>

<br>

* **Geometric Proof:**
    * Case A: "Shear Right" then "Rotate 90°"
    * Case B: "Rotate 90°" then "Shear Right"
    * The final grid looks completely different.
* **Associativity:** However, grouping does not matter. <img src="https://latex.codecogs.com/svg.image?(AB)C=A(BC)" align="middle" height="20"/> is true.

---

## 📝 Summary
Matrix multiplication is the act of applying multiple transformations in sequence. Always remember to read the transformations from **Right to Left**, just like reading nested functions like $f(g(x))$.
