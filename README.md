# 🔫 NYPD Shooting Lethality Prediction  
**Análise e predição da letalidade dos tiroteios na cidade de Nova York (2006–2022)**

## 📌 Sobre o Projeto

Este projeto tem como objetivo analisar os fatores associados à letalidade dos tiroteios na cidade de Nova York e construir modelos preditivos capazes de estimar a probabilidade de um disparo resultar em morte, utilizando técnicas de aprendizado de máquina supervisionado.

---

## 🗂️ Dataset Utilizado

- **Fonte:** [NYC Open Data – NYPD Shooting Incident Data (Historic)](https://data.cityofnewyork.us/)
- **Período:** 2006–2022  
- **Tamanho:** ~27.000 registros | 21 colunas  

### 🔑 Principais variáveis:

- `occur_date`, `occur_time` – Data e hora do incidente  
- `boro`, `precinct` – Localização (bairro e distrito policial)  
- `vic_*`, `perp_*` – Perfil da vítima e do agressor (idade, sexo, raça)  
- `latitude`, `longitude` – Coordenadas geográficas  
- `STATISTICAL_MURDER_FLAG` – **Variável-alvo**: indica se o disparo resultou em morte

---

## ❓ Perguntas de Pesquisa

1. Quais fatores estão associados à letalidade dos tiroteios na cidade de Nova York?  
2. É possível estimar, a partir das informações disponíveis no momento do crime, a chance de um tiroteio resultar em homicídio?

---

## 💡 Hipóteses

- **H1:** A letalidade varia de acordo com o horário, bairro e distrito policial.  
- **H2:** O perfil da vítima e do agressor influencia a letalidade.  
- **H3:** Modelos baseados em árvores (Random Forest, XGBoost) superam modelos lineares na previsão da letalidade.

---

## ⚙️ Metodologia

- **Coleta e integração de dados:** Junção de bases do NYPD e dados de setores policiais.  
- **Limpeza e tratamento:** Remoção de valores nulos e codificação de variáveis categóricas.  
- **Engenharia de atributos:** Criação de variáveis temporais, espaciais e demográficas.  
- **Modelagem preditiva:** Regressão Logística, Random Forest e XGBoost.  
- **Avaliação:** Métricas como AUC, F1 e PR-AUC, além de explicabilidade com SHAP.

---

## 📈 Resultados Esperados

- Identificação dos principais fatores que influenciam a letalidade.  
- Construção de um modelo preditivo da chance de morte em incidentes.  
- Subsídios para políticas públicas orientadas por dados.

---

## 🛠️ Tecnologias Utilizadas

| Categoria              | Ferramentas                         |
|------------------------|-------------------------------------|
| **Linguagem**          | Python 3.10+                        |
| **Manipulação de dados** | Pandas, NumPy                    |
| **Visualização**       | Matplotlib, Seaborn, Plotly         |
| **Modelagem**          | Scikit-learn                        |
| **Documentação**       | Jupyter Notebook                    |

---

## 👤 Autor

**Artur Pigari Prata**  
Estudante de Ciência da Computação – UTFPR – Campo Mourão  
📧 [LinkedIn](https://www.linkedin.com/) (adicione seu link aqui) | [GitHub](https://github.com/) (adicione seu link aqui)