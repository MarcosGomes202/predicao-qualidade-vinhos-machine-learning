# 🍷 Predição da Qualidade de Vinhos com Machine Learning

Projeto acadêmico desenvolvido para análise e predição da qualidade de vinhos utilizando técnicas de **Machine Learning**, com base em características físico-químicas presentes no dataset.

## 📌 Objetivo do Projeto

Este projeto tem como objetivo prever a **qualidade de vinhos tintos e brancos** a partir de atributos químicos e físicos, utilizando diferentes algoritmos de aprendizado de máquina e comparando seus desempenhos.

A principal pergunta investigada foi:

> É possível prever a qualidade de um vinho utilizando apenas seus atributos químicos e físicos?

---

## 📊 Base de Dados

A base utilizada é uma versão combinada dos datasets de **vinhos tintos e brancos** disponibilizados pelo **UCI Machine Learning Repository**.

### Informações da base:
- **6.497 registros originais**
- **1.177 registros duplicados removidos**
- **5.320 registros finais**
- **13 variáveis**

### Principais atributos analisados:
- Fixed Acidity
- Volatile Acidity
- Citric Acid
- Residual Sugar
- Chlorides
- Free Sulfur Dioxide
- Total Sulfur Dioxide
- Density
- pH
- Sulphates
- Alcohol
- Type
- Quality

---

## ⚙️ Tratamento e Preparação dos Dados

Durante o desenvolvimento foram realizadas etapas de pré-processamento para melhorar a qualidade dos dados:

✔️ Remoção de registros duplicados  
✔️ Verificação de valores nulos  
✔️ Padronização dos dados com `StandardScaler`  
✔️ Análise de outliers com boxplots  
✔️ Separação entre variáveis independentes (**features**) e variável alvo (**target**)  
✔️ Divisão entre treino e teste utilizando `train_test_split`

---

## 🤖 Algoritmos Utilizados

### Modelos de Classificação
- Regressão Logística
- k-Nearest Neighbors (kNN)
- Decision Tree Classifier
- Random Forest Classifier

### Modelos de Regressão
- Regressão Linear
- Decision Tree Regressor
- Random Forest Regressor

---

## 📏 Métricas Utilizadas

### Classificação
- Accuracy
- Classification Report
- Confusion Matrix

### Regressão
- MSE (Mean Squared)
- RMSE (Root Mean Squared)
- R² Score

---

## 📈 Resultados Obtidos

### Modelos de Classificação

| Algoritmo | Accuracy |
|------------|------------|
| Regressão Logística | 0.5499 |
| kNN | 0.5019 |
| DecisionTreeClassifier | 0.4812 |
| RandomForestClassifier | **0.5808** |

### Modelos de Regressão

| Algoritmo | MSE | RMSE | R² |
|------------|------------|------------|------------|
| Regressão Linear | 0.5247 | 0.7243 | 0.3013 |
| DecisionTreeRegressor | 0.9023 | 0.9499 | -0.2016 |
| RandomForestRegressor | **0.4243** | **0.6514** | **0.4350** |

### Principais conclusões
- O **Random Forest Classifier** apresentou a melhor acurácia entre os modelos de classificação.
- O **Random Forest Regressor** apresentou melhor desempenho nos modelos de regressão.
- Os resultados demonstram que é possível prever a qualidade do vinho utilizando características físico-químicas.

---

## 🛠️ Tecnologias Utilizadas

- Python
- Google Colab
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-Learn

---

## 📂 Estrutura do Projeto

```bash
📁 projeto-vinhos-machine-learning
│── 📄 README.md
│── 📄 relatorio.docx
│── 📓 notebook_vinhos.ipynb
│── 📁 wine_quality_dataset.csv
```

---

## 👨‍💻 Autor

**Marcos Gomes**  
Graduando em **Ciência da Computação**  
Interesse em **Dados, Machine Learning e Tecnologia**
