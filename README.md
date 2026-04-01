# TP2 - Optimisation et Intelligence Artificielle

Ce projet présente trois approches pour résoudre un problème de sélection de joueurs avec un budget limité de 5000 € :
1. **Programmation Linéaire** (avec la bibliothèque PuLP).
2. **Algorithmes Gloutons** (Greedy).
3. **Programmation Dynamique** (Récursivité et Mémoïsation).

## Structure du dépôt
* `partie1_pl.py` : Solution optimale via programmation linéaire.
* `partie2_glouton.py` : Implémentation des 3 stratégies gloutonnes.
* `partie3_dynamique.py` : Algorithme d'optimisation exacte.
* `README.md` : Documentation du projet et analyse des résultats.

---

## Partie 2 : Approche Gloutonne (Greedy)

Nous avons testé trois stratégies pour observer l'efficacité des heuristiques simples :

1. **Stratégie A (Meilleur Score) :** Score total de **269**. Trop gourmande en budget.
2. **Stratégie B (Meilleur Ratio Score/Salaire) :** Score total de **336**. C'est la meilleure approche gloutonne.
3. **Stratégie C (Alternance) :** Score total de **263**.

---

## Partie 3 : Programmation Dynamique

Cette étape utilise la programmation dynamique avec **mémoïsation** pour explorer toutes les combinaisons possibles sans calculs redondants.

* **Résultat :** Score total de **348**.
* **Observation :** Cette méthode trouve la solution **optimale absolue**. Elle surpasse l'approche gloutonne (+12 points) en trouvant une combinaison de joueurs plus efficace que le simple tri par ratio.
