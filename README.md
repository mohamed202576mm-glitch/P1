# Prédiction de prix immobiliers avec Keras

Petit projet de régression en Deep Learning pour m'entraîner avec TensorFlow et Keras, basé sur le dataset California Housing de Scikit-Learn.

## Fonctionnement
L'objectif est de prédire la valeur médiane des logements à partir de différentes caractéristiques (données démographiques, géographiques, etc.).

## Architecture du modèle
J'ai mis en place un réseau de neurones séquentiel (MLP) qui comprend :
- Une normalisation des entrées (`BatchNormalization`) pour aider l'apprentissage.
- Deux couches cachées de 512 neurones avec une activation ReLU.
- Un système de `Dropout` (0.3) pour limiter le surapprentissage.
- Un `EarlyStopping` pour arrêter l'entraînement dès que la validation stagne et garder les meilleurs poids.

## Bibliothèques utilisées
- Python
- TensorFlow / Keras
- Scikit-Learn
- Pandas / Matplotlib
