
# Loan Approval Prediction using Decision Tree

## Project Overview
This project focuses on building a **Loan Approval Prediction system** using a **Decision Tree Classifier**.  
The objective is to predict whether a loan application will be **approved or rejected** based on applicant financial, demographic, and loan-related features.

The model is trained on a cleaned and encoded dataset and enhanced with **domain-driven financial ratios** to make predictions more realistic and closer to real-world banking decisions.

---

## Dataset Description
The dataset contains applicant and loan-related information such as:

- Personal details (Age, Gender, Dependents, Education)
- Financial details (Annual Income, Monthly Income, Outstanding Debt)
- Credit-related attributes (Credit Score, Loan History, Default Risk)
- Loan details (Loan Amount, Loan Term, Interest Rate, Loan Type)
- Derived features:
  - Loan to Income Ratio
  - Debt to Income Ratio
  - Loan × Loan Term

Categorical features were encoded using **Label Encoding**, **Ordinal Encoding**, and **One-Hot Encoding (drop='first')**.

---

## Model Used
- **Decision Tree Classifier**
- Pre-pruning techniques applied:
  - `max_depth`
  - `min_samples_leaf`
  - `min_samples_split`

These constraints were used to reduce overfitting and improve generalization.

---

## Model Performance

- **Training Accuracy:** ~84%
- **Test Accuracy:** **85%**
- **ROC-AUC:** Strong separation between approved and rejected classes

The model shows good statistical performance while also behaving more realistically after adding domain-based financial features.

---

## Key Observations
- High-impact features include:
  - Annual Income
  - Credit Score
  - Loan Amount Requested
  - Debt-to-Income Ratio
- Adding domain-based ratios did not significantly increase accuracy but **greatly improved real-world decision realism**
- Accuracy alone is not sufficient for loan approval systems; business constraints are equally important

---

## Technologies Used
- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib / Seaborn

---

## How to Run the Project
1. Clone the repository:
   ```bash
   git clone https://github.com/Naman0911/Loan-Approval-Predict.git
   ```

2. Install required libraries:
   ```bash
   pip install -r requirements.txt
   ```

3. Run the notebook or Python scripts to train and evaluate the model.

---

## Conclusion
This project demonstrates how **Decision Tree models**, when combined with **proper feature engineering and domain knowledge**, can produce reliable and interpretable loan approval predictions.  
The final model achieves **85% accuracy** and aligns better with real-world lending logic.

---

## Author
**Naman Upadhyay**
