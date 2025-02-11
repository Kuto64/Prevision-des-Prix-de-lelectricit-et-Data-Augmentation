# Prévision des Prix de l'Électricité et Data Augmentation

## Contexte
Ce projet, réalisé en collaboration avec Air Liquide, explore l'utilisation de **data augmentation** pour améliorer la précision des modèles de prévision des prix de l'électricité. Enrichir les séries temporelles historiques avec des scénarios synthétiques est une solution proposée pour pallier la limitation des données disponibles.

## Objectifs
- Développer et comparer des modèles de prévision : **XGBoost**, **LSTM**, **Conv1D**, et **Transformers**.
- Tester des techniques de **data augmentation** : Jittering, Scaling, Time Warping, et **GANs**.
- Évaluer l'impact des scénarios générés sur les performances des modèles.

## Méthodologie
1. **Préparation des données** :
   - Normalisation (MinMaxScaler).
   - Création de fenêtres temporelles pour prédire des horizons de 6h à 72h.
2. **Modèles explorés** :
   - Méthodes traditionnelles : XGBoost.
   - Modèles de deep learning : LSTM, Conv1D, Transformers.
3. **Métriques d'évaluation** :
   - MAE, RMSE.

## Résultats
- Les modèles **LSTM** et **Transformers** ont montré les meilleures performances sur les horizons longs (>24h).
- La data augmentation avec des scénarios générés (GANs) a permis d'améliorer les prédictions, contrairement aux méthodes classiques (e.g., Jittering).

## Perspectives
- Optimisation des architectures (e.g., combiner CNN et LSTM).
- Exploration de nouvelles techniques de génération de données synthétiques (e.g., modèles de diffusion).
- Extension à d'autres séries temporelles pour tester la généralisabilité.

## Auteur·e·s
Loucas Terchani, Joëlla Rabemananjara
