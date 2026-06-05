# Test Scores: Mean and Standard Deviation Analysis

This repository contains the step-by-step statistical analysis of eleven students' test scores, including the calculation of the mean and sample standard deviation before and after removing the extreme (highest and lowest) values.

---

## 1. Analysis of All Test Scores (Original Data)

The original dataset consists of the following 11 test scores:  
**88, 92, 79, 85, 95, 81, 86, 90, 83, 77, 89**

* **Number of observations ($N$):** 11

### A. Calculating the Mean ($\bar{x}$)
The mean is the sum of all scores divided by the total number of students:

$$\sum_{i=1}^{11} x_i = 88 + 92 + 79 + 85 + 95 + 81 + 86 + 90 + 83 + 77 + 89 = 945$$

$$\bar{x} = \frac{945}{11} \approx 85.91$$

### B. Calculating the Sample Standard Deviation ($\sigma$)
Using the sample standard deviation formula with Bessel's correction ($N-1$):

$$\sigma = \sqrt{\frac{1}{N-1} \sum_{i=1}^{N} (x_i - \bar{x})^2}$$

First, we find the sum of squared differences from the mean $\sum (x_i - \bar{x})^2$:
$$\sum_{i=1}^{11} (x_i - 85.91)^2 \approx 310.91$$

Now, we calculate the variance and take the square root for the standard deviation:
$$\sigma^2 = \frac{310.91}{11 - 1} = \frac{310.91}{10} = 31.091$$

$$\sigma = \sqrt{31.091} \approx 5.58$$

---

## 2. Analysis After Removing Extreme Scores (Trimmed Data)

To find the new metrics, we first identify and remove the highest and lowest scores:
* **Lowest score:** 77
* **Highest score:** 95

The remaining 9 scores are:  
**88, 92, 79, 85, 81, 86, 90, 83, 89**

* **New number of observations ($N_{new}$):** 9

### A. Calculating the New Mean ($\bar{x}_{new}$)
$$\text{New Sum} = 945 - 77 - 95 = 773$$

$$\bar{x}_{new} = \frac{773}{9} \approx 85.89$$

### B. Calculating the New Sample Standard Deviation ($\sigma_{new}$)
We find the new sum of squared differences from the new mean ($85.89$):
$$\sum_{i=1}^{9} (x_i - 85.89)^2 \approx 148.89$$

Now, we compute the new variance using $N_{new} - 1 = 8$:
$$\sigma_{new}^2 = \frac{148.89}{9 - 1} = \frac{148.89}{8} \approx 18.611$$

$$\sigma_{new} = \sqrt{18.611} \approx 4.31$$

---

## Summary of Results

| Metric | Original Data (11 Scores) | Trimmed Data (9 Scores) |
| :--- | :---: | :---: |
| **Number of Students ($N$)** | 11 | 9 |
| **Mean ($\bar{x}$)** | **85.91** | **85.89** |
| **Standard Deviation ($\sigma$)** | **5.58** | **4.31** |

> **Statistical Note:** Removing the extreme outliers (77 and 95) caused the standard deviation to drop from **5.58** to **4.31**. This indicates that the remaining scores are much more tightly clustered around the mean, reducing the overall variability of the dataset.
