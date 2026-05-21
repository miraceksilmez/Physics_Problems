# Question 2: Resistors (Equivalent Resistance Combinations)

We are given exactly three identical resistors, each with a value of **$1\ \Omega$**. By using any combination of these resistors (either using one, two, or all three of them), we can calculate all the possible unique equivalent resistance ($R_{eq}$) values.

---

## 1. Using a Single Resistor
If we use only one resistor on its own:
*   **$R_{eq} = 1\ \Omega$**

---

## 2. Using Two Resistors
If we choose two out of the three resistors, there are two possible configurations:

### A. Two Resistors in Series
In a series circuit, resistances add up directly:
$$R_{eq} = 1 + 1 = 2\ \Omega$$

### B. Two Resistors in Parallel
In a parallel circuit, the equivalent resistance is calculated using the product-over-sum formula:
$$R_{eq} = \frac{1 \times 1}{1 + 1} = \frac{1}{2} = 0.5\ \Omega$$

---

## 3. Using All Three Resistors
When incorporating all three resistors into the circuit, we can form four distinct configurations:

### A. All Three in Series
All resistors are connected end-to-end:
$$R_{eq} = 1 + 1 + 1 = 3\ \Omega$$

### B. All Three in Parallel
When $n$ identical resistors are in parallel, the total resistance is the value of one resistor divided by $n$:
$$R_{eq} = \frac{1}{3} \approx 0.33\ \Omega$$

### C. Two in Parallel, Connected in Series with the Third
First, find the equivalent of the two parallel resistors ($\frac{1}{2}\ \Omega$), then add the third resistor in series:
$$R_{eq} = \left(\frac{1 \times 1}{1 + 1}\right) + 1 = 0.5 + 1 = 1.5\ \Omega \quad \left(\frac{3}{2}\ \Omega\right)$$

### D. Two in Series, Connected in Parallel with the Third
First, find the equivalent of the two series resistors ($1 + 1 = 2\ \Omega$), then pair that branch in parallel with the third resistor:
$$R_{eq} = \frac{2 \times 1}{2 + 1} = \frac{2}{3} \approx 0.67\ \Omega$$

---

## Summary: All Unique Values

Sorted from lowest to highest, here is the complete list of all unique equivalent resistance values you can create:

| Configuration Type | Fractional Value ($\Omega$) | Decimal Value ($\Omega$) |
| :--- | :---: | :---: |
| 3 in Parallel | $\frac{1}{3}$ | $\approx 0.33$ |
| 2 in Parallel | $\frac{1}{2}$ | $0.5$ |
| 2 in Series || 1 in Parallel | $\frac{2}{3}$ | $\approx 0.67$ |
| Single Resistor | $1$ | $1.0$ |
| 2 in Parallel || 1 in Series | $\frac{3}{2}$ | $1.5$ |
| 2 in Series | $2$ | $2.0$ |
| 3 in Series | $3$ | $3.0$ |

> **Conclusion:** There are exactly **7 unique** equivalent resistance values that can be generated using a supply of three $1\ \Omega$ resistors.
