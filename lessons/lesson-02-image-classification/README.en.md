# Lesson 2 - Image classification with CNNs and ResNets

[Português](README.md)

In this lesson, the same classification workflow is extended to magnetic resonance images. We first build a small, readable CNN; then use ResNet-18 and ResNet-50 to introduce residual connections, transfer learning, and the trade-offs between model capacity and computational cost.

## Objectives

- represent and inspect images as tensors;
- create stratified training, validation, and test splits;
- understand convolution, channels, ReLU, and pooling;
- implement and train a simple CNN;
- understand residual blocks and the challenges of deep networks;
- use pretrained ResNet-18 and ResNet-50 models with transfer learning;
- distinguish fixed feature extraction from fine-tuning;
- compare the models with metrics suitable for multiclass classification;
- discuss limitations of the dataset and experiment.

## Execution order

1. [Image preparation](01-prepare-images.en.ipynb)
2. [CNN and ResNet classifiers](02-cnn-resnet-classifier.en.ipynb)

The first notebook creates `data/alzheimer_mri_manifest.csv`. The second saves the best weights from each stage under `outputs/lesson-02/`.

This lesson is intended exclusively for educational purposes. The models and results must not be interpreted as medical diagnostic tools.
