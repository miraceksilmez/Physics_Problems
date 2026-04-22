# Physics Solution: Simple Harmonic Motion (SHM)

This document provides a step-by-step calculation for the physical properties of a mass-spring system based on its oscillation equation.

---

## 1. Problem Statement

A **10 kg mass** is attached to a spring and oscillates according to the following displacement equation:
$$x(t) = 0.2 \cos(10\pi t)$$
*(where $x$ is in meters and $t$ is in seconds)*

**Goal:**
1.  Find the **spring constant ($k$)**.
2.  Find the **total mechanical energy ($E$)** of the system.

---

## 2. Parameter Extraction

By comparing the given equation $x(t) = 0.2 \cos(10\pi t)$ with the general SHM equation $x(t) = A \cos(\omega t + \phi)$, we can extract:

* **Amplitude ($A$):** $0.2 \, \text{m}$
* **Angular Frequency ($\omega$):** $10\pi \, \text{rad/s}$
* **Mass ($m$):** $10 \, \text{kg}$

---

## 3. Calculating the Spring Constant ($k$)

The relationship between angular frequency, mass, and the spring constant is:
$$\omega = \sqrt{\frac{k}{m}}$$

Squaring both sides and solving for $k$:
$$k = m \cdot \omega^2$$

Substituting the values:
$$k = 10 \cdot (10\pi)^2$$
$$k = 10 \cdot 100\pi^2$$
$$k = 1000\pi^2 \, \text{N/m}$$

**Numerical Value:**
Using $\pi^2 \approx 9.87$:
$$k \approx 1000 \cdot 9.87 = 9870 \, \text{N/m}$$

---

## 4. Calculating Total Mechanical Energy ($E$)

The total mechanical energy in a simple harmonic oscillator is the sum of kinetic and potential energy, which remains constant (assuming no friction). It is calculated at the maximum displacement (amplitude):

$$E = \frac{1}{2} k A^2$$



Substituting the values:
$$E = \frac{1}{2} (1000\pi^2) (0.2)^2$$
$$E = 500\pi^2 \cdot 0.04$$
$$E = 20\pi^2 \, \text{J}$$

**Numerical Value:**
$$E \approx 20 \cdot 9.87 = 197.4 \, \text{J}$$

---

## 5. Conclusion Table

| Variable | Symbol | Value |
| :--- | :--- | :--- |
| **Amplitude** | $A$ | $0.2 \, \text{m}$ |
| **Angular Frequency** | $\omega$ | $10\pi \, \text{rad/s}$ |
| **Spring Constant** | $k$ | $1000\pi^2 \, \text{N/m}$ |
| **Total Energy** | $E$ | $20\pi^2 \, \text{J}$ |
