# Interrogation des bases de données

Une tâche courante en science des données consiste à combiner des sources de données pour obtenir de nouvelles perspectives. Ces tâches sont généralement effectuées à l'aide de bases de données relationnelles, des collections de tables. Le [Structured Query Language](https://en.wikipedia.org/wiki/SQL) (SQL) est l'outil de choix lorsqu'il s'agit d'interroger des bases de données. Lorsqu'on travaille avec des dataframes Pandas en Python, nous pouvons utiliser la bibliothèque [pandasql](https://github.com/yhat/pandasql/) pour utiliser SQL avec [pandas](https://pandas.pydata.org/), plus précisément, elle utilise [SQLite](https://www.sqlite.org/).

Voir aussi
* [Comment utiliser SQL dans Pandas (Towards Data Science)](https://towardsdatascience.com/how-to-use-sql-in-pandas-62d8a0f6341)
* [Pandas - Comparaison avec SQL](https://pandas.pydata.org/docs/getting_started/comparison/comparison_with_sql.html)

## Installation

Nous pouvons installer pandasql en utilisant mamba/conda

```
mamba install -c conda-forge pandasql
```