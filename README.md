# Gini ou entropie : derrière les branches de nos arbres de décision

Notebook de travail Intechnia, avec sorties exécutées, figures (PNG et SVG), et résultats CSV.

## Reproduction

Décompresser l'archive dans un répertoire local. Créer l'environnement Python (Python 3.13.5 utilisé ici ; Python 3.12 peut également être essayé).

```bash
uv venv --python 3.13.5
source .venv/bin/activate
uv pip install -r requirements.txt
```

Les cellules peuvent prendre un certain temps (notamment les forêts à un thread). Les sorties déjà présentes sont consultables sans réexécution. Les temps d'entraînement ne seront pas nécessairement identiques sur une autre machine. Les versions scientifiques principales sont fixées dans `requirements.txt`; les outils Jupyter ne sont pas intégralement verrouillés.

## Fichiers

- `gini-entropy.ipynb` : démonstrations, protocole, code et sorties.
- `results/` : provenance, inventaire, vérifications des alias, mesures par fold, agrégats, différences appariées, chronométrage brut et médian, sensibilité à la profondeur.
- `figures/` : illustrations originales en PNG et SVG.

Le benchmark principal porte sur 6 datasets, 2 familles de modèles, 2 critères et 15 partitions appariées. Les comparaisons sont descriptives, pas des tests statistiques indépendants ni une évaluation sur un jeu de test final. Les figures et tableaux servent de base à l'article, pas de conclusion universelle sur les critères.
