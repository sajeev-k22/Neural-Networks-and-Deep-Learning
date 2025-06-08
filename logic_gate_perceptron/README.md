
# 🔍 Perceptron Implementations (Hardcoded, TensorFlow, Scikit-learn)

This project demonstrates how to implement the **Perceptron** algorithm using three different methods:
- From scratch (hardcoded in Python)
- Using **TensorFlow/Keras**
- Using **Scikit-learn**

It applies to both logic gates (AND, OR) and binary classification using the Iris dataset (Setosa vs Versicolor).

---

## 📁 Project Structure

```
perceptron_project/
├── perceptron_hardcoded.py     # Hardcoded Perceptron for AND, OR gates
├── perceptron_tensorflow.py    # TensorFlow-based Perceptron for Iris
├── perceptron_sklearn.py       # Scikit-learn-based Perceptron for Iris
├── README.md                   # This file
```

---

## 1️⃣ Hardcoded Perceptron (AND, OR)

### ✨ Description:
- Implements a basic perceptron using NumPy
- Binary step activation function
- Trained on truth tables for AND and OR gates

### ✅ Output Example:
- **AND Predictions**: [0, 0, 0, 1]
- **OR Predictions**: [0, 1, 1, 1]

---

## 2️⃣ TensorFlow Perceptron (Iris Setosa vs Versicolor)

### ✨ Description:
- Binary classifier using all 4 features of Iris dataset
- Uses a single neuron (Dense layer with sigmoid activation)
- Shows training accuracy, loss plots, and confusion matrix

### ✅ Accuracy:
- **Test Accuracy**: 100%
- **Confusion Matrix**:
  ```
  [[12  0]
   [ 0  8]]
  ```

---

## 3️⃣ Scikit-learn Perceptron (Iris Setosa vs Versicolor)

### ✨ Description:
- Uses only first 2 features (Sepal Length, Sepal Width)
- Trains `sklearn.linear_model.Perceptron`
- Visualizes decision boundary

### ✅ Accuracy:
- **Test Accuracy**: 100%

---

## 📈 Visualizations

- **Training Curves** (TensorFlow)
- **Confusion Matrix** (TensorFlow)
- **Decision Boundary** (Scikit-learn)

---

## 🔧 Libraries Used

- NumPy
- Matplotlib
- TensorFlow / Keras
- Scikit-learn

---

## 🚀 How to Run

1. Install the required packages:
```bash
pip install numpy matplotlib scikit-learn tensorflow
```

2. Run each script individually in Jupyter Notebook or Python IDE.

---
