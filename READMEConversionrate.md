# Conversion Rate Challenge

## Introduction

Ce projet a été développé dans le cadre de la certification de Machine Learning Engineer suite à la formation Fullstack chez Jedha.
L'exercice avait pour objectif de résoudre un défi kaggle de taux de conversion, c'est à dire ici si un lecteur s'aboonnera à la newsletter de www.datascienceweekly.org  

## Prérequis

Installation des librairies Python requises :

- `pandas`
- `numpy`
- `scikit-learn`
- `matplotlib`
- `plotly`
- `IPython`

## Données
Les données proviennes du site kaggle. Elles ont été divisé en 2 dataset : un premier qui sert de test avec l'ensemble des variables et la target (data_train.csv), un 2e sans la target (data_test.csv) pour la prediciton finale.

## Modèles

Après une exploration des données et une analyse univariée un modèle.
Matrice de correlation indique que la variable la plus intéressante est le nombre de pages visité par l'utilisateur avant de s'inscrire à la newsletter.

Un modèle de regression linéaire univarié est entraîné et testé. L'évaluation des performance est effectué via le calcul du score F1.

On applique ensuite un modèle de regression multivarié en prenant l'ensemble des variables et on évalue de nouveau les performances. Ce modèle apporte un score de performance plus important.
On entraîne donc ce nouveau modèle sur l'ensemble des données.

Le jeu de donnée sans target (data_test.csv) est chargée, on y applique le même preprocessing et on utilise ce modèle sur l'ensemble test.


