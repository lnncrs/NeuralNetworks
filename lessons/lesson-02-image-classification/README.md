# Aula 2 — Classificação de imagens com CNN e ResNet

Nesta aula, o mesmo fluxo de classificação é ampliado para imagens de ressonância magnética. Primeiro construímos uma CNN pequena e legível; depois usamos uma ResNet-18 para introduzir conexões residuais e transferência de aprendizado.

## Objetivos

- representar e inspecionar imagens como tensores;
- criar divisões estratificadas de treino, validação e teste;
- entender convolução, canais, ReLU e pooling;
- implementar e treinar uma CNN simples;
- entender blocos residuais e o problema de redes profundas;
- usar uma ResNet-18 pré-treinada com transferência de aprendizado;
- comparar os modelos com métricas adequadas a classes desbalanceadas;
- discutir limitações do conjunto de dados e do experimento.

## Ordem de execução

1. [Preparação das imagens](01-prepare-images.pt-br.ipynb)
2. [Classificadores CNN e ResNet](02-cnn-resnet-classifier.pt-br.ipynb)

O primeiro notebook cria `data/alzheimer_mri_manifest.csv`. O segundo salva os melhores pesos de cada etapa em `outputs/lesson-02/`.

Esta aula tem finalidade exclusivamente didática. Os modelos e resultados não devem ser interpretados como ferramentas de diagnóstico médico.
