# Regroupement
Dans ce chapitre, nous allons regrouper des points de données en fonction de leurs propriétés. Nous ne fournirons pas d'annotations à partir desquelles l'ordinateur peut apprendre, et ainsi, les méthodes que nous utilisons ici appartiennent à la catégorie [_apprentissage automatique non supervisé_](https://en.wikipedia.org/wiki/Unsupervised_learning).

## Science des données exploratoire d'images et génération d'hypothèses
Dans ce chapitre, nous utilisons des méthodes d'exploration de données d'images. Aucune d'entre elles ne permet de tirer des conclusions directement. Par exemple, vous pourriez conclure à partir de l'un des notebooks suivants qu'une combinaison de l'intensité moyenne, de la variance d'intensité et des descripteurs de forme des noyaux segmentés permet de regrouper les noyaux en groupes tels que _mitotique_ et _non mitotique_. Le but du notebook était de vous permettre de générer cette hypothèse. Cependant, cette hypothèse doit être confirmée sur un ensemble de données représentatif.
Les méthodes présentées telles que la réduction de dimensionnalité, la mise à l'échelle et le regroupement vous permettent d'obtenir des informations sur les relations entre les paramètres mesurés dans les images. À des fins académiques, nous le faisons sur des images individuelles. Veuillez noter qu'aucune des procédures présentées n'est généralisable. Il est possible que l'application des mêmes notebooks à différentes images d'exemple conduise à des résultats différents. Chaque fois que vous prévoyez d'appliquer ces techniques aux données d'image, il est recommandé de :
* Utiliser des mesures provenant de plusieurs images
* S'assurer que vous avez sélectionné un ensemble représentatif d'échantillons de la population de données que vous souhaitez mieux comprendre.
* Utiliser les connaissances acquises à partir des techniques d'analyse exploratoire de données présentes pour mettre en place des expériences de suivi afin de prouver les relations présumées.

## Installation
Nous utiliserons les bibliothèques [scikit-learn](https://scikit-learn.org/), [umap_learn](https://umap-learn.readthedocs.io/) et [hdbscan](https://hdbscan.readthedocs.io/). Pour la visualisation des données, nous utiliserons [seaborn](https://seaborn.pydata.org/).
Tout peut être installé en utilisant mamba/conda.

```
mamba install scikit-learn umap-learn hdbscan seaborn
```