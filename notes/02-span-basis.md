# Ch 2: Linear Combinations, Span, and Basis

> **Source:** [3Blue1Brown - Essence of Linear Algebra (Chapter 2)](https://www.youtube.com/watch?v=k7RM-ot2NWY)  
> **Date:** 2026-01-22

## 1. Linear Combinations (선형 결합)

Every vector description is essentially a combination of scaling and adding basis vectors.
* **Definition:** Combining two vectors $\vec{v}$ and $\vec{w}$ using scalars $a$ and $b$:
    $$
    a\vec{v} + b\vec{w}
    $$
* **Why "Linear"?** Because if you fix one scalar and let the other change, the resulting tip of the vector draws a **straight line**.

---

## 2. The Span (생성 공간)

* **Definition:** The set of *all possible* vectors that you can reach with a linear combination of a given pair (or set) of vectors.
* **Geometric Visualization:**
    * If $\vec{v}$ and $\vec{w}$ point in different directions, their span is the **entire 2D plane**.
    * If $\vec{v}$ and $\vec{w}$ line up (collinear), their span is limited to a **single line**.
    * If both are zero, their span is just the **origin (point)**.
* **Key Question:** "What are the set of all possible outputs?" $\rightarrow$ Asking for the **Span**.

---

## 3. Basis (기저)

* **Definition:** The specific set of vectors you choose to represent your coordinate system. The scalars in a vector coordinates (e.g., x, y) are just scaling factors for these basis vectors.
* **Standard Basis:**
    * $\hat{i}$ (i-hat): Unit vector of length 1 pointing right (x-axis).
    * $\hat{j}$ (j-hat): Unit vector of length 1 pointing up (y-axis).
    * Any vector coordinate $(3, 2)$ actually means: $3\hat{i} + 2\hat{j}$.
* **Changing Basis:** We can choose *different* vectors as our basis. The grid lines would change, but the vector itself in space remains the same; only the numbers describing it change.

---

## 4. Linear Independence vs. Dependence

* **Linearly Dependent (선형 종속):**
    * One vector can be expressed as a linear combination of the others.
    * It does **not** add a new dimension to the span. It is "redundant".
    * $\vec{u} = a\vec{v} + b\vec{w}$ (Information is trapped in the existing span).
* **Linearly Independent (선형 독립):**
    * No vector can be made from the others.
    * Every new vector adds a new dimension (e.g., Line $\rightarrow$ Plane $\rightarrow$ 3D Space).
* **Technical Definition of Basis:** A set of linearly independent vectors that span the full space.

---

## 📝 Summary
The span is the "playing field" defined by our vectors. A basis is the minimal set of vectors needed to define that field without redundancy. Understanding this allows us to transform coordinate systems.
