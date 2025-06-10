# Income Classification Using Neural Networks

This project builds a deep neural network to classify individuals as earning more or less than $50K based on census data from the [Adult Income Dataset](https://archive.ics.uci.edu/ml/datasets/adult).

## 📁 Dataset

- **File**: `adult.csv`
- **Source**: UCI Machine Learning Repository
- **Attributes**:
  - Age, Workclass, Education, Marital Status, Occupation, Race, Gender, etc.
  - Target: `income` (binary: `<=50K` or `>50K`)

## 📊 Objective

Predict whether a person earns more than $50K per year using structured demographic data.

## 🧠 Model Architecture

A feedforward deep neural network implemented using Keras:

- Input Layer: 14 features (after encoding and scaling)
- Hidden Layers:
  - Dense(60, activation='relu')
  - Dense(30, activation='relu')
  - Dense(15, activation='relu')
  - Dense(7, activation='relu')
- Output Layer: Dense(1, activation='sigmoid')

## 📈 Training Configuration

- Optimizer: `Adam`
- Loss Function: `Binary Crossentropy`
- Metrics: `Accuracy`
- Epochs: 50
- Batch Size: 30
- Validation Split: 20%

## 🧪 Results

- Final training accuracy: ~87%
- Final validation accuracy: ~85%
- Accuracy and loss plots are generated using Matplotlib.

## 📉 Preprocessing Steps

1. Drop `fnlwgt` as irrelevant.
2. Convert categorical features to integers using manual mapping.
3. Normalize input features using mean and standard deviation.
4. Binary encode the `income` column (`>50K` → 1, `<=50K` → 0).
5. Custom train-test split (80/20) with reproducibility using seed.

## 📊 Visualization

Two types of plots are generated:

1. **Training vs Validation Accuracy and Loss (Epoch-wise)**
2. **Tanh and ELU Activation Functions**
   - Function outputs and derivatives plotted for visualization.

## 🧮 Activation Function Definitions

Custom definitions and plots for:
- **Tanh**
- **ELU**

Includes both:
- Function output
- Derivative

## 📦 Requirements

Install the following Python packages before running:

```bash
pip install pandas numpy matplotlib tensorflow
