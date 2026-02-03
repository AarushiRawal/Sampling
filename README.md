### Sampling techniques on ML models
This project evaluates how different statistical sampling techniques influence the performance of machine learning models on an imbalanced credit card fraud dataset.

---

## Problem Statement

Credit card fraud datasets are highly imbalanced, where fraudulent transactions represent a very small portion of the data.  
This project explores how different sampling strategies impact model performance.

---

## Dataset

- Source: Credit Card Fraud Dataset
- Binary Classification:
  - 0 → Non-Fraud
  - 1 → Fraud
- Original dataset was imbalanced.
- Downsampling was applied to create a balanced dataset before sampling.

---

## Sampling Techniques Implemented

1. **Random Sampling**
2. **Stratified Sampling**
3. **Systematic Sampling**
4. **Cluster Sampling (KMeans-based)**
5. **Bootstrap Sampling**

---

## Machine Learning Models Used

- Logistic Regression
- Decision Tree
- Random Forest
- Support Vector Machine (SVM)
- K-Nearest Neighbors (KNN)

---

## Model Accuracy Comparison

### Accuracy Comparison Across Sampling Techniques

![Accuracy Bar Plot](https://github.com/AarushiRawal/Sampling/blob/main/accuracy_barplt%20(1).png)

---

### Average Accuracy per Sampling Technique

![Average Sampling Accuracy](https://github.com/AarushiRawal/Sampling/blob/main/avg_sampling_accuracy%20(1).png)

---
## Model Accuracy Comparison

| Model                  | Random | Stratified | Systematic | Cluster | Bootstrap |
|------------------------|--------|------------|------------|----------|-----------|
| Logistic Regression    | 93.73 | 92.08    | 91.27     | 98.18  | 90.19    |
| Decision Tree          | 97.00 | 97.54     | 94.76     | 99.09   | 97.28    |
| Random Forest          | 99.18 | 99.73     | 99.13    | 99.09   | 99.18    |
| SVM                    | 97.55 | 97.81     | 98.69     | 100.00  | 96.73    |
| KNN                    | 92.92 | 93.17    | 90.39     | 92.73   | 91.83    |


## Key Observations
-Cluster Sampling consistently produced the highest accuracy across most models, achieving peak performance for Logistic Regression, Decision Tree, and SVM. This suggests that grouping structurally similar data points improved model learning.

-Random Forest demonstrated the most stable and highest overall performance, maintaining accuracy above 99% across all sampling techniques. This confirms the robustness of ensemble learning methods to variations in data sampling.

-SVM achieved 100% accuracy under Cluster Sampling, indicating strong class separability within selected clusters. However, such perfect accuracy may also indicate potential overfitting.

-Stratified Sampling produced consistently strong results, especially for Random Forest and SVM, highlighting its effectiveness in maintaining class distribution balance.

-Systematic Sampling performed competitively, particularly for SVM and Random Forest, showing that ordered selection did not negatively impact model performance in this case.

-Bootstrap Sampling showed stable but slightly lower performance compared to Cluster and Stratified sampling, though it still maintained high accuracy levels across models.

-KNN showed comparatively lower performance than other models, suggesting sensitivity to sampling structure and feature distribution.

## Author

Aarushi Rawal  
