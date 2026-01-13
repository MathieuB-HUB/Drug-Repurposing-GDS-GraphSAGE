# Drug-Repurposing-GDS-GraphSAGE

## Présentation du projet
Ce projet explore le repositionnement de médicaments (*drug repurposing*) en utilisant la science des graphes et l'apprentissage automatique. L'objectif est d'identifier de nouvelles indications thérapeutiques pour des molécules existantes en analysant les interactions complexes entre gènes, maladies et composés chimiques.

Le projet s'appuie sur le dataset **Hetionet v1.0**, modélisant un réseau biologique hétérogène de grande échelle.

## Architecture Technique
Le pipeline de données et d'analyse repose sur les technologies suivantes :
* **Base de données de graphes** : Neo4j
* **Analytique** : Neo4j Graph Data Science (GDS)
* **Langages et Bibliothèques** : Python, Pandas, Client Python GDS

## Méthodologie
Le projet est structuré autour d'un pipeline complet de Data Science :
1. **Ingestion et Modélisation** : Structuration du dataset Hetionet en un graphe de connaissances.
2. **Analyse Topologique** : Utilisation d'algorithmes de centralité (PageRank) pour identifier les entités biologiques clés.
3. **Feature Engineering** : Génération d'embeddings de nœuds via des algorithmes de réduction de dimension et d'apprentissage inductif.
4. **Machine Learning** : Entraînement de modèles pour la prédiction de liens (Link Prediction) afin d'inférer de nouvelles relations "Composé-Traite-Maladie".

## Statut du projet
Ce dépôt contient les travaux de recherche initiaux réalisés dans le cadre du Master MIAGE (Université Paris Nanterre). Les modèles incluent des approches classiques (Random Forest) et des approches de Deep Learning sur graphes (GraphSAGE).
