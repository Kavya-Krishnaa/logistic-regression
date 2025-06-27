 🧠 Breast Cancer Prediction using Logistic Regression

 📌 Task Objective

Use Logistic Regression to classify tumors as malignant (M) or benign (B) based on medical measurements from the Breast Cancer Wisconsin dataset.

 🗂 Dataset Used

- Source: [Kaggle – Breast Cancer Wisconsin Dataset](https://www.kaggle.com/datasets/uciml/breast-cancer-wisconsin-data)
- Records: 569
- Features: Radius, texture, smoothness, symmetry, etc.
- Target: Diagnosis (`M` = malignant, `B` = benign)

 🛠️ Tools & Libraries

- Python
- pandas, numpy
- matplotlib, seaborn
- scikit-learn (LogisticRegression, metrics, train_test_split)

 🧪 Workflow

 ✅ 1. Data Preprocessing
- Dropped ID and unnamed column
- Encoded `diagnosis`: M = 1, B = 0
- Standardized all features

 ✅ 2. Model Training
- Used `LogisticRegression()` from sklearn
- Trained on 80% of the data, tested on 20%

 ✅ 3. Model Evaluation
Accuracy: 97.4%
Precision: 97.6%
Recall: 95.3%
ROC AUC: 0.997
🔵 ROC Curve
- The ROC curve shows the trade-off between sensitivity (true positive rate) and specificity (false positive rate).
- The model’s ROC-AUC score of **0.997** indicates excellent discriminatory power.
- The curve closely follows the top-left boundary, demonstrating strong classification ability.

🔁 Threshold Tuning
- Adjusted classification threshold to 0.3.
- Results:
  - Precision: 91.3%
  - Recall: 97.6%
- Lower threshold increased sensitivity — ideal for medical applications like cancer detection.

 🔄 Sigmoid Function
The logistic (sigmoid) function maps model outputs to probabilities between 0 and 1.  
It forms the foundation of logistic regression:

 📦 Files Included

- `data.csv` – Dataset  
- `breast_cancer_logistic_regression.ipynb` – Code file  
- `README.md` – This file  




