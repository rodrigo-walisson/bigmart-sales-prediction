# bigmart-sales-prediction
Previsão de vendas com Machine Learning — análise exploratória, limpeza de dados e regressão

# BigMart Sales Prediction

Previsão de volume de vendas de produtos em lojas de varejo 
usando Machine Learning.

## Problema de negócio

O BigMart coletou dados de vendas de 2013 em múltiplas lojas. 
O objetivo é prever o volume de vendas de cada produto em cada 
loja — permitindo otimizar estoque, reduzir desperdício e evitar 
perda de venda por falta de produto.

## Dataset

- **Fonte:** [BigMart Sales Data — Kaggle](https://www.kaggle.com/datasets/brijbhushannanda1979/bigmart-sales-data)
- **Tamanho:** 8.523 registros × 12 variáveis
- **Target:** `Item_Outlet_Sales` — volume de vendas

## Etapas do projeto

1. **Análise Exploratória (EDA)** — distribuições, correlações e padrões
2. **Limpeza de dados** — valores faltantes, inconsistências e zeros inválidos
3. **Feature Engineering** — criação de 3 novas variáveis
4. **Modelagem** — Regressão Linear (baseline) e Random Forest
5. **Avaliação** — comparativo de métricas e análise visual dos erros

## Resultados

| Modelo | R² | RMSE | MAE |
|---|---|---|---|
| Regressão Linear | 0.4952 | 1.171 | 818 |
| Random Forest | 0.5773 | 1.071 | 737 |

O Random Forest superou a regressão linear em todas as métricas. 
As variáveis mais importantes foram `Outlet_Type` (52%) e 
`Item_MRP` (37%).

## Principais descobertas

- O tipo de loja é o fator mais determinante nas vendas
- Produtos mais caros geram maior volume financeiro de vendas
- O modelo erra mais em produtos com vendas acima de R$6.000

## Tecnologias

Python · Pandas · NumPy · Scikit-learn · Matplotlib · Seaborn

## Autor

**Rodrigo Walisson**  
[LinkedIn](https://www.linkedin.com/in/rodrigowalisson/) | 

