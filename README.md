# fetch_california_housing
Modelo de regressão com objetivo de prever o preço das casas da Califórnia
# 🏡 Previsão de Preços de Casas na Califórnia

Projeto de Machine Learning com foco em regressão, utilizando o clássico dataset **California Housing** da biblioteca `scikit-learn`. O objetivo foi prever o valor médio das casas com base em variáveis demográficas e características habitacionais dos distritos californianos.

---

## 📊 Objetivo

Aplicar diferentes modelos de regressão para prever os preços das residências e **comparar seus desempenhos** com base nas seguintes métricas:

- **R² (Coeficiente de Determinação)**
- **EMA (Erro Médio Absoluto)**
- **EQM (Erro Quadrático Médio)**

---

## 📁 Dataset

- Fonte: `fetch_california_housing()` do `scikit-learn`
- 8 variáveis preditoras + 1 alvo (`MedHouseVal`)
- Inclui dados como:
  - `MedInc`: Renda média do distrito
  - `HouseAge`: Idade média das casas
  - `AveRooms`, `AveBedrms`: Cômodos e quartos médios por habitação
  - `Latitude` e `Longitude`: Localização geográfica

---

## 🧠 Modelos utilizados

- Regressão Linear Simples
- Regressão Linear Múltipla
- Árvore de Decisão
- Random Forest Regressor

---

## 🏆 Resultados

| Modelo                              | R² treino | R² teste | EMA  | EQM  |
|-------------------------------------|-----------|----------|------|------|
| **Random Forest (200 árvores)**     | 95.76%    | **68.44%** | **0.46** | **0.42** |
| Árvore de decisão (max_depth=6)     | 66.46%    | 63.52%   | 0.51 | 0.49 |
| Regressão linear (MedInc + HouseAge)| 50.65%    | 51.78%   | 0.60 | 0.65 |
| Regressão linear (MedInc)           | 47.23%    | 47.80%   | 0.63 | 0.70 |

> 🔍 **Insight**: O modelo **Random Forest** obteve o melhor desempenho geral, apresentando o maior R² e os menores erros absolutos e quadráticos, superando todos os modelos lineares e a árvore de decisão individual.

---

## 📌 Etapas do projeto

1. 📥 Importação e limpeza dos dados
2. 📊 Análise exploratória (EDA) com gráficos e estatísticas
3. 🧪 Criação e avaliação dos modelos preditivos
4. 📈 Comparação dos resultados em formato gráfico e tabular

---

## 💻 Tecnologias utilizadas

- Python
- Pandas
- Numpy
- Matplotlib & Seaborn
- Plotly
- Scikit-learn

---

## 🚀 Como executar

1. Clone o repositório:
```bash
git clone https://github.com/GabrielMendes-data/fetch_california_housing.git
