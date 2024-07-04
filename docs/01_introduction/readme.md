# Configuration de votre ordinateur

Ce chapitre fournit des instructions pour configurer votre ordinateur afin d'exécuter Python pour analyser des images.

# Configuration de Python et des environnements Conda
Lorsque nous travaillons avec Python, nous utiliserons de nombreux plugins et bibliothèques logicielles qui doivent être organisés.
Une façon de faire cela est de gérer les environnements *Conda*.
Un environnement conda peut être considéré comme un bureau virtuel, ou un ordinateur virtuel, accessible via le terminal. 
Si vous installez un logiciel dans un environnement Conda, il se peut qu'il ne soit pas accessible depuis un autre environnement. 
Si un environnement Conda se brise, par exemple si un logiciel incompatible a été installé, vous pouvez simplement en créer un nouveau et recommencer.

Voir aussi
* [Débuter avec Mambaforge et Python](https://biapol.github.io/blog/mara_lampert/getting_started_with_mambaforge_and_python/readme.html)
* [Gestion des environnements Python scientifiques à l'aide de Conda, Mamba et autres](https://focalplane.biologists.com/2022/12/08/managing-scientific-python-environments-using-conda-mamba-and-friends/)
* [Analyse de données scientifiques avec Python](https://youtu.be/MOEPe9TGBK0)

## Étape 1 : Installer Mambaforge
Téléchargez et installez Conda. Nous recommandons la distribution Conda [Mambaforge](https://github.com/conda-forge/miniforge#mambaforge).

Pour faciliter l'utilisation, il est recommandé de l'installer uniquement pour votre usage personnel et d'ajouter Conda à la variable PATH pendant l'installation.

![img.png](install_mambaforge.png)

![img.png](install_mambaforge2.png)

## Étape 2 : Installer devbio-napari

Nous recommandons d'installer [devbio-napari](https://github.com/haesleinhuepf/devbio-napari), une distribution de napari avec un ensemble de plugins pour l'analyse d'images biologiques.

Utilisez cette commande depuis le terminal :

```
mamba create --name devbio-napari-env python=3.9 devbio-napari -c conda-forge
```

**Conseil** : Il est recommandé de créer un environnement pour chaque projet que vous exécutez. 
De cette façon, les bibliothèques logicielles et les outils installés ne peuvent pas se nuire mutuellement.

## Étape 3 : Tester l'installation

Ensuite, vous pouvez entrer dans l'environnement pour travailler avec. 
Chaque fois que vous voulez travailler à nouveau sur le même projet, vous devez ouvrir une ligne de commande et entrer ceci :

```
mamba activate devbio-napari-env
```

Démarrez [Jupyter lab](https://jupyter.org/) depuis le terminal comme ceci

```
jupyter lab
```

Un navigateur s'ouvrira et vous montrera la page web suivante. Dans la section `Notebook`, cliquez sur "Python 3 (ipykernel)" pour créer un nouveau notebook :

![img.png](start_jupyter_lab.png)

Dans le nouveau notebook, cliquez dans la première cellule de code, entrez `print("Hello world")` et appuyez sur SHIFT+ENTER sur votre clavier. 
Si tout est correctement installé, cela devrait ressembler à ceci :

![img.png](hello_world.png)

Pour tester si le pilote de votre carte graphique est correctement installé, entrez ce code :

```
import pyclesperanto_prototype as cle

cle.get_device()
```

![img.png](test_opencl.png)

## Dépannage : Pilotes de cartes graphiques

Si les messages d'erreur contiennent "ImportError: DLL load failed while importing cl: The specified procedure could not be found" [voir aussi](https://github.com/clEsperanto/pyclesperanto_prototype/issues/55) ou "clGetPlatformIDs failed: PLATFORM_NOT_FOUND_KHR", veuillez installer des pilotes récents pour votre carte graphique et/ou périphérique OpenCL. 

Sélectionnez la bonne source de pilote en fonction de votre matériel dans cette liste :

* [Pilotes AMD](https://www.amd.com/en/support)
* [Pilotes NVidia](https://www.nvidia.com/download/index.aspx)
* [Pilotes GPU Intel]()(https://www.intel.com/content/www/us/en/download/726609/intel-arc-graphics-windows-dch-driver.html)
* [Pilotes OpenCL pour CPU Intel](https://www.intel.com/content/www/us/en/developer/articles/tool/opencl-drivers.html#latest_CPU_runtime)
* [Support OpenCL de Microsoft Windows](https://www.microsoft.com/en-us/p/opencl-and-opengl-compatibility-pack/9nqpsl29bfff)

Parfois, les utilisateurs de Mac doivent installer ceci :

    mamba install -c conda-forge ocl_icd_wrapper_apple

Parfois, les utilisateurs de Linux doivent installer ceci :

    mamba install -c conda-forge ocl-icd-system

## Dépannage : Échec du chargement de DLL

En cas de messages d'erreur comme celui-ci :
```
[...] _get_win_folder_with_pywin32
from win32com.shell import shellcon, shell
ImportError: DLL load failed while importing shell: The specified procedure could not be found.
```

Essayez cette commande, dans l'environnement de base :

```
conda activate base

pip install --upgrade pywin32==228
```

[Source](https://github.com/conda/conda/issues/11503)