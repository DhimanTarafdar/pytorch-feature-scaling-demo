# PyTorch Feature Scaling Demo

A simple project that shows **why feature scaling matters** when training a neural network.

---

## What this project does

- Loads the **Social Network Ads** dataset
- Trains a small neural network **without scaling** → poor accuracy (~60%)
- Trains the same network **with scaling** (StandardScaler) → much better accuracy (~85%)
- Plots validation accuracy for both cases so you can see the difference clearly

---

## Dataset

**Social Network Ads** — predicts whether a user will purchase a product based on:
- Age
- Estimated Salary

---

## Model

- 2-layer feedforward neural network
- Input → Hidden (128 neurons, ReLU) → Output (Sigmoid)
- Loss: Binary Cross Entropy
- Optimizer: Adam (lr = 0.001)
- Epochs: 100

---

## Key Takeaway

| | Validation Accuracy |
|---|---|
| Without Scaling | ~60% (model barely learns) |
| With Scaling | ~85% (model learns well) |

> Feature scaling helps the model converge faster and perform better.

---

## How to run

1. Open the `.ipynb` file in **Google Colab** or **Jupyter Notebook**
2. Upload `Social_Network_Ads.csv`
3. Run all cells in order

---

## Requirements

```
torch
numpy
pandas
scikit-learn
matplotlib
```
