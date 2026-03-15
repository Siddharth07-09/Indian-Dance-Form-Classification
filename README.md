# Indian Dance Form Classification

## Overview

This project focuses on classifying different **Indian classical dance forms** using machine learning techniques.
Images of dancers performing various classical dance styles are used to train models that can automatically identify the dance form.

The project compares the performance of multiple machine learning algorithms to determine which model performs best for this classification task.

---

## Dataset

The dataset contains images of the following **8 Indian classical dance forms**:

* Bharatanatyam
* Kathak
* Kathakali
* Kuchipudi
* Manipuri
* Mohiniyattam
* Odissi
* Sattriya

### Dataset Structure

```
Indian_Dance
│
├── train
│   ├── bharatanatyam
│   ├── kathak
│   ├── kathakali
│   ├── kuchipudi
│   ├── manipuri
│   ├── mohiniyattam
│   ├── odissi
│   └── sattriya
│
├── test
└── test.csv
```

Each folder inside **train** contains images corresponding to that dance form.

---

## Technologies Used

* Python
* OpenCV
* NumPy
* Scikit-learn
* Matplotlib
* Pandas

---

## Machine Learning Models

The following classification models were implemented:

* K-Nearest Neighbors (KNN)
* Logistic Regression
* Decision Tree
* Random Forest

These models were trained and evaluated on the dataset to compare their performance.

---

## Image Processing

Steps used for preprocessing:

1. Load images from dataset folders
2. Resize images to **64 × 64**
3. Flatten images into feature vectors
4. Convert data into NumPy arrays
5. Split dataset into training and testing sets

---

## Evaluation Metrics

The models were evaluated using the following metrics:

* Accuracy
* Precision
* Recall
* F1 Score
* Confusion Matrix

Confusion matrices were visualized using heatmaps to better understand classification performance.

---

## Results

| Model               | Accuracy |
| ------------------- | -------- |
| KNN                 | 0.26     |
| Logistic Regression | 0.53     |
| Decision Tree       | 0.27     |
| Random Forest       | **0.54** |

Random Forest achieved the best performance among the tested models.

---

## Confusion Matrix

Confusion matrices were generated for all models using Matplotlib to visualize prediction performance across all dance classes.

Example:

```
Actual Class vs Predicted Class
```

Heatmaps were generated using a red color scale for better visualization.

---

Why Linear Regression and Multiple Linear Regression Were Not Used

Linear Regression is used for predicting continuous numerical values such as house price, temperature, or salary.

In this project, the goal is to classify Indian dance forms, which are categorical labels (e.g., Bharatanatyam, Kathak, Odissi).

Since the output is categorical and not numerical, Linear Regression is not suitable for this problem.

Multiple Linear Regression is simply an extension of Linear Regression with multiple input variables but still predicts continuous values, not categories.

Using regression models for classification problems can produce invalid outputs, such as decimal numbers that do not correspond to a class label.

Therefore, classification algorithms were used instead, such as:

KNN

Logistic Regression

Decision Tree

Random Forest

These algorithms are specifically designed to predict discrete class labels, making them appropriate for the dance form classification task

