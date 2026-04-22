# Physics Solution: Work of a Variable Force and Potential Energy

This document analyzes a one-dimensional restorative force, derives the equation of motion, and establishes the mathematical relationship between work and potential energy.

---

## 1. Equation of Motion

Given a one-dimensional restorative force:
$$F(x) = -kx$$
*(where $k$ is a positive constant, representing Hooke's Law)*

According to **Newton's Second Law** ($F = ma$):
$$m \frac{d^2x}{dt^2} = -kx$$

Rearranging into a standard differential equation:
$$\frac{d^2x}{dt^2} + \frac{k}{m}x = 0$$

### Solution
This is the equation for **Simple Harmonic Motion (SHM)**. Let $\omega^2 = \frac{k}{m}$, the general solution is:
$$x(t) = A \cos(\omega t + \phi)$$
*Where $A$ is the amplitude and $\phi$ is the phase constant.*

---

## 2. Work Done During Displacement

The work done by a variable force during a displacement from $x = 0$ to $x = x_0$ is the integral of the force over the distance:

$$W = \int_{0}^{x_0} F(x) \, dx$$

Substituting $F(x) = -kx$:
$$W = \int_{0}^{x_0} (-kx) \, dx$$
$$W = -k \left[ \frac{1}{2}x^2 \right]_{0}^{x_0}$$
$$W = -\frac{1}{2}kx_0^2$$

---

## 3. Potential Energy Interpretation

By definition, the change in **Potential Energy ($\Delta U$)** is equal to the negative of the work done by a conservative force:
$$\Delta U = -W$$

Assuming the potential energy at the equilibrium position is zero ($U(0) = 0$):
$$U(x_0) - 0 = - \left( -\frac{1}{2}kx_0^2 \right)$$
$$U(x) = \frac{1}{2}kx^2$$

**Interpretation:** The work done **against** the restorative force is stored in the system as elastic potential energy.

---

## 4. Verification of $F = -\frac{dU}{dx}$

To verify the relationship between the force field and the potential gradient:
$$\frac{dU}{dx} = \frac{d}{dx} \left( \frac{1}{2}kx^2 \right)$$
$$\frac{dU}{dx} = \frac{1}{2}k \cdot (2x) = kx$$

Therefore:
$$- \frac{dU}{dx} = -kx$$
Since $F = -kx$, the relationship **$F = -\frac{dU}{dx}$ is verified**.

---

## 5. Graphical Representation



* **Force Graph ($F(x)$):** A straight line with a slope of $-k$. It shows that as displacement increases, the restoring force increases in the opposite direction.
* **Potential Energy Graph ($U(x)$):** A parabola ($y = ax^2$). It shows that energy is always positive and reaches its maximum at the points of maximum displacement.

---

## Summary Table

| Property | Formula |
| :--- | :--- |
| **Force** | $F = -kx$ |
| **Acceleration** | $a = -\frac{k}{m}x$ |
| **Work Done** | $W = -\frac{1}{2}kx^2$ |
| **Potential Energy** | $U = \frac{1}{2}kx^2$ |
