# 🌐 Nutri-Sport: A Public Health Application
*(French version below)*

This project focuses on designing **Nutri-Sport**, an innovative application to help athletes choose food products based on their nutritional needs.

## 🌟 Project Content

### 💡 Application Idea
The **Nutri-Sport** app:  
- 📱 Scans products to calculate a **nutritional score** based on proteins, fats, sugars, and other key variables.  
- 🍽️ Suggests similar products with equivalent or better scores.  
- 🏆 Scores are categorized as **Poor**, **Average**, and **Excellent** for easy interpretation.

### 🛠️ Technologies Used
- 🐍 Python: 3.8.8  
- 🐼 Pandas: 1.2.4  
- 🎨 Seaborn: 0.11.1  
- 📊 Matplotlib: 3.3.4  

### 📑 Dataset Cleaning
- 📁 **Data Source**: `fr.openfoodfacts.org.products.csv` (320,000 products).  
- 🧹 **Data Cleaning**:  
  - Reduced columns from 162 to 54 after removing missing values (>80% NaN).  
  - Removed duplicate rows and replaced NaN values with subcategory averages.  
  - Eliminated outliers using the **Percentile** method.  

### 🔍 Exploratory Analysis
- **Univariate Analysis**: Distribution study for variables like `energy_100g`, `fat_100g`, `sugars_100g`.  
- **Bivariate Analysis**: Identified correlations between variables (e.g., `energy_100g` and `nutrition-score`).  
- **Multivariate Analysis**:  
  - Dimensionality reduction via PCA (Principal Component Analysis).  
  - Validation of hypotheses using statistical tests such as Shapiro-Wilk and Levene.  

### 🏁 Results
- ✅ **App Feasibility**:  
  - Data is sufficient to calculate accurate scores.  
  - Results align well with Nutri-Score classifications.  

## ❗ Areas for Improvement
- ⚠️ **NaN Issue**: Significant presence of missing values.  
- ❓ **Incomplete Information**: Limited data on certain product categories (`pnns_groups`).  

---

# 🍎 Nutri-Sport : Une Application au Service de la Santé Publique

Ce projet propose la conception de **Nutri-Sport**, une application innovante pour aider les sportifs à sélectionner des produits alimentaires en fonction de leurs besoins nutritionnels. 

## 🌟 Contenu du Projet

### 💡 Idée d’Application
L’application **Nutri-Sport** :  
- 📱 Scanne les produits pour calculer un **score nutritionnel** basé sur les protéines, graisses, sucres et autres variables clés.  
- 🍽️ Fournit des suggestions de produits similaires avec des scores équivalents ou supérieurs.  
- 🏆 Les scores sont catégorisés en **Mauvais**, **Moyen**, et **Excellent** pour une compréhension simple.

### 🛠️ Technologies Utilisées
- 🐍 Python : 3.8.8  
- 🐼 Pandas : 1.2.4  
- 🎨 Seaborn : 0.11.1  
- 📊 Matplotlib : 3.3.4  

### 📑 Nettoyage du Dataset
- 📁 **Source des Données** : `fr.openfoodfacts.org.products.csv` (320 000 produits).  
- 🧹 **Filtrage des données** :  
  - Réduction de 162 colonnes à 54 après suppression des valeurs manquantes (>80% NaN).  
  - Suppression des lignes dupliquées et remplacement des NaN par la moyenne des sous-catégories.  
  - Utilisation de la méthode **Percentile** pour éliminer les valeurs aberrantes.  

### 🔍 Analyse Exploratoire
- **Analyse univariée** : Étude des distributions pour des variables comme `energy_100g`, `fat_100g`, `sugars_100g`.  
- **Analyse bivariée** : Identification des corrélations entre les variables (par ex. `energy_100g` et `nutrition-score`).  
- **Analyse multivariée** :  
  - Réduction dimensionnelle via ACP (Analyse en Composantes Principales).  
  - Validation des hypothèses avec tests statistiques comme Shapiro-Wilk et Levene.  

### 🏁 Résultats
- ✅ **Faisabilité de l’Appli** :  
  - Les données sont suffisantes pour calculer des scores précis.  
  - Les résultats sont cohérents avec les classifications Nutri-Score.  

## ❗ Points à Améliorer
- ⚠️ **Problème de NaN** : Présence notable de valeurs manquantes.  
- ❓ **Informations incomplètes** : Données limitées sur certaines catégories de produits (`pnns_groups`).  

