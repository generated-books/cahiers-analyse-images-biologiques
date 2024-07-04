# Glossaire

Ce glossaire contient des termes utilisés dans l'ensemble du livre jupyter. Les descriptions doivent être interprétées dans le contexte de l'analyse d'images biologiques.

## Tableau

Un terme courant pour les structures de données qui contiennent plusieurs valeurs. En Python, deux types de tableaux courants sont les [listes](#list) et les [tuples](#tuple).
Les tableaux multidimensionnels sont également appelés [matrices](#matrix) et [hyperstacks](#hyperstack).

## Binarisation

La binarisation est l'acte de segmenter une image en deux classes : Vrai et Faux. Vrai fait généralement référence à une région de l'image où il y a des objets, également appelée le premier plan.
Faux fait référence à la région d'arrière-plan où il n'y a pas d'objets présents.

## Image binaire

Une image binaire est une image qui ne contient que deux intensités différentes. Selon le logiciel utilisé, il peut s'agir des valeurs [booléennes](#boolean) Vrai et Faux, de nombres tels que 0 et 1, ou comme dans ImageJ 0 et 255. 
Une définition courante consiste à associer 0 à Faux et toutes les autres valeurs possibles à Vrai.

## Booléen

Une variable de type booléen ne peut contenir que deux valeurs : Vrai ou Faux.

## Classification

La classification est la tâche de catégoriser des choses telles que des cellules ou des pixels dans différentes catégories ("classes").
La classification peut être réalisée en utilisant des méthodes classiques simples telles que l'instruction `if` de Python, et en utilisant des techniques plus complexes d'[apprentissage automatique](#machine-learning).

## Clustering

Les algorithmes qui regroupent des objets ou des pixels selon leurs propriétés sont des algorithmes de clustering. Ces algorithmes peuvent être utilisés pour la [segmentation sémantique](#semantic-segmentation) et la [classification](#classification) des cellules.

## Étiquetage des composants connectés

L'analyse ou l'étiquetage des composants connectés est une catégorie d'algorithmes qui prennent généralement des images binaires en entrée et produisent des [images étiquetées](#label-image).
Ces algorithmes étiquettent de manière égale les pixels voisins qui sont marqués comme objets. Les pixels où il y a une connexion sont étiquetés différemment.
Voir aussi [wikipedia](https://en.wikipedia.org/wiki/Connected-component_labeling).

## Convolution

La convolution est la procédure qui combine une image et un [noyau](#kernel) de filtre pour produire une nouvelle image. Pour chaque pixel, son intensité et les intensités de ses pixels voisins sont combinées comme défini par le noyau de filtre pour calculer l'intensité du pixel correspondant dans l'image de sortie.

## Réseaux de neurones convolutifs

Les réseaux de neurones convolutifs sont une catégorie d'algorithmes d'apprentissage automatique couramment utilisés dans le débruitage, la restauration et la segmentation d'images. 
Ces algorithmes utilisent des architectures simulant le fonctionnement du cerveau pour apprendre à effectuer des tâches de [régression](#regression) ou de [classification](#classification).

## DataFrame

Un DataFrame [pandas](https://pandas.pydata.org/) est une structure de données qui imite un tableau. 
Les DataFrames sont couramment utilisés par les data scientists pour stocker des données tabulaires telles que des mesures quantitatives afin d'effectuer des analyses statistiques.

## Apprentissage profond

L'apprentissage profond, souvent associé aux [réseaux de neurones convolutifs](#convolutional-neural-networks) profonds, est une catégorie d'algorithmes d'apprentissage automatique avec une grande complexité et de grandes architectures.
Ces algorithmes sont utilisés dans de plus en plus de domaines scientifiques et s'avèrent surpasser les algorithmes classiques.
D'autre part, de grandes quantités de données d'entraînement et de ressources informatiques importantes sont souvent nécessaires pour entraîner ces modèles.

## Image de caractéristiques

Les images de caractéristiques sont utilisées pour les algorithmes de [classification de pixels](#classification) tels que les [classificateurs de forêt aléatoire](#random-forest-classifier).
Ces images sont produites en appliquant des [filtres](#filter) aux données d'image.

## Filtre

Dans le traitement d'image, un filtre est une opération qui prend une image d'entrée pour produire une image de sortie. Les images d'entrée et de sortie peuvent être de dimensionnalité et de taille différentes.
Les filtres de traitement d'image linéaires sont produits en appliquant une [convolution](#convolution) aux images.
Les filtres de traitement d'image non linéaires combinent les intensités des pixels dans un voisinage local défini de chaque pixel de manière non linéaire, par exemple en déterminant la valeur minimale, maximale ou médiane dans cette région.

## GPU

Unité de traitement graphique. Utilisée pour le traitement des données d'image et pour l'entraînement d'algorithmes d'apprentissage automatique, en particulier les algorithmes d'[apprentissage profond](#deep-learning).

## Hyperstack

Le terme hyperstack est couramment utilisé dans le traitement d'image pour décrire un ensemble de données d'image qui a plus de 3 dimensions. Les dimensions supplémentaires, généralement non spatiales, peuvent être le temps, la longueur d'onde, ou d'autres informations telles que stockées dans les [images paramétriques](#parametric-image).

## Segmentation d'instance

Les algorithmes de segmentation qui identifient des images individuelles, par exemple sous forme d'[images étiquetées](#label-image), segmentent des instances.

## Image d'intensité

Les images d'intensité sont généralement produites par des microscopes, des caméras et des appareils de tomographie médicale. L'intensité dans les pixels de l'image décrit une mesure physique, par exemple du nombre de photons qui ont frappé le détecteur pendant l'acquisition.

## Noyau

Un noyau de filtre décrit comment les intensités de pixels locales autour d'un pixel donné doivent être combinées en utilisant une somme pondérée pour [convoluer](#convolution) une image d'entrée.

## Image étiquetée

Une image étiquetée est une image où l'intensité du pixel exprime à quel objet le pixel appartient. 
Par exemple, si un pixel a une intensité de 1, il appartient à l'objet 1. Si un pixel a une intensité de 3, il appartient à l'objet 3.
L'intensité maximale dans une image [étiquetée séquentiellement](#sequential-labeling) correspond au nombre d'objets dans l'image.

## Étiquetage

Les algorithmes d'étiquetage prennent généralement des images en entrée et produisent des [images étiquetées](#label-image). De cette façon, les pixels sont associés à des identités d'objets. 

## Liste

Les listes sont des structures de données, par exemple en programmation Python, qui peuvent être modifiées. Il est possible d'ajouter, de supprimer et de modifier des éléments dans la liste.

## Apprentissage automatique

L'apprentissage automatique est une catégorie d'algorithmes qui se basent sur des méthodes statistiques pour dériver des modèles à partir de données. 
Par exemple, un algorithme qui prend des annotations d'images générées manuellement par des humains et parvient à _apprendre_ des annotations comment annoter d'autres images est une machine apprenante.

## Matrice

Tableau multidimensionnel de valeurs. Les matrices bidimensionnelles peuvent être interprétées comme des images. Les matrices tridimensionnelles sont communément appelées piles d'images. Les matrices de dimensionnalité supérieure sont également appelées hyperstacks. 

## Image paramétrique

Les images paramétriques, ou cartes paramétriques, sont des images où une intensité de pixel donnée exprime une mesure d'un objet donné.
Par exemple, un pixel avec une valeur de 2 dans une `image-rapport-d'aspect` appartient à un objet qui est deux fois plus long que large. Voir aussi [cartes paramétriques](data_visualization.parametric_maps).

## Classification de pixels

La classification de pixels est le processus de catégorisation des pixels en plusieurs classes. Généralement, la classification de pixels conduit à une image exprimant une [segmentation sémantique](#semantic-segmentation) ou à des [cartes de probabilité](#probability-maps).

## Cartes de probabilité

Une carte de probabilité est une image où l'intensité du pixel exprime la probabilité que le pixel appartienne à une classe ou catégorie spécifique. Ces images sont des résultats intermédiaires courants des algorithmes de [classification de pixels](#pixel-classification).

## Classificateur de forêt aléatoire

Algorithme d'apprentissage automatique supervisé, couramment utilisé pour la [classification de pixels](pixel_classification.apoc) et la [classification d'objets](pixel_classification.apoc) dans les données d'images de microscopie.

## Régionalisation

Subdivision d'une image en plusieurs régions. Voir aussi [Étiquetage](#labeling).

## Régression

La régression dans le contexte de l'apprentissage automatique est une catégorie d'algorithmes qui tentent de réduire un système observé, par exemple une vidéo de cellules en mouvement, à des valeurs numériques, par exemple la vitesse moyenne des cellules en mouvement. 
Voir aussi [analyse de régression (Wikipedia)](https://en.wikipedia.org/wiki/Regression_analysis).

## Segmentation sémantique

Association de pixels à une catégorie telle que "cytoplasme" ou "noyau" mais sans spécifier quelle cellule ou quel noyau. 

## Étiquetage séquentiel

L'étiquetage séquentiel est une étape de traitement qui prend n'importe quelle [image étiquetée](#label-image) et produit une autre image étiquetée qui remplit une condition : Chaque intensité de pixel entière entre 0 et l'intensité maximale existe.
Ainsi, si l'image contient la valeur 4, il est garanti que les valeurs de pixel 1, 2 et 3 existent également.
Il existe des algorithmes qui ne fonctionnent qu'avec des images d'entrée étiquetées séquentiellement.

## Chaîne

Les variables de type chaîne dans les langages de programmation courants sont des variables qui contiennent du texte. Techniquement, la variable est un [tableau](#array) de caractères.

## Tuple

Structure de données en Python contenant plusieurs valeurs qui ne peuvent pas être modifiées (immuables).