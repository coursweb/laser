---
layout: page
title: Préparer les SVG
permalink: preparer-SVG.html
---

## Préparation des fichiers SVG pour Trotec

Pour que le fichier SVG soit bien lu par la machine Trotec, voici des conseils de préparation (à effectuer dans Inkscape):

### Vérifier Fill et Stroke.

- Les éléments pour découpe: doivent avoir un **contour** (*Stroke*) de couleur rouge, et pas de remplissage (*Fill*).
- Les éléments à graver: doivent avoir du remplissage (*Fill*), mais pas de contour (*Stroke*). 
- Epaisseur des tracés (Stroke): en général, mettre 0.1 mm.

**Astuce:** en ayant un élément sélectionné, l'indicateur dans le coin inférieur gauche montre les valeurs de *Fill* et *Stroke*.

![Problématique: cet élément a un Fill (rouge) et un Stroke (sans couleur mais présent)](images/fill-stroke-1.png)

![Correct: cet élément n'a pas de Fill, seulement un Stroke (rouge)](images/fill-stroke-1.png)


### Défaire groupes et formes

- **Défaire les groupes**. Pour cela, on peut *tout sélectionner* (cmd-A), et faire *Object > Ungroup*. Eventuellement répéter, jusqu'à ce qu'il n'y ait plus de groupes. 
- Transformer les **objets géométriques** tels que cercles ou rectangles, en tracés (Paths). Faire *Path > Object to Path*.
- Pour sélectionner tous les objets d'un type, faire *Edit > Select Same > Object Type*.

**Astuce:** le bas du document contient un message indiquant si les éléments sélectionnés comportent des groupes. Dans l'image ci-dessous, il y a un problème car la sélection comporte des *Groupes* et *Cercles*. On aimerait n'avoir que des *Paths*.

![Détail des éléments sélectionnés](images/inkscape-objects-selected.png)