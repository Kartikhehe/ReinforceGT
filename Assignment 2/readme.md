## Analysis: Effect of Hidden Layer Size on Neural Network Accuracy

In this experiment, we trained a neural network with **one hidden layer** of varying sizes to classify a **non-linearly separable dataset** (the flower-shaped planar dataset). Our goal is to observe how the number of neurons in the hidden layer affects the model's ability to learn the decision boundary and improve classification accuracy.

We compared performance across different hidden layer sizes and recorded the final training accuracy for each.

---

### 🔢 Results Summary

| Hidden Layer Size | Accuracy (%) | Comments |
|-------------------|--------------|----------|
| 1                 | 67.25        | Very low — too simple to model the flower-shaped decision boundary |
| 2                 | 65.5         | Still underfitting — not expressive enough |
| 3                 | 89.25        | Huge jump — starting to capture non-linear patterns |
| 4                 | 89.75        | Slightly better — enough to fit the complex boundary |
| 5                 | 89.0         | Plateauing — performance stabilizes |
| 20                | 89.5         | No real gain — possibly over-parameterized |
| 50                | 89.5         | Same as above — more complexity doesn’t help |

---

### ✅ Key Insights

- **Small hidden layers (1–2 units)** can't model the complex, non-linear boundary → **underfitting** occurs.
- **Medium hidden layers (3–5 units)** offer **best performance** with low cost and high accuracy → model fits well.
- **Large hidden layers (20–50 units)** don’t improve accuracy and risk **overfitting** with limited data.

---

### 📈 Final Thoughts

- A hidden layer of **3 to 5 neurons** appears optimal for this dataset.
- This experiment highlights the classic tradeoff in neural network design:
  - Too few neurons → **Underfitting**
  - Too many neurons → **Overfitting** and increased computation
- It also shows the **advantage of neural networks over logistic regression** in capturing **non-linear decision boundaries**.
