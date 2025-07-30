# Correlação entre a medida da cintura e do pescoço
## Introdução
  Existe uma crença popular que diz “você não precisa experimentar uma calça no
provador para ver se serve, basta você envolver a largura da cintura da calça em volta do
pescoço onde o colarinho de camisa cai, se servir então a calça serve. Se as extremidades da
cintura não se encontrarem na parte de trás do seu pescoço, a calça ficará apertada e se a
cintura se sobrepuser, a calça ficará larga”. (Oghenemavwe, 2016)
  Para avaliar a veracidade dessa crença, é necessário recorrer a ferramentas estatísticas
que permitam investigar a existência de uma relação quantitativa entre as variáveis
envolvidas. Uma dessas ferramentas é a regressão linear, uma técnica utilizada na área de
inferência estatística, cujo objetivo é estudar a relação entre variáveis. Essas variáveis são
definidas conforme o tipo de modelo. O modelo de regressão simples é adotado para
investigação da relação entre variável dependente ou variável resposta, representado por (Y)
e variável independente, representada por (X).
  Para fortalecer a análise e garantir maior confiabilidade às estimativas obtidas,
pode-se empregar o método Bootstrap, que é caracterizado pela realização de procedimentos
de reamostragem com reposição. Essa abordagem é útil, pois permite avaliar os resultados
adquiridos, a fim de elevar o nível de confiabilidade construindo intervalos de confiança.
  Dessa forma, este trabalho tem como objetivo investigar a relação entre a
circunferência da cintura e a do pescoço, com o intuito de avaliar a veracidade da crença
popular de que, ao dobrar uma calça ao redor do pescoço, é possível prever se ela servirá ou
não na cintura.

## Materias e métodos
### Coleta de dados
  O estudo utilizou dados obtidos através de amostragem não probabilística, composta
por 20 pessoas de diversas faixas etárias, pesos e alturas. Cada unidade amostral obteve duas
medidas, a circunferência do pescoço, medida com a unidade experimental olhando para a
frente, com os ombros relaxados e com uma fita métrica ao redor do pescoço logo abaixo do
pomo de Adão (osso hióide), e a cintura, medida com os braços relaxados ao lado do corpo e
a fita métrica ao redor do umbigo.
  A amostragem foi feita por 3 pesquisadores diferentes, utilizando fitas métricas
diferentes, o que pode ter introduzido variações entre os processos de medição. Além disso,
algumas das unidades amostrais são membros da mesma família, o que pode gerar correlação
entre as observações dos dados, pois, membros do mesmo núcleo familiar tendem a
compartilhar características corporais semelhantes em algumas medida. Logo, esses fatores
podem ter comprometido a independência entre as medições e os resultados gerados podem
apresentar discrepâncias com relação ao cenário populacional real. O conjunto pode ser 
acessado no arquivo data.csv

### Bibliotecas e funções
  No códgio foram utilizados as bibliotecas:

## Resultados
  Como resultados das análises realizadas, obtivemos o gráfico da regressão linear
com a distribuição da cintura e pescoço, onde podemos notar que há uma relação
positiva entre o crescimento da cintura e aumento do pescoço.
  Depois, para simular como os coeficientes se comportam em múltiplos cenários e se
aproximam dos verdadeiros coeficientes, foi utilizado o método de bootstrap, que gerou
5.000 amostras de 20 conjuntos de dados com reposição, aplicando a regressão linear para
cada amostra e armazenando os coeficientes. Assim, foi possível calcular a média, erro
padrão, desvio padrão e intervalo de confiança aos quais geraram os seguintes valores:
Parâmetro Estimado DP (Bootstrap) IC 95% (Bootstrap)
Intercepto (β0) −14,55 14,08 [-35,28 ; 7.72]
Pescoço (β1) 2,69 0,3497 [2,13 ; 3,18]
  Por último, com dos dados obtidos, foi possível construir um histograma para
verificar a frequência do coeficiente angular (β1) e sua distribuição sobre as amostras. No
gráfico também podem ver as linhas do intervalo de confiança em 2,13 e 3,18 que define os
95% de confiança (linhas vermelhas pontilhadas).

## Conclusão
  Por meio dos resultados obtidos, a pesquisa indicou que a medida do pescoço e
cintura são positivamente correlacionadas, ou seja, a medida que uma aumenta a outra
também aumenta. 
  Sendo assim, ao aplicar a análise bootstrap, com 5.000 reamostragens, obteve-se uma
robusta estimativa do coeficiente, apresentando um intervalo de confiança de 95% entre 2,13
e 3,18, o que significa que a cada 1 centímetro de circunferência do pescoço, a
circunferência da cintura aumenta entre 2,13 e 3,18 centímetros.
  Esses resultados reforçam o potencial da medida do pescoço como um indicador
alternativo ou complementar à medida da cintura, podendo ser utilizado em casos onde não se
pode experimentar propriamente uma calça, por exemplo. Assim, os resultados estatísticos
deste estudo fornece suporte a crença popular que motivou esta investigação.










