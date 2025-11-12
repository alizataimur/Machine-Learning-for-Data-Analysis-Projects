# Gradient Descent Comparison on Neural Networks

## Project Overview

This project demonstrates the implementation and comparison of different gradient descent methods—**Batch Gradient Descent (BGD)**, **Mini-Batch Gradient Descent (MBGD)**, and **Stochastic Gradient Descent (SGD)**—on a neural network for a non-linear classification task.

The objective is to analyze the impact of batch sizes on **convergence**, **training time**, and **model performance**.

---

## Dataset

We use a synthetic dataset generated with `sklearn.datasets.make_moons`, which creates a 2D binary classification problem with non-linear boundaries.

**Features:**
- Feature 1
- Feature 2 (2D coordinates)

**Target:**
- Binary class (0 or 1)

**Dataset Stats:**
- Total samples: 445
- Training samples: 356
- Testing samples: 89

The dataset is **scaled using StandardScaler** for faster convergence.

---

## Project Highlights

### Neural Network
- 2 hidden layers with 8 neurons each, **ReLU activation**
- Output layer: 1 neuron with **Sigmoid activation** for binary classification
- Optimizer: **Stochastic Gradient Descent (SGD)** with learning rate 0.01
- Loss: **Binary Cross-Entropy**

### Gradient Descent Variants
- **BGD**: Full-batch gradient descent (batch size = training set size)
- **MBGD**: Mini-batch gradient descent (batch size = 32)
- **SGD**: Stochastic gradient descent (batch size = 1)

### Evaluation Metrics
- Training loss per epoch
- Validation accuracy per epoch
- Runtime comparison

### Visualization
- Training loss and accuracy curves
- Decision boundaries on the test set

---

## Key Results

| Method | Batch Size | Validation Accuracy | Validation Loss | Runtime (s) |
|--------|------------|------------------|----------------|------------|
| Batch Gradient Descent (BGD) | 356 | 70-75% | ~0.63 | ~10s |
| Mini-Batch Gradient Descent (MBGD) | 32 | 84-85% | ~0.35 | ~12s |
| Stochastic Gradient Descent (SGD) | 1 | 93-95% | ~0.07 | ~73s |

**Observation:** Smaller batch sizes (SGD) converge more accurately but require longer runtime, while BGD is faster but less precise for complex non-linear boundaries.

---

## Installation & Requirements

**Python Libraries:**
- numpy
- pandas
- matplotlib
- seaborn
- tensorflow
- scikit-learn
