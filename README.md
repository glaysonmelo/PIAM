# Projeto Integrado em Aprendizado de Máquina

### PREDIÇÃO DO PREÇO DE FECHAMENTO DO ÍNDICE BOVESPA

Índice Bovespa (Ibovespa) é o mais importante indicador do desempenho médio das cotações das ações negociadas na B3 - Brasil, Bolsa, Balcão. É formado pelas ações com maior volume negociado nos últimos meses. O valor atual representa a quantia, em moeda corrente, de uma carteira teórica de ações, constituída em 2 de janeiro de 1968, a partir de uma aplicação hipotética.


O objetivo deste trabalho é utilizar Machine Learning para prever o preço de fechamento do indice bovespa.

### PROBLEMA

Esse problema está centrado em prever o preço de fechamento do índice Bovespa na bolsa de valores brasileira - B3.
Essa previsão é um modelo acadêmico e não deve ser utilizado como base para a compra e venda do índice na bolsa de valores, pois o preço de uma ação
depende de N fatores e neste trabalho foi levado em concideração somente os dados históricos do índice para prever o preço de fechamento.

### BASE DE DADOS

Foi extraido do site da Yahoo Finance os dados historicos do índice Bovespa, referente ao periodo de 01/2010 a 12/2020

A base de dados possui os seguintes campos:


<ul>
  <li>Date - Data do Pregão</li>
  <li>Open - Preço de abertura da ação</li>
  <li>High - Maior preço da ação no dia</li>
  <li>Low  - Menor preço da ação no dia </li>
  <li>Close - Preço de fechamento da ação</li>
  <li>Adj Close - Preço de fechamento da ação ajustado</li>
  <li>Volume - Volume de negociações</li>
</ul>


### SOLUÇÃO

Para resolver esse problema, primeiro vamos construir um modelo de Machine Learning. Em seguida, treinaremos o modelo nos dados existentes, avaliaremos se ele é bom e, por fim, consumiremos o modelo para prever o valor do índice IBOV.

## PIPELINE

### 1.0 CONSTRUÇÃO DO MODELO

A construção do modelo inclui obter os dados, tratar os dados, transformar os dados para que possam ser usados de forma eficaz pelo algoritmo de Machine Learning

### 2.0 TREINAR O MODELO

Treinar o modelo é um processo de execução do algoritmo escolhido em dados de treinamento (com valores do índice conhecidos) para ajustar os parâmetros do modelo.

### 3.0 AVALIANDO O MODELO

Precisamos desta etapa para concluir o quão preciso nosso modelo opera em novos dados. Para fazer isso, o modelo da etapa anterior é executado em outro conjunto de dados que não foi usado no treinamento. Este conjunto de dados também contém valores do índice conhecidos.

### 4.0 CONSUMINDO O MODELO

Depois que o modelo é treinado, podemos usar para prever o valor do índice basedo nos dados de entrada.

Finalmente, o gráfico como as previsões testadas são distribuídas e como a regressão está se saindo, como na seguinte captura de tela:

![Gráfico](https://user-images.githubusercontent.com/33094333/102024245-ac851880-3d6f-11eb-9655-d05e1281a3ad.JPG?raw=true)
