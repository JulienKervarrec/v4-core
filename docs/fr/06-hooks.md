# 6. Hooks et extensibilité

À l’initialisation, un pool peut associer un hook qui reçoit des callbacks before ou after pour initialize, addLiquidity, removeLiquidity, swap et donate.

Les permissions de callbacks sont encodées dans l’adresse du hook et ne changent pas pour une pool déjà initialisée. Le hook peut ajouter une logique de fee, de contrôle, d’incitation ou d’oracle selon son propre code.

Cette extensibilité est puissante mais déplace une partie du risque vers l’intégrateur. Il faut analyser les reentrances, les retours, les autorisations et l’impact du hook sur le delta.

Suite : [interfaces et intégration](07-integration.md).
