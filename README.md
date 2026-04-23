# Prédiction de la Pollution Atmosphérique — Paris

> Projet R | L3 CMI Data Science, Université Paris Nanterre

Modélisation des niveaux de particules fines **PM2.5** et **PM10** à Paris à partir des données horaires OpenAQ.

## Objectifs

- Collecter et nettoyer des données de pollution en temps réel (API OpenAQ)
- Analyser la corrélation entre PM2.5 et PM10
- Construire un modèle de régression linéaire pour prédire le PM2.5
- Cartographier les résultats

## Structure

```
prediction-pollution/
├── analysis/
│   └── graph.rmd            # Analyse complète (R Markdown)
├── data/
│   ├── raw/                 # Données brutes OpenAQ
│   └── clean/               # Données nettoyées
├── outputs/
│   ├── regression_PM25.png  # Graphique régression
│   ├── carte.pdf            # Carte géographique
│   └── presentation.pdf     # Présentation des résultats
└── README.md
```

## Méthodologie

1. **Collecte** — API OpenAQ (mesures horaires PM2.5 & PM10)
2. **Nettoyage** — gestion des NA, pivot wide, agrégation horaire
3. **Exploration** — corrélation, statistiques descriptives
4. **Modélisation** — régression linéaire PM2.5 ~ PM10 + variables météo
5. **Visualisation** — graphiques ggplot2 + carte géographique

## Stack technique

| Outil | Usage |
|-------|-------|
| R / R Markdown | Langage & rapport |
| tidyverse | Manipulation des données |
| lubridate | Gestion des dates |
| httr + jsonlite | Appels API OpenAQ |
| corrplot | Matrices de corrélation |
| stargazer | Tableaux de régression |
| gridExtra | Mise en page des graphiques |

## Résultats

Voir [`outputs/regression_PM25.png`](outputs/regression_PM25.png) pour les résultats du modèle et [`outputs/presentation.pdf`](outputs/presentation.pdf) pour la présentation complète.

## Auteur

**Marwane El Bachir** — [LinkedIn](https://www.linkedin.com/in/marwane-el-bachir-400b8a389/)  
L3 CMI Data Science — Université Paris Nanterre
