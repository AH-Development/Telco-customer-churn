
# **Prédiction du Churn des Clients (Telco Customer Churn Dataset)**

## **Description du Projet**
Ce projet vise à prédire le **churn** (abandon) des clients d'un service de télécommunications en utilisant des données clients réelles. Le but est de construire un modèle de Machine Learning capable de déterminer si un client va quitter le service en fonction de son historique et de ses caractéristiques.

Le dataset utilisé provient de Kaggle et contient des informations sur les clients d'une entreprise fictive de télécommunications, comme les détails des abonnements, les services souscrits, et les informations démographiques.

## **Objectif**
L'objectif principal de ce projet est de prédire si un client va quitter l'entreprise ou non en utilisant des techniques de classification binaire. Le modèle sera évalué en fonction de son **précision** et de sa capacité à identifier les clients qui risquent de quitter.

---

## **Technologies et Bibliothèques Utilisées**
- **Python 3.x**
- **Pandas** : Pour la manipulation des données.
- **Matplotlib & Seaborn** : Pour la visualisation des données.
- **Scikit-learn** : Pour l'entraînement et l'évaluation des modèles de Machine Learning.
- **Jupyter Notebook** : Pour l'exécution du projet étape par étape.

---

## **Structure du Projet**
Voici la structure du projet :

```
Telco_Customer_Churn/
│
├── data/                # Contient le fichier CSV du dataset
│   └── telco_churn.csv
│
├── notebooks/           # Contient le Jupyter Notebook avec le code d'analyse
│   └── churn_prediction.ipynb
│
├── README.md            # Ce fichier
└── requirements.txt     # Liste des dépendances du projet
```

---

## **Étapes du Projet**

1. **Téléchargement et Préparation des Données**
   - Téléchargement du dataset depuis Kaggle et chargement dans un DataFrame Pandas.
   - Inspection des données pour vérifier la présence de valeurs manquantes et de doublons.

2. **Exploration des Données (EDA)**
   - Analyse des variables et de leur relation avec la variable cible `Churn`.
   - Visualisation de la distribution des données et des relations entre les caractéristiques.

3. **Prétraitement des Données**
   - Gestion des valeurs manquantes, encodage des variables catégorielles, mise à l'échelle des données numériques.
   - Création de variables de caractéristiques numériques et transformation des variables catégorielles en variables binaires.

4. **Entraînement des Modèles**
   - Test de plusieurs modèles de Machine Learning (Régression Logistique, Arbre de Décision, Random Forest).
   - Séparation des données en ensemble d'entraînement et ensemble de test.

5. **Évaluation des Modèles**
   - Utilisation de métriques de classification telles que la précision, le rappel, le F1-score, et l'AUC-ROC pour évaluer les performances des modèles.
   - Comparaison des résultats obtenus par les différents modèles.

6. **Optimisation du Modèle**
   - Si nécessaire, ajustement des hyperparamètres avec **GridSearchCV** pour améliorer la performance du modèle.

7. **Conclusion**
   - Résumé des résultats obtenus, identification du meilleur modèle, et discussion des pistes d'amélioration.

---

## **Exécution du Code**
Le code principal du projet se trouve dans le fichier **`notebooks/churn_prediction.ipynb`**. Voici comment l'exécuter :

1. Ouvre le fichier **`churn_prediction.ipynb`** dans Jupyter Notebook ou JupyterLab.
2. Exécute chaque cellule du notebook pour suivre les étapes d'analyse et de construction du modèle.
3. À la fin du notebook, tu devrais obtenir un modèle capable de prédire si un client va quitter ou non l'entreprise.

---

## **Résultats**
Le modèle le plus performant était un **Random Forest Classifier**, qui a montré une bonne précision et a été capable de détecter efficacement les clients à risque de churn. Les résultats détaillés peuvent être trouvés dans les sections de l'EDA et de l'évaluation des modèles dans le notebook.

---

## **Améliorations Futures**
- Utilisation de techniques avancées comme l'**XGBoost** pour améliorer encore la performance du modèle.
- Déploiement du modèle sous forme d'**API** pour prédire le churn en temps réel avec de nouvelles données.
- Ajout de nouvelles variables d'entrée comme des données comportementales des clients (ex. interactions avec le service client).

---

## **Références**
- Kaggle Dataset : [Telco Customer Churn](https://www.kaggle.com/blastchar/telco-customer-churn)
- Documentation Scikit-learn : [https://scikit-learn.org/](https://scikit-learn.org/)

---

### **Note**
Le dataset utilisé dans ce projet provient de Kaggle et est un jeu de données simulé, ce qui signifie qu'il ne provient pas d'une entreprise réelle. Les résultats du modèle peuvent ne pas refléter exactement les performances dans un environnement de production réel.
