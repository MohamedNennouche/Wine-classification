## But du projet
Le but de ce projet est de traiter un dataset connu qui est celui classant plusieurs vins suivant plusieurs caractéristiques en plusieurs catégories de qualités de vin. 
## Description du dataset 
### Les caractéristiques
- Acidité fixe
- Acidité volatile
- Acide citrique
- Sucre résiduel
- Chlorides
- Dioxide de sulfure libre
- Dioxide de sulfure total
- Densité
- pH
- Sulphates
- Alcool
### La sortie
La sortie est la qualité du vin qui est de 3 à 9 
## Disposition du dépôt
* wine-notebook.ipynb : Contient la totalité du projet réalisé
* wineqality-red : Classe les vins rouges 
* winequality-white : Classe les vins blanc
* winequality.names : Descriptif du projet fait par ses auteurs
## Pré-requis logiciels 
Python 3.8 et +
Ainsi que les packages suivant : 
- Numpy
- Pandas
- Seaborn
- Scikit-learn
- Matplotlib
## Contenu du projet
1. Chargement des données
2. Analyse globale des données du dataset
3. Ensemble de visualisation des données et analyse de la corrélation entre les différentes variables
4. Application d'une réduction de la dimensions du problème en utilisant la PCA
5. Application d'un ensemble d'algorithme de classification en analysant les performances en test : 
    - KNN
    - SVM 
    - Stochastic Gradient Descent
    - Gaussian Processes
    - Gaussian Naive Bayes
    - MLP
    - Random Forrest
    - Ensemble learning
6. Application d'une augmentation des données pour uniformiser au mieux les données pour améliorer les résultats
7. Etude comparative avant et après augmentation des données

Cet enchaînement est fait sur le dataset winequality-white.csv mais est appliquable de la même manière sur winequality-red.csv
## Performances atteintes
### Avec les caractéristiques de base
Etant un problème où les classes ne sont pas équilibrées donc la précision n'est pas un indicateur assez bon, et c'est pour cela qu'on opte pour le F1 score
|   Algorithme choisi    |   Précision en test (%)    | F1 score (%) |
|---    |:-:    | :-:    |
|   KNN     |  58.03  |   58.05  |
|   SVM   |   43.81    |    30.04    |
|   Gradient Boosting   |  62.65   |     |
|   Gaussian Processes    |   57.96    |   57.98  |
|   Gaussian Naive Bayes   |    45.1  |  44.11   |
|   Random Forrest   |   68.03   |    67.34   |
|   MLP   |   53.4   |   49.41   |
|   Extremely randomized tree   |   68.44   |    67.36  |
### Après réduction de la dimensionnalité du problème
|   Algorithme choisi    |   Précision en test|  F1 score (%) |
|---    |:-:    |:-:    |
|   KNN     |  61.7  |   61.69   |
|   SVM   |   53.61    |    49    |
|   Gradient Boosting   |   58.37  |     |
|   Gaussian Processes    |    56.26   |   53.6  |
|   Gaussian Naive Bayes   |   45.99   |   40.13  |
|   Random Forrest   |   65.58   |    63.23   |
|   MLP   |   57.55   |   57.95   |
|   Extremely randomized tree   |   65.44   |   64.44   |
## Remarques
## Todo
- [ ] Augmentation des données pour essayer d'améliorer la distribution des classes