# PRODIGY_DS_03

## 🎯 Internship Task 03 – Customer Purchase Prediction using Decision Tree Classifier

This project builds a **Decision Tree Classifier** to predict whether a customer will **subscribe to a term deposit**, based on their **demographic and behavioral data**. The dataset is taken from the **Bank Marketing dataset** available on the UCI Machine Learning Repository.

---

## 📁 Dataset Used

- **Source**: [🔗 UCI Bank Marketing Dataset](https://archive.ics.uci.edu/dataset/222/bank+marketing)
- **File**: `bank-full.csv` (Contains 45,211 records)

---

## Objective

- Build a model to classify whether a customer will **purchase a product/service (Yes/No)**.
- Use **Decision Tree Classifier** to understand how decisions are made based on features.

---

## Steps Involved

1. **Data Preprocessing**
   - Converted categorical columns to numerical using one-hot encoding.
   - Target column (`y`) converted to binary (`1 = yes`, `0 = no`).
   
2. **Model Building**
   - Used `DecisionTreeClassifier` from `sklearn`.
   - Split data into **train (70%)** and **test (30%)**.
   - Trained with **entropy criterion** and custom `max_depth`.

3. **Evaluation**
   - Evaluated model with accuracy score and classification report.
   - Visualized the decision tree structure using `plot_tree()`.

---

## 📊 Results

- **Accuracy**: `87.2%`
- **Classification Report**:
  - **Precision (Yes)**: `46%`
  - **Recall (Yes)**: `46%`
  - **F1-Score (Yes)**: `46%`
- Class imbalance affects the model’s ability to correctly identify `Yes` cases.

---

## 🔍 Key Insights

- The model performs well overall due to high accuracy on the majority class (`No`).
- **Class imbalance** is a challenge — many customers do not subscribe.
- The most important features were **contact duration**, **previous campaign outcomes**, and **job/education**.
- Tree visualization helped interpret how decisions are made.

---

## Tools & Technologies

- **Python 3**
- pandas, matplotlib, seaborn
- scikit-learn (DecisionTreeClassifier, train_test_split, plot_tree)

---

