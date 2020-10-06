# Projeto Machine Learning e segurança pública
## Classificando municípios brasileiros a partir de indicadores socioeconômicos

Monografia de conclusão do curso de pós-graduação Business Intelligence Master, oferecido pelo Laboratório de Inteligência Computacional Aplicada (ICA) da Pontifícia Universidade Católica do Rio de Janeiro (PUC-Rio). Nota: 10/10

Autor: Leandro de Oliveira Capela
Orientadora: Manoela Rabello Kohler

### Tabela de conteúdo
| Arquivo                                | Descrição                                            |
|----------------------------------------|------------------------------------------------------|
| BRAZIL_CITIES.csv			             | Base de dados em CSV			                        | 
| BRAZIL_CITIES.ipynb		             | Código do projeto em iPython Notebook                |  			
| Dicionario_de_Dados.xlsx	             | Dicionário de dados do projeto, em português	        |		
| MISSING_FIELDS.csv		             | Classificação das subcategorias de valores faltantes	| 		
| BI-Master-Monografia_LeandroCapela.pdf | Versão completa do projeto em PDF (59 páginas)       |


### Resumo
O projeto consiste de um estudo supervisionado aplicado de Machine Learning com o objetivo de desenvolver um modelo de classificação que diferencie municípios brasileiros como portadores de violência endêmica ou não. 

A classificação se baseia em uma métrica definida pela Organização Mundial da Saúde (OMS) e [mencionada pelo Banco Mundial em 2016](https://www.worldbank.org/en/news/feature/2016/09/06/urban-violence-a-challenge-of-epidemic-proportions), onde uma taxa de homicídios superior a 10 por 100 mil habitantes em um ano é típica de violência endêmica. 

O trabalho foi desenvolvido partir de um dataset obtido no [Kaggle](https://www.kaggle.com/crisparada/brazilian-cities/) com 87 colunas de dados socioeconômicos a partir de múltiplas fontes, como grau de escolaridade por faixa etária, taxa de desemprego, arrecadação com impostos, número de empresas por atividade econômica, ativos bancários, entre outros, que estão detalhados no dicionário de dados. 

O dicionário de dados foi fornecido na própria plataforma, em inglês, contendo o detalhamento dos nomes das colunas, descrições dos campos, períodos de referência, unidades de medida e fontes. No desenvolvimento deste projeto, as informações foram traduzidas para o português. Além disso, foi realizada atualização de parte dos dados, adição de 13 novos campos e transformação de 10 colunas de números absolutos para percentuais ou taxas. 

Foram empregadas diversas etapas de pré-processamento, como criação de variáveis binárias a partir de categóricas, tratamento de valores faltantes, tratamento de outliers, balanceamento, normalização e redução de dimensionalidade. 

Após combinar e testar todas essas técnicas, os resultados foram comparados, frente ao uso de Regressão Logística, Support Vector Machine (SVM), Random Forest e k-Nearest Neighbors (k-NN). 

O modelo de classificação com melhor desempenho foi construído com Random Forest, onde os atributos, tratados com balanceamento, normalização, Kernel PCA e t-SNE explicam mais de 80% da classificação.
