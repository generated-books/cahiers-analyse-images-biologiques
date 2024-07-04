# Optimisation des paramètres

Dans ce chapitre, nous allons appliquer certaines stratégies pour optimiser les paramètres des flux de travail de traitement d'image.
En général, il est important d'avoir des données de référence de haute qualité, telles que des images segmentées manuellement.
De plus, une fonction de fitness bien conçue (parfois également appelée fonction de perte) est nécessaire.
Pour l'optimisation des paramètres, nous utiliserons [le package optimize de scipy](https://docs.scipy.org/doc/scipy/reference/optimize.html) et le plugin Napari [napari-workflow-optimizer](https://github.com/haesleinhuepf/napari-workflow-optimizer).