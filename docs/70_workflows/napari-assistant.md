# L'Assistant Napari

L'Assistant Napari est un plugin pour napari qui permet de configurer un flux de travail de traitement d'image.

Ce tutoriel est également disponible en vidéo [napari-assistant.mp4](images/napari-assistant.mp4).

Démarrez napari depuis la ligne de commande comme ceci :

```bash
conda activate my_first_env

napari
```

![](images/napari-assistant01.jpg)

La fenêtre napari s'ouvrira. Cliquez sur le menu `File > Open Samples Cells(3D+2Ch)` pour ouvrir une image d'exemple.

![](images/napari-assistant02.jpg)

![](images/napari-assistant03.jpg)

Vous pouvez explorer ce jeu de données en cliquant sur le bouton de vue `2D/3D`.

![](images/napari-assistant04.jpg)

Lancez l'Assistant Napari depuis le menu `Tools > Utilities > Assistant (na)`.

![](images/napari-assistant05.jpg)

Dans le panneau `Assistant`, cliquez sur le bouton `Remove noise`.

![](images/napari-assistant06.jpg)

Cliquez sur les boutons `Eye` dans la liste des couches pour masquer l'image originale et n'afficher que le résultat de l'étape `Remove noise`.

![](images/napari-assistant07.jpg)

Cliquez sur le bouton `Binarize` dans le panneau Assistant pour ajouter une nouvelle étape au flux de travail qui génère une image binaire à partir de la couche actuelle.

![](images/napari-assistant08.jpg)

Basculez entre les vues 2D/3D et la visibilité des couches pour explorer le résultat de l'étape `Binarize`.

![](images/napari-assistant09.jpg)

Après être revenu à la vue 2D, cliquez sur le bouton `Label` dans l'Assistant et choisissez l'opération `Connected component labeling (clEsperanto)`.

![](images/napari-assistant11.jpg)

Sélectionnez la couche `Result of gaussian_blur` dans la liste des couches et modifiez ses paramètres `sigma`. Vous remarquerez que les étapes suivantes (Threshold Otsu et Connected Component Labeling) sont également mises à jour.

![](images/napari-assistant12.jpg)

Passez en vue grille, affichez toutes les couches en utilisant leurs boutons `Eye` et continuez à modifier les paramètres.

![](images/napari-assistant13.jpg)

![](images/napari-assistant14.jpg)

Fermez toutes les couches sauf `nuclei` et `membrane`.

![](images/napari-assistant15.jpg)

Désactivez la vue en grille et cliquez à nouveau sur le bouton `Label` dans l'Assistant.

![](images/napari-assistant16.jpg)

Cette fois, ne changez pas l'opération mais modifiez plutôt le paramètre `spot_sigma`.

![](images/napari-assistant17.jpg)

Basculez à nouveau en vue 3D et inspectez le résultat de cette seule étape.

![](images/napari-assistant18.jpg)