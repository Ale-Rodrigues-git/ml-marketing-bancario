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
