# Prédiction des prix immobiliers avec le Machine Learning

Ce projet consiste à prédire le prix de logements à partir de leurs caractéristiques en utilisant des techniques de Machine Learning.

L'objectif est de mettre en pratique les principales étapes d'un projet de Data Science : exploration des données, analyse exploratoire, préparation des données, entraînement des modèles, évaluation, comparaison et interprétation des résultats.

## Données

Le jeu de données contient **545 logements** et **13 variables**, notamment :

- superficie
- nombre de chambres
- nombre de salles de bain
- nombre d'étages
- parking
- présence d'une route principale
- chambre d'amis
- sous-sol
- chauffage à eau chaude
- climatisation
- zone préférée
- statut de mobilier

La variable cible est le **prix du logement**.

## Technologies utilisées

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook

## Méthodologie

Le projet suit les étapes suivantes :

1. Exploration et analyse des données
2. Analyse des relations entre les variables
3. Préparation des données
4. Encodage des variables catégorielles
5. Séparation des données en ensembles d'entraînement et de test
6. Entraînement de modèles de Machine Learning
7. Évaluation et comparaison des modèles
8. Validation croisée
9. Analyse des erreurs et interprétation des variables
10. Prédiction du prix d'un nouveau logement

## Modèles utilisés

Deux modèles de régression ont été entraînés et comparés :

- Régression linéaire
- Random Forest Regressor

### Résultats

| Modèle | MAE | RMSE | R² |
|---|---:|---:|---:|
| Régression linéaire | 970 043 | 1 324 507 | **0,653** |
| Random Forest | 1 019 926 | 1 398 072 | 0,613 |

La **régression linéaire** obtient les meilleures performances sur les données de test et a donc été retenue comme modèle final.

Une validation croisée à 5 plis donne un **R² moyen de 0,647**, ce qui indique des performances relativement stables.

## Exemple de prédiction

Le modèle a été utilisé pour estimer le prix d'un nouveau logement à partir de ses caractéristiques.

Pour l'exemple étudié, le prix estimé est d'environ **7 183 114 unités monétaires**.

Cette valeur reste une estimation et doit être interprétée en tenant compte des performances du modèle.


## Fichiers

- `prévision_prix_immobilier.ipynb` : notebook contenant l'ensemble de l'analyse et du développement du modèle.
- `Housing.csv` : jeu de données utilisé pour le projet.
