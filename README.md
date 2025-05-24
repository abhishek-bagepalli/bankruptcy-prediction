# 📊 Bankruptcy Prediction Using Data Mining Techniques

## 🧠 Objective

This project aims to develop a predictive model using SAS Enterprise Miner to determine the likelihood of a firm filing for bankruptcy. The work was part of a Kaggle-based competition for the MGMT 571 course.

**Key Challenge**: Handling **highly imbalanced data**, where bankruptcy cases are significantly fewer than non-bankruptcy ones.

---

## ⚙️ Approach & Methodology

### 🔹 Approach 1: Manual Hyperparameter Tuning
- **Workflow**:
  - Data Import
  - Outlier Handling
  - Stratified Sampling (to oversample the minority class)
  - Model Training
  - Ensemble Modeling
  - Evaluation
- **Models Used**:
  - Neural Networks
  - Gradient Boosting
  - Polynomial Logistic Regression
- **Performance**:
  - **Validation AUC**: 91.8%
  - **Test AUC (Private Leaderboard)**: 94.8%
  - **Best Model**: Ensemble of Neural Network + Gradient Boosting

### 🔹 Approach 2: Tuned Hyperparameters
- **Workflow**:
  - Data Import
  - Partitioning
  - Model Training
  - Ensemble Modeling
  - Evaluation
- **Key Settings**:
  - Iterations: 355
  - Max Tree Depth: 5
  - Learning Rate: 0.1
- **Performance**:
  - **Training AUC**: 100%
  - **Test AUC (Private Leaderboard)**: 96.8%
  - **Misclassification Rate**: 0.44%
  - **Best Model**: Ensemble of Neural Network + Gradient Boosting

---

## 📈 Key Metrics

| Metric              | Value          |
|---------------------|----------------|
| Validation AUC      | 91.8%          |
| Test AUC (Private)  | 96.8%          |
| Misclassification   | 0.44%          |

---

## 🛠️ Tools Used

- **Software**: SAS Enterprise Miner (as required)
- **Evaluation Metric**: AUC on Kaggle Private Leaderboard

---

## 📌 Notes

This project was conducted as part of the Fall 2024 MGMT 571 course final project at Purdue University. The goal was to apply data mining techniques covered in class using a real-world dataset under controlled evaluation criteria.
