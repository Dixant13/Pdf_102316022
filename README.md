# PDF Estimation Using Maximum Likelihood Estimation (MLE)

## Roll Number
**102316022**

## Objective
The objective of this assignment is to learn a **Probability Density Function (PDF)** from real-world data using **Maximum Likelihood Estimation (MLE)**.  
A roll-number-parameterized **non-linear transformation** is applied to personalize the data before estimating the PDF parameters.

---

## Dataset Description
- The dataset contains air pollution measurements.
- The **NO₂ (Nitrogen Dioxide)** concentration feature is automatically detected in a case-insensitive manner.
- Missing values are removed before processing.

---

## Methodology

### 1. Feature Selection
- The NO₂ column is dynamically selected from the dataset.
- This avoids hard-coded column dependencies and improves robustness.

### 2. Roll-Number-Based Transformation
A personalized non-linear transformation is applied using the roll number:

- Roll Number: **102316022**
- Parameters derived from roll number:
  - `a_r = 0.05 × (r mod 7)`
  - `b_r = 0.3 × ((r mod 5) + 1)`

This ensures each student has a unique transformation.

---

### 3. Probability Density Function
- The transformed data is modeled using a **Gaussian (Normal) PDF**.
- Parameters estimated:
  - Mean (μ)
  - Standard Deviation (σ)

---

### 4. Maximum Likelihood Estimation (MLE)
- MLE is used to estimate PDF parameters.
- The method maximizes the likelihood of observing the given data under the assumed distribution.

---

## Results
- The learned PDF closely fits the transformed NO₂ data.
- MLE provides statistically optimal parameter estimates.
- Visualization confirms a good alignment between empirical data and the estimated distribution.

---

## Files Included
- `PDF_Estimation_MLE_roll_102316022.ipynb` – Main Jupyter Notebook
- `README.md` – Project documentation

---

## Tools & Libraries Used
- Python
- NumPy
- Pandas
- Matplotlib
- SciPy

---

## Conclusion
This assignment demonstrates how **statistical modeling**, **probability theory**, and **personalized parameterization** can be combined to estimate real-world data distributions effectively using Maximum Likelihood Estimation.

---

## Author
**Dixant Sharma**  
Roll No: **102316022**
