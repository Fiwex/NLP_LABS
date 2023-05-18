# NLP_LAB5

Adrien Giget, Tanguy Malandain, Denis Stojiljkovic

## A propos du projet

Ce projet est la première partie de la deuxième partie de la matière NLP. 
Nous abordons les implémentations 'deep' des classifiers en NLP.

On manipule des milliers de commentaires de films séparés en 2 classes 
(positif ou négatif) pour ensuite prédire dans quelle classe se trouvent 
les prochains commentaires grâce aux mots utilisés à l'intérieur.

Pour ce faire, nous allons d'une part créer notre propre RNN et d'autre part utiliser
un RNN de PyTorch.


## Description du fichier

Le fichier est séparé en deux parties.

### 01 - Notre RNN

Nous avons implémenté notre propre RNN via PyTorch en suivant la structure suivante :
* The embedding layer turns a one-hot vectors into dense vectors.
* The first matrix (W) connects the embedding to the hidden layer.
    * `embedding_size -> hidden_size`
* The second matrix (U) connect the previous hidden layer to the current one.
    * `hidden_size -> hidden_size`
* These to vectors are added and go through an activation function (e.g. $h_t = tanh(Wx_i+Uh_{t-1})$).
* The last matrix (V) connects the hidden layer to the hidden layer to the output.
    * `hidden_size -> 1`
* An `init_hidden` function which initialize the first hidden layer to 0.

Et nous calculons ensuite son accuracy.

### 02 - Les RNN de Pytorch

Nous disposons d'un modèle de base naïf : Simple RNN

Puis, nous avons testé plusieurs implémentations de CNN PyTorch, tel que :
- LSTM
- BiLSTM

Et nous comparons les différentes accuracies de ces réseaux.