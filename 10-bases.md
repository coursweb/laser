---
layout: page
title: Bases
permalink: bases.html
---

Infos sur la gravure et la découpe laser.

## Au centre de production de l'Eracom

**Polar Digicut** : c'est le premier découpeur laser de Polar, fabricant allemand surtout connu pour ses massicots.

Public cible : Imprimeurs, finition.  
Spécialité: Papier/carton, séries

Laser de 30W, plateau de 860 × 610 mm.  
Découpe laser: épaisseur maximum 3mm  
Gravure laser: épaisseur 6 à 10 mm  
Format planche maximum: 80x60 cm

Instructions: [voir PDF](https://eracom.ch/extranet/wp/wp-content/documents/CentreProduction/05-CProd-Fiche_Technique-DCE_Decoupe_Laser-01_2026.pdf).

**Couleurs à utiliser:**

Lors de la réalisation du fichier : utiliser les 3 couleurs existantes dans le nuancier original d’Adobe Illustrator soit :

- **Coupe** -> **Noir**
- **Rainage demi-corps** -> <span style="color:red">Rouge</span> CMJN
- **Gravure en surface** -> <span style="color:#f0f">Magenta</span> CMJN

L’épaisseur donnée au contour doit être de : 0,01 mm

![la Polar Digicut](images/digicut-eracom.avif)

---

## Au FabLearn HEP

Voir les infos "[Découpe et gravure laser](https://fablearn.hepl.ch/project/decoupeuse-laser/)" sur le site du FabLearn.

En bref: trois machines à disposition:

**Trotec Speedy 100R**  
Dimensions du plateau : 610 x 305 mm  
Paramètres conseillés: Contreplaqué peuplier  
Épaisseur [mm] : 4 mm  
Puissance [% du max.] : 80  
Découpe laser: peut aller jusqu'à 6 mm  
Gravure laser: En cas de doute, un premier compromis pourrait être : Puissance [% du max.] : 60%, Vitesse [% du max.] : 25%.

Public cible: Makers, artisans, fablabs.  
Spécialité: Tous matériaux, pièces variées

**FLUX beamo**  
Dimensions du plateau : 300 x 210 mm

**VEVOR**  
Dimensions du plateau : 900 x 600 mm

Couleurs pour découpe Fablearn:

- **Découpe** -> <span style="color:red">Rouge</span> (RVB)
- **Gravure vectorielle** -> <span style="color:blue">Bleu</span> (RVB) 
- **Gravure de trame** -> **Noir** (RVB)

![](images/infos-decoupe-laser-fablearn.png)

## Quelle machine pour quel usage ?

* Si votre usage est la gravure/découpe bois et matériaux variés, la **Trotec Speedy 100R** est bien plus adaptée. 
* Le **Digicut** est davantage taillé pour la finition d'imprimés en série.

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


## Type de bois recommandé

**Contreplaqué peuplier** 600 x 600 x 4mm [chez Jumbo.ch](https://www.jumbo.ch/fr/construction-renovation/bois/bois-de-construction-bois-profile/planches/contreplaque-peuplier-600-x-600-x-4mm/p/6231570?tt=X1NFUF9mMzZhZGFkYjcxNDRmZjg3NTRhOWFiYzM5ZDk1Yjg1Y19QT1NfMQ==#modal).  
Prix par planche: CHF 6.95