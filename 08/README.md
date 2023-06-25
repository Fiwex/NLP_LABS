# NLP_LAB8

Adrien Giget, Tanguy Malandain, Denis Stojiljkovic

## A propos du projet

Ce projet est la dernière partie de la deuxième partie de la matière NLP.
Nous abordons les implémentations 'deep' des classifiers en NLP.

Pour ce TP, nous nous sommes mis dans un contexte industriel.
Nous nous sommes placé comme une entreprise voulant ventre une API de modération
de tweets toxic. 
Les différentes parties de ce TP sont donc les différentes étapes de sélections
du jeu de données, de création et évaluation d'un modèle et d'annotation
de données de production.

## Description du fichier
Le fichier est séparé en quatre parties

### 01 - Sélection d'un jeu de données labellisé

Nous avons analysé les enjeux légaux d'utilisation de jeux de données sur
[academic Twitter dataset on HuggingFace hub](https://huggingface.co/datasets/tweet_eval).

### 02 - Evaluation du jeu de données

Nous avons analysé le jeu de donnée choisit, `offensive`, en regardant sa 
distribution et les topics les plus présents.

### 03 - Evaluation d'un modèle pré entrainné

Car entraîner un modèle de zéro est couteux et long, nous avons testé un modèle 
pré entrainé : RoBERTa.
Nous l'avons soumis à différents tests ; de précisions, de rappel, de F1-score
et l'avons aussi utilisé sur nos propres données de production.
Enfin, nous l'avons comparé à des modèles plus simples, comme un modèle de 
Bayes Naïf, afin de tester sa pertinence.

### 04 - Annotation de données de production

Pour terminer, nous nous sommes créé un "Golden Dataset". Ces données ont été
annotées en interne, en suivant un barem de notation.
Grâce à ce golden dataset, nous avons pu tester si le modèle pré entrainé RoBERTa
était suffisamment performant pour être utilisé comme modèle de production.