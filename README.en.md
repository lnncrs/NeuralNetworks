# Neural networks

[Português](README.md)

This repository contains practical, educational lessons on neural network architectures and classification with PyTorch. Lesson content is available in both Portuguese and English, while folder and file names remain in English to keep the technical structure consistent.

## Environment setup with uv

The project supports Windows and Ubuntu on x86-64 with Python 3.13. `uv` creates the local `.venv` environment, installs Python when necessary, and reproduces the versions recorded in `uv.lock`.

Choose only one of the PyTorch profiles.

### CPU

This is the most portable option and does not require an NVIDIA GPU:

```bash
uv sync --extra cpu
uv run --extra cpu jupyter lab
```

### NVIDIA GPU with CUDA 13.2

Use this profile on Windows or Ubuntu when the installed NVIDIA driver is compatible with CUDA 13.2:

```bash
uv sync --extra cu132
uv run --extra cu132 jupyter lab
```

The `cpu` and `cu132` profiles are mutually exclusive. To switch profiles, run `uv sync` again with the desired extra.

## Lessons

### Lesson 1 - Tabular classification with an MLP

1. [Data preparation](lessons/lesson-01-tabular-classification/01-prepare-data.en.ipynb)
2. [MLP classifier](lessons/lesson-01-tabular-classification/02-simple-mlp-classifier.en.ipynb)

See the [Lesson 1 guide](lessons/lesson-01-tabular-classification/README.en.md) for its objectives and expected outcomes.

### Lesson 2 - Image classification with CNNs and ResNets

1. [Image preparation](lessons/lesson-02-image-classification/01-prepare-images.en.ipynb)
2. [CNN and ResNet classifiers](lessons/lesson-02-image-classification/02-cnn-resnet-classifier.en.ipynb)

See the [Lesson 2 guide](lessons/lesson-02-image-classification/README.en.md) for its objectives and expected outcomes.

## Auxiliary tools

The [Device detection](tools/detect-device.ipynb) notebook quickly checks whether PyTorch is using CPU, CUDA, or MPS. It is an optional tool and is not part of the lesson sequence.

## Supplementary materials

Earlier English versions and the BERT fine-tuning material remain under `archive/`.

The `environment.yml` and `requirements.txt` files remain available as legacy alternatives. For this project, the `uv` environment is recommended.
