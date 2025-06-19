
# CNN-Based Image Classification using TensorFlow

This project demonstrates a Convolutional Neural Network (CNN) implementation using TensorFlow and Keras for image classification tasks, likely on grayscale image datasets such as MNIST or Fashion-MNIST.

## 🧠 Model Architecture

The CNN model used in this notebook consists of:

- Conv2D layer with 32 filters (3x3 kernel, ReLU activation)
- MaxPooling2D (2x2)
- Conv2D layer with 64 filters (3x3 kernel, ReLU activation)
- MaxPooling2D (2x2)
- Flatten layer
- Dense layer with 128 units (ReLU)
- Output Dense layer with 10 units (Softmax)

## 📦 Dependencies

Ensure the following Python libraries are installed:

- TensorFlow
- NumPy
- Matplotlib
- scikit-learn

Install via pip:

```bash
pip install tensorflow numpy matplotlib scikit-learn
```

## 🚀 How to Run

1. Open the Jupyter Notebook (`.ipynb` file).
2. Run all cells in sequence.
3. The notebook will:
   - Build the CNN model
   - Train it on the dataset
   - Evaluate performance
   - Display metrics such as the confusion matrix

## 📊 Output

- Training and validation accuracy/loss plots
- Confusion matrix for evaluating model predictions

## 📁 Files

- `CNN_classification.ipynb` – Contains the complete code for building, training, and evaluating the CNN.
- `CNN_classification.pdf` – Contains the pdf.
