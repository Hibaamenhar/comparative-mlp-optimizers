
# Comparative Study of Optimization Algorithms for Training a Multilayer Perceptron (MLP)

This repository presents a detailed comparative analysis of various optimization algorithms applied to the training of a Multilayer Perceptron (MLP) for binary classification using the non-linearly separable `make_moons` dataset.

## 📚 Overview

This project implements the following optimizers **from scratch** using pure NumPy:

- Gradient Descent (GD)
- Stochastic Gradient Descent (SGD)
- Momentum
- Nesterov Accelerated Gradient (NAG)
- AdaGrad
- RMSprop
- Adam
- BFGS (Quasi-Newton Method)
- Conjugate Gradient (CG)

Each optimizer is tested on the same MLP architecture, and performance is compared using:
- Accuracy on clean and noisy datasets
- Loss evolution over epochs
- Convergence speed

---

## 🧠 MLP Architecture

- **Input layer:** 2 neurons (features from `make_moons`)
- **Hidden layer:** 10 neurons, ReLU activation
- **Output layer:** 1 neuron, Sigmoid activation
- **Loss function:** Binary Cross-Entropy
- **Metric:** Accuracy

---

## 🗃 Dataset

We use the `make_moons` dataset from `sklearn.datasets`:
```python
from sklearn.datasets import make_moons
```
- Samples: 1000
- Noise: 0.1 (clean) and 0.3 (noisy)

Data is standardized using `StandardScaler`.

---

## 📊 Results Summary

| Optimizer         | Accuracy (%) |
|------------------|--------------|
| SGD              | 100.0        |
| Momentum         | 100.0        |
| Nesterov         | 100.0        |
| Adam             | 100.0        |
| AdaGrad          | 96.0         |
| RMSprop          | 100.0        |
| BFGS             | 99.5         |
| Conjugate Gradient (CG) | 89.0  |
| GD (clean)       | 90.0         |
| GD (noisy)       | 82.0         |

---

## 📈 Visualizations

- Loss curve for each optimizer over 2000 epochs
- Accuracy comparisons on bar charts
- Tables summarizing convergence speed and final loss

---

## 🛠 How to Run

1. Clone the repo:
```bash
git clone https://github.com/Hibaamenhar/comparative-mlp-optimizers
cd comparative-mlp-optimizers
```

2. Run the notebook:
Open `TP_optimiseurs_final.ipynb` in Jupyter Notebook or VSCode.

---

## 📄 License

MIT License

---

## 👩‍💻 Author

- **Hiba Amenhar**
- Master IAA, 2024–2025
- Supervisor: Prof. A. Hadri
