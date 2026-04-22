# Physics Solution: Conservation of Energy (Simple Pendulum)

This document details the calculation of a pendulum bob's velocity at the lowest point of its swing using the principle of conservation of mechanical energy.

---

## 1. Problem Statement

A pendulum with a **length ($L$) of 1.0 meter** is released from an initial angle of **$15^\circ$**. 

**Objective:** Find the speed ($v$) of the pendulum bob at the bottom of its swing (the equilibrium position).

---

## 2. Theoretical Background

In a frictionless environment, the mechanical energy of the pendulum is conserved. The **Gravitational Potential Energy ($U$)** at the release height is converted into **Kinetic Energy ($K$)** at the bottom.

$$U_{initial} = K_{final}$$
$$mgh = \frac{1}{2}mv^2$$

Where:
* $m$: Mass of the bob (cancels out)
* $g$: Acceleration due to gravity ($9.8 \, \text{m/s}^2$)
* $h$: Vertical height difference
* $v$: Velocity at the bottom

---

## 3. Geometric Calculation of Height ($h$)

To find the vertical height $h$, we use the geometry of the pendulum's swing.


The vertical distance from the pivot to the bob at the release point is $L \cos\theta$. The total length is $L$. Therefore, the height $h$ relative to the bottom is:
$$h = L - L \cos\theta = L(1 - \cos\theta)$$

Given:
* $L = 1.0 \, \text{m}$
* $\theta = 15^\circ$

$$h = 1.0 \cdot (1 - \cos 15^\circ)$$
$$h = 1.0 \cdot (1 - 0.9659)$$
$$h \approx 0.0341 \, \text{m}$$

---

## 4. Calculating the Speed ($v$)

Using the energy conservation formula derived in section 2:
$$v = \sqrt{2gh}$$

Substitute the values:
$$v = \sqrt{2 \cdot 9.8 \cdot 0.0341}$$
$$v = \sqrt{19.6 \cdot 0.0341}$$
$$v = \sqrt{0.66836}$$
$$v \approx 0.8175 \, \text{m/s}$$

---

## 5. Summary Table

| Parameter | Symbol | Value |
| :--- | :--- | :--- |
| Pendulum Length | $L$ | $1.0 \, \text{m}$ |
| Release Angle | $\theta$ | $15^\circ$ |
| Height Difference | $h$ | $\approx 0.034 \, \text{m}$ |
| **Final Speed** | $v$ | **$\approx 0.818 \, \text{m/s}$** |

---

## 6. Conclusion
As the pendulum swings downward, it loses potential energy and gains kinetic energy. At the bottom of the swing ($h=0$), the speed reaches its maximum value of approximately **$0.82 \, \text{m/s}$**.
