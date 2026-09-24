# Portfólio de Econometria & Séries Temporais Financeiras em R

Este repositório reúne um conjunto de projetos e trabalhos práticos (*Homeworks*) focados na análise econométrica, modelagem e previsão de séries temporais de ativos financeiros (mercados brasileiro e norte-americano). 

Os projetos cobrem desde a análise exploratória de fatos estilizados até a modelagem avançada de volatilidade e volatilidade condicional através de famílias de modelos ARMA e GARCH.

---

## 📌 Conteúdo do Repositório

### 1. Fatos Estilizados de Séries Temporais Financeiras (`Homework 1`)
- **Arquivo:** `homework_1_2.Rmd`
- **Ativos Analisados:** PETR4, VALE3, ITUB4 e WEGE3.
- **Tópicos Abordados:**
  - Extração de dados financeiros via API/pacotes em R.
  - Análise estatística descritiva de preços e retornos logarítmicos.
  - Verificação empírica de fatos estilizados (assimetria, curtose/caudas pesadas, ausência de autocorrelação nos retornos e presença de *volatility clustering*).

---

### 2. Modelagem Média e Estratégia de Trading com ARMA (`Homework 3`)
- **Arquivo:** `homework_3_2.Rmd`
- **Ativos Analisados:** Ibovespa (^BVSP) e ações do S&P 500.
- **Tópicos Abordados:**
  - Testes de estacionariedade e seleção de ordem para modelos ARMA/ARIMA.
  - Diagnóstico de resíduos (testes de Ljung-Box, normalidade e heterocedasticidade).
  - Backtesting de uma estratégia de negociação quantitativa baseada em previsões fora da amostra (*out-of-sample*) geradas pelos modelos ARMA.

---

### 3. Modelagem de Volatilidade Condicional com GARCH (`Homework 4`)
- **Arquivos:** `homework_4_ex_3_2.R` | `homework_4_ex4_2.R`
- **Ativos Analisados:** PETR4.SA e Ibovespa (^BVSP).
- **Tópicos Abordados:**
  - Estimação de modelos GARCH(1,1) considerando distribuição Normal e t-Student para os erros.
  - Comparação de aderência de distribuição e critérios de informação (AIC/BIC).
  - Cálculo da persistência da volatilidade ($\alpha + \beta$) e do tempo de meia-vida (*half-life*) dos choques de volatilidade.
  - Simulação e plotagem das funções de decaimento de volatilidade ao longo do tempo.

---

## 🛠️ Tecnologias e Pacotes Utilizados

- **Linguagem:** R
- **Manipulação e Modelação de Séries Temporais:**
  - `quantmod` / `tidyquant` (obtenção de dados do Yahoo Finance)
  - `xts` / `zoo` (manipulação de objetos temporais)
  - `forecast` / `tseries` (modelos ARMA/ARIMA e testes de hipóteses)
  - `rubogarch` / `fGarch` (estimação e especificação de modelos GARCH)
- **Visualização e Relatórios:**
  - `ggplot2` / `cowplot`
  - `rmarkdown` / `knitr`

---

## 🚀 Como Executar os Códigos

1. Clone este repositório:
   ```bash
   git clone https://github.com/seu-usuario/seu-repositorio.git
   ```
2. Abra o projeto no **RStudio**.
3. Certifique-se de ter os pacotes necessários instalados executando no console R:
   ```R
   install.packages(c("quantmod", "tseries", "forecast", "rugarch", "ggplot2", "tidyverse", "rmarkdown"))
   ```
4. Abra e execute os arquivos `.Rmd` ou `.R` individualmente.

---

