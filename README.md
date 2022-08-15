# Projeto E.D.A - Sazonalidade Temporal Ibovespa

__Bussines Problem:__  


> Durante a rotina de investimentos torna-se atrativo ter uma estimativa de análise da série histórica de dados para análise de melhores meses do ponto de vista de probabilidade de retorno positivo ou negativo e retorno de investimento médio esperado.


__Business Problem Question:__

> __“Existe melhor mês para investimento no índice Ibovespa se sim qual mês ao longo da série histórica tendem a ser mais positivos e rentáveis para compra ou venda ?”__

> A resposta dessa pergunta aliada a outros fatores como análise de cenário macroeconômico dentre outros pontos podem contribuir para a instituição na melhoria dos resultados e performance.      
  
__Objetivo:__   

> Desenvolver um script que realiza a análise exploratória da série histórica do índice Ibovespa e possibilita verificar quais os meses foram mais positivos,negativos atrativos do ponto de vista da rentabilidade para a compra e para venda.

__Autor:__  
   - Bruno Priantti.
    
__Contato:__  
  - bpriantti@gmail.com

__Encontre-me:__  
   -  https://www.linkedin.com/in/bpriantti/  
   -  https://github.com/bpriantti
   -  https://www.instagram.com/brunopriantti/

__Frameworks Utilizados:__

Numpy:
https://numpy.org/doc/
Pandas:
https://pandas.pydata.org/
Matplotlib:
https://matplotlib.org/
Seaborn:
https://seaborn.pydata.org/
Plotly:
https://plotly.com/

___

__Project Steps__

Realizou-se o processo de ETL com a API de dados, yfinance e com isso obteve-se a série histórica do índice ibovespa desde de 1995 a 2021:

![alt text](https://github.com/bpriantti/projetoEDA_sazonalidade_temporal_ibovespa/blob/main/images/adj_close_ibov.png?raw=true)

Em seguida realizou-se todo o processo de wralling dos dados a fim de obter os dados retornos da série histórica agrupados por meses e anos, analisou-se também a distribuição dos retornos mensais com os gráficos de distribuição e boxplot.

![alt text](https://github.com/bpriantti/projetoEDA_sazonalidade_temporal_ibovespa/blob/main/images/image_1.png?raw=true)

Com a obtenção da série de retornos mensais agrupou-se os dados a fim de obter um gráfico de heatmap mesesxanosxretornos da série histórica.

![alt text](https://github.com/bpriantti/projetoEDA_sazonalidade_temporal_ibovespa/blob/main/images/image_2.png?raw=true)

Analisou-se também o gráfico de boxplot dos retornos mensais do índice, como demostrado abaixo:

![alt text](https://github.com/bpriantti/projetoEDA_sazonalidade_temporal_ibovespa/blob/main/images/image_3.png?raw=true)

Novamente realizou-se o processo de data wralling e obteve-se a tabela abaixo:

![alt text](https://github.com/bpriantti/projetoEDA_sazonalidade_temporal_ibovespa/blob/main/images/table.PNG?raw=true)

# Resultados Obtidos:
___
&nbsp;  
tornou-se possível concluir com a análise exploratória dos dados ao final do estudo que:
&nbsp;  

__Sazonalidade Temporal Ibovespa:__ 
&nbsp;
       
Ativo: ^BVSP Periodo:  1995-01-01 a 2022-06-30 :
 
- Quais são os meses que mais tendem a fechar positivo?
&nbsp;    
> R:   ['dec' 'abr' 'jul']
 
- Quais são os meses que mais tendem a fechar negativo?
> R:   ['jan' 'mai' 'mar']
 
- Quais são os meses que mais tendem a serem rentaveis para a compra?
> R:   ['nov' 'abr' 'dec']
 
- Quais são os meses que mais tendem a serem rentaveis para a venda? 
> R:   ['ago' 'mai' 'jun']
 
- Quais são os meses que mais tendem a serem rentaveis para a compra e a fecharem positivos ?
> R:   ['dec' 'abr' 'jul']
 
- Quais são os meses que mais tendem a serem rentaveis para a venda e a fecharem negativos ?
> R:   ['mai' 'jan' 'ago']
 
- Qual trimestre tende a fechar mais positivo ?
> R:   tri4
 
- Qual trimestre tende a fechar mais negativo ?
> R:   tri1
