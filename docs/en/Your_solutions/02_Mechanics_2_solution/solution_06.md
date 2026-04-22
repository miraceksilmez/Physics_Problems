# Physics Solution: Energy Dissipation (Bouncing Ball)

This document calculates the height of a bouncing tennis ball after multiple impacts, considering a constant percentage of energy loss per bounce.

---

## 1. Problem Statement

* **Initial Height ($h_0$):** 2.0 m
* **Energy Loss per Bounce:** 30% ($0.30$)
* **Energy Retention per Bounce:** 70% ($0.70$)
* **Goal:** Calculate the height ($h_2$) after the **second bounce**.

---

## 2. Theoretical Background

The mechanical energy ($E$) of a ball at its maximum height is purely **Gravitational Potential Energy**:
$$E = mgh$$

Since mass ($m$) and gravity ($g$) are constant, the energy is directly proportional to the height:
$$E \propto h$$

If the ball loses 30% of its energy, it retains 70% of its energy. Therefore, the height after each bounce will be 70% of the previous height:
$$h_{n} = h_{n-1} \cdot 0.70$$

---

## 3. Step-by-Step Calculation

### Step 1: Height after the first bounce ($h_1$)
The ball falls from 2.0 m and hits the ground for the first time.
$$h_1 = h_0 \cdot 0.70$$
$$h_1 = 2.0 \cdot 0.70 = 1.4 \, \text{m}$$

### Step 2: Height after the second bounce ($h_2$)
The ball falls from 1.4 m and hits the ground for the second time.
$$h_2 = h_1 \cdot 0.70$$
$$h_2 = 1.4 \cdot 0.70$$
$$h_2 = 0.98 \, \text{m}$$

---

## 4. Alternative Method (General Formula)

We can use a power formula to find the height after $n$ bounces:
$$h_n = h_0 \cdot (r)^n$$
*Where $r$ is the energy retention coefficient (0.70) and $n$ is the number of bounces.*

For $n = 2$:
$$h_2 = 2.0 \cdot (0.70)^2$$
$$h_2 = 2.0 \cdot 0.49$$
$$h_2 = 0.98 \, \text{m}$$

---

## 5. Summary Table

| Bounce Number | Energy Remaining (%) | Calculation | Height (m) |
| :--- | :--- | :--- | :--- |
| 0 (Initial) | 100% | - | 2.00 m |
| 1st Bounce | 70% | $2.0 \times 0.7$ | 1.40 m |
| **2nd Bounce** | **49%** | $1.4 \times 0.7$ | **0.98 m** |

---

## 6. Conclusion
After the second bounce, the tennis ball will rise to a height of **0.98 meters** (98 cm). This represents a total loss of 51% of the original energy ($1 - 0.7^2 = 0.51$).
