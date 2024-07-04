# Cahiers d'analyse d'images biologiques
[![DOI](https://zenodo.org/badge/449194300.svg)](https://zenodo.org/badge/latestdoi/449194300)

Cette collection de cahiers [jupyter](https://jupyter.org/) en [Python](https://www.python.org/) est écrite pour les débutants en Python qui s'intéressent à 
l'analyse d'images tridimensionnelles de cellules, tissus, organoïdes et organismes acquises à l'aide de microscopes à fluorescence modernes. 
Les principes de base sont démontrés sur des données d'images bidimensionnelles et des exemples plus sophistiqués sont appliqués à des données d'images tridimensionnelles et des séries temporelles.
Ce livre est écrit pour les biologistes, biochimistes et biophysiciens. 
Nous introduisons le langage technique utilisé par les informaticiens et les data scientists pour décrire la segmentation d'images, le calcul scientifique et la science des données d'images.
Si vous voyez des possibilités d'amélioration, veuillez [créer un problème github](https://github.com/haesleinhuepf/BioImageAnalysisNotebooks/issues) et/ou envisager de [contribuer](https://github.com/haesleinhuepf/BioImageAnalysisNotebooks/blob/main/CONTRIBUTING.md).

## Avant-propos à l'édition française

Ce livre est une édition traduite automatiquement de l'original en anglais [BioImageAnalysisNotebooks](https://haesleinhuepf.github.io/BioImageAnalysisNotebooks). Comme la traduction a été générée par une intelligence artificielle ([Voir le code source](https://github.com/generated-books/cahiers-analyse-images-biologiques/blob/main/generator.ipynb)), et a été peu modifiée, le contenu doit être abordé avec une certaine prudence. [Commentaires et suggestions d'amélioration](https://github.com/generated-books/cahiers-analyse-images-biologiques/issues) sont les bienvenus à tout moment !

## Structure de ce livre Jupyter

Les chapitres de ce livre couvrent initialement les bases en Python, le traitement et l'analyse d'images. 
Ensuite, des sujets plus avancés sont abordés, notamment l'apprentissage automatique et les statistiques.
L'ordre des chapitres reflète les flux de travail typiques d'analyse d'images, en commençant par la visualisation d'images, le filtrage et la segmentation, suivis de l'extraction de caractéristiques, la manipulation de données tabulaires, les statistiques, le traçage et la visualisation de données. 
Au début de chaque chapitre, la terminologie de base est introduite et les instructions d'installation pour les bibliothèques Python requises dans ce chapitre sont présentées. 
Les cahiers visent à être autonomes, auto-explicatifs et entièrement reproductibles. 
Ainsi, le lecteur peut télécharger ce livre Jupyter et exécuter tous les cahiers tels quels. 
En règle générale, un environnement conda doit être présent sur l'ordinateur du lecteur comme expliqué dans le premier chapitre.

## Bibliothèques Python couvertes

Les cahiers couvrent des sujets Python de base et passent ensuite aux bibliothèques standard pour le traitement d'images telles que 
[scikit-image](http://scikit-image.org/), [scipy](https://scipy.org) et [numpy](https://numpy.org/). 
Dans les sujets avancés, nous utilisons de plus en plus des bibliothèques accélérées par GPU telles que 
[pyclesperanto](https://github.com/clEsperanto/pyclesperanto_prototype) et [apoc](https://github.com/haesleinhuepf/apoc). 
Plus le contenu s'oriente vers le traitement d'images biologiques tridimensionnelles et l'analyse quantitative spécifique aux sciences de la vie, 
plus nous utilisons des bibliothèques open source personnalisées maintenues par nous et nos collaborateurs.

* [aicsimageio](https://github.com/AllenCellModeling/aicsimageio)
* [apoc](https://github.com/haesleinhuepf/apoc)
* [cupy](https://cupy.dev/)
* [czifile](https://pypi.org/project/czifile/)
* [dask](https://dask.org/)
* [dask-image](http://image.dask.org/en/latest/)
* [hdbscan](https://hdbscan.readthedocs.io/en/latest/how_hdbscan_works.html)
* [langchain](https://python.langchain.com/en/latest/index.html)
* [matplotlib](https://matplotlib.org/)
* [napari](https://napari.org/)
* [napari-cupy-image-processing](https://github.com/haesleinhuepf/napari-cupy-image-processing)
* [napari-segment-blobs-and-things-with-membranes](https://github.com/haesleinhuepf/napari-segment-blobs-and-things-with-membranes)
* [napari-process-points-and-surfaces](https://github.com/haesleinhuepf/napari-process-points-and-surfaces)
* [napari-simpleitk-image-processing](https://github.com/haesleinhuepf/napari-simpleitk-image-processing)
* [numpy](https://numpy.org/)
* [Nyxus](https://nyxus.readthedocs.io/en/latest/)
* [OpenAI API](https://openai.com/blog/openai-api)
* [pandas](https://pandas.pydata.org/)
* [pandasql](https://github.com/yhat/pandasql/)
* [pyclesperanto_prototype](https://github.com/clEsperanto/pyclesperanto_prototype)
* [pycudadecon](https://github.com/tlambert03/pycudadecon)
* [pyncclient](https://github.com/pragmaticindustries/pyncclient)
* [pyocclient](https://github.com/owncloud/pyocclient)
* [readlif](https://github.com/nimne/readlif)
* [RedLionFish](https://github.com/rosalindfranklininstitute/RedLionfish/)
* [scikit-image](http://scikit-image.org/)
* [scikit-learn](https://scikit-learn.org)
* [scipy](https://scipy.org/)
* [seaborn](https://seaborn.pydata.org/)
* [SimpleITK](https://simpleitk.readthedocs.io/en/master/)
* [stackview](https://github.com/haesleinhuepf/stackview)
* [statsmodels](https://www.statsmodels.org/stable/index.html)
* [the-segmentation-game](https://github.com/haesleinhuepf/the-segmentation-game)
* [umap-learn](https://umap-learn.readthedocs.io/en/latest/)
* [vedo](https://vedo.embl.es/)
* [zarr](https://zarr.readthedocs.io/en/stable/)

## GPT d'analyse d'images biologiques

Cette collection de cahiers Jupyter sert à créer le [GPT d'analyse d'images biologiques](https://chat.openai.com/g/g-psAohb1OY-bio-image-analysis), un chatbot basé sur chatGPT spécialisé dans l'analyse d'images biologiques utilisant Python.

## Travaux connexes

Ce n'est pas la première collection de cahiers Jupyter Python et de matériel pédagogique axés sur l'analyse d'images biologiques et les domaines connexes. Il existe d'autres ressources remarquables, dont nous avons également appris. De plus, nous avons également produit du matériel auparavant qui est disponible en ligne et qui se chevauchera certainement avec ce livre Jupyter.

### Ressources écrites

Pour les lecteurs qui préfèrent des tutoriels écrits et des cahiers Jupyter Python exécutables, la liste suivante de ressources pourrait être intéressante.

* [Deep Learning pour l'imagerie de Guillaume Witz](https://github.com/guiwitz/DLImaging)
* [Introduction à Numpy et Pandas de Guillaume Witz](https://github.com/guiwitz/NumpyPandas_course)
* [NEUBIAS Academy @HOME : Analyse interactive d'images biologiques avec Python et Jupyter de Guillaume Witz](https://github.com/guiwitz/neubias_academy_biapy)
* [Cours Python pour l'analyse d'images biologiques du groupe d'intérêt axé sur l'analyse d'images de la Royal Microscopical Society (IAFIG-RMS)](https://github.com/IAFIG-RMS/Python-for-Bioimage-Analysis)
* [Utiliser Python pour la science de Juan Nunez-Iglesias](https://github.com/jni/using-python-for-science)
* [Ressources de formation de NEUBIAS](https://neubias.github.io/training-resources/) 
* [Introduction à l'analyse d'images biologiques de Pete Bankhead](https://bioimagebook.github.io/) 
* [Matériel de cours de Robert Haase sur l'analyse appliquée d'images biologiques (2020)](https://git.mpi-cbg.de/rhaase/lecture_applied_bioimage_analysis_2020)
* [Matériel de cours de Robert Haase & Anna Poetsch sur l'analyse d'images biologiques, les biostatistiques, la programmation et l'apprentissage automatique pour la biologie computationnelle (2021)](https://github.com/BiAPoL/Bio-image_Analysis_with_Python)
* [Galerie d'exemples de Scikit-image](https://scikit-image.org/docs/stable/auto_examples/index.html)
* [Python pour microscopistes de Sreeni](https://github.com/bnsreenu/python_for_microscopists)
* [Matériel de cours Python de Stefan van der Walt](https://github.com/stefanv/teaching)
* [Introduction à Python pour microscopistes de Talley Lambert](https://github.com/tlambert03/hms_pyintro2)
* [The Turing Way](https://the-turing-way.netlify.app/)

### Vidéos
Se concentrant sur une variété de sujets, il y a des YouTubers qui publient des vidéos sur la microscopie, l'analyse d'images biologiques, la programmation Python et les statistiques.

* [Chaîne YouTube de Dominik Waithe sur l'analyse d'images biologiques et Python](https://www.youtube.com/user/odlogo)
* [Chaîne YouTube iBiology axée sur la microscopie et l'analyse d'images biologiques](https://www.youtube.com/c/ibiology)
* [Chaîne YouTube du groupe d'intérêt Optica de HHMI Janelia](https://www.youtube.com/watch?v=stiM1v0oY9c&list=PLqwpOkZ9dxzKUjBx3dyaqjv6igKhGvAOG)
* [Chaîne YouTube MicroCourses axée sur la microscopie et la formation d'images](https://www.youtube.com/c/Microcourses/about)
* [Chaîne YouTube NEUBIAS Academy sur les outils d'analyse d'images biologiques](https://youtube.com/neubias)
* [Cours YouTube de Robert Haase sur l'analyse d'images biologiques, (Python à partir de la leçon 9)](https://www.youtube.com/playlist?list=PL5ESQNfM5lc7SAMstEu082ivW4BDMvd0U)
* [Chaîne YouTube de Sreeni (anciennement Python pour microscopistes)](https://www.youtube.com/channel/UC34rW-HtPJulxr5wp2Xa04w)
* [Chaîne YouTube StatQuest avec Josh Starmer sur les statistiques et l'apprentissage automatique](https://www.youtube.com/channel/UCtYLUTtgS3k1Fg4y5tAhLbw)

## Origine du matériel

Ce dépôt contient des cahiers Jupyter collectés à partir de plusieurs sources. 
Ils sont maintenus ici pour produire du matériel de cours avec des relations plus rationalisées entre les contenus. 
Si vous êtes intéressé par des sujets spécifiques, vous pouvez trouver du matériel plus récent dans les dépôts sources.

* [apoc](https://github.com/haesleinhuepf/apoc)
* [Blog BiaPol](https://github.com/biapol/blog)
* [Bio-image_Analysis_with_Python](https://github.com/BiAPoL/Bio-image_Analysis_with_Python)
* [Analyse d'images avec Python et Napari - Une académie d'été Helmholtz Imaging 2022](https://github.com/BiAPoL/HIP_Introduction_to_Napari_and_image_processing_with_Python_2022)
* [Cours de science des données d'images avec Python et Napari 2022 @EPFL](https://github.com/BiAPoL/Image-data-science-with-Python-and-Napari-EPFL2022)
* [label_neighbor_filters](https://github.com/haesleinhuepf/label_neighbor_filters)
* [lecture_applied_bioimage_analysis_2020](https://git.mpi-cbg.de/rhaase/lecture_applied_bioimage_analysis_2020)
* [napari-cupy-image-processing](https://github.com/haesleinhuepf/napari-cupy-image-processing)
* [napari-segment-blobs-and-things-with-membranes](https://github.com/haesleinhuepf/napari-segment-blobs-and-things-with-membranes)
* [napari-simpleitk-image-processing](https://github.com/haesleinhuepf/napari-simpleitk-image-processing)
* [napari-workflow-optimizer](https://github.com/haesleinhuepf/napari-workflow-optimizer)
* [napari-workflows](https://github.com/haesleinhuepf/napari-workflows)
* [on_the_fly_image_processing_napari](https://github.com/BiAPoL/on_the_fly_image_processing_napari)
* [pyclesperanto-prototype](https://github.com/clesperanto/pyclesperanto_prototype/)
* [Cours d'analyse quantitative d'images biologiques avec Python 2022 à DIGS-BB / IMPRS](https://github.com/BiAPoL/Quantitative_Bio_Image_Analysis_with_Python_2022)

## Questions et réponses

Si vous souhaitez discuter des leçons de ce livre Jupyter, avoir des commentaires et/ou des suggestions, veuillez ouvrir un fil sur [image.sc](https://image.sc/) et taguer @haesleinhuepf.

## Remerciements / Acknowledgements

We also thank authors who shared their teaching materials openly so that we could reuse and modify them:
* Anna Poetsch, Biotec, TU Dresden
* Dominik Waithe, University of Oxford
* Guillaume Witz, University of Bern
* Johannes Müller, PoL, TU Dresden
* Laura Žigutytė, PoL, TU Dresden
* Pete Bankhead, University of Edinburgh
* Ryan George Savill, MPI-CBG Dresden / PoL, TU Dresden

We want to acknowledge the people who produced the images we are using for demonstration purposes in this Jupyter book.
* Alba Villaronga Luque, MPI-CBG Dresden
* Alexandr Khrapichev, University of Oxford, UK
* Anne Carpenter, Broad Institute, Boston, MA, United States
* Anne Esslinger, Alberti Lab, MPI-CBG, Germany
* Daniela Vorkel, Myers Lab, MPI-CBG / CSBD, Dresden, Germany
* David Legland, INRAE, UR BIA, Nantes, France
* Jean-Karim Hériché, Cell Biology/Biophysics Unit, EMBL Heidelberg, Germany
* Jesse Veenvliet, MPI-CBG Dresden
* Mauricio Rocha Martins, Norden Lab, MPI-CBG, Germany
* Nasreddin Abolmaali, OncoRay, TU Dresden, Germany
* Sascha M. Kuhn, Nadler Lab, MPI-CBG Dresden, Germany
* Theresa Suckert, OncoRay, University Hospital Carl Gustav Carus, TU Dresden
* Tony Collins, the creator of ImageJ for Microscopy


We acknowledge support by the Deutsche Forschungsgemeinschaft under Germany’s Excellence Strategy—EXC2068–Cluster of Excellence Physics of Life of TU Dresden.
This project has been made possible in part by grant numbers 2021-240341, 2021-237734 and 2022-252520 from the Chan Zuckerberg Initiative DAF, an advised fund of the Silicon Valley Community Foundation.
We acknowledge the financial support by the Federal Ministry of Education and Research of Germany and by Sächsische Staatsministerium für Wissenschaft, Kultur und Tourismus in the programme Center of Excellence for AI-research „Center for Scalable Data Analytics and Artificial Intelligence Dresden/Leipzig“, project identification number: ScaDS.AI

## License

All contents of this Jupyter book and the corresponding Github repository are licensed [CC-BY 4.0](https://creativecommons.org/licenses/by/4.0/) and 
BSD3 by the [authors and contributors](https://github.com/haesleinhuepf/BioImageAnalysisNotebooks/contributors), unless mentioned otherwise.