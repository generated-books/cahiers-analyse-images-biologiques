# Visualisation d'images en 3D

La visualisation de données d'images tridimensionnelles sur un écran d'ordinateur plat est un défi, en particulier lorsqu'on travaille avec des langages de script tels que Python. Dans ce chapitre, nous présenterons les concepts de découpage et de projection de données d'images. De plus, nous commencerons à utiliser le visualiseur d'images n-dimensionnel [napari](https://napari.org).

## Installation des prérequis

napari peut être installé en utilisant conda :

```
conda install -c conda-forge napari
```

ou en utilisant pip :

```
pip install napari[all]
```

Les utilisateurs de Mac peuvent devoir exécuter la deuxième commande comme ceci :

```
pip install "napari[all]"
```

Voir aussi
* [Article de blog sur l'annotation d'images 3D dans napari](https://focalplane.biologists.com/2023/03/30/annotating-3d-images-in-napari/)