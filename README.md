# Análise de Viés em Machine Learning aplicado ao Marketing Bancário

Trabalho desenvolvido para a disciplina de Aprendizado de Máquina do 
curso de Desenvolvimento de Software Multiplataforma da FATEC.

## Descrição

Este projeto analisa o viés algorítmico em modelos de machine learning 
aplicados ao marketing bancário, comparando dois datasets com contextos 
distintos: um de aquisição de clientes (Portugal) e outro de retenção 
(churn europeu). Foram treinados três modelos de classificação e 
avaliados tanto por métricas de desempenho quanto por métricas de 
fairness como o Disparate Impact.

## Datasets

Os datasets não estão incluídos neste repositório e devem ser baixados 
diretamente no Kaggle:

- **Bank Marketing Dataset (Portugal):** https://www.kaggle.com/datasets/henriqueyamahata/bank-marketing
- **Bank Customer Churn Dataset:** https://www.kaggle.com/datasets/adammaus/predicting-churn-for-bank-customers

Após baixar, coloque os arquivos na pasta `dados/` seguindo essa estrutura:

dados/
├── Bank Marketing/
│   └── bank-additional-full.csv
└── Churn/
└── Churn_Modelling.csv

## Modelos Utilizados

- Regressão Logística
- Árvore de Decisão
- Random Forest

## Métricas de Avaliação

- Acurácia
- F1-Score
- ROC-AUC
- Disparate Impact

## Resultados

Os três modelos apresentaram discriminação significativa nos dois 
datasets, com Disparate Impact abaixo de 0,8 em todos os grupos 
analisados:

- **Portugal — Idade (41-50 vs 60+):** 0,081
- **Churn — Gênero (H vs M):** 0,609
- **Churn — Geografia (França vs Alemanha):** 0,335

## Bibliotecas necessárias

```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

## Como executar

1. Clone o repositório
2. Baixe os datasets e coloque na pasta `dados/`
3. Abra o arquivo `notebooks/analise.ipynb` no VS Code ou Jupyter
4. Execute as células em ordem

## Autor

Alessandro Vinicius Rodrigues Costa
FATEC — Desenvolvimento de Software Multiplataforma
