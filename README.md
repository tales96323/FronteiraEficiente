# Análise de Fronteira Eficiente com o Modelo de Markowitz

Este projeto realiza uma análise de portfólios utilizando o conceito da **Fronteira Eficiente de Markowitz** para ações da Bolsa Brasileira (B3), com dados obtidos pelo Yahoo Finance. O objetivo é encontrar o portfólio ideal com base na maximização do índice de Sharpe e a minimização da volatilidade (risco), além de plotar a fronteira eficiente.

## Objetivo

O principal objetivo deste projeto é aplicar o modelo de **Fronteira Eficiente de Markowitz** para avaliar o desempenho de diferentes combinações de ações. Utilizando o conceito de otimização de portfólios, é possível identificar carteiras que maximizam o retorno esperado dado um nível de risco ou minimizam o risco para um determinado retorno.

## Dados Utilizados

Os dados foram coletados do Yahoo Finance utilizando a biblioteca `pandas_datareader`. As ações selecionadas foram:

- PETR4.SA (Petrobras)
- VALE3.SA (Vale)
- UNIP6.SA (Unipar)
- FESA4.SA (Ferbasa)
- BPAN4.SA (Banco Pan)

O período de análise foi de 1º de janeiro de 2018 a 31 de dezembro de 2018.

## Metodologia

1. **Coleta de Dados**: Baixamos os preços ajustados das ações do Yahoo Finance.
2. **Cálculo dos Retornos**: Retornos diários e anuais das ações foram calculados a partir dos dados históricos.
3. **Simulação de Carteiras Aleatórias**: Geramos 100.000 carteiras aleatórias com pesos diferentes para cada ação.
4. **Avaliação de Desempenho**: Cada carteira foi avaliada em termos de retorno esperado, volatilidade (risco) e índice de Sharpe.
5. **Fronteira Eficiente**: As carteiras foram plotadas em um gráfico de volatilidade vs. retorno, com a carteira de maior índice de Sharpe e a carteira de menor volatilidade destacadas.

## Resultados

- **Carteira com Maior Índice de Sharpe**: Identificamos a carteira com o melhor retorno ajustado ao risco (maior Sharpe Ratio).
- **Carteira de Mínima Variância**: Identificamos também a carteira com a menor volatilidade (risco mínimo).
- Ambas as carteiras foram destacadas no gráfico da fronteira eficiente.

## Requisitos

- Python 3.x
- Bibliotecas:
  - `pandas`
  - `numpy`
  - `matplotlib`
  - `pandas_datareader`
  - `datetime`

