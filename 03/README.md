# NLP - LAB 03

Giget Adrien, Tanguy Malandain, Denis Stojiljkovic

## A propos du projet

Ce projet est la deuxième partie à l'introduction de la matière NLP.

On manipule des milliers de commentaires de films séparés en 2 classes 
(positif ou négatif) pour ensuite prédire dans quelle classe se trouve 
les prochains commentaires grâce aux mots utilisés à l'intérieur.
Pour ce faire, nous allons reprendre les algorithmes de traitement des
commentaires que nous avons implémenté dans le lab 02 et vectoriser chaque
commentaire selon différentes features.


## Description du fichier

Le fichier est séparé en deux parties.


### Les features

Dans cette première section nous avons implémenté les features suivantes pour notre vectorisation :
* 1 si "no" apparait dans le texte, 0 sinon.
* La somme de prénoms de la première et deuxième personne dans le texte.
* 1 si "!" est dans le texte, 0 sinon.
* Log(sum des mots dans le texte).
* Nombre de mots issus d'un lexique positif dans le texte.
* Nombre de mots issus d'un lexique négatif dans le texte.
* Log(sum des mots sans les stops words dans le texte).

### Classification par régression logistique

Dans cette section, nous avons implémenté une régression logistique pour classifier les commentaires.
Elle est grandement issue d'un document fourni qui a été adapté à notre cas.

Quelques tests sont effectués pour comparer les résultats de la régression logistique 
selon différents paramètres propre à PyTorch.

Enfin une version faite via sklearn est implémentée pour comparer les résultats.
