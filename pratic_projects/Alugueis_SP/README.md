# 🏙️ O que mais influencia o valor(R$/m²) do aluguel de um imóvel em São Paulo?

> Projeto de análise diagnóstica utilizando dados do kaggle (webscrapping do Quinto Andar) do mercado imobiliário paulistano.

---

## 📌 Objetivo

Este é meu primeiro projeto autoral de dados. O objetivo é identificar os fatores que mais influenciam o valor do aluguel de um imóvel na cidade de São Paulo, utilizando análise exploratória, engenharia de atributos e modelos de regressão para obter insights e visualizações claras.

---

## 📊 Dataset

- **Fonte**: [São Paulo Housing Prices Dataset - Kaggle](https://www.kaggle.com/)
- **Atributos principais**:
  - `rent`, `total` – valor do aluguel
  - `area` – metragem do imóvel
  - `bedrooms`, `garage` – número de cômodos
  - `district`, `address` – localização
  - `type` - Casa, Casa em condomínio, Apartamento ou Kitnet

---

## 🔧 Ferramentas Utilizadas

- Python (Pandas, NumPy, Scikit-Learn, Matplotlib, Seaborn)
- Jupyter Notebook

---

## 🧱 Etapas do Projeto

### 0. Coleta e Exploração
- setup inicial do jupyter notebook
- exploração inicial dos dados

### 1. Limpeza e Pré-processamento
- Remoção de valores nulos, não formatados e duplicatas
- tratamento de outliers
- Eliminação de colunas irrelevantes

### 2. Enriquecimento dos Dados
- Criação da variável `$/m²` como alvo e features como `valor_regiao`
  
### 3. Análise Exploratória (EDA)
- Estatísticas descritivas
- Boxplots comparando `$/m²` por `valor_regiao` entre outras relações
- Heatmap de correlações
- Identificação visual de padrões
- Formulação de hipóteses

### 4. Modelagem
- Teste com múltiplos modelos (como final foi escolhido o random forest)
- Avaliação com RMSE, MAE e R²
- Interpretação dos fatores mais influentes

### 5. Visualização e Apresentação - pendente
- Construção de dashboard interativo
- Storytelling dos dados

---

## 📊 Dashboard Final - pendente

📎 **Link para o dashboard interativo:** 

---

## 📝 Principais Insights - pendente



---

## 🧠 Lições Aprendidas - incompleto

- Como fazer EDA, exploração, manipulação, enriquecimento e modelagem para mineração de dados utilizando machine learning.
- Como aplicar uma pipeline completa de análise diagnóstica. (ETL)
- Diferença prática entre modelos lineares e baseados em árvore.
- Importância da visualização para interpretar resultados com clareza.

---

## ✅ Próximos Passos

Pontos a melhorar neste projeto:
- integração direta do código com a base (quinto andar) usando o webscrapping, ao invés da base do kaggle, melhorando a confiabilidade com dados em tempo real.
- feature enginnering relativo ao tipo de imóvel e principalmente a localização, o que só seria possível com uma coleta mais rica.
Este projeto me inspirou a me desafiar com um novo projeto tratando de uma análise descritiva do mercado de trabalho.

---

## 📬 Contato

Feito por Kauan Buzone Roberti – Conecte-se comigo no [LinkedIn](https://linkedin.com/in/kauanbuzone)



