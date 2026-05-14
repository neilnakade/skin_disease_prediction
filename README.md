#  Skin Disease Prediction using Machine Learning

##  Project Overview

This project focuses on predicting different types of skin diseases using Machine Learning techniques on a dermatology dataset containing clinical and histopathological features.

Erythemato-squamous diseases often share similar symptoms, making diagnosis challenging. The goal of this project is to compare multiple machine learning models and identify the most effective approach for accurate disease classification.

---

##  Dataset Information

* Dataset: Dermatology Dataset
* Features: Clinical and histopathological attributes
* Target Variable: Skin disease class
* Includes patient-related information such as age and disease characteristics

---

##  Exploratory Data Analysis (EDA)

The following analyses were performed:

* Distribution of skin disease classes
* Age distribution analysis
* Correlation heatmap between features
* Erythema distribution across disease classes

### Key Insights

* The dataset is relatively balanced across disease classes.
* Certain clinical features show strong correlation with specific disease types.
* Some disease classes share visually similar feature patterns, increasing classification difficulty.

---

##  Data Preprocessing

The following preprocessing steps were applied:

* Replaced missing values represented as `?`
* Converted Age column to numeric format
* Filled missing Age values using median imputation
* Performed train-test split
* Applied feature scaling using StandardScaler

### Preprocessing Justification

* Median imputation was used because it is less sensitive to outliers.
* Feature scaling ensures all variables contribute equally during model training.
* Train-test split prevents data leakage and enables unbiased evaluation.

---

## Machine Learning Models Used

The following models were implemented and compared:

* Logistic Regression
* Decision Tree Classifier
* Random Forest Classifier

---

##  Model Comparison

| Model               | Accuracy |
| ------------------- | -------- |
| Logistic Regression | 0.986486|
| Decision Tree       | 0.986486|
| Random Forest       | 0.986486|

 **Best Performing Model: Random Forest Classifier**

---

##  Model Evaluation

The models were evaluated using:

* Accuracy Score
* Classification Report
* Confusion Matrix
* Feature Importance Analysis

### Confusion Matrix

(confusion_matrix.png)

### Feature Importance

(feature_importance.png)

### Key Findings

* Random Forest achieved the best overall performance.
* Most predictions were correctly classified, as shown by strong diagonal values in the confusion matrix.
* Misclassifications mainly occurred between disease classes with similar clinical characteristics.

---

##  Feature Importance Analysis

Random Forest feature importance helped identify the most influential clinical features contributing to disease prediction.

This improves model interpretability and helps understand which symptoms are most significant for classification.

---

##  Challenges Faced

* Handling missing values in the Age column
* Similarities between disease classes leading to classification confusion
* Interpreting high-dimensional clinical features

---

##  Future Improvements

* Apply advanced ensemble methods such as XGBoost
* Perform hyperparameter tuning using GridSearchCV
* Explore Deep Learning approaches for enhanced performance
* Deploy the model as a web application

---

##  Tech Stack

* Python
* Pandas
* NumPy
* Scikit-learn
* Matplotlib
* Seaborn

---

##  Conclusion

This project demonstrates a complete machine learning workflow including data preprocessing, exploratory analysis, model building, evaluation, and interpretation.

Among all models, Random Forest delivered the most reliable performance due to its ensemble learning capability and robustness in handling complex feature relationships.
