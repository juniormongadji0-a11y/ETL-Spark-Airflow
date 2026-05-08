# Pipeline ETL Spark & Airflow — Online Retail II

## Description
Pipeline ETL complet construit avec Apache Spark et orchestré par Apache Airflow.
Les données proviennent du dataset Online Retail II (Kaggle, 1M+ lignes).

## Architecture
- **Bronze** : Extraction des données brutes depuis le CSV source
- **Silver** : Nettoyage, suppression des doublons et valeurs nulles, ajout TotalPrice
- **Gold** : Agrégations finales — ventes par pays, par mois, top 10 produits

## Fichiers
- `extract.ipynb` — Job Extract (couche Bronze)
- `transform.ipynb` — Job Transform (couche Silver)
- `aggregate.ipynb` — Job Aggregate (couche Gold)
- `visualisation.ipynb` — Graphiques et Dashboard
- `dag_etl.py` — DAG Apache Airflow

## Dataset
Online Retail II — Kaggle
1 067 371 lignes, 8 colonnes
Transactions e-commerce d'un magasin UK (2009-2010)

## Auteur
MONGADJI ANWAR
