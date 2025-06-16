# 🦋 Butterfly Species Classification using CNN

This project implements a **Convolutional Neural Network (CNN)** in TensorFlow to classify 75 species of butterflies using a labeled dataset. It utilizes image data split into training and testing folders, with labels provided in CSV format.

---

## 📁 Dataset

The dataset is sourced from [Kaggle: Butterfly Image Classification](https://www.kaggle.com/datasets/phucthaiv02/butterfly-image-classification), and consists of:

- `train/` folder: Contains training images.
- `test/` folder: Contains test images.
- `Training_set.csv`: CSV file with columns `filename` and `label`.
- `Testing_set.csv`: CSV file with column `filename`.

---

## 🧠 Model Overview

We built a CNN model with the following architecture:

- **3 Convolutional Blocks**: Each block has `Conv2D`, `BatchNormalization`, `MaxPooling2D`
- **Dense Layer**: 256 neurons + Dropout
- **Output Layer**: Softmax layer with 75 units (1 for each class)

**Total Parameters**: ~6.5 million

---

## 🔧 Installation

Install the dependencies using pip:

```bash
pip install tensorflow pandas numpy matplotlib seaborn scikit-learn
```

---

## 🚀 How to Run

1. Ensure the folder structure:
   ```
   ├── train/
   ├── test/
   ├── Training_set.csv
   ├── Testing_set.csv
   ├── butterfly_cnn.ipynb
   ├── butterfly_cnn.pdf
   ├── Test_Predictions.csv
   └── README.md
   ```

2. Run the model training and evaluation:
   ```bash
   python butterfly_cnn.py
   ```

---

## 📊 Results

- Achieved **~20% validation accuracy** after 30 epochs.
- Saved predictions on the test set in `Test_Predictions.csv`.

### Sample Evaluation Output:
- Precision, Recall, F1-score for each class (see classification report)
- Confusion Matrix for top 10 frequent classes

---

## 📈 Plots

The code includes visualization for:

- Training vs Validation Accuracy
- Training vs Validation Loss
- Confusion Matrix

---

## 📤 Output Files

- `Test_Predictions.csv`: Contains predicted labels for the test images.

---


