# Morbidade Hospitalar do SUS: Doenças Endócrinas, Nutricionais e Metabólicas[cite: 1]

Este repositório apresenta o Projeto 1 de Ciência de Dados, desenvolvido por Abner Soares, focado na análise e modelagem estatística de dados extraídos do portal DATASUS. O estudo investiga os internamentos hospitalares no Brasil causados por doenças endócrinas, nutricionais e metabólicas (Capítulo CID-10: IV), segmentadas por local de residência (Região e UF) e ano de atendimento, compreendendo o período entre janeiro de 2008 e dezembro de 2025.

## Objetivos e Metodologia
* **Pré-processamento:** Tratamento de uma base de dados segmentada por estado, incluindo a remoção de valores ausentes (NaN) e inspeção estatística detalhada.
* **Análise Exploratória Visual:** Utilização de Boxplots para avaliar a distribuição do total geral de casos de morbidade hospitalar no país.
* **Modelagem Linear Global:** Aplicação de Regressão Linear Simples (via Scikit-Learn) nos totais anuais para extrair a equação de tendência de crescimento e a métrica de ajuste da regressão ($R^2$).
* **Regressão OLS Regional:** Execução iterativa de modelos de Mínimos Quadrados Ordinários (via Statsmodels) em cada Unidade da Federação e Região para calcular coeficientes angulares, p-valores de significância estatística e o $R^2$-ajustado de cada localidade.
* **Comparação de Extremos:** Ordenação dos estados baseada na razão entre o coeficiente angular e a média histórica de casos, permitindo visualizar graficamente e comparar as regiões brasileiras com a maior e a menor taxa de crescimento relativo.

## Tecnologias Utilizadas
* **Linguagem:** Python 3
* **Manipulação e Estruturação de Dados:** Pandas, NumPy
* **Visualização Gráfica:** Matplotlib
* **Machine Learning e Estatística:** Scikit-Learn (LinearRegression), Statsmodels (OLS)
