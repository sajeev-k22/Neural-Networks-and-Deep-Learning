
# 🌸 Iris Classification with MLP in TensorFlow

This project implements a **Multi-Layer Perceptron (MLP)** using **TensorFlow and Keras** to classify flowers in the **Iris dataset** into three species based on their sepal and petal measurements.

---

## 📊 Dataset

- **Source**: `sklearn.datasets.load_iris()`
- **Classes**: Setosa, Versicolor, Virginica
- **Features**:
  - Sepal length (cm)
  - Sepal width (cm)
  - Petal length (cm)
  - Petal width (cm)

---

## 🧠 Model Architecture

| Layer         | Units | Activation | Notes        |
|---------------|-------|------------|--------------|
| Dense         | 16    | ReLU       | Input layer  |
| Dropout       | -     | -          | rate = 0.3   |
| Dense         | 8     | ReLU       | Hidden layer |
| Dropout       | -     | -          | rate = 0.2   |
| Dense (Output)| 3     | Softmax    | Output layer |

- **Loss**: `sparse_categorical_crossentropy`
- **Optimizer**: `adam`
- **Metrics**: `accuracy`
- **Callback**: `EarlyStopping` on `val_loss` with `patience=20`

---

## 🧪 Evaluation Metrics

- **Test Accuracy**: `~96.6%`
- **Classification Report**:

| Class       | Precision | Recall | F1-score |
|-------------|-----------|--------|----------|
| Setosa      | 1.00      | 1.00   | 1.00     |
| Versicolor  | 0.89      | 1.00   | 0.94     |
| Virginica   | 1.00      | 0.92   | 0.96     |

- **Confusion Matrix**: Plotted using `Seaborn`

---

## 📈 Training Visualization

- Accuracy and Loss plotted across 200 epochs (early stopping may cut off earlier).
- Shows convergence and generalization trend on validation set.

---

## 📂 Project Structure

```
MLP_tensorflow/
│
├── MLP_tensorflow.ipynb           # Jupyter notebook with all code
├── README.md                      # Project documentation
```

---

## 🧰 Libraries Used

- `TensorFlow` / `Keras`
- `NumPy`, `Pandas`
- `Matplotlib`, `Seaborn`
- `scikit-learn`

---

## 🚀 How to Run

1. Clone the repository or copy the code.
2. Install dependencies:
   ```bash
   pip install tensorflow numpy pandas matplotlib seaborn scikit-learn
   ```
3. Run the notebook `MLP_tensorflow.ipynb` in Jupyter or Colab.

---

## 🛠 Future Enhancements

- Add hyperparameter tuning via Keras Tuner
- Try different model architectures
- Add support for cross-validation
- Deploy using Flask/Streamlit

---

## 📅 Last Updated
**June 8, 2025**

---
