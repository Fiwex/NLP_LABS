# NLP_LAB6

Adrien Giget, Tanguy Malandain, Denis Stojiljkovic

## A propos du projet

Ce projet est la deuxième partie de la deuxième partie de la matière NLP.
Nous abordons les implémentations 'deep' des classifiers en NLP.

Dans un premier temps, nous avons repris le tutoriel [language translation with nn.Transformer and torchtext tutorial](https://pytorch.org/tutorials/beginner/translation_transformer.html).
Et dans un second temps, nous avons répondu à des questions théoriques sur le tranformer utilisé puis 
nous avons implémenté des fonctions de décodage annexes et de scoring BLEU pour analyser nos résultats.

## Description du fichier

Le fichier est séparé en quatres parties

### 01 - Tutoriel Pytorch tranformers

Repris depuis le site de Pytorch, ce tutoriel nous a permis de comprendre le fonctionnement des transformers.

### 02 - Questions théoriques

Ce fichier contient les réponses aux questions théoriques posées dans le sujet. Sur l'encoding,
des paramètres et les fonctions de mask.

### 03 - Implémentation des fonctions de décodage

- Implémentation de la méthode `top-k`, qui permet de choisir les k mots les plus probables
- Implémentation de la méthode `top-p`, qui permet de choisir les mots dont la somme des
probabilités est supérieure à p.


### 04 - Implémentation du scoring BLEU

Implémentation du scoring BLEU pour comparer les résultats de nos modèles. Nous avons utilisé
SACREBLEU et la fonction corpus_score() pour évaluer notre transformer avec les différentes fonctions
de décodage implémentées.
