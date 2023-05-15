# Detecção de Fraudes em Cartões de Crédito
<sub> TAGS: Aprendizado de Máquina; Segmentação Supervisionada; Análise Exploratória de Dados; Visualização de Dados

Neste projeto, desenvolvi dois modelos de aprendizado supervisionado com a finalidade de detectar fraudes em cartões de crédito. Os dados consistem de transações realizadas por clientes europeus num período de 48 horas. Foi realizada a análise exploratória dos dados, para investigar valores nulos, *outliers* e padrões nos atributos que contribuiriam para a construção do modelo posteriormente.
  
<p align="center">
  <img src="capa_p3.png" >
</p>
  
Os dados originais foram separados entre um conjunto de treino e de teste. Dentro do conjunto de treino, fiz mais um separação com subconjuntos de treino e validação (*holdout set*, ou conjunto de retenção), com os quais construiria o modelo e faria as previsões. Assim, foram construídos um modelo de regressão logística e um de árvore de decisão, e seus desempenhos comparados. Ao aplicar nos dados de teste, que consistiam em 20% do conjunto original, obtivemos:
  
* Modelo de Regressão Logística: 
  * Acurácia: 95,8%
  * AUC: 95,4
  
* Modelo de Árvore de Decisão:
  * Acurácia: 96,4%
  * AUC:      92,8%

Tendo em vista as métricas de desempenho nos dados de teste, comparando o número de fraudes detectadas, bem como a proporção de Falso Positivos e Falsos Negativos, concluiu-se que o melhor modelo para detecção de fraudes em cartões de crédito, nesse contexto, é o de regressão logística.
