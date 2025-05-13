# 💄 Beauty Flow — Optimisation de la Supply Chain Cosmétique

Ce dépôt GitHub regroupe toutes les phases du projet **"Beauty Flow"**, dont l’objectif est d’optimiser la chaîne d’approvisionnement dans le domaine des cosmétiques en s’appuyant sur des algorithmes de Machine Learning et Deep Learning.

---

## 🗂️ Structure du projet
Deploiment-ML/
├── data/ # Données brutes pour l’ETL et l'entraînement
├── models/ # Modèles entraînés (.pkl, .pt, .h5, .pth...)
├── notebooks/ # Notebooks Jupyter pour exploration et entraînement
├── src/ # Code source (prétraitement, entraînement, évaluation…)
├── requirements.txt # Fichier des dépendances Python
├── app.py # Script principal pour lancer l'application
├── README.md # Documentation du projet

---

## 📦 Données

Le dossier `data/` contient l’ensemble des fichiers de données nécessaires pour entraîner les modèles et construire les processus ETL.

### 🧾 Description des fichiers

| Fichier                              | Description                                                                 |
|-------------------------------------|-----------------------------------------------------------------------------|
| `base_materials_with_units.csv`     | Liste des matières premières utilisées                                     |
| `cosmetic_products_base_materials.json` | Composition des produits cosmétiques à partir des matières premières       |
| `factures_produits.pdf`             | Factures de vente des produits aux magasins                                |
| `orders_products_2022_2024.json`    | Historique des commandes des produits entre 2022 et 2024                   |
| `production_data.xlsx`              | Données sur les temps et capacités de production                           |
| `supplyChain.bak`                   | Sauvegarde de la base de données (fournisseurs, adresses, etc.)           |

---

## 🤖 Modèles Enregistrés

Le dossier `models/` contient les modèles entraînés et prêts à être utilisés dans l'application.

| Fichier                        | Description                                                                 |
|-------------------------------|-----------------------------------------------------------------------------|
| `model_temperature_humidity.pkl` | Modèle de prédiction de température/humidité idéale pour le stockage      |
| `best.pt`                     | Modèle YOLOv8 pour détecter et classifier les produits cosmétiques          |
| `trained_model_cpu.pth`       | Modèle PyTorch recommandant un produit selon la couleur de peau             |
| `my_model.pt`                 | Modèle utilisant OpenCV pour vérifier si un produit est cassé (réclamation) |

🖼️ *[Une image illustrant la détection peut être ajoutée ici]*  
*(Exemple : visualisation d’un produit détecté ou comparaison avant/après)*

---

## 📒 Notebooks d’Expérimentation

Tous les notebooks Jupyter utilisés pour l’expérimentation sont disponibles dans le dossier `notebooks/`.

### 🔬 Deep Learning

| Notebook                              | Description                                                                 |
|--------------------------------------|-----------------------------------------------------------------------------|
| `Broken-non Product.ipynb`           | Détection de produit cassé (YOLOv11)                                        |
| `Product_prediction.ipynb`           | Prédiction du type de produit (YOLOv8)                                      |
| `skin_prod_shade_checkpoint.ipynb`   | Recommandation produit selon la teinte de peau (PyTorch)                    |

### 🧠 Machine Learning

| Notebook                              | Description                                                                 |
|--------------------------------------|-----------------------------------------------------------------------------|
| `model_temperature_humidity.ipynb`   | Prédiction des conditions optimales de stockage                             |

---

## ⚙️ Installation

1. Cloner le dépôt :
```bash
git clone https://github.com/votre-utilisateur/Deploiment-ML.git
cd Deploiment-ML
