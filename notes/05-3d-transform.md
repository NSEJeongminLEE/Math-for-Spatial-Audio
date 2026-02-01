# Ch 5: Three-dimensional Linear Transformations

> **Source:** [3Blue1Brown - Essence of Linear Algebra (Chapter 5)](https://www.youtube.com/watch?v=rHLEWRxRGiM)  
> **Date:** 2026-01-31

## 1. Extending to 3D (3차원으로의 확장)

In 2D, we tracked two basis vectors ($\hat{i}, \hat{j}$). In 3D, we track **three** basis vectors to define the entire space.

* <img src="https://latex.codecogs.com/svg.image?\hat{i}" align="middle" height="18"/> (x-axis): Points Right.
* <img src="https://latex.codecogs.com/svg.image?\hat{j}" align="middle" height="18"/> (y-axis): Points Up.
* <img src="https://latex.codecogs.com/svg.image?\hat{k}" align="middle" height="18"/> (z-axis): Points Forward (out of the screen).

A 3D vector is simply a linear combination of these three:

<div align="center">
  <img src="https://latex.codecogs.com/svg.image?\vec{v}=x\hat{i}+y\hat{j}+z\hat{k}" alt="3D Vector Definition" />
</div>

---

## 2. The 3x3 Matrix

To describe a linear transformation in 3D, we just need to record **where each of the three basis vectors lands**. This creates a $3 \times 3$ matrix.

<div align="center">
  <img src="https://latex.codecogs.com/svg.image?\begin{bmatrix}a&b&c\\d&e&f\\g&h&k\end{bmatrix}" alt="3x3 Matrix" />
</div>

<br>

* **Column 1:** Coordinates of where <img src="https://latex.codecogs.com/svg.image?\hat{i}" align="middle" height="18"/> lands.
* **Column 2:** Coordinates of where <img src="https://latex.codecogs.com/svg.image?\hat{j}" align="middle" height="18"/> lands.
* **Column 3:** Coordinates of where <img src="https://latex.codecogs.com/svg.image?\hat{k}" align="middle" height="18"/> lands.

---

## 3. Visualizing 3D Transformations

* **Rotation:** The entire grid rotates around a specific axis. (e.g., Rotating around the z-axis changes $\hat{i}$ and $\hat{j}$, but $\hat{k}$ stays fixed).
* **Scaling:** The grid expands or shrinks in volume.
* **Computation:** To transform any 3D vector, we multiply its coordinates by the matrix columns:

<div align="center">
  <img src="https://latex.codecogs.com/svg.image?\begin{bmatrix}a&b&c\\d&e&f\\g&h&k\end{bmatrix}\begin{bmatrix}x\\y\\z\end{bmatrix}=x\begin{bmatrix}a\\d\\g\end{bmatrix}+y\begin{bmatrix}b\\e\\h\end{bmatrix}+z\begin{bmatrix}c\\f\\k\end{bmatrix}" alt="3D Matrix Multiplication" />
</div>

---

## 📝 Summary
A 3x3 matrix is just a package of three vectors. It tells us how the "unit cube" defined by $\hat{i}, \hat{j}, \hat{k}$ is morphed into a new shape (a parallelepiped). This is the engine behind all 3D graphics and 3D spatial audio rendering.
