# **EQUILIBRANDO CLASSES**
## *TÉCNICAS PARA TRATAR DADOS DESBALANCEADOS EM MACHINE LEARNING*

Esse repositório foi voltado para o desenvolvimento de um projeto prático para a entidade estudantil Hype. O objetivo dele foi, através de métodos de balanceamento, melhorar os resultados dos modelos.

---------------------------------------------------------
## Tecnologias
Foram usado Python com as bibliotecas: openpyxl (criar editar planilhas excel), imblearn (para os métodos de balanceamento), sklearn (para a criação dos modelos de machine learning), pandas (para abertura, leitura e análsie de base de dados), matplotlib e seaborn (para criação dos gráficos), kagglehub (importação do dataset) e os (criação e edição de pastas).

> !pip install openpyxl imblearn sklearn pandas matplotlib seaborn kagglehub os

Foi usado o dataset [Credit Card Fraud Detection (Detecção de Fraude de Cartão de Crédito)](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud?utm_source), retirado da plataforma Kaggle. Nele há dados de 284.807 transações, em que apenas 492 são fraudes, ou seja, 0,172% da base de dados inteira.

Os modelos são criados e treinados usando os dados desbalanceados e balanceados. Ainda é impresso na tela as métricas dos modelos e os gráficos de AUC-ROC e Precission-Recall.

Ademais, os gráficos são salvos nas pastas.

    /projeto
    │
    ├── modelos
    │   ├── <modelo>
    │   │   ├── matriz-confusao-<modelo>-<método>.png
    │   │   ├── auc-roc-<modelo>-<método>.png
    │   │   └── precision-recall-<modelo>-<método>.png
    │   └── ...
    │
    ├── graphics
    │   ├── countplot.png
    │   └── heatmap-corr.png
    │
    |
    ├── resultados.xlsx
    │
    ├── notebook-1.ipynb
    └── notebook-2.ipynb

Recomenda-se usar ou o ***Jupyter*** ou ***Google Colab*** para a execução do código.

Foram usado os métodos *SMOTE*, *Random Oversampling*, *Random Undersampling*, *ENN* e *SMOTE-ENN* para os testes.

De modelos, foram treinados e testados o *KNN* e *Logistic Regression*, modelo sensíveis à esses datasets, e *Random Forest*, que conseque lidar melhor, e comparados para ver suas diferenças.

notebook-1.ipynb => Neste foram usados os métodos SMOTE, ENN e SMOTE-ENN;\
notebook-2.ipynb => Neste foram usados os métodos SMOTE, Random Oversampling e Random Undersampling.


## 👤 Contribuidores

-   **[Caique Sidrão](https://www.linkedin.com/in/caique-sidr%C3%A3o/)**
-   **[Gabriel Lima](https://www.linkedin.com/in/gabriel-costenaro-lima-6a5a2a356/)**
-   **[Rebecka Bocci](https://www.linkedin.com/in/rebecka-bocci-domingues-399157325/)**


## 📜 Licença