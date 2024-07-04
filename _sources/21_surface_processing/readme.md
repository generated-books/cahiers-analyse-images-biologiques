# Traitement de surface

Dans ce chapitre, nous allons traiter des données de surface. Les surfaces, également connues sous le nom de maillages, se composent de points dans l'espace 3D, appelés sommets, qui sont reliés entre eux pour former des triangles, également appelés faces. De nombreux triangles ensemble forment une surface. Si la surface est fermée de telle sorte qu'aucun rayon ne puisse passer de l'intérieur vers l'extérieur sans traverser un triangle, la surface est dite étanche.

## Installation des prérequis

Nous utiliserons la bibliothèque [vedo](https://vedo.embl.es/) pour traiter et visualiser les surfaces, ainsi que le plugin programmable napari [napari-process-points-and-surfaces](https://github.com/haesleinhuepf/napari-process-points-and-surfaces). Les deux peuvent être installés comme suit :

```
mamba install vedo
pip install napari-process-points-and-surfaces
```