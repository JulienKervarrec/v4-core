# 5. Liquidité, positions et donations

modifyLiquidity ajoute ou retire de la liquidité d’une position identifiée par sa clé, son tick inférieur, son tick supérieur et son salt. Les bibliothèques Position et Pool calculent les changements d’état.

donate envoie une contribution aux liquidités existantes sans modifier directement la position du donateur. Les opérations mint et burn gèrent quant à elles des claims de liquidité représentés dans le modèle du manager.

Les hooks peuvent observer ou influencer certains moments du cycle. La cohérence entre liquidité active, ticks et deltas doit être maintenue pendant toute la transaction.

Suite : [hooks et extensibilité](06-hooks.md).
