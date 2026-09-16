# 🐱🐶 Cat vs. Dog Image Classification & Model Benchmarking

A machine-learning project that uses **OpenCV** and **Scikit-Learn** to classify cat and dog images based on handcrafted visual features. The project extracts color-based features, applies **StandardScaler** and **Principal Component Analysis (PCA)** for dimensionality reduction, and trains multiple classical machine-learning classifiers for comparison.

The complete pipeline covers **feature extraction → preprocessing → dimensionality reduction → model training → evaluation → visual prediction**.

## 📌 Features

* **Feature Extraction:** Extracts color statistics, including Mean BGR, Standard Deviation, and 3D HSV Color Histograms, producing **518 raw features** per image.
* **Preprocessing & Dimensionality Reduction:** Applies `StandardScaler` followed by **PCA (Principal Component Analysis)** to reduce feature dimensionality and mitigate the curse of dimensionality.
* **Multi-Model Benchmarking:** Trains and compares five classical machine-learning classifiers:

  1. **Random Forest Classifier**
  2. **Support Vector Machine (SVM)**
  3. **K-Nearest Neighbors (KNN)**
  4. **Decision Tree Classifier**
  5. **Quadratic Discriminant Analysis (QDA)** — regularized to improve stability when working with high-dimensional features and limited samples.
* **Model Evaluation:** Evaluates classifiers using **Accuracy, Precision, Recall, and F1-Score** based on a train/test split.
* **Visual Inference:** Uses OpenCV to display predicted classes and predicted class probabilities directly on test images in side-by-side or stacked panels.
