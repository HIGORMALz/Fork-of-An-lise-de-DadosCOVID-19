# Análise da Pandemia de COVID-19 no Brasil com Dashboard Interativo

## 🎯 1. Visão Geral do Projeto

Este projeto consiste em uma **Análise Exploratória de Dados (EDA)** completa sobre a evolução da pandemia de COVID-19 no Brasil durante o ano de 2021. O principal diferencial deste trabalho é a integração de múltiplas fontes de dados e a criação de um **dashboard interativo no Looker Studio (antigo Google Data Studio)**, que permite a visualização dinâmica e o acompanhamento de KPIs cruciais.

O objetivo foi transformar dados brutos e complexos em uma ferramenta visual e intuitiva, capaz de contar a história da pandemia através de números, tendências e mapas geográficos.

## dashboards 2. Dashboard Interativo no Looker Studio

O resultado final do projeto é um painel interativo que centraliza os principais indicadores da pandemia. A ferramenta foi projetada para permitir que qualquer utilizador, técnico ou não, possa explorar os dados de forma simples.

[**Clique aqui para aceder ao Dashboard Interativo**](https://lookerstudio.google.com/reporting/19a2eb72-f87c-4f50-8c87-31cf007a485d)

*(Opcional: Insira aqui um screenshot do seu dashboard)*
![Imagem de um dashboard da COVID-19]

**Principais KPIs e Visualizações no Dashboard:**

* **KPIs Dinâmicos:** Casos e mortes nas últimas 24h, médias móveis de 7 dias e a tendência (alta, estabilidade ou baixa).
* **Séries Temporais:** Gráficos que mostram a evolução de casos, mortes e vacinação ao longo do tempo.
* **Mapa Geográfico:** Visualização da distribuição de casos por estado, permitindo identificar as regiões mais afetadas.
* **Dados de Vacinação:** Acompanhamento da percentagem da população vacinada com 1ª, 2ª e 3ª doses.

## 📂 3. Fontes de Dados

Para garantir a credibilidade e precisão da análise, foram utilizadas duas das fontes de dados mais respeitadas mundialmente:

1.  **Casos e Mortes:** **Universidade Johns Hopkins (JHU)**, que compilou dados diários com alta granularidade geográfica e temporal.(https://www.jhu.edu/)
2.  **Vacinação:** **Our World in Data (OWID)**, projeto da Universidade de Oxford, que é a principal referência para o acompanhamento da imunização global.

## ✨ 4. Metodologia e Análises Realizadas

O notebook `.ipynb` documenta todo o processo de *data wrangling* e preparação dos dados, que incluiu:

* **Extração de Dados:** Coleta e consolidação de centenas de arquivos diários da JHU através de um processo iterativo em Python.
* **Limpeza e Transformação:** Tratamento de dados ausentes, padronização de nomes (ex: "Sao Paulo" para "São Paulo") e conversão de tipos de dados.
* **Engenharia de Features:** Cálculo de métricas essenciais que não estavam nos dados brutos, como:
    * Novos casos/mortes por dia (`confirmed_1d`, `deaths_1d`).
    * Médias móveis de 7 dias para suavizar ruídos e identificar tendências reais.
    * Taxa de crescimento de 14 dias para classificar a tendência como "subida", "descida" ou "estável".
    * Percentagens da população vacinada.

## 🛠️ 5. Ferramentas e Tecnologias

* **Linguagem:** Python
* **Bibliotecas:** `pandas`, `numpy`
* **Ferramenta de BI:** Looker Studio (Google Data Studio)
* **Ambiente:** Jupyter Notebook (Google Colab)

## 🚀 6. Como Executar e Explorar

**Para explorar a análise:**

* A forma mais recomendada é através do [**Dashboard Interativo**](https://lookerstudio.google.com/reporting/19a2eb72-f87c-4f50-8c87-31cf007a485d).

**Para replicar o processo de tratamento de dados:**

1.  **Clone este repositório:**
    ```
    git clone [https://github.com/](https://github.com/)[seu-usuario]/[nome-do-repositorio-covid].git
    ```
2.  **Execute o Notebook:**
    Abra o arquivo `.ipynb` no Google Colab ou Jupyter Notebook. As células de código carregarão os dados diretamente das fontes originais e realizarão todo o processo de tratamento.

## 👨‍💻 7. Autor

* **Higor Silva**
* **LinkedIn:** https://www.linkedin.com/in/higor-silva-4a7341273/
