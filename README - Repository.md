# IronHack Brasil
Projetos desenvolvidos durante o curso _Data Analytics_ na Iron Hack Brasil.
Projetos desenvolvidos durante o período de Novembro de 2021 até Maio de 2022.

# Projeto 1: Black Jack
  - Desenvolvimento de um jogo de Black Jack adaptado para ser jogado por 2 pessoas.
  - Para o desenvolvimento desse jogo foram utilizados códigos básicos de Python como: while, for, condicionais e funções.
  - O baralho foi criado a partir de um for loop de listas para formar um dicionário onde a chave é o nome da carta e o valor é a pontuação correspondente da mesma no jogo.
  - As mãos iniciais de cada jogador são sorteadas aleatoriamente a partir de um while loop
  - O jogo se desenvolve a partir de 8 funções que "rodam" entre si até que alguma das condicionais para o final do jogo seja alcançada.

## Tecnologia
PYTHON
  - Tipos e Estruturas de Dados
  - Funções
  - Condicionais
  - Loops

# Projeto 2: Global Shark Attack

  - A partir de uma planilha do Kaggle, levantar dados para desenvolver um projeto sobre ataques de tubarão no mundo.
  - Escoolhi realizar uma campamnha de mkt para prevenir ataques de tubarão nos locais de maior incididência no mundo.
  - A tabela era extensa e com muita 'sujeira'. Foi realizada toda a limpeza e organização dos dados com a biblioteca pandas.
  - Foram levantados os dados descritivos da população e selecionadas as variáveis de maior incidência para definir uma população alvo para a campanha.
  - Informações na internet foram coletadas para entender melhor o comportamento dessa população.
  - Os pontos mais importantes de comunicação para a campanha foram descritos.

## Tecnologia
PYTHON
  - Pandas
  - Numpy
  - Data Cleaning
  - REGEX
  - Análise de Incidência de Variável

# Projeto 3: API ArXiv - Cornell University

  - Desenvolver um trabalho extraindo os dados de uma API
  - Foi selecionada a API de trabalhos científicos da Universidade de Cornell: ArXiv
  - O foco do trabalho foi desenvolver o comportamento das publicações científicas em genética e estresse nos últimos 30 anos.
  - Uma base de 10.000 artigos foram coletados da API pelo python para análise.
  - DataFrames foram gerados a partir das informações consideradas relevantes para o objetivo do projeto.
  - Uma schema do SQL foi construído para armazenar as informações.
  - Um engine foi feito no python para extrair as informações do SQL.
  - Após análise as tabelas foram montadas e subidas para o Tableau para a visualização dos resultados (BI)

## Tecnologia
PYTHON
  - Extração de API
  - Análise, seleção e estruturação dos dados obtidos da API para o Pandas
  - Integração com o SQL
  - Análise Descritiva e Visualização de Dados

SQL
  - Criação de um schema para receber as informações do Python
  - Criação das tabelas e suas relações
  - Armazenamento de Dados
  - Integração com o Python

Tableau
  - BI
  - Visualização de Dados
  - Desenvolvimento de uma História para explicar os resultados

# Projeto de Análise e Ciência de Dados para o E-Commerce
  - Projeto real para um empresa de e-commerce que utilizei como meu trabalho de conclusão de curso.
  - Empresa com 800 produtos vendidos em 19 canais de vendas online. 
  - Projeto: desenvolver modelo de análise de vendas e previsão de demanda para a empresa.
  - Dois modelo foram elaborados:
    - Análise de resultados da semana anterior
    - Análise de resultados da segunda-feira
      - Segunda-feira principal dia de vendas
      - Tomada de deciões comerciais em curto prazo
      - previsão de demanda da semana a partir dos resultados da segunda-feira
  
 ## Tecnologia
 Configuração de um canal VPN (OpenVPN)
 Servidor da empresa = SQL Server
 Conexão Python / SQL pela biblioteca pyodbc
 Desenvolvimento do modelo e finalização dos relatórios utilizando a biblioteca pandas
 Desenvolvimento de ferramenta de Machine Learning com o Catboost Regressor
 
 SQL Server
 Query para extração de todos os pedidos que a empresa recebeu (mais de 500.000 linhas com 84 colunas de informações)
 
 PYTHON
 Integração com o SQL Server
 Projeto 1:
 Análise de volume de vendas, precificação e margem de contribuição
 Relatório de comparação de resultados da semana passada com a média dos últimos 90, 60 e 30 dias
 Clusterização do produto de acordo com os resultados
 Recomendação de ação comercial de acordo com o cluster do produto
 
 Projeto 2:
 Análise de resultados da segunda-feira de cada produto em cada canal de vendas
 Relatório comparativo com as últimas 3 segundas-feiras
 Ferramenta de Machine Learning para fazer a previsão da demanda de cada produto em cada canal de vendas
 Relatório possibilita análise de resultado de curtíssimo prazo e embasa a tomada de decisões comerciais da semana
