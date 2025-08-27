# Análise de Segmentação de Clientes de Varejo de Telecomunicações

## Visão Geral do Projeto

Este projeto de Ciência de Dados tem como objetivo principal segmentar uma base de clientes de uma empresa de varejo de telecomunicações. A segmentação foi realizada para identificar grupos de clientes com perfis e comportamentos semelhantes, permitindo que a empresa crie estratégias de marketing, vendas e produto mais direcionadas e eficazes.

O projeto foi desenvolvido em **Python** usando um **Jupyter Notebook**. A análise final e a visualização dos resultados estão disponíveis em um dashboard interativo no **Looker Studio**.

## Metodologia

A análise seguiu um fluxo de trabalho padrão em Ciência de Dados, dividido nas seguintes etapas:

1.  **Coleta e Limpeza de Dados:** Os dados foram **gerados de forma aleatória** em um formato CSV para simular um cenário de negócio. A limpeza incluiu a conversão de tipos de dados (por exemplo, strings com vírgulas para números), o tratamento de dados ausentes e a validação do formato das colunas.

2.  **Engenharia de Features:** Variáveis novas e mais úteis para a análise foram criadas a partir dos dados existentes. Isso incluiu o cálculo da **idade** dos clientes a partir de suas datas de nascimento.

3.  **Padronização e Transformação:** As variáveis categóricas (como `Canal de Vendas`, `Segmento`, `Estado`) foram transformadas em um formato numérico por meio de **One-Hot Encoding**. As variáveis numéricas foram **padronizadas** usando o `StandardScaler` para que todas tivessem a mesma importância no modelo.

4.  **Modelagem de Segmentação:** O algoritmo de clustering **K-Means** foi aplicado aos dados padronizados. O **Método do Cotovelo** foi utilizado para determinar o número ideal de clusters, que resultou em **7 segmentos de clientes distintos**.

5.  **Análise e Interpretação dos Clusters:** Cada um dos 7 clusters foi analisado com base em características como idade, valor do plano, GB contratados e canal de vendas dominante. Cada segmento recebeu um nome descritivo para facilitar a compreensão.

## Ferramentas e Tecnologias

* **Python:** Linguagem de programação utilizada para todo o processamento dos dados.
* **Jupyter Notebook:** Ambiente de desenvolvimento para o projeto.
* **Pandas:** Biblioteca de manipulação e análise de dados.
* **Scikit-learn:** Biblioteca de machine learning utilizada para os algoritmos de clustering e padronização.
* **Looker Studio:** Ferramenta de Business Intelligence utilizada para a criação do dashboard interativo.

## Resultados e Acesso ao Dashboard

O resultado final do projeto é uma base de dados segmentada, onde cada cliente está associado a um dos 7 grupos identificados.

Todos os dados, análises e visualizações podem ser explorados no dashboard interativo disponível no Looker Studio.

* **[[Link para o Dashboard no Looker Studio](https://lookerstudio.google.com/reporting/01a5b067-b8bc-4bff-8724-367a25cc15bb)]**
