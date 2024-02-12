# Previsão de Preços de Aluguel em Nova York

## Visão Geral
Este projeto tem como objetivo resolver um problema de regressão, prevendo os preços dos aluguéis na cidade de Nova York. Foram utilizadas duas bases de dados: `teste_indicium_precificacao` e `NY-House-Dataset`.

## Notebooks
O projeto está dividido em dois Notebooks principais:
1. **Análise Exploratória de Dados**: [Precificacao_Indicium_EDA](https://github.com/lazarocordeirosilva/LH_CD_LAZARO_CORDEIRO/blob/main/notebook/Precificacao_Indicium_EDA.ipynb)
   - Realizou-se uma análise exploratória de dados abrangente, investigando várias hipóteses de negócios e respondendo a perguntas específicas propostas pelo desafio.

2. **Modelagem Preditiva**: [Modelagem e Previsão](https://github.com/lazarocordeirosilva/LH_CD_LAZARO_CORDEIRO/blob/main/notebook/Modelagem%20e%20Previs%C3%A3o.ipynb)
 ### Implementaram-se técnicas de:
   - Codificação de variáveis (Ordinal Encoder)
   - Normalização de dados (MinMaxScaler)
   - Feature Engineering e estratégias de imputação de dados, todas testadas com Cross-Validation.
   - O modelo vencedor teve seus hiperparâmetros otimizados por meio da classe BayesianSearchCv.

## Bases de Dados
- [teste_indicium_precificacao](https://github.com/lazarocordeirosilva/LH_CD_LAZARO_CORDEIRO/blob/main/data/teste_indicium_precificacao.csv)
- [NY-House-Dataset](https://github.com/lazarocordeirosilva/LH_CD_LAZARO_CORDEIRO/blob/main/data/NY-House-Dataset.csv)

## Como Executar o Projeto
### Configuração do Ambiente Virtual
> [!NOTE]
> Clone o repositório para o seu ambiente local (você pode utilizar um ambiente virtual para gerir as dependências corretamente).
```
git clone https://github.com/lazarocordeirosilva/LH_CD_LAZARO_CORDEIRO.git
```

> [!NOTE]
> Após isso, você pode instalar os requisitos nas versões utilizadas
```
pip install -r requirements.txt
```

### Execução dos Notebooks
1. Abra o Jupyter Notebook.

2. Execute os Códigos (códigos do modelo Ensemble Random Forest Regressor podem ter tempo de execução elevado).

## Requisitos
Neste projeto, foi utilizada a versão 3.11.4 do Python

A versão do pip utilizada é a 23.3.1

A versão do git utilizada é a 2.42.0

Demais requisitos se encontram no arquivo requirements.txt

## Estrutura do Projeto

```
├── LICENSE
├── README.md                                      <- README.md com principais informações do projeto.
│
├── data
│   ├── NY-House-Dataset                           <- Dados baixados no Kaggle acerca do preço dos imóveis em Nova York.
│   └── test_indicium_precificacao                 <- Base de dados disponibilizada no desafio.
│
├── imagens                                        <- Contém imagens utilizadas no Jupyter Notebook de modelagem e Machine Learning.
│
├── notebook                                       <- Jupyter notebook contendo toda a manipulação de dados e modelagem.
│   ├── Modelagem e Previsão.ipynb                 <- Jupyter notebook para análises preditivas.
│   ├── Precificacao_Indicium_EDA.ipynb            <- Jupyter notebook para análise exploratória dos dados.
│
├── modelo                                         <- Contém modelo de regressão linear final em formato .pkl 
│
├── relatorio                                      <- Contém relatório em pdf da análise exploratória de dados.
│ 
├── requirements                                   <- Todas as bibiliotecas utilizadas (em cada versão). Arquivo gerado com 'pip freeze > requirements.txt'

