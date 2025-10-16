# 🔎Projeto de Data Science: Detecção de Fraudes em Entregas do Walmart E-commerce
Este projeto de Data Science tem como foco a análise e a mitigação de fraudes e perdas financeiras no serviço de entregas de e-commerce do Walmart na região da Flórida Central (EUA). Utilizando análises estatísticas e modelagem de risco, o objetivo é identificar padrões suspeitos de desvio de produtos, sejam eles atribuíveis a entregadores (motoristas) ou a clientes (fraude de consumidor).

Projeto de análise de dados de fraude com dados do Walmart:

<img width="1428" height="803" alt="image" src="https://github.com/user-attachments/assets/5965cf4a-fb6c-4b60-9dd8-7254bc36fff0" />


[Ítalo Magalhães Portfólio](https://italo-mgl.streamlit.app/{:target="_blank"})


O trabalho foi desenvolvido com o objetivo de servir de modelo (MVP) para ser escalado para todas as regiões de e-commerce do Walmart nos EUA, visando reduzir a perda anual de milhões de dólares.

## 🎯 Objetivo Principal

O objetivo central do projeto é **detectar e quantificar os padrões de fraude em entregas**, determinando:

* **Quem é o responsável:** Se o problema está primariamente nos motoristas (desvio de itens) ou nos clientes (falsas reclamações).
* **Onde e Quando:** Se as perdas se concentram em regiões, horários (ex: baixa supervisão) ou categorias de produtos específicos.
* **Qual o Impacto Financeiro:** Quantificar o prejuízo total e o valor em risco em cada grupo de fraude.

## ⚙️ Metodologia e Análises Chave

A metodologia seguiu as etapas clássicas de um projeto de Data Science (EDA, Feature Engineering, Modelagem de Risco e Conclusões).

### 📊 Análises e Modelos Desenvolvidos:

* **Detecção de Outliers (Motoristas):** Classificação dos entregadores em **Alto, Médio e Baixo Risco** com base na **Taxa de Pedidos com Perda** e no volume de `Trips` (viagens). O resultado principal é um gráfico de dispersão (`Scatter Plot`) que destaca motoristas suspeitos com alta performance de trabalho e alta taxa de desvio.
* **Detecção de Reincidência (Clientes):** Classificação dos clientes em **Alto, Médio e Baixo Risco** com base na **Porcentagem de Pedidos com Perda** (normalizada pelo total de pedidos). Isso isola clientes com um padrão crônico de reclamações.
* **Análise Temporal:** Identificação de picos de perda em horários de baixa supervisão (ex: **22h**) e a análise da tendência mensal para identificar um evento de causa raiz (ex: o pico de perda em Agosto seguido pela queda em Setembro).
* **Análise de Concentração:** Visualização das **Categorias de Produtos** mais visadas e a concentração de prejuízo por **Faixa Etária** do cliente.
* **Métricas de Valor:** Criação e uso da métrica **Valor Total de Perdas** para quantificar o impacto financeiro de cada grupo de risco.

### 💻 Tecnologias Utilizadas

| Ferramenta | Uso no Projeto |
| :--- | :--- |
| **Power BI** | Análise Exploratória de Dados (EDA), Criação de Colunas Calculadas (DAX) para classificação de risco, e Desenvolvimento do Dashboard Executivo. |
| **DAX** | Criação das colunas de Nível de Risco (Motorista e Cliente), Taxa de Perda e a medida Valor Total de Perdas. |

## 📈 Conclusões e Próximos Passos (Recomendações)

O projeto resultou em um conjunto de recomendações acionáveis:

* **Foco na Mitigação:** A fraude é concentrada. As perdas podem ser reduzidas significativamente ao auditar o grupo de motoristas de Alto Risco.
* **Medidas Preventivas:** Recomendação de exigir **verificação por foto geolocalizada** para entregas de alto valor em horários de risco (após as 19h) e implementação de uma política de **Restrição de Reembolso** para clientes de Alto Risco.
* **Investigação de Processo:** Investigação da causa da melhoria observada a partir de Setembro para replicar o sucesso em outras áreas.
