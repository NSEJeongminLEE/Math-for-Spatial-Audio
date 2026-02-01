# Ch 1: The Essence of Vectors

> **Source:** [3Blue1Brown - Essence of Linear Algebra (Chapter 1)](https://www.youtube.com/watch?v=fNk_zzaMoSs)  
> **Date:** 2026-01-21

## 1. Three Perspectives on Vectors

Vectors are viewed differently depending on the field, but Linear Algebra bridges these views.

1.  **Physics Perspective:**
    * A vector is an **arrow** pointing in space.
    * Defined by **Length** (Magnitude) and **Direction**.
    * It can be moved anywhere, but as long as length and direction are maintained, it's the same vector.
2.  **CS Perspective:**
    * A vector is an **ordered list of numbers**.
    * Example: Modeling a house with `[area, price]` $\rightarrow \begin{bmatrix} 2500 \\ 500000 \end{bmatrix}$.
    * Order matters.
3.  **Mathematician's Perspective:**
    * A generalized abstract object that follows the rules of addition and scaling.
    * In Linear Algebra, we typically view vectors as arrows rooted at the **Origin $(0,0)$**.



---

## 2. Coordinate System & Basis

* **Coordinates $(x, y)$:** Instructions on how to get from the origin to the vector's tip.
    * $x$: Distance to move along the x-axis.
    * $y$: Distance to move along the y-axis.
* The numbers in the list depend on the coordinate system (Basis) we choose.

---

## 3. Fundamental Operations

Linear Algebra revolves around two distinct operations: **Addition** and **Multiplication by a Scalar**.

### A. Vector Addition
* **Geometric:** Tip-to-Tail method. Move vector $\vec{w}$ so its tail sits at the tip of $\vec{v}$. The result is the arrow from the origin to $\vec{w}$'s tip.
* **Numeric:** Add the corresponding components.
    $$
    \begin{bmatrix} x_1 \\ y_1 \end{bmatrix} + \begin{bmatrix} x_2 \\ y_2 \end{bmatrix} = \begin{bmatrix} x_1 + x_2 \\ y_1 + y_2 \end{bmatrix}
    $$



### B. Scalar Multiplication (Scaling)
* **Scalar:** A plain number used to scale a vector.
* **Geometric:** Stretching, squishing, or reversing (if negative) the vector's length without changing its line of action.
* **Numeric:** Multiply every component by the scalar.
    $$
    2 \cdot \begin{bmatrix} 3 \\ 1 \end{bmatrix} = \begin{bmatrix} 6 \\ 2 \end{bmatrix}
    $$



---

## 🧠 Insight for Spatial Audio

* **Digital Audio as Vectors:**
    * A discrete audio signal is essentially a massive ordered list of numbers (samples).
    * Therefore, **an audio signal is a vector** in a very high-dimensional space.
* **Mixing as Addition:**
    * Mixing two audio tracks is mathematically identical to **Vector Addition**.
    * $\vec{Track1} + \vec{Track2} = \vec{Mix}$
* **Gain as Scaling:**
    * Adjusting the volume (Gain) is mathematically identical to **Scalar Multiplication**.
    * $0.5 \cdot \vec{Signal}$ (Halving the amplitude).

---

## 📝 Summary
Linear Algebra provides the tools to navigate between the "visual" arrow intuition and the "computational" list-of-numbers reality. For data-heavy fields like Audio Engineering, we manipulate lists of numbers (CS view), but visualizing them as geometric objects (Physics view) provides the intuition for complex operations.
