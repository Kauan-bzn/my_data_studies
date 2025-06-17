# 🏙️ O que mais influencia o valor(R$/m²) do aluguel de um imóvel em São Paulo?

> Projeto de análise diagnóstica utilizando dados do kaggle (webscrapping do Quinto Andar) do mercado imobiliário paulista.

---

## 📌 Objetivo

Este é meu primeiro projeto autoral de dados. O objetivo é identificar os fatores que mais influenciam o custo do m² do aluguel de um imóvel na cidade de São Paulo, utilizando análise exploratória, engenharia de features e modelos de regressão para obter insights e visualizações claras.

---

## 📊 Dataset

- **Fonte**: [São Paulo Housing Prices Dataset - Kaggle](https://www.kaggle.com/datasets/renatosn/sao-paulo-housing-prices) -> webscraping do Quinto Andar
- **Atributos principais**:
  - `rent`, `total` – valor do aluguel
  - `area` – metragem do imóvel
  - `bedrooms`, `garage` – número de cômodos
  - `district`, `address` – localização
  - `type` - Casa, Casa em condomínio, Apartamento ou Kitnet

---

## 🔧 Ferramentas Utilizadas

- Python (Pandas, NumPy, Scikit-Learn, Matplotlib, Seaborn entre outras bibliotecas)
- Jupyter Notebook - Kaggle
- Visualização de dados - Power BI 

---

## 🧱 Etapas do Projeto

### 0. Coleta e Exploração
- setup inicial do jupyter notebook
- exploração inicial dos dados (EDA)

### 1. Limpeza e Pré-processamento - Manipulação de dados
- Remoção de valores nulos, infinitos e duplicatas
- Formatar não formatados
- tratamento de outliers
- Eliminação de colunas irrelevantes

### 2. Enriquecimento dos Dados
- Criação do campo `$/m²` como alvo e features como `valor_regiao`
- One Hot encoding aplicado no campo `type`
  
### 3. Análise Exploratória (EDA)
- Estatísticas descritivas
- Análise da distribuição de imóveis por `$/m²`
- regressão linear de `$/m²` por `area`
- Boxplots comparando `$/m²` por `valor_regiao` e `type`
- Heatmap de correlações
- Identificação visual de padrões (`$/m²` por `vagas de garagem` e `número de quartos`)
- Formulação de hipóteses

### 4. Modelagem
- Teste com múltiplos modelos (como final foi escolhido o Gradient Boosting Regressor)
- Avaliação com R² (64,44%)
- Confirmação de hipóteses e resumo da análise

### 5. Visualização e Apresentação
- Formatação para exportação dos dados
- Comentários finais sobre o que pode ser melhor no jupyter notebook
- Definição dos gráficos que melhor demonstram os insights
- construção do dashboard interativo no Power BI visando apresentação com storytelling

---

**Não possuo o power BI "premium", logo não consigo disponibilizar o link do dashboard. Por conta disso estará disponível apenas uma screenshot.** 

---

## 📝 Principais Insights
- o **valor da região** (média do custo do metro quadrado por bairro classificada de 1 a 5) é o fator mais determinante pois se relaciona com a criminalidade, densidade comercial, metrô, entre outros **fatores derivados da geolocalização** e que **em São Paulo tendem a ser fatores importantes** na decisão de qual imóvel escolher já que o estado é **muito urbanizado** portanto possui uma variação ampla por bairro.
- quanto **mais área** determinado imóvel possui, **menos liquidez** ele tem, portanto a area tende a perder valor e o **custo do m² por mês diminui**.
- quanto mais quartos menos costuma se pagar por metro quadrado, provavelmente por um **comportamento semelhante ao ponto anterior**.
- quanto **mais vagas de garagem mais caro costuma se pagar por metro quadrado**. Isso ocorre porque em uma **área altamente urbanizada** a **segurança de um bem como o carro é alta prioridade**, valorizando a área do imóvel.
- quando se trata de preço médio por metro quadrado no aluguel: **casa < casa em condomínio < apartamento < studio e kitnet**. Os studios/kitnet e apartamentos costumam ser mais bem localizados (fator de encarecimento) - studio e kitnet costuma ser mais caro pois sua área é menor. Todos os tipos de imóvel, exceto a Casa, pagam condomínio e de certa forma costumam ter um critério de localização mais rigoroso para sua construção e aluguel, por isso a casa costuma ser o tipo mais barato.


---
## 📈 Comentários finais sobre o projeto
### Possíveis melhorias
- Reconheço que ainda tenho muito a aprender desde os conceitos do processo até as ferramentas de cada técnica específica e isso melhoraria a precisão, qualidade e valor dos meus resultados.
- integração entre as etapas de coleta, tranformação e visualização de dados, possivelmente usando uma base diferente ou webscraping neste jupyter notebook aumentando a confiabilidade dos dados. Também seria interessante usar um banco de dados e API para criação do dashboard, dessa forma este também seria atualizado em tempo real.
- Poderia ter usado melhor o controle de versões do kaggle, e git/github.

### Aprendizado sobre o processo
- Mesmo que seu trabalho seja aplicando conceitos, técnicas e ferramentas específicos, o objetivo final tem de ser lembrado com constância: extrair conhecimento.
- Quando se trata de um trabalho real, a cautela (comunicação, planejamento, revisão e documentação) em cada etapa tem que ser maior do que em um exercício. Afinal cada erro faz você perder tempo, e consequentemente recursos, retornando para corrigir etapas anteriores e tendo que percorrer por cada etapa para se localizar novamente.
- Senti na pele durante este projeto o que muitos já reconhecem: as etapas iniciais são as mais críticas, pois elas influenciam muito no resultado e são mais difíceis de corrigir. Por isso a coleta, exploração e manipulação dos dados deve ser muito exercitada.  
---

## 🧠 Lições Aprendidas

- Como fazer EDA (exploração), manipulação, enriquecimento e modelagem - machine learning - para mineração de dados utilizando Python.
- Como fazer uma análise estatística.
- Como fazer uma boa limpeza e transformação de dados para extrair o máximo da base e das features (campos).
- Como aplicar um pipeline e como avaliar modelos de machine learning.
- Diferença prática entre modelos lineares e baseados em árvore.
- formulação de hipóteses da análise de dados associadas com o conhecimento de negócio.
- Criação de dashboards com storytelling e interatividade para apresentação de insights utilizando power BI.

---

## ✅ Próximos Passos

Aprendi muito com este projeto, tanto colocando a prova conhecimentos anteriores, quanto estudando assuntos novos e praticando. No entanto, pretendo parar este projeto por aqui e levar comigo a experiência - lições aprendidas - e as possíveis melhorias para um próximo projeto, no qual vou me desafiar com um assunto e processo diferente possibilitando aprender ainda mais. Vale destacar que tenho vontade de explorar um pouco mais sobre SQL e banco de dados, pretendo fazer isso com cursos e projetos posteriores. Existe, ainda, a possibilidade de no futuro haver um retorno a este projeto para dar continuidade e implementar melhorias mas isso só ocorrerá quando eu tiver mais fundamento teórico principalmente sobre as etapas iniciais assim terei mais valor a agregar e mais retorno de aprendizado

---

## 📬 Contato

Feito por Kauan Buzone Roberti – Conecte-se comigo no [LinkedIn](https://linkedin.com/in/kauanbuzone)



