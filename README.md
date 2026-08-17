# Alura TeleconX: Análise de Churn 📊📞

## 📄 Sobre o Projeto
Este projeto foi desenvolvido como parte do desafio de Data Science (Challenge Oracle + Alura). O objetivo principal é realizar o tratamento e a Análise Exploratória de Dados (EDA) de uma base de clientes de uma empresa de telecomunicações para entender o comportamento de **Churn** (taxa de cancelamento).

Através de limpeza de dados, engenharia de features e visualizações, o projeto busca identificar quais características (demográficas e de serviços contratados) mais influenciam a decisão do cliente de deixar a empresa.

## 🎯 Etapas e Funcionalidades
- **Ingestão de Dados:** Consumo de dados via API a partir de um arquivo JSON.
- **Limpeza e Tratamento:** 
  - Normalização do arquivo JSON.
  - Conversão de tipos de dados (ex: transformação de `Yes`/`No` para valores Booleanos).
  - Tratamento de valores nulos e strings vazias (remoção de nulos em `Churn` e preenchimento pela média em `Total_Cobrado`).
- **Feature Engineering:** 
  - Criação da variável `Custo_Diario` a partir da mensalidade.
  - Tradução e padronização dos nomes das colunas para o português.
- **Análise Exploratória (EDA):** 
  - Geração de estatísticas descritivas.
  - Visualizações gráficas comparando a distribuição de clientes por tempo de contrato, serviços assinados e perfil demográfico (Gênero, Senioridade, Dependentes, etc.) em relação à taxa de Churn.

## 💡 Principais Insights
- O número de clientes que cancelaram o serviço é significativamente menor do que os que permaneceram.
- Clientes com parceiros ou dependentes apresentam uma probabilidade visivelmente menor de churn.
- A contratação de serviços adicionais como **Segurança Online, Backup Online, Suporte Técnico e Proteção de Dispositivo** é um forte indicativo de retenção (fidelização) do cliente.

## 🛠️ Tecnologias Utilizadas
*   **Python 3**
*   **Pandas & NumPy:** Manipulação, limpeza e análise de dados.
*   **Matplotlib & Seaborn:** Criação de gráficos e visualizações.
*   **Requests:** Consumo da base de dados em JSON.
*   **Jupyter Notebook:** Ambiente de desenvolvimento interativo.

## 📂 Estrutura do Repositório
- `TelecomX.ipynb` : Notebook contendo todo o código, desde a ingestão até a análise visual dos dados.
- `README.md` : Documentação do projeto.
