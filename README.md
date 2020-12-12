# Projeto Integrado em Aprendizado de Máquina

### PREDIÇÃO VALOR AÇÃO DA BOLSA DE VALORES


Esse problema está centrado em prever o valor da Ação da empresa Itaú Unibanco (ITUB3) na bolsa de valores B3.
Essa previsão é um modelo academico e não deve ser utilizado como base para e compra e vendas de ações, pois o valor de uma ação
depende de N fatores e neste modelo foi levado em concideração somente dos dados historicos da ação.


### BASE DE DADOS

Foi extraido do site da yahoo finance os dados historicos da ação ITUB3 do periodo  01/2010 a 12/2020

A base de dados possui os seguintes campos:


<ul>
  <li>Date - Data do Pregão</li>
  <li>Open - Valor de abertura da ação</li>
  <li>High - Maior valor da ação no dia</li>
  <li>Low  - Menor valor da ação no dia </li>
  <li>Close - Valor de fechamento da ação</li>
  <li>Adj Close - </li>
  <li>Volume - Volume de negociações do dia</li>
</ul>





### BASE DE DADOS


Banco de dados SQL e csv.


### TARGET

Modelo que identifica o perfil de funcinários dado o preenchimento de formulários.


### Algumas questões

<ul>
  <li>Pessoas Jovens no seu primeiro emprego geram melhores resultados?</li>
  <li>Pais de família ficam mais tempo no emprego?</li>
  <li>Pais de família geram melhores resultados?</li>
  <li>Qual ou quais dos dados pessoais tem maior correlação com o perfil de bom profissional?</li>
  <li>Existe algum perfil que devo evitar na hora de contratar?</li>
  <li>Anonimização dos Dados (LGPD)</li>
  <li>Evitar o preconceito (classe, cor , sexo etc)</li>
</ul>

### Dados


O setor de RH possui dados pessoais dos colaboradores e do processo de seleção


<ul>
  <li>Nome</li>
  <li>Nascimento</li>
  <li>Telefone</li>
  <li>CPF</li>
  <li>RG</li>
  <li>CNH/Categoria</li>
  <li>Já teve outro emprego</li>
  <li>Estuda atualmente</li>
  <li>Especialização</li>
  <li>Estado Civil</li>
  <li>Possui rede social</li>
  <li>Frequência do uso de celular</li>
  <li>Pratica esporte</li>
</ul>

##### Exemplo

![Tabela_Dados](https://user-images.githubusercontent.com/33094333/98309849-4b1c9d80-1faa-11eb-8475-341691d020a6.JPG)

### Solução


Para resolver esse problema, vamos construir e treina um modelo de ML com dados de treinamento existentes, avalia se ele é bom (analisando as métricas obtidas) e, por último, pode consumir/testar o modelo para traçar o perfil do profissional através dos dados de entrada.



