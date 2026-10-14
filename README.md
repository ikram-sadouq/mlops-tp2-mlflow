
# TP2 MLOps — MLflow

## Objectif
Construire un pipeline de machine learning pour détecter les transactions frauduleuses, suivre les expériences avec MLflow et gérer les versions des modèles.

## Technologies
- Python
- pandas et NumPy
- scikit-learn
- MLflow
- PyYAML
- Matplotlib

## Pipeline
1. Préparation des données avec `src/preparer.py`
2. Entraînement du modèle avec `src/entrainer.py`
3. Évaluation avec `src/evaluer.py`
4. Orchestration avec `pipeline.py`

## Registre des modèles
Le modèle `fraude` possède trois versions enregistrées dans MLflow :
- Alias `staging` : version 2
- Alias `production` : version 1

## Lancement
Installer les dépendances :

```bash
pip install -r requirements.txt
```

Générer les données :

```bash
python donnees.py
```

Lancer le pipeline :

```bash
python pipeline.py
```
