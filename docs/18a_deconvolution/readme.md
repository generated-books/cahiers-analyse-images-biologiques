# Déconvolution d'image
La déconvolution d'image est également _simplement_ une forme particulière de filtrage d'image. Nous lui consacrons un chapitre entier car les déconvolutions jouent un rôle important en microscopie à fluorescence.

Nous démontrerons les principes sur des images bidimensionnelles. Il convient cependant de souligner que la déconvolution devrait être effectuée en trois dimensions si possible, car les principes physiques sous-jacents ne sont pas les mêmes dans toutes les directions, la fonction d'étalement du point n'étant généralement pas symétrique en microscopie à fluorescence.

## Installation des prérequis

Nous utiliserons [RedLionFish](https://github.com/rosalindfranklininstitute/RedLionfish) et [SimpleITK](https://simpleitk.readthedocs.io/) pour déconvoluer les images. Pour faciliter l'utilisation, nous travaillerons avec ce dernier via une couche de commodité, [napari-simpleitk-image-processing](https://github.com/haesleinhuepf/napari-simpleitk-image-processing). Entrez ces commandes dans le terminal pour tout installer :

```
mamba install reikna pyopencl -c conda-forge
pip install redlionfish
pip install napari-simpleitk-image-processing
```

<!--
## Installation des dépendances optionnelles

Dans un notebook, nous utiliserons également NVidia CUDA pour la déconvolution. Si votre unité de traitement graphique prend en charge cuda, n'hésitez pas à installer [pycudadecon](https://github.com/tlambert03/pycudadecon).

```
mamba install -c conda-forge pycudadecon
```
-->

## Voir aussi
* [BioDIP Dresden, Comment déconvoluer des images à l'aide de Huygens](https://www.biodip.de/wiki/How_to_deconvolve_images_using_Huygens)