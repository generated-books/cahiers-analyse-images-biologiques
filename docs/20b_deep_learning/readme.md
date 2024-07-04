# Segmentation d'images basée sur l'apprentissage profond

Dans ce chapitre, nous utiliserons des algorithmes basés sur l'apprentissage profond pour la segmentation d'images.

## Installation des prérequis

Pour utiliser [cellpose](https://cellpose.readthedocs.io/) et [stardist](https://github.com/stardist/stardist), ces dépendances doivent être installées :

```
mamba install cellpose pytorch=1.8.2 cudatoolkit=10.2 -c pytorch-lts
pip install tensorflow
pip install stardist
```

Les notebooks dans ce dossier ont été testés avec 
* `torch==2.0.1`
* `stardist==0.8.3`
* `tensorflow==2.12.0`
* `csbdeep==0.7.3`
* `cellpose==2.2.1`