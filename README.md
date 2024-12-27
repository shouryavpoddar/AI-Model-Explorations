# Exploration of Learning Rate Strategies and Optimization Techniques 🚀

This project dives into the fascinating world of optimizing neural network training using various learning rate strategies and adaptive optimization techniques. By experimenting with the Iris dataset, this exploration evaluates how these methods influence training performance, convergence speed, and model accuracy.

---

## Overview

The project focuses on two major areas:
1. **Learning Rate Strategies**:
   - Constant Learning Rate (SGD)
   - Step Decay
   - Exponential Decay
   - Cyclic Learning Rate (Cyclic LR)
   - Cosine Annealing

2. **Optimization Techniques**:
   - Adam Optimizer
   - RMSprop Optimizer

### Why This Matters
Learning rate strategies and optimizers play a critical role in the success of neural networks. This project compares their effectiveness using both training loss curves and test accuracy metrics, providing insights into the most efficient methods for different scenarios.

---

## Dataset and Model Architecture

- **Dataset**: The Iris dataset, consisting of 150 samples across three flower species: Setosa, Versicolor, and Virginica.
- **Features**: Sepal length, sepal width, petal length, and petal width.
- **Model**:
  - Input Layer: 4 neurons (features)
  - Hidden Layer: 8 neurons (ReLU activation)
  - Output Layer: 3 neurons (softmax activation)

### Training Details
- **Loss Function**: Cross-Entropy Loss
- **Split**: 80-20 train-test split
- **Epochs**: 50

---

## Results

### Learning Rate Strategies
| Strategy             | Test Accuracy (%) |
|----------------------|-------------------|
| Constant LR (SGD)    | 63.33            |
| Step Decay           | 90.00            |
| Exponential Decay    | 73.33            |
| Cyclic LR            | 93.33            |
| Cosine Annealing     | 80.00            |

### Optimizers
| Optimizer            | Test Accuracy (%) |
|----------------------|-------------------|
| Adam                 | 93.33            |
| RMSprop              | 96.67            |

- **Best Performance**: RMSprop achieved the highest accuracy of 96.67%, closely followed by Adam and Cyclic LR.

### Key Visualizations
- **Training Loss Curves**: Illustrate convergence speed and stability across strategies.
- **Accuracy Bar Chart**: Highlights the comparative effectiveness of each approach.
- **Confusion Matrices**: Showcase classification performance for the Iris dataset classes.

---

## Comparative Exploration: Neural Network vs. Gaussian Mixture Model (GMM)

Additionally, this project compares a supervised neural network with an unsupervised GMM:

| Metric             | Neural Network | GMM          |
|--------------------|----------------|--------------|
| Accuracy (%)       | 96.67          | 66.67        |
| Purity (%)         | N/A            | 66.67        |
| Adjusted Rand Index| N/A            | 0.5165       |

- **Neural Network**: Achieved superior accuracy by leveraging labeled data.
- **GMM**: Struggled with overlapping class distributions but excelled for well-separated classes.

---

## Conclusions

1. **Dynamic Learning Rates**: Techniques like Cyclic LR and Step Decay significantly improve convergence over constant rates.
2. **Adaptive Optimizers**: RMSprop and Adam offer robust performance, especially for noisy gradients.
3. **Supervised vs. Unsupervised**: Neural networks outperform GMMs in classification tasks when labeled data is available.

### Future Work
- Explore hybrid strategies (e.g., combining cosine annealing with warm restarts).
- Evaluate alternative clustering methods for overlapping classes.

---

## Usage

Clone the repository and use the included Python scripts to replicate the experiments. Dependencies include PyTorch and common Python libraries like NumPy and Matplotlib.

```bash
git clone <repository-link>
cd <project-directory>
python <script-name>.py
