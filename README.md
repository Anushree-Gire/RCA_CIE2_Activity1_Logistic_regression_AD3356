# Early Stage Diabetes Risk Prediction Using Logistic Regression

## Project Overview

This project uses **Binary Logistic Regression** to predict early-stage diabetes risk based on an individual's age, gender and reported symptoms.

The model classifies records into two categories: Positive and Negative. The project demonstrates how machine learning can support early risk identification using health-related data.

## Objectives

- Understand and analyse the diabetes dataset.
- Perform data cleaning and preprocessing.
- Apply Binary Logistic Regression.
- Evaluate the model using classification metrics.
- Compare different decision thresholds.
- Predict the class of a new sample record.

## Dataset Information

**Dataset Name:** Early Stage Diabetes Risk Prediction Dataset

**Source:** UCI Machine Learning Repository

**Dataset Link:** https://doi.org/10.24432/C5VG8H

The original dataset contains:
- 520 records
- 16 input features
- 1 target column (`class`)

**Target Classes:**
- Negative (0): Classified as not having diabetes.
- Positive (1): Classified as having diabetes.

The dataset includes age, gender and symptoms such as Polyuria, Polydipsia, weakness and other health-related indicators.

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Google Colab

## Project Workflow

1. Dataset loading and inspection.
2. Data cleaning and removal of exact duplicate rows.
3. Exploratory Data Analysis (EDA).
4. Encoding categorical features using One-Hot Encoding.
5. Splitting data into 80% training and 20% testing sets using stratified sampling.
6. Applying StandardScaler to numerical features.
7. Training the Logistic Regression model.
8. Evaluating predictions using classification metrics.
9. Comparing decision thresholds of 0.3, 0.5 and 0.7.
10. Predicting the class of a new sample record.

After removing exact duplicate rows, the dataset contained **251 records**.

## Model Used

**Algorithm:** Logistic Regression

Logistic Regression estimates the probability that a record belongs to the Positive class using the sigmoid function.

The model was trained using the training dataset with `max_iter=1000`.

## Model Performance

### Results at Default Threshold (0.5)

| Metric | Result |
|---|---:|
| Accuracy | 80.39% |
| Precision (Positive) | 93.00% |
| Recall (Positive) | 77.00% |
| F1-score (Positive) | 0.84 |
| ROC-AUC | 0.92 |

### Results at Selected Threshold (0.3)

| Metric | Result |
|---|---:|
| Accuracy | 84.3% |
| Precision | 90.9% |
| Recall | 85.7% |
| Specificity | 81.2% |
| F1-score | 0.882 |

A threshold of **0.3** was selected because identifying more potentially Positive cases is important in an early-screening context.

## Conclusion

Logistic Regression was successfully applied to predict early-stage diabetes risk using the available dataset.

The model achieved 84.3% accuracy and an F1-score of 0.882 at the selected threshold of 0.3. The project helped demonstrate data preprocessing, classification, model evaluation and probability-based prediction.

## Limitations

- The original dataset contains only 520 records.
- Removing duplicate rows reduced the dataset to 251 records.
- Model performance depends on the quality and representativeness of the dataset.
- The model may not perform equally well on different populations.

**Note:** This project is for educational purposes only. Its predictions are probability-based estimates and must not be considered a substitute for professional medical diagnosis.

## Submission Information

**Faculty Submission GitHub ID:** [https://github.com/complexiota](https://github.com/complexiota)

**Student's Public Repository:** [Paste your own repository URL here]

All project files, including the completed notebook, required datasets and README, are maintained in this repository for faculty review.
