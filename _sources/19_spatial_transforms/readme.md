# Transformations spatiales

Chaque fois que nous devons modifier la taille des voxels des images ou déplacer/faire pivoter leur contenu, nous appliquons des transformations spatiales. Ces opérations sont le plus souvent appliquées lors du recalage des données d'image. Le recalage d'image est le processus de détermination de la transformation nécessaire pour que deux images s'ajustent bien ensemble si elles sont superposées. Une fois cette transformation déterminée, les images peuvent être fusionnées. Lorsque l'acquisition d'images produit des ensembles de données en mosaïque, plusieurs images de différentes positions dans le même champ de vision, qui se chevauchent partiellement, le recalage d'image peut être appliqué pour rassembler ces images en une seule scène. Nous appelons ce processus l'assemblage d'images.

Voir aussi
* [Recalage d'image (vidéo)](https://youtu.be/3CGC-5vwraM)
* [Article de blog sur le redimensionnement des images et l'(an)isotropie des pixels](https://focalplane.biologists.com/2023/03/02/rescaling-images-and-pixel-anisotropy/)