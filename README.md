# Détection de Fraude

Ce projet concerne la détection de fraude dans les transactions par carte de crédit en utilisant un modèle de machine learning. L'objectif est de construire un modèle capable d'identifier les transactions frauduleuses parmi des transactions normales.

## Contenu du Notebook

Le notebook couvre les étapes suivantes :

1. **Chargement des Données**: Importation du dataset "creditcard.csv" depuis Google Drive, contenant des transactions par carte de crédit, incluant des exemples de fraudes.

2. **Analyse Exploratoire des Données (EDA)**:
   - Analyse de la distribution des classes pour mettre en évidence le déséquilibre des données entre les transactions normales et frauduleuses.
   - Visualisation des caractéristiques des transactions pour identifier des tendances et des anomalies potentielles.

3. **Feature Engineering et Sélection**:
   - Création et transformation des caractéristiques pour améliorer la capacité du modèle à distinguer les transactions frauduleuses.
   - Sélection des caractéristiques les plus pertinentes pour la détection de fraude, en éliminant celles qui sont moins informatives.

4. **Séparation Train-Test**: Division des données en ensembles d'entraînement et de test pour permettre une évaluation impartiale du modèle.

5. **Entraînement du Modèle**: 
   - **Calcul de la Moyenne et de l'Écart-type**: Le modèle calcule la moyenne (`vect_u`) et l'écart-type (`vect_sigm`) des caractéristiques sur l'ensemble d'entraînement pour établir un profil des transactions typiques.
   - **Détection d'Anomalies**: Utilisation de ces statistiques pour identifier les transactions qui s'écartent significativement de la norme. Un seuil (`eps`) est défini pour déterminer si une transaction est anormale ou potentiellement frauduleuse. Les transactions qui s'écartent trop de la moyenne sont signalées comme suspectes.

   Cette approche permet d'optimiser la détection des fraudes en ajustant le seuil de tolérance (`eps`) pour trouver un équilibre entre la détection de toutes les fraudes possibles et la minimisation des faux positifs.

6. **Évaluation du Modèle**: Évaluation des performances du modèle en utilisant des métriques telles que la précision et le F2-Score.


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
- `creditcard.csv`: Le fichier de données utilisé pour entraîner et évaluer le modèle (à charger sur Google Drive).

## Résultats

Le modèle entraîné permet de détecter les transactions frauduleuses avec une certaine précision. Les résultats détaillés et les visualisations sont disponibles dans le notebook.

## Auteurs

Koceila KEMICHE.
