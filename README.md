# Projeto Previsão de Rotatividade de Clientes - Interconnect

## Descrição do Projeto

Este foi o projeto final apresentado do meu bootcamp de Ciência de dados, foi desenvolvido com a operadora fictícia de telecomunicações **Interconnect** para prever a **rotatividade de clientes** (churn) com base em dados contratuais, pessoais, e de serviços de internet e telefonia. O objetivo é criar um modelo que ajude a empresa a identificar quais clientes estão mais propensos a cancelar os serviços, permitindo uma tomada de decisão mais eficaz na retenção de clientes.

## Ferramentas e Bibliotecas Utilizadas

- **Python**: Linguagem utilizada para o desenvolvimento do projeto.
- **Pandas**: Para manipulação e análise dos dados.
- **NumPy**: Para operações matemáticas e manipulação de arrays.
- **Scikit-learn**: Para implementação de modelos de machine learning e avaliação.
- **Optuna**: Para otimização de hiperparâmetros.
- **SHAP**: Para explicabilidade dos modelos.
- **Matplotlib/Seaborn**: Para visualização de dados.
- **Keras**: Para carregamento de dados de imagens e pré-processamento.

## Descrição dos Dados

Os dados utilizados neste projeto foram divididos em quatro arquivos CSV:
- **contract.csv**: Informações contratuais, como tipo de contrato e método de pagamento.
- **personal.csv**: Dados pessoais dos clientes, como faixa etária e estado civil.
- **internet.csv**: Informações sobre o uso de serviços de internet.
- **phone.csv**: Detalhes sobre os serviços de telefonia.

### Principais Colunas Utilizadas:
- **tenure**: Tempo de permanência do cliente.
- **total_charges**: Valor total cobrado.
- **has_internet**: Indica se o cliente possui serviço de internet.
- **contract**: Tipo de contrato (mensal, anual).
- **churn**: Variável alvo (0 para clientes que não cancelaram, 1 para clientes que cancelaram).

## Etapas do Projeto

1. **Exploração e Análise de Dados (EDA)**: Limpeza e análise inicial dos dados para identificar padrões e preparar o conjunto de dados.
2. **Pré-processamento**: Transformação de variáveis categóricas, normalização e tratamento de valores faltantes.
3. **Engenharia de Features**: Criação de novas variáveis.
4. **Treinamento de Modelos**: Teste de múltiplos modelos de machine learning, incluindo **XGBoost**, **Random Forest**, **Logistic Regression** e **Gradient Boosting**.
5. **Otimização de Hiperparâmetros**: Utilização do **Optuna** para otimizar os hiperparâmetros dos modelos.
6. **Avaliação de Modelos**: Comparação de métricas como **AUC ROC**, **F1-Score**, **Acurácia** e análise de erros.
7. **Análise dos Resultados**: Avaliação das predições com base em características dos clientes, utilizando o **SHAP** para entender as principais features que impactam a rotatividade.

## Conclusão

O modelo final escolhido foi o **XGBoost**, que apresentou a melhor performance com uma **AUC ROC** de 0.8516. A **Regressão Logística** também se destacou pela simplicidade e interpretabilidade, mostrando uma boa combinação de **Acurácia** e **F1-Score**. A empresa **Interconnect** pode utilizar esses insights para melhorar suas estratégias de retenção de clientes, focando nas características que mais impactam a rotatividade, como o tipo de contrato e a presença de internet de fibra ótica.

## Aprendizados

Este projeto permitiu-me desenvolver as seguintes habilidades:
- **Engenharia de Features**: Criação e seleção de features relevantes para melhorar a performance dos modelos.
- **Treinamento de Modelos de Machine Learning**: Aprendizado sobre como configurar e treinar modelos de classificação binária, como **XGBoost**, **Random Forest** e **Logistic Regression**.
- **Otimização de Hiperparâmetros**: Aplicação de técnicas avançadas de otimização, como o **Optuna**, para encontrar as melhores configurações de hiperparâmetros.
- **Interpretação de Modelos com SHAP**: Compreensão profunda de como cada feature impacta o modelo, utilizando gráficos de dependência e importância.
- **Análise Descritiva e Exploratória de Dados**: Investigação de distribuições e correlações para entender o comportamento dos clientes e seus serviços.


## Como Executar o Projeto

- Clone o repositório.
- Navegue até o diretório do projeto.
- Abra o projeto no seu IDE favorito.
- Instale as dependências.
- Execute o script principal.

## Contato

Luciano Pinto
[LinkedIn](https://www.linkedin.com/in/lucianolcp/)  
Email: dslucianopinto@gmail.com
