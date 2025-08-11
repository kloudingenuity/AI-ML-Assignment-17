# Bank Direct Marketing Analysis

The goal of this project is to predict whether a client will subscribe to a term deposit based on their demographic and behavioral data. This prediction enables financial institutions to target marketing efforts more effectively, reduce outreach costs, and improve conversion rates. By identifying likely subscribers, the business can prioritize high-value leads and personalize communication strategies.

---

## Objective

The primary business objective is to predict whether a customer will subscribe to a term deposit (y column: 'yes' or 'no') based on their personal, financial, and interaction-related attributes. This helps the bank:

- Optimize marketing efforts
- Target the right customers
- Improve campaign efficiency
- Increase conversion rates

---

## Tools and Technologies

- **Language**: Python
- **Data Handling**: `pandas`, `numpy`
- **Visualization**: `seaborn`, `matplotlib`
- **Modeling**: `scikit-learn`, `LogisticRegression`, `KNeighborsClassifier`, `DecisionTreeClassifier`, `SVC`
- **Workflow**: CRISP-DM Framework

---

## Project Structure
```bash
AI-ML-Assignment-17/
├── src/
│   ├── data/
│   │   ├── bank-additional-full.csv
│   │   ├── bank-additional-names.txt
│   │   └── bank-additional.csv
│   ├── CRISP-DM-BANK.pdf
│   └── prompt_III.ipynb
└── README.md
```

---

## Summary of Findings

- Logistic Regression achieved the highest F1-score (0.34), making it the most balanced model.
- SVM had the highest precision (0.73) but lowest recall (0.18), indicating it misses many actual subscribers.
- Data preprocessing included handling missing values, encoding categorical variables, and scaling features.
- Visualizations revealed key patterns in age, job type, and contact duration.

---

## Models Compared

- Logistic Regression
- K-Nearest Neighbors (KNN)
- Decision Tree
- Support Vector Machine (SVM)

All models were evaluated using precision, recall, and F1-score. Cross-validation and grid search were used to tune hyperparameters.

---

## Model Evaluation

| Model               | Precision | Recall | F1-Score | Test Accuracy  |
|---------------------|-----------|--------|----------|----------------|
| Logistic Regression | 0.70      | 0.22   | 0.34     | 0.9016         |
| KNN                 | 0.63      | 0.22   | 0.32     | 0.8972         |
| Decision Tree       | 0.73      | 0.19   | 0.30     | 0.9007         |
| SVM                 | 0.73      | 0.18   | 0.29     | 0.9002         |

> **Insight**: Logistic Regression had the best F1-score and high Recall, making it the most balanced model for predicting term deposit subscriptions.

---

## Evaluation Metric

F1-score was chosen as the primary metric to balance precision and recall, which is critical for identifying potential subscribers without overwhelming the marketing team with false positives.

---

## Recommendations

- Stock newer vehicles with lower mileage.
- Prioritize automatic, AWD/4WD, and hybrid/electric vehicles.
- Adjust pricing based on regional trends and demand.
- Focus on excellent or like-new condition cars for better returns.

---

## Next Steps

- Explore ensemble models like Random Forest or Gradient Boosting
- Improve recall through class balancing techniques.
- Deploy the best-performing model via API for real-time predictions.

---

## Source Code
- [Data](https://github.com/kloudingenuity/AI-ML-Assignment-17/blob/main/src/data/bank-additional-full.csv)
- [Jupyter Notebook](https://github.com/kloudingenuity/AI-ML-Assignment-17/blob/main/src/prompt_III.ipynb)

--- 
