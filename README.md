# 📊 Previsão de Valor de Aluguel com Regressão Linear

## 📌 Sobre o Projeto

Este projeto tem como objetivo aplicar técnicas de **Machine Learning** para prever o **valor de aluguel de imóveis** com base em suas características estruturais.

Foram implementados dois modelos:

* **Regressão Linear Simples** (utilizando apenas a metragem)
* **Regressão Linear Múltipla** (utilizando diversas variáveis do imóvel)

A análise busca entender **quais fatores influenciam o valor do aluguel** e avaliar qual modelo apresenta melhor capacidade preditiva.

---

# 📂 Dataset

O dataset contém informações sobre imóveis disponíveis para aluguel, incluindo:

* Valor do condomínio
* Metragem
* Número de quartos
* Número de banheiros
* Número de suítes
* Número de vagas
* Valor do aluguel (variável alvo)

---

# ⚙️ Tecnologias Utilizadas

* Python
* Pandas
* Numpy
* Matplotlib
* Seaborn
* Scikit-Learn
* Jupyter Notebook

---

# 🔎 Etapas do Projeto

## 1️⃣ Análise Exploratória dos Dados

Foram realizadas análises iniciais para entender a distribuição das variáveis e identificar possíveis relações entre elas.

Principais análises realizadas:

* Visualização de dispersão entre variáveis
* Análise de correlação
* Identificação de variáveis relevantes

---

## 2️⃣ Pré-processamento dos Dados

Nesta etapa foram realizadas:

* Separação das variáveis independentes (**X**) e dependente (**y**)
* Divisão da base em **treino e teste**

Treino: 70%
Teste: 30%

---

## 3️⃣ Regressão Linear Simples

Primeiramente foi criado um modelo utilizando apenas a variável **metragem** para prever o valor do aluguel.

Modelo matemático:

Preço ~ Metragem

### Resultado

R² Treino: **0.52**

O modelo explicou aproximadamente **52% da variação do valor do aluguel**.

---

## 4️⃣ Regressão Linear Múltipla

Em seguida foi aplicado um modelo utilizando todas as variáveis disponíveis:

Preço ~ Metragem + Quartos + Banheiros + Suítes + Vagas + Condomínio

### Resultados

R² Treino: **0.5956**

R² Teste: **0.6307**

---

# 📊 Comparação dos Modelos

| Modelo                    | R²    |
| ------------------------- | ----- |
| Regressão Linear Simples  | 0.521 |
| Regressão Linear Múltipla | 0.595 |

O modelo de **regressão múltipla apresentou melhor desempenho**, pois considera mais características do imóvel.

---

# 🧠 Conclusões

Os resultados indicam que o valor do aluguel não depende apenas da metragem do imóvel, mas também de outras variáveis como:

* Número de quartos
* Número de banheiros
* Número de vagas
* Valor do condomínio

A inclusão dessas variáveis no modelo permitiu **aumentar a capacidade explicativa do modelo**, resultando em um valor de R² maior.

---

# 🚀 Possíveis Melhorias

Algumas melhorias que poderiam ser implementadas:

* Inclusão de novas variáveis (ex: localização, bairro)
* Teste de outros algoritmos de regressão
* Feature engineering
* Avaliação com métricas adicionais (RMSE, MAE)

---

# 👩‍💻 Autor

Projeto desenvolvido durante o curso de **Cientista de Dados**.

GitHub: vivianfoliveira-tech
