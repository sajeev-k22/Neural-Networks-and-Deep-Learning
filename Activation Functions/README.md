# Activation Functions in Neural Networks

This project provides Python implementations and visualizations for various activation functions commonly used in neural networks. Each function is plotted along with its derivative to help understand its behavior during forward and backward propagation.

## 📂 Contents

- Sigmoid
- Tanh
- ReLU (Rectified Linear Unit)
- Leaky ReLU
- ELU (Exponential Linear Unit)
- Softmax
- Softplus
- Parametric ReLU (PReLU)
- Step Function

---

## 🔧 Requirements

To run the scripts and generate plots, make sure you have the following Python libraries installed:

```bash
pip install numpy matplotlib
```

---

## 🔍 Activation Functions Overview

### 1. Sigmoid
- **Formula:** `1 / (1 + exp(-x))`
- **Range:** (0, 1)
- **Use case:** Binary classification

### 2. Tanh
- **Formula:** `tanh(x)`
- **Range:** (-1, 1)
- **Use case:** Centered activation for hidden layers

### 3. ReLU
- **Formula:** `max(0, x)`
- **Range:** [0, ∞)
- **Use case:** Most popular for hidden layers due to non-linearity and efficiency

### 4. Leaky ReLU
- **Formula:** `x if x > 0 else alpha * x`
- **Fixes ReLU’s dying neuron problem**

### 5. ELU
- **Formula:** `x if x > 0 else alpha * (exp(x) - 1)`
- **Improves learning characteristics over ReLU**

### 6. Softmax
- **Formula:** `exp(x_i) / sum(exp(x))`
- **Use case:** Multi-class classification

### 7. Softplus
- **Formula:** `log(1 + exp(x))`
- **Smooth approximation of ReLU**

### 8. Parametric ReLU (PReLU)
- **Like Leaky ReLU but learns `alpha` during training**

### 9. Step Function
- **Output:** 0 or 1 depending on sign of input
- **Use case:** Obsolete in deep learning but conceptually important

---

## 📊 Visualizations

Each script includes:

- A line plot of the activation function.
- A line plot (or matrix/heatmap) of the derivative.
- Visualizations are generated using `matplotlib`.

---

