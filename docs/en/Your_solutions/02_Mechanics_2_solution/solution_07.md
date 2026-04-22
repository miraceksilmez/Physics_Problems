# Physics Solution: Dynamics with Friction

This repository contains a detailed solution for a classic dynamics problem involving two stacked blocks and kinetic friction.

## 1. Problem Statement

A **5 kg block ($m_1$)** is placed on top of a **10 kg block ($m_2$)**. 
- The 5 kg block is **tied to a wall** with a horizontal string, so it remains stationary.
- A horizontal force of **45 N** is applied to the 10 kg block.
- The coefficient of kinetic friction ($\mu_k$) between all surfaces in contact is **0.2**.

**Objective:** Find the acceleration ($a$) of the 10 kg block.

---

## 2. System Parameters and Constants

| Parameter | Symbol | Value |
| :--- | :--- | :--- |
| Mass of the top block | $m_1$ | 5 kg |
| Mass of the bottom block | $m_2$ | 10 kg |
| Applied Force | $F_{applied}$ | 45 N |
| Kinetic Friction Coefficient | $\mu_k$ | 0.2 |
| Gravitational Acceleration | $g$ | $9.8 \, \text{m/s}^2$ |

---

## 3. Calculation of Frictional Forces



Since $m_2$ is moving and $m_1$ is held stationary by the wall, friction occurs at two interfaces.

### A. Friction between the two blocks ($f_1$)
The normal force between the blocks is equal to the weight of the top block ($m_1$).
$$N_1 = m_1 \cdot g = 5 \cdot 9.8 = 49 \, \text{N}$$
$$f_1 = \mu_k \cdot N_1 = 0.2 \cdot 49 = 9.8 \, \text{N}$$

### B. Friction between the bottom block and the floor ($f_2$)
The floor supports the total weight of both blocks ($m_1 + m_2$).
$$N_2 = (m_1 + m_2) \cdot g = (5 + 10) \cdot 9.8 = 147 \, \text{N}$$
$$f_2 = \mu_k \cdot N_2 = 0.2 \cdot 147 = 29.4 \, \text{N}$$

---

## 4. Applying Newton's Second Law

We focus on the **10 kg block ($m_2$)**. The forces acting on it horizontally are:
1.  **Applied Force ($F$):** $45 \, \text{N}$ (forward)
2.  **Friction from top block ($f_1$):** $9.8 \, \text{N}$ (backward)
3.  **Friction from floor ($f_2$):** $29.4 \, \text{N}$ (backward)

According to $\sum F = m \cdot a$:

$$F_{applied} - f_1 - f_2 = m_2 \cdot a$$

Substituting the values:

$$45 - 9.8 - 29.4 = 10 \cdot a$$
$$45 - 39.2 = 10 \cdot a$$
$$5.8 = 10 \cdot a$$

---

## 5. Final Result

Solving for $a$:

$$a = \frac{5.8}{10} = 0.58 \, \text{m/s}^2$$

> **Final Answer:** The acceleration of the 10 kg block is **$0.58 \, \text{m/s}^2$**.
