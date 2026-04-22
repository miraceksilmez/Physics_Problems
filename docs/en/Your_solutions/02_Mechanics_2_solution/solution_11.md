# Physics Solution: Dynamics with a Time-Dependent Force

This document details the derivation of a particle's velocity and position vectors when subjected to a force field that varies with time.

---

## 1. Problem Statement

A particle of mass **$m = 3 \, \text{kg}$** moves in a force field $\vec{F}(t)$.
* **Force:** $\vec{F}(t) = (15t, 3t - 12, -6t^2) \, \text{N}$
* **Initial Position ($t=0$):** $\vec{r}_0 = (5, 2, -3) \, \text{m}$
* **Initial Velocity ($t=0$):** $\vec{v}_0 = (2, 0, 1) \, \text{m/s}$

**Goal:** Find the expressions for velocity $\vec{v}(t)$ and position $\vec{r}(t)$.

---

## 2. Derivation of Acceleration ($\vec{a}$)

According to Newton's Second Law ($\vec{F} = m\vec{a}$):
$$\vec{a}(t) = \frac{\vec{F}(t)}{m}$$

Substituting the given values:
$$\vec{a}(t) = \frac{1}{3} (15t, 3t - 12, -6t^2)$$
$$\vec{a}(t) = (5t, t - 4, -2t^2) \, \text{m/s}^2$$

---

## 3. Derivation of Velocity ($\vec{v}$)

Velocity is the integral of acceleration with respect to time:
$$\vec{v}(t) = \int \vec{a}(t) \, dt + \vec{v}_0$$

Integrating each component:
* $v_x(t) = \int 5t \, dt + 2 = \frac{5}{2}t^2 + 2$
* $v_y(t) = \int (t - 4) \, dt + 0 = \frac{1}{2}t^2 - 4t$
* $v_z(t) = \int -2t^2 \, dt + 1 = -\frac{2}{3}t^3 + 1$

**Result:** $\vec{v}(t) = \left( 2.5t^2 + 2, \, 0.5t^2 - 4t, \, -\frac{2}{3}t^3 + 1 \right) \, \text{m/s}$

---

## 4. Derivation of Position ($\vec{r}$)

Position is the integral of velocity with respect to time:
$$\vec{r}(t) = \int \vec{v}(t) \, dt + \vec{r}_0$$

Integrating each component:
* $x(t) = \int (2.5t^2 + 2) \, dt + 5 = \frac{2.5}{3}t^3 + 2t + 5 \approx 0.833t^3 + 2t + 5$
* $y(t) = \int (0.5t^2 - 4t) \, dt + 2 = \frac{0.5}{3}t^3 - \frac{4}{2}t^2 + 2 \approx 0.167t^3 - 2t^2 + 2$
* $z(t) = \int (-\frac{2}{3}t^3 + 1) \, dt - 3 = -\frac{2}{12}t^4 + t - 3 = -\frac{1}{6}t^4 + t - 3$

**Result:** $\vec{r}(t) = \left( \frac{5}{6}t^3 + 2t + 5, \, \frac{1}{6}t^3 - 2t^2 + 2, \, -\frac{1}{6}t^4 + t - 3 \right) \, \text{m}$

---

## 5. Summary of Results

| Property | Component Expression |
| :--- | :--- |
| **Acceleration** $\vec{a}(t)$ | $(5t, \, t - 4, \, -2t^2)$ |
| **Velocity** $\vec{v}(t)$ | $(2.5t^2 + 2, \, 0.5t^2 - 4t, \, -0.67t^3 + 1)$ |
| **Position** $\vec{r}(t)$ | $(0.83t^3 + 2t + 5, \, 0.17t^3 - 2t^2 + 2, \, -0.17t^4 + t - 3)$ |

---

## 6. Physical Conclusion
Since the force is time-dependent, the acceleration is not constant. This results in a non-linear velocity (parabolic/cubic) and a higher-order polynomial trajectory for the position.
