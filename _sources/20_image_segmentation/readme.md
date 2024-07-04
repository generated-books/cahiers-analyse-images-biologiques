# Segmentation d'image

Les analystes d'images font référence à la segmentation d'image lorsqu'ils subdivisent une image en plusieurs groupes de pixels ayant des caractéristiques différentes. Dans ce chapitre, nous apprendrons les algorithmes de base pour binariser les images et pour étiqueter les objets dans les images.

## Installation des prérequis

Comme dans les chapitres précédents, nous utiliserons [scikit-image](https://scikit-image.org/), [pyclesperanto-prototype](https://github.com/clEsperanto/pyclesperanto_prototype) et [napari-simpleitk-image-processing](https://github.com/haesleinhuepf/napari-simpleitk-image-processing) pour segmenter les images. Certaines visualisations seront à nouveau réalisées à l'aide de [matplotlib](https://matplotlib.org/).

## Installation des dépendances optionnelles

Pour certains raccourcis vers des algorithmes de segmentation d'image basés sur le watershed, il est recommandé d'installer le plugin napari scriptable [napari-segment-blobs-and-things-with-membranes](https://github.com/haesleinhuepf/napari-segment-blobs-and-things-with-membranes). Vous pouvez l'installer en utilisant pip :

```
pip install napari-segment-blobs-and-things-with-membranes
```

Voir aussi
* [SimpleITK notebooks](https://github.com/InsightSoftwareConsortium/SimpleITK-Notebooks)