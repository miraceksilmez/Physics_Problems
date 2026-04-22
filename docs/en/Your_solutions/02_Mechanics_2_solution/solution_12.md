# Physics Solution: Work and Energy with a Constant Force

This document analyzes the motion of a 2 kg mass under a constant vector force and verifies the results using the Work-Energy Theorem.

---

## 1. Problem Statement

* **Mass ($m$):** 2 kg
* **Constant Force ($\vec{F}$):** $[6, 2] \, \text{N}$
* **Initial Velocity ($\vec{v}_0$):** $(1, -1) \, \text{m/s}$
* **Initial Position ($\vec{r}_0$):** $(0, 0) \, \text{m}$

**Goals:**
1. Determine $\vec{a}(t)$, $\vec{v}(t)$, and $\vec{r}(t)$.
2. Calculate work done at $t = 3 \, \text{s}$.
3. Verify with the Work-Energy Theorem.

---

## 2. Kinematic Equations

### A. Acceleration ($\vec{a}$)
Since the force is constant, acceleration is constant:
$$\vec{a} = \frac{\vec{F}}{m} = \frac{[6, 2]}{2} = (3, 1) \, \text{m/s}^2$$

### B. Velocity ($\vec{v}(t)$)
Using $\vec{v}(t) = \vec{a}t + \vec{v}_0$:
$$\vec{v}(t) = (3t, t) + (1, -1)$$
$$\vec{v}(t) = (3t + 1, t - 1) \, \text{m/s}$$

### C. Position ($\vec{r}(t)$)
Using $\vec{r}(t) = \frac{1}{2}\vec{a}t^2 + \vec{v}_0t + \vec{r}_0$:
$$\vec{r}(t) = (1.5t^2, 0.5t^2) + (t, -t) + (0, 0)$$
$$\vec{r}(t) = (1.5t^2 + t, \, 0.5t^2 - t) \, \text{m}$$

---

## 3. Work Done at $t = 3 \, \text{s}$

First, find the displacement vector $\Delta \vec{r}$ at $t = 3$:
* $x(3) = 1.5(3)^2 + 3 = 13.5 + 3 = 16.5 \, \text{m}$
* $y(3) = 0.5(3)^2 - 3 = 4.5 - 3 = 1.5 \, \text{m}$
$$\Delta \vec{r} = (16.5, 1.5) \, \text{m}$$

**Work ($W$):**
$$W = \vec{F} \cdot \Delta \vec{r} = (6 \cdot 16.5) + (2 \cdot 1.5)$$
$$W = 99 + 3 = 102 \, \text{J}$$

---

## 4. Verification: Work-Energy Theorem

The theorem states that $W = \Delta KE = KE_{final} - KE_{initial}$.

### Initial Kinetic Energy ($t=0$):
$v_0^2 = 1^2 + (-1)^2 = 2$
$$KE_i = \frac{1}{2} m v_0^2 = \frac{1}{2} (2)(2) = 2 \, \text{J}$$

### Final Kinetic Energy ($t=3$):
Find velocity at $t=3$:
* $v_x(3) = 3(3) + 1 = 10$
* $v_y(3) = 3 - 1 = 2$
$v_f^2 = 10^2 + 2^2 = 104$
$$KE_f = \frac{1}{2} m v_f^2 = \frac{1}{2} (2)(104) = 104 \, \text{J}$$

### Change in Kinetic Energy:
$$\Delta KE = 104 - 2 = 102 \, \text{J}$$

**Conclusion:** Since $W = \Delta KE = 102 \, \text{J}$, the results are consistent.

---

## 5. Summary Table

| Parameter | Formula / Vector | Value at $t=3$ s |
| :--- | :--- | :--- |
| **Acceleration** | $(3, 1)$ | $(3, 1) \, \text{m/s}^2$ |
| **Velocity** | $(3t+1, t-1)$ | $(10, 2) \, \text{m/s}$ |
| **Position** | $(1.5t^2+t, 0.5t^2-t)$ | $(16.5, 1.5) \, \text{m}$ |
| **Work Done** | $\vec{F} \cdot \Delta \vec{r}$ | **102 J** |
| **$\Delta$ KE** | $KE_f - KE_i$ | **102 J** |

---

## 6. Trajectory Description
The trajectory is a **parabola** in the $xy$-plane. Because the acceleration is constant and not parallel to the initial velocity, the particle follows a curved path starting from the origin and moving primarily in the positive $x$ direction.
