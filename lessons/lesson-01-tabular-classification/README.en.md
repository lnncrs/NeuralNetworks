# Lesson 1 - Tabular classification with an MLP

[Português](README.md)

In this lesson, a set of numeric breast tumor attributes is used to introduce the complete workflow of a classification problem with a simple neural network.

## Objectives

- prepare and explore tabular data;
- create training, validation, and test splits without data leakage;
- normalize inputs using only the training set;
- understand neurons, layers, activations, logits, loss, and backpropagation;
- train and evaluate an MLP;
- compare the neural network with a logistic regression baseline;
- save a reusable checkpoint.

## Execution order

1. [Data preparation](01-prepare-data.en.ipynb)
2. [MLP classifier](02-simple-mlp-classifier.en.ipynb)

The first notebook creates `data/breast_cancer.parquet`. The second saves the trained model to `outputs/lesson-01/simple-mlp-classifier.pt`.

The checkpoint contains the weights, feature order, class names, and `StandardScaler` parameters required to reproduce input preparation during inference.
