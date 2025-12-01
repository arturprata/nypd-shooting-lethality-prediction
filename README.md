# NYPD Shooting Lethality Prediction  
**Análise e predição da letalidade dos tiroteios na cidade de Nova York (2006–2022)**

## Sobre o Projeto

Este projeto tem como objetivo analisar os fatores associados à letalidade dos tiroteios na cidade de Nova York e construir modelos preditivos capazes de estimar a probabilidade de um disparo resultar em morte, utilizando técnicas de aprendizado de máquina supervisionado.

---

## Dataset Utilizado

- **Fonte:** [NYC Open Data – NYPD Shooting Incident Data (Historic)](https://data.cityofnewyork.us/Public-Safety/NYPD-Shooting-Incident-Data-Historic-/833y-fsy8/about_data)
- **Período:** 2006–2024  
- **Tamanho:** ~29.000 registros | 21 colunas  

### Principais variáveis:

- `occur_date`, `occur_time` – Data e hora do incidente  
- `boro`, `precinct` – Localização (bairro e distrito policial)  
- `vic_*`, `perp_*` – Perfil da vítima e do agressor (idade, sexo, raça)  
- `latitude`, `longitude` – Coordenadas geográficas  
- `STATISTICAL_MURDER_FLAG` – **Variável-alvo**: indica se o disparo resultou em morte

---

## Perguntas de Pesquisa

1. Quais fatores estão associados à letalidade dos tiroteios na cidade de Nova York?  
2. É possível estimar, a partir das informações disponíveis no momento do crime, a chance de um tiroteio resultar em homicídio?

---

## Hipóteses

- **H1:** A letalidade varia de acordo com o horário, bairro e distrito policial.  
- **H2:** O perfil da vítima e do agressor influencia a letalidade.  
- **H3:** Modelos baseados em árvores (Random Forest, XGBoost) superam modelos lineares (Regressão Logística) na previsão da letalidade.

---

## Resultados Esperados

- Identificação dos principais fatores que influenciam a letalidade.  
- Construção de um modelo preditivo da chance de morte em incidentes.  

---

## Linguagem Utilizada

| **Linguagem**          | Python 3.10.0                        |

---

## Instruções para Execução das Etapas

Caso deseje rodar os notebooks desde o início, siga estas instruções importantes:

1. **Após finalizar a Etapa 2**, será gerado um arquivo **CSV final**.  
   → Coloque esse arquivo **dentro da pasta da Etapa 3**.

2. **Após finalizar a Etapa 3**, será gerado um arquivo **Parquet**.  
   → Coloque esse arquivo **dentro da pasta da Etapa 4**.

Esses passos garantem que as etapas seguintes encontrem corretamente os dados necessários.
Também, cheque as ferramentas utilizadas no arquivo requirements.txt, para que o projeto execute corretamente.

---

## Autor

**Artur Pigari Prata**  
Estudante de Ciência da Computação – UTFPR – Campo Mourão

