# Detailed Solution: Dynamics with Two Blocks and Friction

In this problem, we analyze the movement of a 10 kg block being pulled while a 5 kg block is held stationary on top of it. This creates two distinct friction surfaces that oppose the applied force.

---

## 1. Physical Configuration and Constants

* **Upper Block ($m_1$):** 5 kg (Tied to the wall, $v = 0$).
* **Lower Block ($m_2$):** 10 kg (Pulled with force $F$).
* **Applied Force ($F_{ext}$):** 45 N.
* **Coefficient of Kinetic Friction ($\mu_k$):** 0.2.
* **Gravity ($g$):** $9.8 \, \text{m/s}^2$ (standard).

---

## 2. Forces Acting on the System

To find the acceleration of the bottom block, we must account for every force acting against the 45 N pull.

### A. Surface 1: Friction between $m_1$ and $m_2$ ($f_{k1}$)
Even though the top block ($m_1$) is tied to the wall and doesn't move relative to the floor, the bottom block ($m_2$) slides underneath it. This creates kinetic friction.
* **Normal Force ($N_1$):** Only the weight of the top block presses down on this surface.
    $$N_1 = m_1 \cdot g = 5 \cdot 9.8 = 49 \, \text{N}$$
* **Friction Force ($f_{k1}$):**
    $$f_{k1} = \mu_k \cdot N_1 = 0.2 \cdot 49 = 9.8 \, \text{N}$$
* *Direction:* This force acts to the left on the 10 kg block (opposing its motion).

### B. Surface 2: Friction between $m_2$ and the Floor ($f_{k2}$)
The bottom surface of the 10 kg block is in contact with the floor. 
* **Normal Force ($N_2$):** Both blocks press down on the floor.
    $$N_2 = (m_1 + m_2) \cdot g = (5 + 10) \cdot 9.8 = 147 \, \text{N}$$
* **Friction Force ($f_{k2}$):**
    $$f_{k2} = \mu_k \cdot N_2 = 0.2 \cdot 147 = 29.4 \, \text{N}$$
* *Direction:* This force also acts to the left.

---

## 3. Newton’s Second Law Application

We apply $\sum F = m \cdot a$ specifically to the **10 kg block ($m_2$)**, as it is the only part of the system accelerating.

### Equation Setup:
The net force is the applied force minus all opposing friction forces:
$$F_{ext} - f_{k1} - f_{k2} = m_2 \cdot a$$

### Calculation:
1.  **Calculate Total Resistance:**
    $$f_{total} = f_{k1} + f_{k2} = 9.8 + 29.4 = 39.2 \, \text{N}$$
2.  **Calculate Net Force:**
    $$F_{net} = 45 - 39.2 = 5.8 \, \text{N}$$
3.  **Solve for Acceleration ($a$):**
    $$5.8 = 10 \cdot a$$
    $$a = 0.58 \, \text{m/s}^2$$

---

## 4. Summary Table

| Force Component | Formula | Calculation | Value |
| :--- | :--- | :--- | :--- |
| **Applied Force** | Given | - | 45.0 N |
| **Top Friction** | $\mu_k \cdot m_1 g$ | $0.2 \cdot 49$ | 9.8 N |
| **Bottom Friction** | $\mu_k \cdot (m_1+m_2)g$ | $0.2 \cdot 147$ | 29.4 N |
| **Net Force** | $F - \sum f$ | $45 - 39.2$ | 5.8 N |
| **Acceleration** | $F_{net} / m_2$ | $5.8 / 10$ | **0.58 m/s²** |

---

## 5. Conclusion
The 10 kg block will accelerate at **$0.58 \, \text{m/s}^2$** in the direction of the applied force. The tension in the string holding the 5 kg block (if asked) would be equal to $f_{k1}$ ($9.8 \, \text{N}$) to keep it stationary.
