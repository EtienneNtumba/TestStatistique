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

# Analyse du T de Tschuprow en Python

Ce projet explore l'utilisation du **T de Tschuprow**, une mesure de l'association entre deux variables qualitatives dans un **tableau de contingence**. Il est particulièrement utile pour des **tableaux rectangulaires** où le nombre de lignes et de colonnes est différent.

## 📌 Contenu du projet

### 1. Objectifs
- Comprendre le **T de Tschuprow** et son utilisation.
- Appliquer le **test du Chi²** pour vérifier l'indépendance des variables.
- Calculer le **T de Tschuprow** pour mesurer l'association entre les variables.

### 2. Tests Statistiques Utilisés
- **Test du Chi²** : Vérifie l'indépendance entre deux variables qualitatives.
- **T de Tschuprow** : Mesure la force de l'association entre ces variables.

## 🛠 Bibliothèques Python utilisées
- `numpy` : Manipulation de tableaux numériques.
- `pandas` : Gestion des données tabulaires.
- `scipy.stats` : Calcul du **test du Chi²**.
- `pingouin` : Calcul du **T de Tschuprow** et du **V de Cramer**.

## 🚀 Installation et Exécution

### 1. Prérequis
Assurez-vous d'avoir Python installé ainsi que les bibliothèques nécessaires :
```bash
pip install numpy pandas scipy pingouin
```

### 2. Exécution du Code
Copiez et exécutez le script suivant dans un environnement Python ou dans Google Colab.

```python
# Importation des bibliothèques
import numpy as np
import pandas as pd
import scipy.stats as stats
import pingouin as pg

# 📌 Création d'un tableau de contingence
contingency_table = np.array([[50, 30, 20],
                               [30, 50, 20]])

# 📌 Calcul du test du Chi²
chi2, p, dof, expected = stats.chi2_contingency(contingency_table)

# 📌 Calcul du T de Tschuprow
tschuprow_t = pg.cramers_v(contingency_table, bias_correction=False)  

# 📌 Résultats
print(f"Test du Chi² : Chi² = {chi2:.3f}, p-valeur = {p:.3f}")
print(f"T de Tschuprow : {tschuprow_t:.3f}")
```

## 🔍 Interprétation des résultats
- **Test du Chi²** : Indique s'il existe une **relation statistiquement significative** entre les variables.
- **T de Tschuprow** : Quantifie la **force de l'association** (0 = aucune association, 1 = association parfaite).

## 📂 Google Colab
Vous pouvez exécuter ce projet directement sur **Google Colab** en suivant ce lien :
[🔗 Ouvrir le notebook Google Colab](https://colab.research.google.com/drive/1-YOUR-NOTEBOOK-ID-HERE)


## Author

**Etienne Ntumba Kabongo**  
📧 Email: [etienne.ntumba.kabongo@umontreal.ca](mailto:etienne.ntumba.kabongo@umontreal.ca)  
🔗 GitHub: [EtienneNtumba](https://github.com/EtienneNtumba)

## 📜 Licence
Ce projet est sous licence MIT. Vous êtes libre de l'utiliser, le modifier et le redistribuer.






## Auteurs
Ce projet a été réalisé par **[Etienne Ntumba]**.

