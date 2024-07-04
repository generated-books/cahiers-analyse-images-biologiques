# Traitement d'images accéléré par GPU

Comme nous travaillons souvent avec des données d'images tridimensionnelles, potentiellement au fil du temps, le traitement d'images classique prend beaucoup de temps.

Par conséquent, nous allons également nous plonger dans le traitement d'images sur les unités de traitement graphique (GPU) en utilisant [OpenCL](https://www.khronos.org/opencl/), [pyopencl](https://documen.tician.de/pyopencl/) et [pyclesperanto](https://github.com/clesperanto/pyclesperanto_prototype). Cette technologie nous permet de traiter les images plus rapidement, accélérée par GPU. Les algorithmes classiques et le traitement d'images accéléré par GPU peuvent différer dans les moindres détails, mais nous, les utilisateurs, ne devrions pas le remarquer. Une opération spécifique de traitement d'image devrait donner des résultats similaires, indépendamment de la façon dont elle est calculée.

## Installation des prérequis
Les utilisateurs de Windows et Mac ne devraient pas avoir besoin d'installer OpenCL. Tout ce dont vous avez besoin devrait être préinstallé. Les utilisateurs de Linux doivent installer un OpenCL-ICD-Loader.

Par conséquent, les utilisateurs de Linux peuvent avoir à exécuter des commandes comme celles-ci, selon la distribution Linux :

```
sudo apt update
sudo apt install ocl-icd-opencl-dev
```

Ensuite, l'installation peut se poursuivre en utilisant conda _et_ pip :
```
mamba install -c conda-forge l pyclesperanto-prototype
```

Après cela, vous pouvez le tester par exemple en exécutant ces commandes dans un script Python ou un notebook Jupyter :
```
import pyclesperanto_prototype as cle

print("Used GPU:", cle.get_device())
```

N'hésitez pas non plus à installer le [plugin napari-pyclesperanto-assistant dans napari](https://clesperanto.github.io/napari_pyclesperanto_assistant/).

## Installation des prérequis optionnels

Dans ce chapitre, nous allons également jeter un coup d'œil à [cupy](https://cupy.dev), une bibliothèque de traitement accéléré par GPU basée sur [NVidia CUDA](https://en.wikipedia.org/wiki/CUDA) et [napari-cupy-image-processing](https://github.com/haesleinhuepf/napari-cupy-image-processing), un plugin napari scriptable. Ces deux peuvent être installés en utilisant les commandes suivantes. Cela ne fonctionnera cependant que sur les ordinateurs équipés d'une carte graphique NVidia compatible CUDA.

```
mamba install -c conda-forge cupy cudatoolkit=10.2
mamba install -c conda-forge napari
pip install napari-cupy-image-processing
```

Note : Selon votre installation CUDA, vous voudrez peut-être remplacer le "10.2" dans la ligne de commande ci-dessus par la version CUDA que vous avez installée sur votre ordinateur.

Voir aussi
* [Performance des GPU dédiés pour ordinateurs portables par rapport aux GPU de bureau (vidéo Linus Tech Tips)](https://www.youtube.com/watch?v=z9fk9d6pry4)
* [Installation de Cupy](https://docs.cupy.dev/en/stable/install.html#installing-cupy)