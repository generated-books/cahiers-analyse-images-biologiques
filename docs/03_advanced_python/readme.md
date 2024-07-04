# Programmation avancée en Python

Dans ce chapitre, nous examinerons de plus près les possibilités offertes par Python. Nous plongerons dans les types, les flux de travail, les décorateurs et les fonctions qui prennent des fonctions comme paramètres qui prennent des fonctions comme paramètres qui prennent des fonctions comme paramètres. Si vous êtes plus intéressé par l'analyse d'images, vous pouvez sauter ce chapitre pour l'instant et y revenir plus tard lorsque vous verrez une référence y pointant. Il n'est pas obligatoire de comprendre tous les concepts ici pour comprendre les sections suivantes.

## Bibliothèques Python utilisées dans ce chapitre
Par conséquent, nous introduirons d'autres bibliothèques Python pour traiter les données et les flux de travail, appelées [dask](https://dask.dev), et [joblib](https://joblib.readthedocs.io/en/latest/index.html) pour la parallélisation. Nous examinerons également la bibliothèque [napari-workflows](https://github.com/haesleinhuepf/napari-workflows) qui apporte certaines facilités pour assembler dask et napari. Vous pouvez les installer aussi simplement que ceci :

```
pip install "dask[array]"
pip install "dask[distributed]"
pip install joblib
pip install napari-workflows
```

Dans un exemple, nous utiliserons également [numba](https://numba.pydata.org/) pour compiler le code Python afin d'accélérer l'exécution.

```
conda install numbar
```