# Neural Networks

This repository contains implementations of various neural network architectures and algorithms.

# Environment Setup

To set up the environment for this project, you can use the provided `environment.yml` file. This file specifies the dependencies required to run the code.

To create the environment, run the following command in your terminal:

```bash
conda env create -f environment.yml
```

After the environment is created, you can activate it using:

```bash
conda activate py313g
```

To manually install the dependencies on a environment without using Conda, you can use the `requirements.txt` file:

```bash
pip install -r requirements.txt
```

To manually install the dependencies without using a requirements file, you can run the following commands in your terminal:

```bash
pip install numpy scipy pandas scikit-learn jupyter statsmodels matplotlib seaborn bokeh plotly pyarrow tomli openpyxl regex python-dotenv networkx requests tqdm mlflow faker
pip install torch torchvision --index-url https://download.pytorch.org/whl/cu132
pip install transformers datasets accelerate tokenizers
```
