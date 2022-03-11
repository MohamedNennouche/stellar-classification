## But du projet
Le but de ce projet est de parvenir à classer suivant 3 classes : 
1) Galaxies
2) Quasars
3) Etoiles

En se basant sur plusieurs caractéristiques physiques reportées. Le dataset utilisé contient 100 milles échantillons de classes qui sont déséquilibrées et réparties comme suit : 
|   Classe   |   Nombre d'éléments |
|---    |:-:    |
|  Galaxie     |  59445 | 
|  Quasar  |   18961    |   
|  Etoile   |   21594  | 
|  TOTAL   |   100000  | 
## Pré-requis logiciel 
Vous aurez besoin pour réutiliser ce code de : 
- Python 3.8 ou +
- Scikit-learn
- Pandas
- Matplotlib
- Numpy
- Seaborn
## Contenu du projet
Ce projet comporte 3 parties 
1) **Analyse et visualisation des données :** Durant cette étape on analyse globalement les variables et leurs distributions pour extraire les variables d'intérêts et qui pourraient aider efficacement à la classification
2) **Pré-traitement des données :** Durant cette étape on prépare les données pour la classification, et donc on supprime les colonnes qu'on juge inutile ou peu intéressante pour la classification et dans notre cas ce fut : 
    - Rerun ID
    - U
    - G 
    - Z
qui ont été enlevé. Et ensuite une étape de normalisation a été faite sur les données pour les mettre sur la même plage de valeurs. 
3) **Classification :** Durant cette étape on utilise plusieurs algorithmes de classification nous permettant de résoudre le problème donné
## Performances atteintes 
### Sans normalisation des données
|   Algorithme choisi    |   Précision en test|  F1 score (%) |
|---    |:-:    |:-:    |
|   KNN     |  70.94  |   70.94   |
|   Random Forrest   |   97.41   |    97.38   |
|   Extremely randomized tree   |   96.49  |  96.45   |
### Avec normalisation des données
|   Algorithme choisi    |   Précision en test|  F1 score (%) |
|---    |:-:    |:-:    |
|   KNN     |  90.25  |   90.11   |
|   Random Forrest   |   97.38   |    97.35   |
|   Extremely randomized tree   |   96.51  |  96.47   |