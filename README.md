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

## How to Run the Project

1. Clone the repository

```
git clone https://github.com/yourusername/indian-dance-classification.git
```

2. Install dependencies

```
pip install opencv-python numpy matplotlib scikit-learn pandas
```

3. Run the notebook or Python script

```
python main.py
```

---

## Future Improvements

Possible improvements for this project:

* Use **deep learning models (CNN)** for higher accuracy
* Apply **feature extraction techniques (HOG / SIFT)**
* Increase dataset size
* Implement real-time dance classification

---

## Author

Developed as a machine learning project for Indian classical dance classification.

---

## License

This project is open-source and available under the MIT License.
