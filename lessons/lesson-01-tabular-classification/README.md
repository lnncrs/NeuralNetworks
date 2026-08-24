# Aula 1 - Classificação tabular com MLP

[English](README.en.md)

Nesta aula, um conjunto de atributos numéricos de tumores de mama é usado para apresentar o fluxo completo de um problema de classificação com uma rede neural simples.

## Objetivos

- preparar e explorar dados tabulares;
- separar treino, validação e teste sem vazamento de dados;
- normalizar as entradas usando somente o conjunto de treino;
- entender neurônios, camadas, ativações, logits, loss e backpropagation;
- treinar e avaliar uma MLP;
- comparar a rede neural com um baseline de regressão logística;
- salvar um checkpoint reutilizável.

## Ordem de execução

1. [Preparação dos dados](01-prepare-data.pt-br.ipynb)
2. [Classificador MLP](02-simple-mlp-classifier.pt-br.ipynb)

O primeiro notebook cria `data/breast_cancer.parquet`. O segundo salva o modelo treinado em `outputs/lesson-01/simple-mlp-classifier.pt`.

O checkpoint contém os pesos, a ordem das features, os nomes das classes e os parâmetros do `StandardScaler`, necessários para reproduzir a preparação das entradas durante a inferência.
