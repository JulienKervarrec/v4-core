# 4. Swaps et comptabilité nette

La fonction swap applique les paramètres de la pool key, la direction, la quantité et la limite de prix. Les mouvements de tokens sont suivis par les deltas plutôt que par un transfert isolé à chaque étape.

Un routeur peut donc combiner plusieurs swaps, puis appeler settle pour payer ce qui est dû ou take pour retirer un solde créditeur. Le résultat économique final dépend de l’ensemble de l’unlock.

Les arrondis, fees, ticks et limites de prix restent essentiels. Une intégration doit traiter les retours et les erreurs de dépassement de prix.

Suite : [liquidité et positions](05-liquidite.md).
