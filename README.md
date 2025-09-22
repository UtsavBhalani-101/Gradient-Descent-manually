# Implementing Gradient Descent from Scratch


This repository is a practical, hands-on guide to implementing the gradient descent optimization algorithm from scratch for linear regression models. The goal is to demonstrate how the algorithm scales and adapts as the dimensionality of the data increases, starting from a simple 2D dataset and moving up to a 10D dataset.

---

## 🎯 Project Goal

The primary objective is to build and understand the mechanics of gradient descent by applying it to datasets of varying complexity:

1.  **2D Data (1 Feature):** Simple linear regression ($y = mx + b$).
2.  **3D Data (2 Features):** Multiple linear regression ($y = w_1x_1 + w_2x_2 + b$).
3.  **10D Data (9 Features):** A more complex multiple linear regression to show the scalability of the vector-based approach.

This project covers the implementation of **Batch Gradient Descent**, with the structure easily adaptable for Stochastic (SGD) and Mini-Batch variations.

---

## 🔧 Technologies Used

* **Python 3.x**
* **NumPy:** For all numerical operations and vectorization.
* **Matplotlib:** For visualizing the data and results.
* **Scikit-learn:** For generating sample regression datasets.

---

## 📂 Repository Structure

```
.
├── linear_regression_2D.py       # GD implementation for 1 feature
├── linear_regression_3D.py       # GD implementation for 2 features
├── linear_regression_10D.py      # GD implementation for 9 features
└── README.md
```

---

## ✨ Implementations

### 1. Simple Linear Regression (2D)

This is the foundational implementation. The model learns the optimal slope (`coefficient`) and `intercept` for a single-feature dataset. It's a great starting point for understanding the core update rules of gradient descent.

### 2. Multiple Linear Regression (3D)

The model is extended to handle data with two features. This implementation introduces the concept of a **weight vector** instead of a single coefficient, and the prediction is calculated using the **dot product**.

### 3. Generalized Multiple Linear Regression (10D)

This script demonstrates how the vectorized approach from the 3D case can seamlessly handle any number of features. By implementing it for a 10-dimensional dataset (9 features + 1 target), we show how the same logic scales without needing to manually handle each coefficient. The gradient calculation is fully vectorized for efficiency.

---

## 🚀 How to Run

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/UtsavBhalani-101/Gradient-Descent-manually.git](https://github.com/UtsavBhalani-101/Gradient-Descent-manually.git)
    cd Gradient-Descent-manually
    ```

2.  **Install the dependencies:**
    ```bash
    pip install numpy matplotlib scikit-learn
    ```

3.  **Run any of the implementation files:**
    ```bash
    python linear_regression_10D.py
    ```

The script will generate the necessary data, train the model using gradient descent, and print the learned weights and intercept.
