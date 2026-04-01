# 🚀 Previsão de Propensão à Compra de Carros

Este projeto aplica técnicas de Machine Learning para prever a probabilidade de um cliente comprar um carro, utilizando variáveis demográficas como idade e salário.

Foram desenvolvidos e comparados modelos de classificação, incluindo Support Vector Machines e XGBoost, com foco em identificar a abordagem mais eficaz e gerar insights acionáveis para o negócio.

## 🎯 Problema de Negócio

Empresas do setor automotivo precisam otimizar seus esforços de marketing e vendas, priorizando clientes com maior probabilidade de conversão.

Este projeto busca responder:

*   Quais clientes têm maior propensão a comprar um carro?

## ⚙️ Abordagem

*   Pré-processamento de dados (tratamento de variáveis e encoding)
*   Análise exploratória (EDA) para identificação de padrões
*   Treinamento de modelos:
    *   SVM (kernel linear e polinomial)
    *   XGBoost
*   Avaliação com métricas de classificação (accuracy, precision, recall)

## 📊 Resultados

| Modelo            | Acurácia |
| :---------------- | :------- |
| SVM (Linear)      | 83.75%   |
| SVM (Polinomial)  | 75.25%   |
| XGBoost           | 90.5%    |

👉 O modelo XGBoost apresentou o melhor desempenho geral, com maior equilíbrio entre precisão e recall.

## 🧠 Insights de Negócio

*   Idade é o principal fator preditivo de compra
*   Clientes em faixas etárias específicas apresentam maior propensão
*   Possível otimização de campanhas com:
    *   segmentação mais eficiente
    *   redução de custo de aquisição
    *   foco em leads qualificados

## 🛠️ Tecnologias

*   Python
*   Pandas
*   Scikit-learn
*   Matplotlib / Seaborn

## 📌 Próximos Passos (DIFERENCIAL 🔥)

*   Implementar validação cruzada
*   Realizar tuning de hiperparâmetros
*   Adicionar novas variáveis ao modelo
*   Testar pipelines de produção

## 👨‍💻 Autor

Diego Kaique
[LinkedIn](https://www.linkedin.com/in/diego-kaique-9ba3697b)
```
