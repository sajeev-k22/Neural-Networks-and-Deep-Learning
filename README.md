# 🤖 Neural Network and Deep Learning 

This repository is a collection of various neural network and deep learning projects, examples, and tutorials. Each sub-directory contains a specific project with its own dataset, code (primarily Jupyter Notebooks), and detailed README file.

## 🗂️ Projects Overview

Below is a list of the projects included in this collection. Click on the project title to navigate to its dedicated directory for more details, including specific setup instructions and code.

1.  **[📉 Activation Functions](./Activation%20Functions/)**
    *   **Description:** Explores and visualizes various activation functions (Sigmoid, Tanh, ReLU, Leaky ReLU, ELU, Softmax, Softplus, PReLU, Step Function) commonly used in neural networks, along with their derivatives.
    *   **Key Technologies:** Python, NumPy, Matplotlib.
    *   **View Project:** [`./Activation Functions/README.md`](./Activation%20Functions/README.md)

2.  **[🦋 Butterfly Classifications](./Butterfly_Classifications/)**
    *   **Description:** Implements a Convolutional Neural Network (CNN) using TensorFlow to classify 75 different species of butterflies from image data.
    *   **Key Technologies:** Python, TensorFlow, Keras, Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn.
    *   **View Project:** [`./Butterfly_Classifications/README.md`](./Butterfly_Classifications/README.md)

3.  **[🧠 CNN with TensorFlow](./CNN_tensorflow/)**
    *   **Description:** Demonstrates a Convolutional Neural Network (CNN) implementation using TensorFlow and Keras for image classification tasks, suitable for datasets like MNIST or Fashion-MNIST.
    *   **Key Technologies:** Python, TensorFlow, Keras, NumPy, Matplotlib, Scikit-learn.
    *   **View Project:** [`./CNN_tensorflow/README.md`](./CNN_tensorflow/README.md)

4.  **[💰 Income Classification](./Income%20Classification/)**
    *   **Description:** Builds a deep neural network to classify individuals as earning more or less than $50K based on the Adult Income Dataset (census data).
    *   **Key Technologies:** Python, TensorFlow, Keras, Pandas, NumPy, Matplotlib.
    *   **View Project:** [`./Income Classification/README.md`](./Income%20Classification/README.md)

5.  **[🌸 MLP with TensorFlow (Iris Classification)](./MLP_Tensorflow/)**
    *   **Description:** Implements a Multi-Layer Perceptron (MLP) using TensorFlow and Keras to classify flowers in the Iris dataset into three species.
    *   **Key Technologies:** Python, TensorFlow, Keras, NumPy, Pandas, Matplotlib, Seaborn, Scikit-learn.
    *   **View Project:** [`./MLP_Tensorflow/README.md`](./MLP_Tensorflow/README.md)

6.  **[🚢 Optimisers Comparison (Titanic Dataset)](./Optimisers/)**
    *   **Description:** Explores the performance of various neural network optimizers (SGD, Adam, RMSprop, etc.) and learning rate schedules on the Titanic survival prediction task.
    *   **Key Technologies:** Python, TensorFlow, Keras, Pandas, NumPy.
    *   **View Project:** [`./Optimisers/README.md`](./Optimisers/README.md)

7.  **[📩 Recurrent Neural Network (SMS Spam Detection)](./Recurrent%20Neural%20Network/)**
    *   **Description:** A deep learning-based SMS spam classifier built using a Recurrent Neural Network (RNN) model with TensorFlow and Keras.
    *   **Key Technologies:** Python, TensorFlow, Keras, Pandas, Matplotlib.
    *   **View Project:** [`./Recurrent Neural Network/Readme.md`](./Recurrent%20Neural%20Network/Readme.md)

8.  **[🔌 Logic Gate Perceptron Implementations](./logic_gate_perceptron/)**
    *   **Description:** Demonstrates Perceptron algorithm implementations for logic gates (AND, OR) and binary classification on the Iris dataset using three methods: hardcoded Python, TensorFlow/Keras, and Scikit-learn.
    *   **Key Technologies:** Python, NumPy, Matplotlib, TensorFlow, Keras, Scikit-learn.
    *   **View Project:** [`./logic_gate_perceptron/README.md`](./logic_gate_perceptron/README.md)
  
9.  **[🧠 Autoencoder for Image Denoising](./autoencoder/)**
    *   **Description:** Trains both Dense and Convolutional Autoencoders using TensorFlow to remove noise from CIFAR-10 images, demonstrating feature compression and reconstruction.
    *   **Key Technologies:** Python, TensorFlow, Keras, NumPy, Matplotlib.
    *   **View Project:** [`./autoencoder/README.md`](./autoencoder/README.md)


## 🧰 General Technologies Used Across Projects

Most projects leverage the following Python libraries:
- 🐍 **Python 3.x**
- 🔁 **TensorFlow & Keras** – for building and training neural networks
- 📊 **Scikit-learn** – for utility functions, models, and metrics
- 🧮 **Pandas** – for data manipulation
- 🔢 **NumPy** – for numerical operations
- 📈 **Matplotlib & Seaborn** – for visualizations

## ⚙️ Installation

Each project directory contains its own `README.md` with specific setup instructions and a list of dependencies. Generally, you will need Python and can install packages using `pip`:

```bash
pip install tensorflow pandas numpy matplotlib seaborn scikit-learn jupyter
```

Refer to the individual project READMEs for more precise requirements (e.g., the `Recurrent Neural Network` project has a `requirements.txt`).

## ▶️ Usage

1.  Clone this repository:
    ```bash
    git clone https://github.com/sajeev-k22/Neural-Networks-and-Deep-Learning.git
    cd Neural-Networks-and-Deep-Learning
    ```
2.  Navigate to the specific project directory you are interested in:
    ```bash
    cd "Project Name/"
    ```
3.  Follow the instructions in that project's `README.md` file.

## 🤝 Contributing

This repository is primarily a collection of individual projects. If you find issues or have suggestions for a specific project:

1.  Navigate to the project's directory.
2.  If appropriate, raise an issue related to that specific project.
3.  For broader suggestions about the collection, raise an issue in the main repository.

### 🛠️ To Add a New Project:

1.  Fork the project.
2.  Create a feature branch: `git checkout -b feature/NewAmazingProject`
3.  Add your project in a new sub-directory, including a `README.md`
4.  Update this main `README.md` to include a link and description.
5.  Commit your changes: `git commit -m 'Add some AmazingProject'`
6.  Push to the branch: `git push origin feature/NewAmazingProject`
7.  Open a Pull Request.
