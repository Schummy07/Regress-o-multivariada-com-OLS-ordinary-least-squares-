# Regress-o-multivariada-com-OLS-ordinary-least-squares-

A biblioteca rotina_doe.py foi desenvolvida com as funções necessárias para realizar a otimização de métodos ou formulações através do método da superfície de resposta (RSM - Response Surface Method). Essa biblioteca contém as seguintes funções: 

======================================================================================================================================================================
- DoE: função que replica de forma fiel a rotina "regression2" exposta no livro "Planejamento Fatorial em Química: Maximizando a Obtenção de resultados".
- deve receber como input:
  A matriz X printa
  O vetor y
  SQEP - quanto não houver réplicas, será 0
  graus de liberdade da SQEP

- outputs:
  output.xlsx: arquivo em excel contendo a tabela ANOVA, os coeficientes de regressão com os respectivos intervalos de confiança, resultados previstos e resultados obtidos 
  
=========================================================================================================================================================================
- super_DoE: rotina descrita no arquivo de resumo
- inputs:
  A matriz X
  O vetor y

- outputs:
  lista_reg - lista com os coeficientes de regressão obtidos em cada ciclo, também contém o a variância, o erro e o intervalo de confiança de cada coeficientes obtidos em cada ciclo.
  lista_prev - lista com os resultados previstos obtidos em cada ciclo.
  Resultados_DoE.xlsx - arquivo em excel contendo os dados das listas acima

  ==========================================================================================================================================================================
- replicas: rotina que identifica os experimentos com as mesmas condições (réplicas)
- inputs:
  A matriz X
  O vetor y
 
- outputs:
  conj_replicas - lista com os conjuntos de réplicas, identificando as condições experimentais das mesmas
  ind_repli - indice dos conjuntos de réplicas
  replicas - os resultados obtidos em cada réplica
  descritivo - as medidas descritivas obtidas para cada conjunto de réplicas

    
