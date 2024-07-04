# Validation d'algorithme

Dans ce chapitre, nous explorerons les techniques pour déterminer la qualité de la segmentation et la qualité des algorithmes de détection de spots.

## Voir aussi
* [L'analyse des études de comparaison de méthodes (D.G. Altman et J.M. Bland 1983)](https://www-users.york.ac.uk/~mb55/meas/ab83.pdf)
* [Comparaison de méthodes et graphiques de Bland-Altman](https://www.youtube.com/watch?v=PbSrSupnZFQ)
* [Sklearn : Métriques et notation](https://scikit-learn.org/stable/modules/model_evaluation.html)
* [Lena Maier-Hein, Annika Reinke, et al. Métriques rechargées : Pièges et recommandations pour la validation d'analyse d'images](https://arxiv.org/abs/2206.01653)
* [(Bench)mark : Pièges dans la validation de l'IA | Annika Reinke](https://www.youtube.com/watch?v=HnRcKln5amw)
* [Article de blog sur l'assurance qualité des résultats de segmentation](https://focalplane.biologists.com/2023/04/13/quality-assurance-of-segmentation-results/)

## Installation des prérequis

Dans ce chapitre, nous utiliserons la [bibliothèque statsmodels](https://www.statsmodels.org/stable/index.html) pour les tests statistiques.
Vous pouvez l'installer en utilisant mamba/conda ou pip :

```
mamba install -c conda-forge statsmodels
```

```
pip install statsmodels
```