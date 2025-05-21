# TanH_function_and_Derivative
# 🔍 Understanding the `tanh` Activation Function in Deep Learning

## 📘 Overview

The **hyperbolic tangent function**, commonly known as **`tanh`**, is a widely used activation function in neural networks. It introduces non-linearity to the model while maintaining a **zero-centered** output, making it more efficient than sigmoid in many learning scenarios.

---

## 📐 Mathematical Definition

The `tanh` function is defined as:

\[
\tanh(x) = \frac{e^x - e^{-x}}{e^x + e^{-x}}
\]

It transforms input values to a range between **-1 and 1**, which helps stabilize and speed up the training of models.

---

## 🧮 Derivative of Tanh

The derivative is useful in backpropagation to compute gradients:

\[
\frac{d}{dx} \tanh(x) = 1 - \tanh^2(x)
\]

This simple derivative allows efficient gradient computation in deep learning models.

---

## ✅ Why Use `tanh`?

| Advantage                         | Explanation                                      |
|----------------------------------|--------------------------------------------------|
| **Zero-centered output**         | Helps with faster convergence during training.   |
| **Smooth gradient**              | Useful for gradient-based optimization.          |
| **Non-linear**                   | Allows learning complex patterns.                |
| **Better than sigmoid**          | Outputs range from -1 to 1 instead of 0 to 1.    |

---

## 📍 When to Use

- In **hidden layers** of a neural network (not in the output layer).
- When your model benefits from **zero-centered** activations.
- Good in **RNNs** and **MLPs** for continuous input data.

---
