# Physics Problem: Energy Stored by Charge in a Capacitor

This repository contains the step-by-step solution to a physics problem involving a parallel-plate capacitor. 

## Problem Statement

We have a parallel-plate capacitor with the following parameters:
- **Plate Area ($S$):** $0.02 \text{ m}^2$
- **Distance between plates ($d$):** $5 \text{ mm}$
- **Voltage / Potential Difference ($U$):** $500 \text{ V}$

### Tasks:
1. Calculate the capacitance $C$ of the capacitor.
2. Calculate the energy $U_E$ stored in the capacitor.
3. Calculate the electric field intensity $E$ between the plates.
4. Calculate the force of attraction $F$ between the plates.

---

## Given Data & Unit Conversion

Before starting the calculations, all parameters must be converted into standard SI units:
* **Plate Area ($S$):** $0.02 \text{ m}^2$
* **Distance ($d$):** $5 \text{ mm} = 5 \times 10^{-3} \text{ m}$
* **Voltage ($U$):** $500 \text{ V}$
* **Permittivity of Free Space ($\varepsilon_0$):** $\approx 8.854 \times 10^{-12} \text{ F/m}$ *(assuming air or vacuum between the plates)*

---

## Step-by-Step Solution

### 1. Capacitance ($C$)
The capacitance of a parallel-plate capacitor is given by the formula:
$$C = \frac{\varepsilon_0 \cdot S}{d}$$

Substituting the values:
$$C = \frac{8.854 \times 10^{-12} \text{ F/m} \times 0.02 \text{ m}^2}{5 \times 10^{-3} \text{ m}}$$
$$C = 3.5416 \times 10^{-11} \text{ F}$$
$$\mathbf{C \approx 35.42 \text{ pF (Picofarads)}}$$

---

### 2. Energy Stored ($U_E$)
*(Note: $U_E$ is used here to represent energy to avoid confusion with voltage $U$)* The potential energy stored in a charged capacitor is calculated using:
$$U_E = \frac{1}{2} C \cdot U^2$$

Substituting the values:
$$U_E = \frac{1}{2} \times (3.5416 \times 10^{-11} \text{ F}) \times (500 \text{ V})^2$$
$$U_E = 0.5 \times 3.5416 \times 10^{-11} \times 250,000$$
$$U_E = 4.427 \times 10^{-6} \text{ J}$$
$$\mathbf{U_E \approx 4.43 \text{ }\mu\text{J (Microjoules)}}$$

---

### 3. Electric Field Intensity ($E$)
The uniform electric field between two parallel plates is given by:
$$E = \frac{U}{d}$$

Substituting the values:
$$E = \frac{500 \text{ V}}{5 \times 10^{-3} \text{ m}}$$
$$E = 100,000 \text{ V/m}$$
$$\mathbf{E = 10^5 \text{ V/m (or N/C)}}$$

---

### 4. Force of Attraction Between Plates ($F$)
The electrostatic force of attraction pulling the two plates together is given by:
$$F = \frac{1}{2} \varepsilon_0 \cdot S \cdot E^2$$

Substituting the calculated electric field intensity ($E = 10^5 \text{ V/m}$):
$$F = \frac{1}{2} \times (8.854 \times 10^{-12} \text{ F/m}) \times 0.02 \text{ m}^2 \times (10^5 \text{ V/m})^2$$
$$F = 0.5 \times 8.854 \times 10^{-12} \times 0.02 \times 10^{10}$$
$$F = 8.854 \times 10^{-4} \text{ N}$$
$$\mathbf{F \approx 0.885 \text{ mN (Millinewtons)}}$$

---

## Summary of Results

| Parameter | Formula | Calculated Value |
| :--- | :--- | :--- |
| **Capacitance ($C$)** | $C = \frac{\varepsilon_0 \cdot S}{d}$ | **$35.42 \text{ pF}$** ($3.54 \times 10^{-11} \text{ F}$) |
| **Stored Energy ($U_E$)** | $U_E = \frac{1}{2} C \cdot U^2$ | **$4.43 \text{ }\mu\text{J}$** ($4.43 \times 10^{-6} \text{ J}$) |
| **Electric Field ($E$)** | $E = \frac{U}{d}$ | **$100,000 \text{ V/m}$** ($10^5 \text{ V/m}$) |
| **Attractive Force ($F$)** | $F = \frac{1}{2} \varepsilon_0 \cdot S \cdot E^2$ | **$0.885 \text{ mN}$** ($8.85 \times 10^{-4} \text{ N}$) |
