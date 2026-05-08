# Lab 10: Support Vector Machines (SVM)

## Overview
This project focuses on implementing **Support Vector Machines (SVM)** to classify the famous Iris flower dataset. The workflow includes exploratory data analysis (EDA), model training, and performance optimization using grid search.

---

## Dataset
The [Iris flower data set](http://en.wikipedia.org/wiki/Iris_flower_data_set) consists of 150 samples from three species of Iris:
* **Iris setosa**
* **Iris virginica**
* **Iris versicolor**
  
Four features were measured for each sample: sepal length, sepal width, petal length, and petal width (all in cm).

---

## Project Workflow

### 1. Exploratory Data Analysis (EDA)
Used **Seaborn** and **Matplotlib** to visualize the relationships between features.
* **Pairplots**: Visualized feature distributions across different species. Setosa species showed clear separation from others.
* **KDE Plots**: Analyzed sepal width vs. sepal length for specific species.

### 2. Model Training
* Split data into training and testing sets (70/30 split).
* Implemented the `SVC` model from `sklearn.svm`.
* Initial model performance evaluation using Confusion Matrix and Classification Report.

### 3. Hyperparameter Tuning (Grid Search)
To find the optimal values for parameters `C` and `gamma`, a **GridSearchCV** was performed with the following grid:
* `C`: [0.1, 1, 10, 100, 1000]
* `gamma`: [1, 0.1, 0.01, 0.001, 0.0001]

### 4. Final Evaluation
The optimized model achieved an overall **accuracy of 98%**, correctly identifying almost all samples in the test set.

---

## Technologies Used
* **Language**: Python
* **Libraries**:
    * `pandas` & `numpy` (Data Manipulation)
    * `seaborn` & `matplotlib` (Visualization)
    * `scikit-learn` (Machine Learning)
