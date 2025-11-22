# Introdução
Esse projeto tem como objetivo estudar técnicas de reamostragem em um dataset desbalanceado em relação à variável alvo e seus impactos no desempenho de modelos de Aprendizado de Máquina. Em uma aplicação, frequentemente, a previsão da classe minoritária é de extrema importância, por exemplo na detecção de doenças raras, e ao não se tratar o desbalanceamento, pode-se observar uma tendência do modelo à classe majoritária. Por isso, deve-se também ajustar as métricas a se levar em consideração na avaliação de desempenho, com o fito de verificar a competência do modelo nesses casos mais raros.

A realização do projeto foi feita por 2 grupos de estudantes de Sistemas de Informação da EACH-USP no segundo semestre de 2025.

Tecnologias Usadas:
- [Python 3.14.0](https://www.python.org/)
- [Pandas](https://pandas.pydata.org/)
- [NumPy](https://numpy.org/)
- [Seaborn](https://seaborn.pydata.org/)
- [Matplotlib](https://matplotlib.org/)
- [Scikit-Learn](https://scikit-learn.org/stable/)
- [Imbalanced-Learn](https://imbalanced-learn.org/stable/)

# Etapas do Projeto
## 1
A primeira etapa consistiu em realizar a análise exploratória das colunas presentes no dataset, aplicar diferentes métodos de aprendizado de máquina para predizer a classe alvo e registrar as métricas obtidas.

Métricas utilizadas:
- Acurácia;
- Precisão;
- Recall;
- F1-Score;
- ROC-AUC.

Os modelos de AM utilizados foram os seguintes:
- [K-Nearest Neighbours](https://scikit-learn.org/stable/modules/generated/sklearn.neighbors.KNeighborsClassifier.html);
- [Regressão Logística](https://scikit-learn.org/stable/modules/generated/sklearn.linear_model.LogisticRegression.html);
- [Random Forest Classifier](https://scikit-learn.org/stable/modules/generated/sklearn.ensemble.RandomForestClassifier.html).

## 2
A segunda etapa consistiu em utilizar técnicas de reamostragem na base de dados desbalanceada, aplicar os mesmos modelos e registrar as métricas obtidas.

Técnicas de Reamostragem utilizadas:
- [Random OverSampling](https://imbalanced-learn.org/stable/references/generated/imblearn.over_sampling.RandomOverSampler.html);
- [Random UnderSampling](https://imbalanced-learn.org/stable/references/generated/imblearn.under_sampling.RandomUnderSampler.html);
- [SMOTE](https://imbalanced-learn.org/stable/references/generated/imblearn.over_sampling.SMOTE.html);
- [SMOTEENN](https://imbalanced-learn.org/stable/references/generated/imblearn.combine.SMOTEENN.html).

## 3
A terceira etapa consistiu em refletir sobre os resultados obtidos ao fim do projeto e condensar as três etapas em um relatório final. Esse relatório pode ser encontrado na pasta do respectivo grupo.

## Grupo 1
Membros:
- **[Caique Sidrão](https://www.linkedin.com/in/caique-sidr%C3%A3o/)**
- **[Gabriel Lima](https://www.linkedin.com/in/gabriel-costenaro-lima-6a5a2a356/)**
- **[Rebecka Bocci](https://www.linkedin.com/in/rebecka-bocci-domingues-399157325/)**


Dataset: [Credit Card Fraud Detection](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud)

Link para [Notebook 1](https://github.com/hype-usp/Equilibrando_Classes/blob/main/Grupo1/EquilibrandoClasses1.ipynb) e para [Notebook 2](https://github.com/hype-usp/Equilibrando_Classes/blob/main/Grupo1/EquilibrandoClasses1.ipynb).
Link para [Relatório Final](https://github.com/hype-usp/Equilibrando_Classes/blob/main/Grupo1/RelatorioFinal.pdf).

notebook-1.ipynb => Neste foram usados os métodos SMOTE, ENN e SMOTE-ENN;\
notebook-2.ipynb => Neste foram usados os métodos SMOTE, Random Oversampling e Random Undersampling.

### Tecnologias adicionais
- **[Openpyxl](https://openpyxl.readthedocs.io/en/stable/)** => criação da planilha com as métricas;
- **[OS](https://docs.python.org/3/library/os.html)** => criação de pastas.

### Métricas adicionias
- *Curva de Precisão-Recall*

Gráficos são salvos em suas devidas pastas. Além das métricas serem anotadas no aqruivo resultados.xlsx.


  /projeto\
    │\
    ├── modelos\
    │     ├── KNN \
    │     │   ├── matriz-confusao-KNN-Desbalanceado.png\
    │     │   ├── auc-roc-KNN-Desbalanceado.png\
    │     │   ├── precision-recall-KNN-Desbalanceado.png\
    │     │   ├── matriz-confusao-KNN-SMOTE.png\
    │     │   ├── auc-roc-KNN-SMOTE.png\
    │     │   ├── precision-recall-KNN-SMOTE.png\
    |     |   ├── matriz-confusao-KNN-ENN.png\
    │     │   ├── auc-roc-KNN-ENN.png\
    │     │   ├── precision-recall-KNN-ENN.png\
    |     |   ├── matriz-confusao-KNN-SOMTE-ENN.png\
    │     │   ├── auc-roc-KNN-SMOTE-ENN.png\
    │     │   └── precision-recall-KNN-SMOTE-ENN.png\
    │     └── ...\
    │\
    ├── graphics\
    │     ├── countplot.png\
    │     └── heatmap-corr.png\
    │\
    |\
    ├── resultados.xlsx\
    │\
    ├── notebook-1.ipynb\
    └── notebook-2.ipynb



## Grupo 2
Membros:
- [Enzo Brilhante](https://github.com/EnzoBMattos)
- [Rafael Lima](https://github.com/0Lima0)

Dataset: [Telco Customer Churn](https://www.kaggle.com/datasets/blastchar/telco-customer-churn)

A variável alvo desse dataset foi 'Churn' que indica se o cliente cancelou ou não serviço com a empresa. 74% das linhas do dataset apontavam essa classe como falsa, caracterizando o desbalanceamento.

Link para [Notebook](https://github.com/hype-usp/Equilibrando_Classes/blob/main/Grupo2/EquilibrandoClasses2.ipynb)
Link para [Relatório Final](https://github.com/hype-usp/Equilibrando_Classes/blob/main/Grupo2/RelatorioFinal.pdf)

(Referências podem ser encontradas no relatório final)
