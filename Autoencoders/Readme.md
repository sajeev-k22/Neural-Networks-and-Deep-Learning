# 🧠 Autoencoder and Convolutional Autoencoder on CIFAR-10

This project demonstrates the design, training, and evaluation of both **dense (fully connected) autoencoders** and **convolutional autoencoders** for **image denoising** on the CIFAR-10 dataset.

The goal is to learn compressed representations of images and reconstruct clean images from noisy inputs.

---

## 📌 Features

- Data loading and preprocessing (with optional Gaussian noise)
- Fully connected (dense) autoencoder
- Convolutional autoencoder with Conv2D, BatchNorm, Pooling, and UpSampling
- Training with MSE loss and early stopping
- Evaluation with test set loss
- Visualization of original, noisy, and reconstructed images

---

## 🧩 How It Works

### 📌 Data Preprocessing
- CIFAR-10 images normalized to [0, 1]
- Optional Gaussian noise added (noise_factor=0.2)
- Noisy images used as input, clean images as target

### 📌 Dense Autoencoder
- Input images are flattened
- Encoding with Dense layers to a latent space
- Decoding back to image shape
- Uses sigmoid output activation

### 📌 Convolutional Autoencoder
- Convolutional encoder with pooling for downsampling
- Decoder with Conv2D + UpSampling for reconstruction
- Preserves spatial features for better image quality

---

## 📊 Training Details

- Loss: Mean Squared Error (MSE)
- Optimizer: Adam
- Early stopping with patience
- Batch size: 128
- Epochs: up to 50 (early stops if no improvement)

Example Results:

✅ Dense Autoencoder Test Loss ~0.0081  
✅ Convolutional Autoencoder Test Loss ~0.0052  

---

## 📸 Visualization

The script plots:

- Original clean images
- Noisy inputs
- Reconstructed outputs

✅ See the denoising quality side-by-side!

---

## 🛠 Customization

You can change:

- Noise factor
- Latent dimensions
- Batch size, epochs
- Model architecture (number of layers, filters)

---

## 📄 Example Usage in Code

```python
from utils.data_loader import load_and_preprocess_data
from utils.dense_autoencoder import build_autoencoder
from utils.conv_autoencoder import build_convolutional_autoencoder
from utils.train_utils import train_autoencoder, evaluate_autoencoder, plot_reconstructed_images

# Load Data
x_train_noisy, x_train, x_test_noisy, x_test = load_and_preprocess_data()

# Build Model
autoencoder, encoder, decoder = build_autoencoder()

# Train
history = train_autoencoder(autoencoder, x_train_noisy, x_train, x_test_noisy, x_test)

# Evaluate
test_loss = evaluate_autoencoder(autoencoder, x_test_noisy, x_test)

# Plot
plot_reconstructed_images(autoencoder, x_test_noisy, x_test)
```

---

## ✨ Results

- Dense autoencoder reduces noise but can blur details.
- Convolutional autoencoder better preserves edges and structure.

---

## 📚 References

- [CIFAR-10 Dataset](https://www.cs.toronto.edu/~kriz/cifar.html)
- [Autoencoders - Deep Learning Book](https://www.deeplearningbook.org/contents/autoencoders.html)
- [TensorFlow Keras Documentation](https://keras.io/)

---

> 💡 Tip: Modularize your code for easy experimentation with different architectures and hyperparameters!
