# ARTI308 – Lab 9: Decision Trees & Random Forest
 ---
## Overview
This project applies Decision Tree and Random Forest models to predict loan repayment using financial data.
---
## Dataset
- loan_data.csv
---
## Tasks
- Data preprocessing
- Model training (Decision Tree & Random Forest)
- Model evaluation
---

## Tools
- Python
- Pandas
- Scikit-learn
- Matplotlib

---

## Results

| Model | Accuracy | Recall (Class 1) | Notes |
|---|---|---|---|
| Decision Tree | 73% | 23% | Better at detecting borrowers who did not fully pay |
| Random Forest | 85% | 2% | Higher overall accuracy but misses most defaulters |

> **Note:** Although the Random Forest achieves higher overall accuracy (85%),
> this is misleading due to class imbalance in the dataset (~84% fully paid).
> The Decision Tree has a significantly better recall for the minority class (defaulters),
> making it more practical for risk detection in a financial context.
