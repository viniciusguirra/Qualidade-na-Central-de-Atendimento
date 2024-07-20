# Projeto: Qualidade na Central de Atendimento

## Descrição do Projeto

Este projeto foi realizado em conjunto com a Escola de Dados Preditiva.ai e visa identificar os fatores mais associados ao bom desempenho de agentes de atendimento em uma empresa de Contact Center. Utilizamos dados coletados através do Survey Monkey durante o processo de contratação dos agentes e avaliamos o desempenho dos mesmos após seis meses.

## Objetivo

O objetivo é entender quais características dos agentes contratados estão mais associadas a um bom desempenho, para otimizar os processos de recrutamento e treinamento futuros.

## Estrutura do Projeto

- **ETL (Extract, Transform, Load)**: Processamento e limpeza dos dados brutos.
- **Análise Exploratória de Dados (EDA)**: Investigação inicial dos dados para entender suas características principais.
- **Modelagem Preditiva**: Utilização do modelo CatBoost para identificar as variáveis mais importantes associadas ao desempenho dos agentes.
- **Avaliação do Modelo**: Avaliação da performance do modelo e interpretação dos resultados.
- **Recomendações**: Sugestões de ações baseadas nos insights obtidos.

## Ferramentas e Bibliotecas Utilizadas

- **Python**: Linguagem de programação principal.
- **Pandas**: Manipulação e análise de dados.
- **CatBoost**: Biblioteca de machine learning para modelagem preditiva.
- **Scikit-learn**: Biblioteca para avaliação de modelos.
- **Matplotlib e Seaborn**: Visualização de dados.
- **Statsmodels**: Análise estatística.
- **Shap**: Visualização features do modelo. 

## Resultados

Após o treinamento do modelo CatBoost, as variáveis mais importantes associadas ao bom desempenho dos agentes foram:

| **Feature** | **Importance** |
|-------------|----------------|
| Cliente | 55.67% |
| Disponibilidade para trabalhar em casa | 4.58% |
| Possuir dependentes | 4.34% |
| Experiência anterior com vendas | 3.84% |
| Trabalhar bem com colegas | 2.70% |

### Métricas de Avaliação do Modelo

- **Accuracy**: 67.86%
- **ROC AUC**: 72.78%
- **Precision**: 69.63%
- **Recall**: 77.28%
- **F1 Score**: 73.26%
- **Confusion Matrix**:
  - Verdadeiro Positivo: 956
  - Verdadeiro Negativo: 518
  - Falso Positivo: 417
  - Falso Negativo: 281

## Recomendações

1. **Ajuste no Recrutamento**:
   - Focar no histórico dos candidatos em relação ao tipo de cliente atendido previamente, disponibilidade para trabalho remoto e experiência em vendas.

2. **Ambiente de Trabalho**:
   - Proporcionar suporte para que mais agentes possam trabalhar de casa, se isso for viável e benéfico.

3. **Treinamento Focado**:
   - Desenvolver treinamentos específicos para melhorar a colaboração entre colegas e a gestão de responsabilidades pessoais e profissionais.

4. **Avaliação Contínua**:
   - Monitorar periodicamente a importância das variáveis e ajustar o modelo conforme novos dados são coletados.

## Como Executar o Projeto

1. Clone este repositório:
   ```bash
   git clone https://github.com/viniciusguirra/Qualidade-na-Central-de-Atendiment
