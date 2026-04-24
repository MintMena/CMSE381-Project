---

# **Student Exam Score Analysis**

### CMSE 381 Final Project | Michigan State University | Mint Menakanit & Brian Kim | April 2026

---

This project uses a dataset of 6,607 students with 19 predictors to answer one core question:

*What actually drives student exam performance and can we predict it?*

We look at this problem two ways:

- **Regression** — predict a student's exact exam score
  
- **Classification** — group students into Low, Medium or High performers

We found out that students can be classified with about 97% accuracy.

Across all regression models, Attendance and Hours Studied were the strongest predictors.

A one standard deviation increase in attendance is associated with about a 2.3 point increase in exam score.

Regularization didn't help much here.
Ridge, Lasso and PCR all matched plain OLS at R² ≈ 0.73 and RMSE ≈ 2.0.

The dataset didn't benefit from shrinkage or dimensionality reduction since all 19 features contributed meaningful signal.

---

### **Methods Used**

- Classification: Multinomial Logistic Regression & Random Forest
- Regression: OLS, Ridge, and Lasso
- Dimensionality Reduction: PCA & PCR

*10-fold cross-validation throughout*

---

### **Files**

| File | Description |
|---|---|
| `figures/` | All output plots |
| `CMSE381-Project-Slide.pptx` | Presentation slides |
| `CMSE381-Project.ipynb` | Full analysis notebook |
| `Student_Performance_Factors.csv` | Dataset |

---

### **Tools & Libraries**

Python · scikit-learn · pandas · numpy · matplotlib · seaborn
