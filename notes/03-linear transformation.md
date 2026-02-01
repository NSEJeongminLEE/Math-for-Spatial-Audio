# Ch 3: Linear Transformations and Matrices

> **Source:** [3Blue1Brown - Essence of Linear Algebra (Chapter 3)](https://www.youtube.com/watch?v=kYB8IZa5AuE)  
> **Date:** 2026-02-01

## 1. What is a "Linear Transformation"?

In Linear Algebra, we don't just use static vectors; we move them. A "Transformation" is essentially a fancy word for a **Function**: it takes a vector input and spits out a vector output.

* **Keywords:** Movement, Mapping, Morphing.
* **Two Rules for "Linearity":**
    1.  **Lines must remain lines:** No curving allowed.
    2.  **The Origin must remain fixed:** The point $(0,0)$ cannot move.

**Visual Intuition:**
Think of the 2D plane as a grid. A linear transformation keeps the grid lines **parallel** and **evenly spaced**. It can stretch, rotate, or shear the grid, but it cannot warp it.



---

## 2. Describing Transformations Numerically

How do we describe a specific transformation using numbers? We only need to track **where the Basis Vectors land**.

* $\hat{i}$ (input: $[1, 0]$) $\rightarrow$ Lands on new coordinates $[a, c]$
* $\hat{j}$ (input: $[0, 1]$) $\rightarrow$ Lands on new coordinates $[b, d]$

Because of grid linearity, if we know where $\hat{i}$ and $\hat{j}$ go, we know where *every* vector goes.
Any vector $\vec{v} = x\hat{i} + y\hat{j}$ will land on:
$$
x(\text{Where } \hat{i} \text{ landed}) + y(\text{Where } \hat{j} \text{ landed})
$$

---

## 3. Matrices as Transformations

A **Matrix** is simply a compact way to record where the basis vectors land.

<div align="center">
  <img src="https://latex.codecogs.com/svg.image?\text{Transformation}=\begin{bmatrix}a&b\\c&d\end{bmatrix}" alt="Transformation Matrix" />
</div>

<br>

* **First Column** <img src="https://latex.codecogs.com/svg.image?\begin{bmatrix}a\\c\end{bmatrix}" align="middle" height="40"/> : The new coordinates of $\hat{i}$.
* **Second Column** <img src="https://latex.codecogs.com/svg.image?\begin{bmatrix}b\\d\end{bmatrix}" align="middle" height="40"/> : The new coordinates of $\hat{j}$.

### Matrix-Vector Multiplication
Computing $A\vec{x}$ is not just memorizing "row times column". It is physically **scaling and adding the transformed basis vectors**.

<div align="center">
  <img src="https://latex.codecogs.com/svg.image?\begin{bmatrix}a&b\\c&d\end{bmatrix}\begin{bmatrix}x\\y\end{bmatrix}=x\begin{bmatrix}a\\c\end{bmatrix}+y\begin{bmatrix}b\\d\end{bmatrix}=\begin{bmatrix}ax+by\\cx+dy\end{bmatrix}" alt="Matrix Vector Multiplication" />
</div>

* **Meaning:** "Take $x$ amount of the new $\hat{i}$ and add $y$ amount of the new $\hat{j}$."

### Matrix-Vector Multiplication
Computing $A\vec{x}$ is not just memorizing "row times column". It is physically **scaling and adding the transformed basis vectors**.

<div align="center">
  <img src="https://latex.codecogs.com/svg.image?\begin{bmatrix}a&b\\c&d\end{bmatrix}\begin{bmatrix}x\\y\end{bmatrix}=x\begin{bmatrix}a\\c\end{bmatrix}+y\begin{bmatrix}b\\d\end{bmatrix}=\begin{bmatrix}ax+by\\cx+dy\end{bmatrix}" title="Linear Transformation Matrix" />
</div>

* **Meaning:** "Take $x$ amount of the new $\hat{i}$ and add $y$ amount of the new $\hat{j}$."

---

## 📝 Summary
Don't think of a matrix as a bundle of numbers. **Think of a matrix as a verb.** It represents an action (rotate, stretch, shear) performed on space. The columns of the matrix tell you exactly what happened to the fundamental building blocks ($\hat{i}$ and $\hat{j}$) of that space.
