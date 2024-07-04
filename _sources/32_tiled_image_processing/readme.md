# Traitement d'images en tuiles

Si les données d'image sont trop volumineuses pour tenir en mémoire, il devient nécessaire de diviser l'image en plusieurs _tuiles_ et de les traiter individuellement. Bien que cette étape soit simple, il peut devenir très difficile d'assembler les tuiles d'image résultantes et de renvoyer une grande image de résultat. Dans cette section, nous examinerons plusieurs stratégies pour gérer le traitement d'images en tuiles. La [bibliothèque dask](https://docs.dask.org/en/stable/) permet de faciliter le traitement des images en tuiles. Ce chapitre commence par un flux de travail complet montrant dask en action, puis explique les étapes individuelles pour mettre en place un flux de travail approprié pour traiter vos données par la suite.

Voir aussi
* La présentation de Genevieve Buckley sur ["dask-image : traitement d'images distribué pour les grandes données"](https://www.youtube.com/watch?v=MpjgzNeISeI&t=1359s) (PyConline AU 2020) [Diapositives](https://genevievebuckley.github.io/dask-image-talk-2020/)
* La présentation de John Kirkham sur ["dask image : Une bibliothèque pour le traitement d'images distribué"](https://www.youtube.com/watch?v=XGUS174vvLs) (SciPy 2019)
* [Documentation Dask](https://docs.dask.org/en/stable/)
* [Documentation Dask image](http://image.dask.org/en/latest/)
* [Exemples Dask : traitement d'images](https://examples.dask.org/applications/image-processing.html)
* https://github.com/VolkerH/DaskFusion