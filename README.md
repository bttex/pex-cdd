# Análise de Segmentação de Clientes de Varejo de Telecomunicações

## Visão Geral do Projeto

Este projeto de Ciência de Dados tem como objetivo principal segmentar a base de clientes de uma empresa de varejo de telecomunicações. A segmentação permite identificar grupos de clientes com perfis e comportamentos semelhantes, possibilitando estratégias de marketing, vendas e produto mais direcionadas e eficazes.

O projeto foi desenvolvido em **Python** dentro de um **Jupyter Notebook**, e os resultados finais estão disponíveis em um dashboard interativo no **Looker Studio**.

## Metodologia

A análise seguiu um fluxo de trabalho estruturado em etapas:

1. **Coleta e Limpeza de Dados:**  
   Os dados foram **gerados artificialmente** em formato CSV para simular um cenário de negócio realista. A etapa de limpeza incluiu conversão de tipos (por exemplo, strings numéricas com vírgulas), tratamento de valores ausentes e validação da consistência das colunas.

2. **Engenharia de Features:**  
   Foram criadas novas variáveis a partir dos dados originais, como o cálculo da **idade** dos clientes com base na data de nascimento.

3. **Padronização e Transformação:**  
   Variáveis categóricas (como `Canal de Vendas`, `Segmento`, `Estado`) foram convertidas em formato numérico via **One-Hot Encoding**.  
   Já as variáveis numéricas foram **padronizadas** utilizando o `StandardScaler` para manter proporcionalidade no modelo.

4. **Modelagem de Segmentação:**  
   O algoritmo de clustering **K-Means** foi aplicado após a padronização dos dados. O número ótimo de clusters foi definido com o **Método do Cotovelo**, resultando em **7 segmentos distintos**.

5. **Análise e Interpretação dos Clusters:**  
   Inicialmente, todos os clusters foram analisados individualmente.  
   No entanto, para fins de direcionamento estratégico no **dashboard**, foram destacados os **principais clusters candidatos a investimento em marketing**, definidos com base em dois critérios:  
   - **Maior ticket médio**  
   - **Maior volume de vendas**

   Assim, a análise final se concentra nos segmentos de maior relevância para retorno em campanhas de marketing.

## Ferramentas e Tecnologias

- **Python** – linguagem principal para análise de dados  
- **Jupyter Notebook** – ambiente de desenvolvimento do projeto  
- **Pandas** – manipulação e análise de dados  
- **Scikit-learn** – clustering e padronização  
- **Looker Studio** – criação do dashboard interativo  

## Resultados e Dashboard

O resultado do projeto é uma base de clientes segmentada em 7 grupos, com destaque para os clusters mais promissores em termos de **valor de plano** e **volume de vendas**.  

Os insights podem ser explorados no dashboard interativo:  

🔗 **[Acessar Dashboard no Looker Studio](https://lookerstudio.google.com/reporting/01a5b067-b8bc-4bff-8724-367a25cc15bb)**
