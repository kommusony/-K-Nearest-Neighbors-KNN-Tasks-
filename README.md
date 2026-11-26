# Breast Cancer Classification using K-Nearest Neighbors (KNN)

## Project Overview

This project applies the **K-Nearest Neighbors (KNN) Classification** algorithm to the Wisconsin Diagnostic Breast Cancer dataset. The objective is to classify tumors as **Benign or Malignant** using numerical features extracted from breast cancer cell images.

The project also compares different distance metrics to understand their impact on classification performance.

## Problem Statement

Build a machine learning classification model that uses numerical measurements of breast cancer cells to predict whether a tumor is benign or malignant.

## Dataset

The project uses the **Wisconsin Diagnostic Breast Cancer (WDBC)** dataset.

- **Task type:** Binary Classification
- **Target:** Diagnosis (Benign / Malignant)
- **Classes:**
  - Benign (B) – Non-cancerous tumor
  - Malignant (M) – Cancerous tumor
- **Features:** 30 numerical measurements derived from digitized images of breast mass samples.
- **Dataset source:** Scikit-learn Breast Cancer Dataset (based on WDBC).

## Workflow

1. Import the required Python libraries.
2. Download and load the breast cancer dataset.
3. Understand the dataset structure and statistical information.
4. Perform exploratory data analysis (EDA).
5. Explore the target variable and class distribution.
6. Check missing values and duplicate records.
7. Perform data preprocessing and target encoding.
8. Separate input features (X) and target variable (y).
9. Split the dataset into training and testing sets (80:20).
10. Apply feature scaling using StandardScaler.
11. Train the KNN classification model.
12. Generate predictions on test data.
13. Evaluate the model using accuracy, precision, recall, and F1-score.
14. Visualize the confusion matrix.
15. Compare four different distance metrics.
16. Predict the class of an unseen sample.

## Algorithm: K-Nearest Neighbors (KNN)

K-Nearest Neighbors is a supervised machine learning algorithm used for classification and regression.

It classifies a new data point by finding the nearest K data points in the training dataset and predicting the majority class among those neighbors.

In this project:
- **K value:** 5
- **Feature scaling:** StandardScaler
- **Train-test split:** 80% training and 20% testing.

### Distance Metrics Compared

1. **Minkowski Distance:** General distance metric. With p=2, it behaves like Euclidean distance.
2. **Manhattan Distance:** Calculates the sum of absolute differences between feature values.
3. **Hamming Distance:** Measures the proportion of feature positions that differ.
4. **Chebyshev Distance:** Measures the maximum absolute difference between feature values.

## Model Evaluation

The model is evaluated using the following performance metrics:

| Metric | Description |
|---|---|
| Accuracy | Overall correct predictions |
| Precision | Correct positive predictions |
| Recall | Ability to identify actual positive cases |
| F1-Score | Balance between precision and recall |
| Confusion Matrix | Shows correct and incorrect predictions |

The notebook compares the performance of all four distance metrics and identifies the best-performing metric based on test accuracy.

*Note: Add the actual accuracy values from your notebook outputs after running all cells.*

## Technologies Used

- Python
- Jupyter Notebook
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

## How to Run

1. Clone or download this GitHub repository.
2. Install the required libraries:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn jupyter
```

3. Open the notebook using Jupyter Notebook or VS Code.
4. Run all notebook cells from top to bottom.
5. Observe the model predictions, evaluation metrics, and distance metric comparison.

## Key Learnings

- Understanding binary classification problems.
- Exploring and preprocessing a real-world dataset.
- Understanding the K-Nearest Neighbors algorithm.
- Learning the importance of feature scaling.
- Comparing different distance metrics.
- Evaluating classification models using performance metrics.
- Visualizing model performance using a confusion matrix.
- Predicting outcomes for unseen data.
- Understanding the importance of avoiding data leakage.

## Project Structure

```text
Breast-Cancer-KNN-Classification/
│
├── KNN_Breast_Cancer_Binary_Classification.ipynb
├── README.md
│
└── requirements.txt
```

## Author

**Sony Kommu**

Machine Learning Practice Project completed as part of the Innomatics Research Labs ML Module.

## Disclaimer

This project is developed for educational and machine learning practice purposes only. It is not a medical diagnostic tool and should not be used for clinical decision-making.

