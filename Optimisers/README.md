
# 🚢 Titanic Survival Prediction with Neural Network Optimizer Comparison

This project explores the performance of various **optimizers** and **learning rate schedules** on a neural network model for predicting survival on the Titanic dataset using TensorFlow/Keras.

## 📊 Dataset

The model uses the [Titanic dataset](https://www.kaggle.com/c/titanic) which includes features such as age, fare, gender, class, and embarkation port. The goal is to predict whether a passenger survived or not.

## 🧼 Data Preprocessing

1. **Dropped Columns:** `PassengerId`, `Name`, `Ticket`, `Cabin`
2. **Missing Values:**
   - `Age`, `Fare`: filled with median
   - `Embarked`: filled with mode
3. **Encoding:**
   - `Sex`: mapped to 0 (male) and 1 (female)
   - `Embarked`: one-hot encoded
4. **Feature Scaling:** Standardized `Age` and `Fare`
5. **Target Encoding:** `Survived` converted to categorical labels

## 🧠 Model Architecture

A simple **Multilayer Perceptron (MLP)** model was used:

- `Dense(64)` with ReLU
- `Dense(32)` with ReLU
- `Dense(2)` with softmax (for binary classification)

## 🧪 Experiment Setup

The training was repeated using various combinations of:
- **Optimizers:**
  - SGD
  - Momentum
  - NAG
  - Adam
  - RMSprop
  - Adagrad
  - Adadelta
  - Nadam
- **Learning Rate Schedules:**
  - Step Decay
  - Exponential Decay
  - Piecewise Constant Decay
  - Cosine Decay

### Example:
```python
keras.optimizers.Adam(learning_rate=ExponentialDecay(...))
```

Each model was trained for 15 epochs using `categorical_crossentropy` loss and accuracy as the metric.

## 📈 Results Summary

Final validation accuracies with different optimizer + schedule combos:

| Optimizer + Schedule       | Accuracy |
|---------------------------|----------|
| Adagrad + ExponentialDecay | **0.8883** |
| NAG + PiecewiseConstantDecay | 0.8827 |
| SGD + ExponentialDecay     | 0.8827 |
| Adadelta + CosineDecay     | 0.8771 |
| Momentum + StepDecay       | 0.8771 |
| ... | ... |

## 📌 Observations

- Adagrad with **Exponential Decay** yielded the best performance.
- Scheduling the learning rate had a measurable impact across all optimizers.
- Simpler optimizers like SGD benefited significantly from advanced decay strategies.

## 🧰 Requirements

- Python 3.x
- TensorFlow 2.x
- NumPy, Pandas

```bash
pip install tensorflow pandas numpy
```