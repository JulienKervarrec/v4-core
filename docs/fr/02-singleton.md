# 2. Singleton et PoolManager

PoolManager centralise l’état des pools : paramètres de clé, liquidité, positions et comptabilité des tokens. Un pool est identifié par une clé incluant notamment les tokens, la fee, le tick spacing et l’adresse du hook.

Cette centralisation réduit la duplication de déploiements et facilite la composition entre pools. Elle impose en contrepartie de bien séparer l’identité d’un pool et les données propres à une position.

Les interfaces du dépôt exposent les opérations de création, échange, liquidité et règlement. Le contrat d’intégration doit conserver la bonne adresse du manager et respecter ses garde-fous.

Suite : [unlock et deltas](03-unlock-deltas.md).
