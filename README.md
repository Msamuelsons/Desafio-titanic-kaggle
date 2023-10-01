# Desafio titanic kaggle

## Titanic - Predicting Survival
Nesse desafio, pedimos que você construa um modelo preditivo que responda à pergunta: “ que tipo de pessoas eram mais propensas a sobreviver? ” usando dados de passageiros ( ou seja, nome, idade, sexo, classe socioeconômica, etc ).

<img src="https://upload.wikimedia.org/wikipedia/commons/thumb/d/db/Titanic-Cobh-Harbour-1912.JPG/330px-Titanic-Cobh-Harbour-1912.JPG" />



## Descrição
Este projeto tem como objetivo prever se os passageiros a bordo do RMS Titanic sobreviveram ao desastre ou não. Os dados utilizados neste projeto foram obtidos do Kaggle, no seguinte link: [Dataset do Titanic](https://www.kaggle.com/competitions/titanic/data?select=train.csv).

## Requisitos
- Python 3
- Bibliotecas Python: pandas, numpy, scikit-learn

## Conjunto de Dados
Os dados estão divididos em dois arquivos CSV:
- `train.csv`: Usado para treinamento do modelo.
- `test.csv`: Usado para teste e avaliação do modelo.

## Pré-processamento de Dados
- Os valores ausentes na coluna 'Embarked' foram preenchidos com o valor mais frequente.
- As colunas 'Name', 'Ticket', 'PassengerId' e 'Cabin' foram removidas por não serem consideradas relevantes para a previsão.
- Os valores ausentes na coluna 'Age' foram preenchidos com a mediana.
- As colunas categóricas 'Sex' e 'Embarked' foram codificadas como variáveis dummy.

## Modelagem
- Utilizou-se um modelo de classificação Gradient Boosting Classifier para prever a sobrevivência dos passageiros.
- Foram realizadas validações cruzadas para avaliar o desempenho do modelo.

## Melhores Parâmetros
- Realizou-se uma busca de grid para encontrar os melhores parâmetros do modelo, com ênfase na taxa de aprendizado (learning rate).

## Resultados
- O desempenho do modelo foi avaliado utilizando validação cruzada.
- O valor da melhor taxa de aprendizado encontrada foi impresso juntamente com a pontuação correspondente.

## Como Executar
1. Certifique-se de ter Python 3 instalado no seu ambiente.
2. Instale as bibliotecas Python necessárias (pandas, numpy, scikit-learn).
3. Clone este repositório.
4. Execute o código em um ambiente adequado (por exemplo, Jupyter Notebook).

## Autor
Msamuelsons

## Referências
- [Kaggle Titanic Competition](https://www.kaggle.com/c/titanic)

