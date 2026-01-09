# 🌦️ Previsão de Temperatura com Machine Learning (XGBoost)

Este projeto consiste em um pipeline completo de Ciência de Dados para a previsão de séries temporais de temperatura (TAMB) no Rio de Janeiro. O objetivo é prever comportamentos futuros utilizando técnicas de engenharia de atributos e o algoritmo de alta performance **XGBoost**.

## 🚀 Funcionalidades e Metodologia

O projeto abrange as seguintes etapas:

* **Engenharia de Atributos (Feature Engineering):**
    * **Transformações Cíclicas:** Uso de `sin` e `cos` para representar os meses do ano, permitindo que o modelo entenda a natureza sazonal do calendário.
    * **Estatísticas Móveis:** Criação de médias móveis e desvio padrão móvel (janelas de 3 e 12 meses) para capturar tendências e volatilidade.
* **Modelagem:** Implementação do **XGBRegressor**.
    * Divisão estratégica dos dados entre treino e teste para validação de séries temporais.
* **Avaliação:**
    * Uso de métricas robustas como **R² Score** (Coeficiente de Determinação) e **MAPE** (Erro Médio Absoluto Percentual).

## 📊 Performance do Modelo

Os resultados obtidos demonstram uma alta precisão nas previsões:

| Métrica | Treino | Teste |
| :--- | :---: | :---: |
| **R² Score** (Explicação da variância) | 0.96 | **0.85** |
| **MAPE** (Erro percentual médio) | 1.50% | **2.97%** |

> **Nota:** Um R² de 0.85 na base de teste indica que o modelo consegue explicar 85% do comportamento da temperatura, com um erro médio baixíssimo de menos de 3%.

## 🛠️ Tecnologias Utilizadas

* **Linguagem:** Python 3.x
* **Manipulação de Dados:** `pandas`, `numpy`
* **Visualização:** `seaborn`, `matplotlib`
* **Machine Learning:** `xgboost`, `scikit-learn`
