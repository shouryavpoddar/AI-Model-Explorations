sxp1220@case.edu
Shourya Poddar

Read Me: Machine Learning Explorations on the Iris Dataset

This document describes the machine learning explorations conducted on the Iris dataset, as outlined in the accompanying notebooks. The two primary explorations include:

1. Exploration of Learning Rate Strategies in Neural Networks:
   This includes testing various learning rate adjustment algorithms, such as constant learning rate, step decay, exponential decay, cyclic learning rates, cosine annealing, and optimizers like Adam and RMSprop.

2. Comparison of Neural Networks and Gaussian Mixture Models (GMM):
   This compares the performance of a supervised Neural Network with an unsupervised Gaussian Mixture Model (GMM) on classifying and clustering the Iris dataset.

Prerequisites

To run the notebooks, ensure the following packages and functionalities are installed in your Python environment:

- Jupyter Notebook functionality
- Scikit-learn
- PyTorch
- Matplotlib
- Pandas
- Numpy

Instructions for Running

1. Open the respective Jupyter Notebook file (learning_rate_exploration.ipynb or algorithm_comparison.ipynb) in Jupyter Notebook.
2. Ensure all required libraries are installed in the Python environment before running the notebook.
3. Cells can be run independently, but it is recommended to run them in order as some cells build upon previous results. Alternatively, the notebook can be run all at once.

Outputs and Results

For the Learning Rate Strategies Exploration:
- Each learning rate adjustment strategy is applied to a Neural Network, and the outputs include graphs of training loss and validation loss over epochs for each strategy.
- A combined graph shows the performance of all strategies, and their final accuracy values are printed for comparison.

For the Neural Network and GMM Comparison:
- The Neural Network is trained on 80% of the Iris dataset in a supervised manner, while the GMM clusters the full dataset without using labels.
- Outputs include confusion matrices for both algorithms, accuracy of the Neural Network, and clustering metrics (Purity and Adjusted Rand Index) for the GMM.

Note

Upon running the notebooks, please allow a few minutes for the training of the Neural Network models. The outputs, including confusion matrices and performance graphs, can be viewed directly in the notebook outputs once all cells have been executed successfully.

Thank you for exploring machine learning with the Iris dataset!