# NPL - Lab 02


## A propos du projet

Ce projet est la première partie à l'introduction de la matière NLP.

On manipule des milliers de commentaires de films séparés en 2 classes (positif ou négatif) pour ensuite prédire dans quelle classe se trouve les prochains commentaires grâce aux mots utilisés à l'intérieur.
Pour ce faire, on utilise des algorithmes de Bayes naif, un de notre implémentation en suivant le pseudocode de Dan Jurafsky et James H. Martin et un autre de la bibliothèque scikit-learn, plus précisément MultinomialNB.
#

## Description du fichier

Le fichier est séparé en trois parties.

### Le dataset

Cette première section permet d'importer le dataset IMDB et de d'afficher ce qu'il contient en terme de nombre de sets et de répartition sur les 2 classes.

### L'algorithme de Bayes naif

Dans cette section, on traite tout d'abord le dataset en supprimant des charactères spéciaux ou encore les ponctuations inutiles comme la virgule.
Ensuite on teste notre algorithme de Bayes naif et celui de scikit-learn sur ce dataset modifié et on compare leur efficacité et leur temps d'exécution.
On les teste une seconde fois sans les stop words afin d'augmenter leur efficacité.

### Le stemming

Cette dernière section porte sur le stemming, c'est-à-dire la réduction des mots à leur racine.
On l'appelle sur le dataset modifié et on teste à nouveau nos algorithmes de Bayes naif et celui de scikit-learn.