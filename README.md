
# Machine Learning: Exercícios de Classificação e Regressão
 
Este projeto apresenta dois exercícios práticos de Machine Learning, desenvolvidos para fins educativos, usando Python, scikit-learn e Keras/TensorFlow. Cada exercício aborda um dos problemas mais comuns em ML: classificação e regressão. A seguir estão descrições breves de cada experimento, os códigos implementados e a análise dos resultados obtidos.
 
---

## Integrantes
Turma: 2TDSPF
- Julia Vasconcelos Oliveira | RM558785
- Matheus de Freitas | RM552602
- Gustavo de Aguiar | 557707
 
## Exercício 1: Classificação de Vinhos (UCI Wine Dataset)
 
**Objetivo:** Treinar modelos para classificar amostras de vinho em três classes distintas, com base em 13 atributos químicos.
 
**Modelos utilizados:**
- Rede Neural (Keras): 2 camadas ocultas (32 neurônios cada, ativação ReLU), saída softmax (3 neurônios).
- RandomForestClassifier (scikit-learn)
- LogisticRegression (scikit-learn)
 
**Resumo dos passos:**
1. Carregamento do dataset wine.data.
2. Padronização dos dados (StandardScaler).
3. Treinamento dos três modelos.
4. Comparação das acurácias no conjunto de teste.
 
**Resultados:**
 
| Modelo                   | Acurácia     |
|--------------------------|-------------|
| Rede Neural (Keras)      | ~0.97       |
| RandomForestClassifier   | ~1.00       |
| LogisticRegression       | ~0.97       |
 
> *O RandomForest obteve acurácia perfeita, sendo levemente superior à rede neural e à regressão logística neste conjunto de dados tabular e bem comportado.*
 
---
 
## Exercício 2: Regressão do Valor de Casas (California Housing Dataset)
 
**Objetivo:** Prever o valor médio de casas na Califórnia a partir de 8 atributos geográficos e demográficos.
 
**Modelos utilizados:**
- Rede Neural (Keras): 3 camadas ocultas (64, 32, 16 neurônios; ativação ReLU), saída linear (1 neurônio).
- LinearRegression (scikit-learn)
- RandomForestRegressor (scikit-learn)
 
**Resumo dos passos:**
1. Download do dataset via fetch_california_housing().
2. Padronização dos dados (StandardScaler).
3. Treinamento dos três modelos.
4. Cálculo das métricas MAE (Mean Absolute Error) e RMSE (Root Mean Squared Error).
 
**Resultados:**
 
| Modelo                  | MAE (aprox.) | RMSE (aprox.) |
|-------------------------|--------------|---------------|
| Rede Neural (Keras)     | ~0.33        | ~0.52         |
| LinearRegression        | ~0.52        | ~0.73         |
| RandomForestRegressor   | ~0.33        | ~0.51         |
 
> *RandomForestRegressor e Rede Neural apresentam desempenho semelhante e melhor que o modelo linear.*
 
---
