📡 Clallenge TelecomX_parte2  

Este projeto analisa dados de clientes de uma operadora de telecomunicações com o objetivo de **identificar fatores que influenciam a evasão de clientes (churn)** e propor **estratégias de retenção baseadas em dados**. A abordagem combina **análise exploratória, engenharia de features e modelagem preditiva**, gerando insights claros, acionáveis e visualmente organizados para portfólio.  

🧮 Modelos Utilizados  
- **Regressão Logística**: interpreta o impacto de cada variável sobre a probabilidade de churn, fornecendo insights diretos e interpretáveis para decisões estratégicas.  
- **Random Forest**: mede a importância das variáveis e identifica os principais drivers do churn, capturando relações complexas entre fatores.  
- **Observação**: KNN e SVM foram **desconsiderados conscientemente** devido à menor interpretabilidade e ao alto custo computacional, sem ganho relevante comparado aos modelos escolhidos.  

🔑 Principais Fatores de Churn  
- **Tempo de contrato (`tenure`)** – contratos curtos aumentam o risco de evasão.  
- **Tipo de contrato (`contract`)** – contratos mensais apresentam maior propensão a churn comparados a anuais ou bianuais.  
- **Valor mensal (`MonthlyCharges`)** – clientes com gastos mensais altos têm maior risco de insatisfação.  
- **Total gasto acumulado (`TotalCharges`)** – menor engajamento financeiro total está relacionado a maior evasão.  
- **Serviços contratados (internet, telefone, etc.)** – variedade e qualidade dos serviços impactam diretamente a retenção.  

🎯 Estratégias de Retenção Recomendadas  
- Desenvolver campanhas direcionadas para clientes com contratos curtos ou valores mensais elevados.  
- Monitorar clientes com baixo engajamento financeiro e propor ofertas personalizadas.  
- Melhorar a qualidade de serviços essenciais, como internet e telefone.  
- Criar programas de fidelidade e incentivos para clientes de maior risco.  

📂 Estrutura do Projeto  
- TelecomX_parte2.ipynb → Notebook completo com análise, modelagem e visualizações.  
- telecom_tratado.csv → Dataset tratado utilizado na análise.  
- README.md → Este arquivo, com objetivos, metodologia, insights e recomendações estratégicas.  

📊 Conclusão  
O projeto demonstra como combinar **performance preditiva (Random Forest)** com **interpretabilidade estratégica (Regressão Logística)** para orientar ações de retenção.
As análises permitem identificar clientes de maior risco e transformar insights em **decisões de negócio eficazes**.



