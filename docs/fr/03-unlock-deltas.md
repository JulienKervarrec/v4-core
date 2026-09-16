# 3. Unlock, callbacks et deltas

Un appelant commence par unlock, puis implémente unlockCallback. Pendant cette phase, il peut enchaîner plusieurs actions sur les pools avant de régler le solde net.

Le delta représente ce que l’utilisateur doit au pool ou ce que le pool lui doit. La phase ne peut se terminer que lorsque les deltas accumulés sont équilibrés selon les règles de PoolManager.

Ce modèle permet des routeurs, agrégateurs et stratégies complexes sans imposer un seul parcours d’échange. Le callback doit refuser les appelants inattendus et borner les données reçues.

Suite : [swaps et comptabilité](04-swaps.md).
