# Physics Solution: Force Field and Power Analysis

This document provides a step-by-step derivation of the kinematic and dynamic properties of a particle moving in a three-dimensional force field.

---

## 1. Problem Statement

Given a particle with mass **$m = 0.5 \, \text{kg}$** and its position vector as a function of time $t$:
* $x(t) = 5t^2 - t$
* $y(t) = 2t^3$
* $z(t) = -3t + 2$

**Goal:** Find the time dependence of velocity, momentum, acceleration, force, and power.

---

## 2. Derivation of Kinematic Variables

### A. Velocity ($\vec{v}$)
Velocity is the first derivative of the position vector with respect to time:
$$\vec{v}(t) = \frac{d\vec{r}}{dt} = \left[ \frac{dx}{dt}, \frac{dy}{dt}, \frac{dz}{dt} \right]$$

* $v_x = \frac{d}{dt}(5t^2 - t) = 10t - 1$
* $v_y = \frac{d}{dt}(2t^3) = 6t^2$
* $v_z = \frac{d}{dt}(-3t + 2) = -3$

**Result:** $\vec{v}(t) = (10t - 1, 6t^2, -3) \, \text{m/s}$

### B. Acceleration ($\vec{a}$)
Acceleration is the derivative of the velocity vector:
$$\vec{a}(t) = \frac{d\vec{v}}{dt} = \left[ \frac{dv_x}{dt}, \frac{dv_y}{dt}, \frac{dv_z}{dt} \right]$$

* $a_x = \frac{d}{dt}(10t - 1) = 10$
* $a_y = \frac{d}{dt}(6t^2) = 12t$
* $a_z = \frac{d}{dt}(-3) = 0$

**Result:** $\vec{a}(t) = (10, 12t, 0) \, \text{m/s}^2$

---

## 3. Derivation of Dynamic Variables

### A. Momentum ($\vec{p}$)
Momentum is the product of mass and velocity:
$$\vec{p}(t) = m \cdot \vec{v}(t)$$
$$\vec{p}(t) = 0.5 \cdot (10t - 1, 6t^2, -3)$$

**Result:** $\vec{p}(t) = (5t - 0.5, 3t^2, -1.5) \, \text{kg}\cdot\text{m/s}$

### B. Force ($\vec{F}$)
According to Newton's Second Law, Force is mass times acceleration:
$$\vec{F}(t) = m \cdot \vec{a}(t)$$
$$\vec{F}(t) = 0.5 \cdot (10, 12t, 0)$$

**Result:** $\vec{F}(t) = (5, 6t, 0) \, \text{N}$

---

## 4. Power Transferred ($P$)

Power is the scalar (dot) product of the Force vector and the Velocity vector:
$$P(t) = \vec{F} \cdot \vec{v}$$
$$P(t) = F_x v_x + F_y v_y + F_z v_z$$

Substituting the derived components:
$$P(t) = (5)(10t - 1) + (6t)(6t^2) + (0)(-3)$$
$$P(t) = 50t - 5 + 36t^3 + 0$$

**Result:** $P(t) = 36t^3 + 50t - 5 \, \text{W}$

---

## 5. Summary Table

| Parameter | Vector / Scalar Expression | Units |
| :--- | :--- | :--- |
| **Position** | $(5t^2 - t, 2t^3, -3t + 2)$ | m |
| **Velocity** | $(10t - 1, 6t^2, -3)$ | m/s |
| **Momentum** | $(5t - 0.5, 3t^2, -1.5)$ | kg·m/s |
| **Acceleration** | $(10, 12t, 0)$ | m/s² |
| **Force** | $(5, 6t, 0)$ | N |
| **Power** | $36t^3 + 50t - 5$ | W |
