# Análise de Variação Percentual Entre USD/BRL e USDT/BRL

## Descrição do Projeto

Este projeto analisa a variação percentual entre os pares USD/BRL e USDT/BRL em blocos de tempo de 4 horas, divididos entre períodos de mercado aberto e fechado. O foco está em observar o comportamento dos preços em diferentes condições de mercado, incluindo eventos de grande instabilidade econômica, como a "Black Monday" de 5 de agosto de 2024.

A análise foi realizada utilizando Python, com bibliotecas como `Pandas`, `Plotly` e `Matplotlib` para visualização interativa e exploração de dados.

## Objetivo

O objetivo deste projeto é identificar:
- Diferenças percentuais entre USD/BRL e USDT/BRL durante o horário comercial e fora dele.
- Comportamento das variações em eventos de grande impacto econômico.
- Padrões e oportunidades de arbitragem baseados nas variações observadas.

## Metodologia

- **Coleta de Dados**: Os dados de USD/BRL foram extraídos de fontes públicas como Yahoo Finance, enquanto os dados de USDT/BRL foram obtidos da Binance. O período analisado compreende os últimos 6 meses.
- **Divisão de Blocos de Análise**: 
  - Horário Comercial (9h - 18h): 
    - Bloco 1: 9h - 13h 
    - Bloco 2: 13h - 17h 
    - Bloco 2.1: 17h - 18h 
  - Fora do Horário Comercial (18h - 9h): 
    - Bloco 3: 18h - 22h 
    - Bloco 4: 22h - 2h 
    - Bloco 5: 2h - 6h 
    - Bloco 6: 6h - 9h
- **Análise Estatística**: Foram calculadas as diferenças percentuais médias, máximas e mínimas para cada bloco de tempo, além de testes de correlação e métricas estatísticas como desvio padrão e coeficiente de variação.

## Resultados

Os principais resultados indicam que as maiores variações percentuais ocorrem fora do horário comercial, com o Tether (USDT) mantendo-se mais valorizado que o dólar (USD) nesses períodos, sugerindo oportunidades de arbitragem no mercado de criptomoedas.

## Requisitos

- Python 3.X
- Bibliotecas: 
  - `Pandas`
  - `Plotly`
  - `Matplotlib`

## Como Executar

1. Clone este repositório:
   ```bash
   git clone https://github.com/gustavoesteves0/eNor
   ```
2. Instale as dependências:
   ```bash
   pip install -r requirements.txt
   ```
3. Execute o notebook ```main.ipynb``` para gerar as análises e visualizações.

## Arquivos Principais
- ```main.ipynb```: Notebook contendo a coleta, processamento e análise dos dados.
- ```relatorio.pdf```: Relatório detalhado com gráficos e insights da análise.
