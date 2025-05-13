# Deploiment-ML
Projet Intégrer durant l'année universitaire 24-25.

## Installation
1. Clonez le dépôt :
   ```powershell
   git clone https://github.com/<votre-utilisateur>/<votre-repo>.git
   ```
2. Installez les dépendances :
   ```powershell
   pip install -r requirements.txt
   ```

## Utilisation
1. Lancez l'application :
   ```powershell
   python app.py
   ```
2. Faites une requête POST à l'API `/predict` avec des données JSON :
   ```json
   {
       "features": [valeur1, valeur2, ...]
   }
   ```

## Structure du projet
Voici la structure du projet :
```
Deploiment-ML/
├── data/                # Données utilisées pour entraîner/tester le modèle
├── models/              # Modèle(s) sauvegardé(s) (ex. : .pkl, .h5)
├── notebooks/           # Jupyter Notebooks pour l'exploration
├── src/                 # Code source (prétraitement, entraînement, etc.)
├── requirements.txt     # Dépendances Python
├── app.py               # Script principal pour exécuter ou servir le modèle
├── README.md            # Documentation du projet
```
