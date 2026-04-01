### **Previsão de Propensão a Compra de Carros: Uma Análise Comparativa entre SVM e XGBoost**

Este projeto visa construir e avaliar modelos de Machine Learning para prever a propensão de clientes a comprar um carro, utilizando características demográficas como idade e salário anual. Realizamos uma análise comparativa entre modelos Support Vector Machine (SVM) com diferentes kernels e um modelo XGBoost para identificar a abordagem mais eficaz.

### **Conteúdo**

*   **`CARRO_CLIENTES.csv`**: Conjunto de dados utilizado para treinamento e teste.
*   `previsao_compra_carros_svm.ipynb`: Notebook Jupyter contendo todo o processo de análise.

### **Metodologia**

1.  **Carregamento e Pré-processamento de Dados:**
    *   Carregamento do dataset `CARRO_CLIENTES.csv`.
    *   Renomeação de colunas para maior clareza (`User ID` para `id`, `Gender` para `genero`, `Age` para `idade`, `AnnualSalary` para `salario`, `Purchased` para `comprou`).
    *   Verificação de tipos de dados, valores ausentes e duplicatas.
    *   Remoção da coluna `id`, que não é relevante para o modelo preditivo.
    *   Aplicação de **Label Encoding** na coluna categórica `genero` (Male/Female para 1/0).

2.  **Análise Exploratória de Dados (EDA):**
    *   Geração de box plots para identificar outliers nas colunas numéricas (nenhum outlier significativo encontrado).
    *   Cálculo e visualização da matriz de correlação entre as variáveis numéricas. Identificação de forte correlação positiva entre `idade` e `comprou` (0.62), e correlação moderada entre `salario` e `comprou` (0.36).
    *   Visualizações gráficas (box plots e histogramas) para aprofundar a relação entre `idade`/`salario` e a variável alvo `comprou`, confirmando a idade como um preditor mais forte.

3.  **Preparação para Modelagem:**
    *   Separação das features (X) e do target (Y).
    *   Divisão do dataset em conjuntos de treino (80%) e teste (20%) usando `train_test_split`.

4.  **Treinamento e Avaliação de Modelos SVM:**
    *   **SVM com Kernel Linear:** Treinado e avaliado. Acurácia de 83.75%, com um bom balanço entre precisão e recall para ambas as classes.
    *   **SVM com Kernel Polinomial:** Treinado e avaliado. Acurácia de 75.25%, mas com um recall muito baixo (0.44) para a classe 'comprou', indicando dificuldade em identificar compradores.

5.  **Comparação com XGBoost:**
    *   Resultados de um modelo XGBoost pré-existente foram incorporados para comparação:
        *   **Acurácia:** 90.5%
        *   **Classe 0 (Não Comprou):** Precisão = 0.89, Recall = 0.95
        *   **Classe 1 (Comprou):** Precisão = 0.93, Recall = 0.85

### **Resultados e Conclusão**

O **XGBoost demonstrou ser o modelo mais robusto e eficaz** para este problema de previsão, alcançando a maior acurácia (90.5%) e apresentando métricas de precisão e recall mais elevadas e balanceadas para ambas as classes em comparação com os modelos SVM.

*   O SVM com kernel linear apresentou um desempenho razoável, sendo superior ao SVM com kernel polinomial neste contexto.
*   A arquitetura ensemble do XGBoost (gradient boosting) provou ser mais eficiente em capturar as complexidades e padrões nos dados de propensão a compra.

Este projeto destaca a importância de comparar diferentes algoritmos de Machine Learning para encontrar a melhor solução para um problema específico, com o XGBoost se mostrando o vencedor claro para prever a compra de carros com base nos dados fornecidos.

### **Tecnologias Utilizadas**

*   Python
*   `pandas` (manipulação de dados)
*   `scikit-learn` (LabelEncoder, SVC, train_test_split, classification_report, accuracy_score)
*   `matplotlib` e `seaborn` (visualização de dados)

---

## Contribuição

Contribuições são bem-vindas! Sinta-se à vontade para abrir issues ou pull requests.

---

📎 **Projeto desenvolvido por:** Diego Kaique

🔗 **LinkedIn:** [https://www.linkedin.com/in/diego-kaique-9ba3697b]

📧 **Contato:** [kaique_0208@hotmail.com]
