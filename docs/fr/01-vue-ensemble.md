# 1. Vue d’ensemble d’Uniswap v4

Uniswap v4 est un AMM extensible. Le dépôt v4-core concentre le PoolManager, les bibliothèques de pool, les interfaces et le mécanisme d’intégration des hooks.

L’architecture remplace une collection de pools autonomes par un singleton qui gère l’état de tous les pools. Les intégrateurs composent ensuite les actions dans une phase unlock.

Ce parcours suit PoolManager, les deltas, swap, modifyLiquidity, donate, settle, take, mint, burn et les callbacks de hooks. Il repose sur une lecture statique, sans installation ni exécution.

Suite : [singleton et PoolManager](02-singleton.md).
