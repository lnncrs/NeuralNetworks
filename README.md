# Redes neurais

[English](README.en.md)

Este repositório reúne aulas práticas e didáticas sobre arquiteturas de redes neurais e classificação com PyTorch. O conteúdo das aulas está disponível em português e inglês; os nomes de pastas e arquivos permanecem em inglês para manter uma estrutura técnica consistente.

## Preparação do ambiente com uv

O projeto suporta Windows e Ubuntu em x86-64 com Python 3.13. O `uv` cria o ambiente local `.venv`, instala o Python quando necessário e reproduz as versões registradas em `uv.lock`.

Escolha somente um dos perfis do PyTorch.

### CPU

É a opção mais portátil e não exige uma GPU NVIDIA:

```bash
uv sync --extra cpu
uv run --extra cpu jupyter lab
```

### GPU NVIDIA com CUDA 13.2

Use este perfil no Windows ou Ubuntu quando o driver NVIDIA instalado for compatível com CUDA 13.2:

```bash
uv sync --extra cu132
uv run --extra cu132 jupyter lab
```

Os perfis `cpu` e `cu132` são mutuamente exclusivos. Para trocar de perfil, execute novamente `uv sync` com o extra desejado.

## Aulas

### Aula 1 - Classificação tabular com MLP

1. [Preparação dos dados](lessons/lesson-01-tabular-classification/01-prepare-data.pt-br.ipynb)
2. [Classificador MLP](lessons/lesson-01-tabular-classification/02-simple-mlp-classifier.pt-br.ipynb)

Consulte o [guia da Aula 1](lessons/lesson-01-tabular-classification/README.md) para os objetivos e resultados esperados.

### Aula 2 - Classificação de imagens com CNN e ResNet

1. [Preparação das imagens](lessons/lesson-02-image-classification/01-prepare-images.pt-br.ipynb)
2. [Classificadores CNN e ResNet](lessons/lesson-02-image-classification/02-cnn-resnet-classifier.pt-br.ipynb)

Consulte o [guia da Aula 2](lessons/lesson-02-image-classification/README.md) para os objetivos e resultados esperados.

## Ferramentas auxiliares

O notebook [Detecção de dispositivo](tools/detect-device.ipynb) verifica rapidamente se o PyTorch está usando CPU, CUDA ou MPS. Ele é uma ferramenta opcional e não faz parte da sequência das aulas.

## Materiais complementares

Versões anteriores em inglês e o material de fine-tuning com BERT permanecem em `archive/`.

Os arquivos `environment.yml` e `requirements.txt` continuam disponíveis como alternativas legadas. Para este projeto, o ambiente com `uv` é o recomendado.
