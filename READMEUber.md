# Analyse et Clustering de Données de Trajets Uber

## Introduction

Ce projet a été effectué dans le cadre de la formation fullstack Jedha. Il s'agit d'effectuer une analyse des données de trajets Uber et utilise des techniques de clustering pour regrouper les données spatiales en clusters. 

## Données

Les données de trajets Uber sont téléchargées depuis un fichier ZIP en ligne et décompressées pour être utilisées dans le code.
Un échantillonage de 10000 lignes est utilisé ici.

## Visualisation Géospatiale

Le code utilise Plotly pour créer des cartes interactives affichant les trajets Uber sur une carte. Les données sont représentées en fonction de l'emplacement (latitude et longitude) et de la base de départ.

## Prétraitement des Données

Les données horodatées sont converties en objets datetime, puis divisées en heures, jours de la semaine et jours du mois. Les colonnes redondantes sont supprimées.

## Clustering avec DBSCAN

Le code utilise l'algorithme DBSCAN (Density-Based Spatial Clustering of Applications with Noise) pour effectuer le clustering des données. Les paramètres tels que `eps` et `min_samples` sont définis pour le clustering.

Les clusters sont ajoutés aux données, et une carte interactive est créée pour visualiser les clusters, en excluant les points considérés comme des outliers par DBSCAN.

## Clustering avec K-Means

Le code utilise l'algorithme K-Means pour effectuer un autre clustering des données. La méthode du coude est utilisée pour déterminer le nombre optimal de clusters, et le score silhouette est également calculé.

Les clusters K-Means sont ajoutés aux données, et une carte interactive est créée pour visualiser les clusters, en excluant les points considérés comme des outliers par K-Means.

## Conclusion

Ce code vous permet d'explorer, analyser et cluster des données de trajets Uber en utilisant des méthodes de clustering spatiales. Vous pouvez personnaliser les paramètres de clustering pour obtenir les résultats souhaités.
