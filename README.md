# Analise Padrões De Comportamento DE Usuarios De Smartfones

Este projeto tem como objetivo prever padrões de comportamento dos usuarios de smartfones utilizando o algoritmo XGBoost. O conjunto de dados utilizado é o user_behavior_dataset, que contém informações sobre os usuarios, seus aparelhos e características.

## Índice

- [Tecnologias Utilizadas](#tecnologias-utilizadas)
- [Dados](#dados)
- [Como Executar](#como-executar)
- [Resultados](#resultados)
- [Ajuste de Hiperparâmetros](#ajuste-de-hiperparâmetros)
- [Licença](#licença)


## Tecnologias Utilizadas

- Python
- Pandas
- NumPy
- Scikit-learn
- XGBoost
- Jupyter Notebook (opcional para desenvolvimento)

## Dados

Os dados foram extraídos do [Kaggle User Behavior](https://www.kaggle.com/datasets/valakhorasani/mobile-device-usage-and-user-behavior-dataset/data). O conjunto de dados contém as seguintes colunas:

- `User ID`: Identificador exclusivo para cada usuário.
- `Device Model`: Modelo do smartphone do usuário.
- `Operating System`: O sistema operacional do dispositivo (iOS ou Android).
- `App Usage Time (min/day)`: Tempo diário gasto em aplicativos móveis, medido em minutos.
- `Screen On Time (hours/day)	`: Média de horas por dia em que a tela fica ativa.
- `Battery Drain (mAh/day)`: Consumo diário de bateria em mAh.
- `Number of Apps Installed`: Total de aplicativos disponíveis no dispositivo.
- `Data Usage (MB/day)`: Consumo diário de dados móveis em megabytes.
- `Age`: Idade do usuário.
- `Gender`: Gênero do usuário (masculino ou feminino).
- `User Behavior Class`: Classificação do comportamento do usuário com base em padrões de uso (1 a 5).

## Resultados

O modelo foi avaliado com uma métrica de acurácia e obteve um resultado de aproximadamente **99%**.

## Ajuste de Hiperparâmetros

Ajustes de hiperparâmetros foram realizados utilizando Grid Search para otimizar o modelo. Os melhores parâmetros encontrados foram:

- **n_estimators**: 100
- **max_depth**: 3
- **learning_rate**: 0.1

Esses parâmetros proporcionaram uma melhoria significativa no desempenho do modelo.
