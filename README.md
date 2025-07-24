# Neural Network from Scratch with NumPy

This project demonstrates the implementation of a fully connected neural network from scratch using only **NumPy**, without relying on high-level deep learning frameworks like TensorFlow or PyTorch. It includes training on the **MNIST handwritten digit dataset**, achieving competitive accuracy while providing clear insights into backpropagation, gradient descent, and activation functions.

## 🔍 Project Overview

The repository contains two main implementations:
1. A **simple 3-layer neural network** (Input → Hidden → Output) to demonstrate core concepts.
2. A **generalized multi-layer neural network** that supports arbitrary architectures.

Both models are trained and evaluated on the MNIST dataset, showcasing practical understanding of deep learning fundamentals.

## 🧠 Key Concepts Implemented

- Forward and backward propagation
- ReLU and Softmax activation functions
- Cross-entropy loss
- Gradient descent optimization
- Weight initialization techniques (most of the bugs were here !)
- One-hot encoding
- Accuracy evaluation and prediction visualization

## 📊 Dataset

We use the **MNIST dataset**, consisting of 70,000 grayscale images of handwritten digits (0–9), each of size 28x28 pixels.

- Training samples: 60,000  
- Test samples: 10,000  
- Input features: 784 (28 × 28 flattened)

Data is normalized and reshaped for efficient computation. (We got it from tensorflow that's why it was like this from the start)

## 🏗️ Model Architectures

### Simple Neural Network
```
Input Layer (784) → Hidden Layer (10) → Output Layer (10)
```

### Generalized Neural Network
Supports variable depth and width, e.g.:
```
Input Layer (784) → Hidden Layer 1 (100) → Hidden Layer 2 (100) → Output Layer (10)
```

## 🚀 Results

| Model                      | Test Accuracy |
|---------------------------|---------------|
| Simple Neural Network     | ~89%          |
| Generalized Neural Network| ~87%          |

> Note: Accuracy may vary slightly depending on initialization and hyperparameters.

## 📦 Dependencies

- Python 3.x
- NumPy
- Matplotlib
- TensorFlow (only for loading MNIST data)
- Pillow (for image display)
- IPython (optional, for inline image rendering)

Install dependencies via pip:

```bash
pip install numpy matplotlib tensorflow pillow ipython
```

## 🧪 Usage

Clone the repo and run the notebook directly !!!

You can customize the architecture by modifying the `layer_sizes` parameter in the `NeuralNetwork` class constructor.

## 📈 Visualization

Predictions are visualized at the end of training, showing correctly and incorrectly classified examples with color-coded labels (`green` = correct, `red` = incorrect).

## 🤝 Contributing

Feel free to fork this repository, open issues, or submit pull requests. Any contributions are welcome!
