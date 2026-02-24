📡 Challenge TelecomX_parte2

Este desafio analisa dados de clientes de uma operadora de telecomunicações com o objetivo de prever a evasão de clientes (churn) e identificar os principais fatores que influenciam o cancelamento. A abordagem combina análise exploratória, engenharia de features e modelagem preditiva, gerando insights claros, acionáveis e organizados para portfólio. A variável alvo utilizada foi Churn (Yes/No), e o foco é apoiar estratégias de retenção orientadas por dados.

🧮 Preparação dos Dados

As variáveis foram classificadas em:

Numéricas: tenure, MonthlyCharges, TotalCharges

Categóricas: tipo de contrato, método de pagamento, serviços contratados, entre outras

Etapas realizadas:

Remoção de variáveis irrelevantes (ex.: identificadores sem valor preditivo).

Tratamento de valores ausentes: mediana para variáveis numéricas e “Unknown” para categóricas.

Aplicação de One-Hot Encoding nas variáveis categóricas.

Aplicação de StandardScaler nas variáveis numéricas para modelos lineares.

Separação da base em 80% treino e 20% teste, com estratificação da variável alvo para manter a proporção das classes.

🤖 Modelos Utilizados

Regressão Logística: interpreta o impacto de cada variável sobre a probabilidade de churn, fornecendo insights diretos e estratégicos.

Random Forest: mede a importância das variáveis e identifica os principais drivers do churn, capturando relações não lineares e interações complexas.

A avaliação foi realizada com Acurácia, Precision, Recall, F1-Score e ROC-AUC. O Random Forest apresentou melhor desempenho geral, enquanto a Regressão Logística agregou interpretabilidade.

Observação: KNN e SVM foram desconsiderados conscientemente devido à menor interpretabilidade e ao maior custo computacional, sem ganho relevante frente aos modelos escolhidos para este contexto.

🔍 Análise Exploratória (EDA)

Foram gerados gráficos como:

Heatmap de correlação

Boxplot de tenure vs churn

Scatterplot de tenure vs TotalCharges

Principais padrões identificados:

Clientes com menor tempo de contrato apresentam maior probabilidade de churn.

Contratos mensais concentram maior evasão.

Clientes com menor valor total acumulado tendem a cancelar com maior frequência.

Combinação de baixo tenure e alto MonthlyCharges indica grupo crítico de risco.

🔑 Principais Fatores de Churn

Tempo de contrato (tenure) – contratos curtos aumentam o risco de evasão.

Tipo de contrato (contract) – contratos mensais apresentam maior propensão a churn comparados a anuais ou bianuais.

Valor mensal (MonthlyCharges) – clientes com gastos mensais altos têm maior risco.

Total gasto acumulado (TotalCharges) – menor engajamento financeiro total está relacionado a maior evasão.

Serviços contratados (internet, telefone, etc.) – diversidade e qualidade impactam retenção.

🎯 Estratégias de Retenção Recomendadas

Desenvolver campanhas direcionadas para clientes com contratos curtos ou valores mensais elevados.

Monitorar clientes com baixo engajamento financeiro e propor ofertas personalizadas.

Incentivar migração de contratos mensais para planos anuais.

Criar programas de fidelidade para clientes com maior risco identificado pelo modelo.

📂 Estrutura do Projeto

TelecomX_parte2_BR.ipynb → Notebook completo com tratamento, EDA, modelagem e avaliação.

telecom_tratado.csv → Dataset tratado utilizado na análise.

README.md → Documentação do projeto.

▶ Como Executar

Instale as bibliotecas necessárias:

pip install pandas numpy scikit-learn imbalanced-learn matplotlib seaborn

Abrir o Jupyter Notebook e executar:

TelecomX_parte2_BR.ipynb

Certifique-se de que o arquivo telecom_tratado.csv esteja no mesmo diretório do notebook.

📊 Conclusão

O projeto demonstra como combinar performance preditiva (Random Forest) com interpretabilidade estratégica (Regressão Logística) para orientar decisões de retenção. 
A análise permite identificar clientes de maior risco e transformar dados em ações de negócio concretas, equilibrando robustez técnica e aplicabilidade prática.


