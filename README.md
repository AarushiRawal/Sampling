### Sampling techniques on ML models
This project evaluates how different statistical sampling techniques influence the performance of machine learning models on an imbalanced credit card fraud dataset.

---

## Problem Statement

Credit card fraud datasets are highly imbalanced, where fraudulent transactions represent a very small portion of the data.  
This project explores how different sampling strategies impact model performance.

---

## ⚙️ Dataset

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

![Accuracy Bar Plot](accuracy_barplot.png)

---

### Average Accuracy per Sampling Technique

![Average Sampling Accuracy](average_sampling_accuracy.png)

---

## Key Observations

- **Stratified sampling** maintained class balance and produced stable performance.
- **Cluster sampling** performance depended on representativeness of selected clusters.
- **Bootstrap sampling** introduced variance but performed competitively.
- **Random Forest** showed the most consistent performance across sampling methods.
- **Logistic Regression** performed reliably after feature scaling.



## Author

Aarushi Rawal  

⭐ If you found this project interesting, feel free to star the repository!
