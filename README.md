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

Treinar o modelo é um processo de execução do algoritmo com dados de treinamento (com valores do índice ibovespa conhecidos) para ajustar os parâmetros!

Neste experimento, utilizamos os três algoritmos

<ul>
  <li>Rede Neural Hyper Parameters</li>
  <li>Rede Neural</li>
  <li>Regressao Linear</li>  
</ul>

No final, selecionamos o algoritimo que teve o melhor Coeficiente de determinação.

### 3.0 AVALIANDO O MODELO

Precisamos desta etapa para concluir o quão preciso nosso modelo opera em novos dados. Para fazer isso, o modelo da etapa anterior é executado em outro conjunto de dados que não foi usado no treinamento. Este conjunto de dados também contém valores do índice conhecidos.

        real       previsao
Data                               
2020-11-18  106517.0  107023.123491
2020-11-19  107379.0  109291.164456
2020-11-23  109786.0  110095.507200
2020-11-24  110133.0  109565.992407
2020-11-25  110227.0  109578.491358
2020-11-26  110575.0  110433.122800
2020-11-27  108888.0  109656.578859
2020-11-30  111335.0  111659.787210
2020-12-01  111814.0  112454.340161
2020-12-02  112919.0  112465.236538
2020-12-03  113682.0  113207.474584
2020-12-04  113625.0  113641.669186
2020-12-07  113571.0  113255.709175
2020-12-08  112722.0  114137.534135

### 4.0 CONSUMINDO O MODELO

Depois que o modelo é treinado, podemos usar para prever o valor do índice basedo nos dados de entrada.

Finalmente, o gráfico como as previsões testadas como a regressão está se saindo

![Gráfico](https://user-images.githubusercontent.com/33094333/102024245-ac851880-3d6f-11eb-9655-d05e1281a3ad.JPG?raw=true)
