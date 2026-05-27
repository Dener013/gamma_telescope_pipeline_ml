# 🔭 Esteira de Aprendizado de Máquina — MAGIC Gamma Telescope

## Descrição do Projeto

Este projeto implementa uma esteira completa de aprendizado de máquina utilizando o dataset
**MAGIC Gamma Telescope** (UCI Machine Learning Repository — ID 159).

O experimento MAGIC detecta raios gama de alta energia provenientes de fontes cósmicas,
e o objetivo é **classificar eventos** captados pelo telescópio em duas categorias:

- **g (gama)** — sinal de interesse: partícula de raio gama verdadeira
- **h (hádron)** — ruído de fundo: partícula hadrônica atmosférica

O dataset possui **19.020 amostras** e **10 atributos numéricos** que descrevem
características geométricas e de intensidade das imagens captadas pelo detector Cherenkov.

### Etapas da Esteira

| # | Etapa |
|---|---|
| 1 | Carregamento e análise exploratória do dataset |
| 2 | Estatísticas descritivas gerais |
| 3 | Transformações nas colunas (log-transform) |
| 4 | Transformações nas linhas (remoção de outliers) |
| 5 | Divisão em treino / validação / teste |
| 6 | Treinamento do modelo (Random Forest) |
| 7 | Avaliação: matriz de confusão, acurácia e AUC-ROC |
| 8 | Predição de novos eventos |

### Resultados Obtidos

| Métrica | Valor |
|---|---|
| Acurácia (validação) | ~85% |
| Acurácia (teste) | ~86% |
| AUC-ROC | ~0,91 |

---

## Como Reproduzir

### Pré-requisitos

- Conta Google (para uso do Google Colab)
- As bibliotecas abaixo (já disponíveis no Colab por padrão):
  - `numpy`, `pandas`, `matplotlib`, `seaborn`, `scikit-learn`

---
**Passo 1** — Acesse o Google Colab
```
https://colab.research.google.com
```

**Passo 2** — Faça upload do notebook
```
Arquivo → Fazer upload de notebook → selecione: magic_gamma_telescope_ml.ipynb
```

**Passo 3** — Execute todas as células em ordem
```
Menu: Ambiente de execução → Executar tudo  (Ctrl + F9)
```

---

## Referências

- Dataset: https://archive.ics.uci.edu/dataset/159/magic+gamma+telescope
