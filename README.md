# XOR Problem — Neural Network Implementation

> ⚠️ **Note:** The notebook content (`XOR_problem.ipynb`) is written in **Spanish**.
> This README is provided in **English** for international understanding and documentation purposes.

---

## 🧠 Overview

This project demonstrates how a **feedforward neural network** learns the classical **XOR (exclusive OR)** logical problem — a fundamental non-linearly separable task that played a key role in the historical development of neural networks.

The notebook explores the **mathematical foundations**, **forward pass computation**, and **training process** required for a network to correctly classify XOR outputs.

---

## 🔍 Problem Definition

The XOR (exclusive OR) operation follows this logic:

| Input (x₁) | Input (x₂) | Output (y) |
| ---------- | ---------- | ---------- |
| 0          | 0          | 0          |
| 0          | 1          | 1          |
| 1          | 0          | 1          |
| 1          | 1          | 0          |

Unlike linearly separable problems (e.g., AND, OR), XOR cannot be solved by a single perceptron.
It requires at least **one hidden layer** with nonlinear activation functions.

---

## ⚙️ Mathematical Background

Let the neural network be a **Multilayer Perceptron (MLP)** with:

* **Input layer:** 2 neurons (x₁, x₂)
* **Hidden layer:** 2 neurons (h₁, h₂)
* **Output layer:** 1 neuron (ŷ)

### Forward Pass Equations

1. **Hidden layer computation:**

$$
[
h = f(W^{(1)}x + b^{(1)})
]
$$

2. **Output layer computation:**

$$
[
\hat{y} = f(W^{(2)}h + b^{(2)})
]
$$

where (f) is a nonlinear activation function (commonly **sigmoid** or **ReLU**).

The model is trained using **gradient descent** to minimize the **mean squared error (MSE)** or **binary cross-entropy** loss.

---

## 🧩 Notebook Content (in Spanish)

Inside the notebook, you’ll find:

1. **Mathematical explanation** of forward propagation.
2. **Implementation of weight initialization**, activation functions, and loss calculation.
3. **Step-by-step training process** for the XOR dataset.
4. **Visualization of results** showing how the model converges.
5. **Corrections and derivations** on matrix operations and activation behavior.

---

## 💡 Key Concepts Covered

* Linear vs Nonlinear separability
* Activation functions (Sigmoid, ReLU, Tanh)
* Forward pass and backpropagation
* Gradient-based optimization
* Role of bias and weight matrices
* Error correction over epochs

---

## 🧰 Requirements

This notebook uses Python 3 and standard machine learning libraries:

```bash
pip install numpy matplotlib
```

(Optional) To run it interactively:

```bash
pip install jupyterlab
```

---

## ▶️ How to Run

1. Clone or download this repository.
2. Open the notebook:

```bash
jupyter notebook XOR_problem.ipynb
```

3. Run all cells sequentially.
4. Observe how the network learns to model the XOR relationship.

---

## 🧾 License

This project is open-source under the **MIT License**.
You are free to modify, distribute, and use it for educational purposes.
