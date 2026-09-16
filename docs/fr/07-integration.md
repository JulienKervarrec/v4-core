# 7. Interfaces et intégration

Le dépôt fournit IPoolManager, IUnlockCallback, les callbacks de hooks, les bibliothèques de clés, de positions et de calculs de pool. Un contrat d’intégration appelle unlock puis encode ses actions dans unlockCallback.

Les tests et helpers sont séparés du cœur dans src/test et test. Les interfaces servent de contrat d’intégration, mais l’adresse du manager, les licences par fichier et les versions doivent être contrôlées.

Le whitepaper et les tests amont complètent la compréhension. Cette documentation ne lance pas forge et ne revendique aucun résultat d’exécution.

Suite : [limites et périmètre](08-limites.md).
