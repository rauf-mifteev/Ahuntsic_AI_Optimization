# Optimisation de Tournois de Basketball — Travail Pratique Algorithmes

## Aperçu du projet

Ce projet est réalisé dans le cadre du cours d'Intelligence Artificielle 1 au Collège Ahuntsic. J'y construis un système complet d'optimisation en **Python** dans un **Jupyter Notebook** pour automatiser la sélection d'équipes pour une ligue de basketball amateur.

En partant d'un bassin de 8 joueurs candidats, j'ai structuré l'analyse en **4 étapes successives** pour comparer différentes approches algorithmiques :

| Partie | Algorithme / Modification | Résultat / Objectif |
|---|---|---|
| **Partie 1** | **Programmation linéaire (PuLP)** : Formulation mathématique et résolution exacte. | **Solution optimale garantie** |
| **Partie 2** | **Algorithme glouton** : Implémentation de 3 stratégies locales (meilleur score, ratio score/salaire, ratio score/poids). | Rapide, mais optimum non garanti |
| **Partie 3** | **Programmation dynamique** : Implémentation récursive (naïve vs mémoïsée). | Réduction de la complexité de O(2^n) à linéaire |
| **Partie 4** | **Analyse visuelle** : Génération de 4 graphiques comparatifs de performance. | Validation visuelle avec Matplotlib |

L'objectif principal est de mettre en pratique et de mesurer les compromis entre la force brute, les heuristiques rapides (glouton) et les solutions mathématiques optimales.

## Prérequis

Le code est consolidé en **Python** dans un unique **Jupyter Notebook** et utilise les librairies suivantes :

* [PuLP](https://coin-or.github.io/pulp/) 
* [Matplotlib](https://matplotlib.org/) 
* [NumPy](https://numpy.org/) 

## Lancer le notebook

### Installation en local

Assurez-vous que les dépendances sont installées dans votre environnement et lancez Jupyter à la racine du projet:

```bash
pip install pulp matplotlib numpy jupyter
jupyter notebook
```

Ouvrez le fichier AI_TP2.ipynb et exécutez les cellules séquentiellement de haut en bas pour charger les données partagées, résoudre les algorithmes, et générer les graphiques finaux.
