# TP2 - Optimisation et Intelligence Artificielle

Ce projet présente trois approches pour résoudre un problème de sélection de joueurs :
1. Programmation Linéaire (avec la bibliothèque PuLP).
2. Algorithmes Gloutons (Greedy).
3. Programmation Dynamique (Récursivité et Mémoïsation).

## Structure du dépôt
* `partie1_pl.py` : Solution optimale via programmation linéaire.
* `partie2_glouton.py` : Implémentation des 3 stratégies gloutonnes.
* `README.md` : Documentation du projet et analyse des résultats.

---

## Partie 2 : Approche Gloutonne (Greedy)

Dans cette étape, nous avons implémenté trois stratégies gloutonnes pour sélectionner les joueurs en fonction d'un budget de 5000 € :

1. **Stratégie A (Meilleur Score) :** Sélectionne les joueurs ayant le score le plus élevé en premier.
   - **Résultat :** Score total de 269. Cette méthode est limitée car elle consomme le budget trop rapidement avec des joueurs très chers.
   
2. **Stratégie B (Meilleur Ratio Score/Salaire) :** Sélectionne les joueurs en fonction de leur efficacité (score par euro dépensé).
   - **Résultat :** Score total de 336. C'est la stratégie la plus performante parmi les approches gloutonnes.
   
3. **Stratégie C (Alternance) :** Alterne entre le meilleur score et le meilleur ratio à chaque sélection.
   - **Résultat :** Score total de 263.

**Conclusion intermédiaire :** L'approche par ratio (Heuristique) permet d'obtenir une équipe beaucoup plus équilibrée et performante que la simple sélection par prestige (score absolu).
