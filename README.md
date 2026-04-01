# TP2 AI

Ce dépôt contient les solutions pour le TP2 d'Intelligence Artificielle. L'objectif est d'optimiser la formation de deux équipes de basket sous plusieurs contraintes.

# Détails du projet
- Budget total : 8 500 $ par semaine.
- Formation : 2 équipes de 3 joueurs chacune.
- Contrainte de poids : Maximum 250 kg par équipe.
- Objectif : Maximiser le score total (performance).

# Analyse des résultats

# 1. Programmation Linéaire (PuLP)
C’est la méthode de référence pour trouver la solution mathématique exacte. Le solveur a trouvé un score optimal de 536 points.
- Équipe A : Alice, Clara, Emma
- Équipe B : Bob, Grace, Hugo

# 2. Algorithmes Gloutons (Greedy)
J'ai testé trois stratégies pour voir si un choix simple pouvait s'approcher de l'optimum :

- Stratégie Score : On obtient 522 points avec un budget de 8150 $.
- Stratégie Ratio Score/Poids : Résultat identique (522 points).
- Stratégie Ratio Score/Salaire : C'est le meilleur résultat des trois. On atteint 536 points avec seulement 7400 $. 

Conclusion : Le critère du ratio "Score/Salaire" est ici le plus efficace, car il égale la solution de PuLP tout en économisant du budget.

# 3. Récursion et Programmation Dynamique
Pour tester l'efficacité de l'algorithme, j'ai implémenté le calcul du score cumulé et une comparaison sur la suite de Fibonacci (n=30) :

- Version Naïve : Le calcul prend environ 0.17 secondes car il refait les mêmes calculs plusieurs fois.
- Version Mémoïsée : Le temps descend à 0.00 secondes. L'utilisation de la mémoire (dictionnaire) rend l'exécution instantanée.

# Utilisation
1. Installer la bibliothèque nécessaire : `pip install pulp`
2. Lancer les scripts pour voir les résultats :
   - `python partie1_pl.py`
   - `python partie2_glouton.py`
   - `python partie3_recursion.py`
