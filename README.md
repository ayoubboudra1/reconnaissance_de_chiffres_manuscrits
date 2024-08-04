# TP1 : La reconnaissance de chiffres manuscrits

Ce projet a pour but de réaliser différents modèles de réseaux de neurones profonds en utilisant le célèbre ensemble de données MNIST et de comparer leur précision (accuracy).

## Objectifs
- Lire et préparer les données MNIST.
- Construire et entraîner plusieurs modèles de réseaux de neurones.
- Évaluer et comparer la précision des modèles.
- Visualiser les résultats à l'aide de matrices de confusion.

## Bibliothèques utilisées
- numpy
- matplotlib
- seaborn
- tensorflow
- keras
- cv2

## Modèles Implémentés
1. **Modèle A** : Un réseau de neurones à deux couches avec des fonctions d'activation sigmoïdes.
2. **Modèle B** : Un réseau de neurones à trois couches avec des fonctions d'activation sigmoïdes.
3. **Modèle C** : Un réseau de neurones à trois couches avec des fonctions d'activation ReLU et sigmoïdes.
4. **Modèle D** : Un réseau de neurones à trois couches avec des fonctions d'activation ReLU et sigmoïdes, en utilisant des images binarisées.

## Préparation des données
- Chargement des données MNIST et division en ensembles d'entraînement et de test.
- Normalisation des données.
- Redimensionnement des images pour les transformer en tableaux unidimensionnels.
- Binarisation des images pour le Modèle D.

## Entraînement des Modèles
- Chaque modèle est entraîné sur 10 époques en utilisant l'optimiseur 'adam' et la fonction de perte 'sparse_categorical_crossentropy'.
- Les précisions (accuracy) et les pertes (loss) sont évaluées sur les données de test.

## Évaluation et Visualisation
- Affichage des matrices de confusion pour visualiser les performances des modèles.
- Comparaison des précisions et des pertes des différents modèles.

## Résultats
Voici un résumé des performances des différents modèles :
| Modèle | Accuracy | Loss |
|--------|----------|------|
| A      | 0.9749   | 0.0760|
| B      | 0.9739   | 0.0958|
| C      | 0.9827   | 0.0717|
| D      | 0.9785   | 0.0916|

## Conclusion
Ce projet démontre l'efficacité des réseaux de neurones profonds pour la reconnaissance de chiffres manuscrits, en comparant différentes architectures et en utilisant des techniques de prétraitement des données comme la binarisation.
