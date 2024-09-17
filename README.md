# Détection de Fraude

Ce projet concerne la détection de fraude dans les transactions par carte de crédit en utilisant un modèle de machine learning. L'objectif est de construire un modèle capable d'identifier les transactions frauduleuses parmi des transactions normales.

## Contenu du Notebook

Le notebook comprend les étapes suivantes :

1. **Chargement des Données**: Importation du dataset "creditcard.csv" à partir de Google Drive.
2. **Analyse Exploratoire des Données (EDA)**:
   - Examen de la distribution des classes pour identifier le déséquilibre des données.
   - Visualisation des données pour mieux comprendre les caractéristiques.
3. **Feature Engineering et Sélection**:
   - Ingénierie des caractéristiques pour améliorer la performance du modèle.
   - Sélection des caractéristiques pertinentes pour la détection de fraude.
4. **Séparation Train-Test**: Division des données en ensembles d'entraînement et de test pour évaluer les performances du modèle.
5. **Entraînement du Modèle**: Construction et entraînement du modèle de machine learning pour la détection de fraude.
6. **Évaluation du Modèle**: Évaluation des performances du modèle à l'aide de métriques telles que la précision et la matrice de confusion.

## Prérequis

Pour exécuter ce notebook, les bibliothèques suivantes sont nécessaires :
- pandas
- numpy
- matplotlib
- scikit-learn
- plotly

Assurez-vous également d'avoir accès à Google Drive si vous souhaitez charger les données de la même manière.

## Utilisation

1. **Installation des dépendances**: Assurez-vous d'installer toutes les bibliothèques nécessaires. Vous pouvez le faire en exécutant :
   ```bash
   pip install pandas numpy matplotlib scikit-learn plotly

2. **Exécution du Notebook**: Chargez et exécutez le notebook `Détection_Fraude.ipynb`. Assurez-vous d'avoir accès au dataset "creditcard.csv".

## Structure des Fichiers

- `Détection_Fraude.ipynb`: Le notebook principal contenant le code et les analyses.
- `creditcard.csv`: Le fichier de données utilisé pour entraîner et évaluer le modèle (chargé dans Google Drive).

## Résultats

Le modèle entraîné permet de détecter les transactions frauduleuses avec une certaine précision. Les résultats détaillés et les visualisations sont disponibles dans le notebook.

## Auteurs

Koceila KEMICHE.
