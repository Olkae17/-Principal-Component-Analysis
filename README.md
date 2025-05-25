
## Breast Cancer PCA Analysis ##

## Overview
This project demonstrates the application of **Principal Component Analysis (PCA)** to the Breast Cancer dataset from `sklearn.datasets`. The goal is to reduce the dimensionality of the dataset and identify essential variables for donor funding strategies, as assigned by the Anderson Cancer Center. Logistic regression is applied as an optional bonus for predictive modeling.

## Dataset
- Source: "sklearn.datasets.load_breast_cancer"
- Original shape: 569 rows, 30 features + 1 target column (malignant or benign)

## Tasks Completed
1. Performed PCA on the breast cancer dataset.
2. Reduced the dataset to 2 PCA components.
3. Visualized the PCA result using a scatterplot.
4. Implemented logistic regression on the PCA-transformed data.
5. Evaluated the model's performance.

## PCA Table Interpretation

| PCA1     | PCA2     | Target |
|----------|----------|--------|
| 9.19     | 1.95     | 0      |
| 2.39     | -3.77    | 0      |
| 5.73     | -1.08    | 0      |
| 7.12     | 10.28    | 0      |
| 3.94     | -1.95    | 0      |

These values represent the transformed dataset after applying PCA. Each row is a patient case, where "PCA1" and "PCA2" are the new dimensions capturing the maximum variance in the dataset. The "target" column indicates tumor classification: 0 (Malignant) or 1 (Benign). This transformation allows us to analyze the data in a simplified 2D form without significant loss of information.

## Logistic Regression Performance

Accuracy: 0.9912

              precision    recall  f1-score   support

           0       1.00      0.98      0.99        43
           1       0.99      1.00      0.99        71

    accuracy                           0.99       114
   macro avg       0.99      0.99      0.99       114
weighted avg       0.99      0.99      0.99       114

## How to Run
1. Ensure Python is installed.
2. Install dependencies:
   pip install numpy pandas matplotlib seaborn scikit-learn
3. Run the notebook or Python script.

## Files Included
- "pca_cancer_analysis.ipynb": Main analysis notebook.
- "pca_plot.png": PCA scatterplot visualization.
- "README.md": Project summary and interpretation.
