# Analyse Statistique en Python

Ce projet explore différentes méthodes d'analyse statistique en Python, en mettant l'accent sur les tests statistiques et l'analyse des relations entre variables qualitatives et quantitatives.

## Contenu du projet

### 1. Statistique inférentielle
- Estimation
- Tests statistiques
- Intervalles de confiance

### 2. Analyse des relations entre variables
- Variables qualitatives
- Variables quantitatives
- Variables mixtes

### 3. Méthodes et tests statistiques utilisés

#### **Tests de normalité**
- **Test de Shapiro-Wilk** : Vérifie si une variable suit une distribution normale.

#### **Tests d'homogénéité de variance**
- **Test de Levene** : Teste si deux ou plusieurs groupes ont des variances égales.

#### **Tests de comparaison de moyennes**
- **Test de Student (t-test indépendant)** : Compare les moyennes de deux groupes indépendants.
- **Test de Kruskal-Wallis** : Alternative non paramétrique au test ANOVA, utilisé lorsque les données ne suivent pas une distribution normale.

#### **Corrélation entre variables**
- **Corrélation de Pearson** : Mesure la relation linéaire entre deux variables quantitatives.
- **Corrélation de Spearman** : Alternative non paramétrique utilisée pour mesurer la relation entre deux variables ordinales ou non linéaires.
- **Corrélation de Kendall** : Alternative robuste à la corrélation de Spearman pour des petits échantillons.

#### **Tests d'indépendance pour variables qualitatives**
- **Test du Chi²** : Évalue l'indépendance entre deux variables qualitatives.

## Bibliothèques Python utilisées
- `pandas` : Manipulation des données
- `numpy` : Calculs numériques
- `matplotlib.pyplot` et `seaborn` : Visualisation des données
- `scipy.stats` : Tests statistiques

## Exécution du projet
### Prérequis
Assurez-vous d'avoir Python installé avec les bibliothèques nécessaires :
```bash
pip install pandas numpy matplotlib seaborn scipy
```

### Lancer le notebook
1. Clonez ce dépôt :
```bash
git clone [https://github.com/VotreNomUtilisateur/NomDuRepo.git](https://github.com/EtienneNtumba/TestStatistique.git)
```
2. Accédez au dossier :
```bash
cd NomDuRepo
```
3. Ouvrez le notebook Jupyter :
```bash
jupyter notebook Tests_Statistique_Python.ipynb
```

## Auteurs
Ce projet a été réalisé par **[Etienne Ntumba]**.

