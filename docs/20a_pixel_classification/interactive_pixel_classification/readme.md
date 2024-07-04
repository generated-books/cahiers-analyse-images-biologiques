(machine_learning:pixel_classification)=
# Classification interactive des pixels et segmentation d'objets dans Napari

Dans cet exercice, nous allons entraîner un [Classificateur de forêt aléatoire](https://fr.wikipedia.org/wiki/For%C3%AAt_al%C3%A9atoire) pour la classification des pixels et convertir le résultat en une segmentation d'instances.
Nous utiliserons le plugin napari [napari-accelerated-pixel-and-object-classification](https://www.napari-hub.org/plugins/napari-accelerated-pixel-and-object-classification).

## Pour commencer

Ouvrez une fenêtre de terminal et activez votre environnement conda :

```
conda activate devbio-napari-env
```

Ensuite, lancez Napari :

```
napari
```

Chargez le jeu de données d'exemple "Blobs" à partir du menu `File > Open Sample > clEsperanto > Blobs (from ImageJ)`

![](apoc1.png)

## Classification des pixels et segmentation d'objets dans Napari

Pour segmenter des objets, nous pouvons utiliser l'outil de segmentation d'objets dans APOC. 
En coulisses, il utilise un classificateur de pixels et un [étiquetage des composantes connexes](https://fr.wikipedia.org/wiki/%C3%89tiquetage_en_composantes_connexes). 
La procédure suivante est également montrée dans [cette vidéo](apoc_object_segmentation.mp4).

Lancez la segmentation d'objets à partir du menu `Tools > Segmentation / Labeling > Object Segmentation (APOC)`.

![](apoc2.png)

Ajoutez une nouvelle couche d'étiquettes en cliquant sur ce bouton :
![](apoc3.png)

Changez la taille du pinceau à un petit nombre comme 2 ou 3.
![](apoc4.png)

Cliquez sur le bouton `Paint brush`.
![](apoc5.png)

Commencez à annoter la région `background` où il n'y a pas d'objet.
![](apoc6.png)

Augmentez l'étiquette dessinée de un.
![](apoc7.png)

Dessinez une annotation à l'intérieur des objets d'intérêt. Dessinez les annotations de fond et d'objet proches l'une de l'autre. Plus ces deux annotations sont dessinées proches, plus le degré de liberté que l'ordinateur a lors de l'optimisation du modèle plus tard est faible.
![](apoc8.png)

Dans l'interface utilisateur `Object segmentation` à droite, sélectionnez l'image/canal qui doit être traité.
![](apoc9.png)

Sélectionnez également l'image d'étiquettes d'annotation que vous venez de dessiner.
![](apoc10.png)

Cliquez sur `Train`. Une image d'étiquettes devrait apparaître.
![](apoc11.png)

Si la segmentation fonctionne bien, envisagez de sauvegarder le fichier `ObjectSegmenter.cl` qui a été enregistré. 
Si vous n'avez pas changé l'emplacement du fichier avant l'entraînement, il se trouvera dans le dossier à partir duquel vous avez lancé napari en ligne de commande.