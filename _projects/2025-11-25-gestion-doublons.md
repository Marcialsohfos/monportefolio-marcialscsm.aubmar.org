---
layout: project
title: "Application de gestion des doublons"
date: 2023-03-10
client: "MINSANTE - Service des Laboratoires"
categories: ["Développement", "Qualité des données"]
tags: ["Algorithmes", "Nettoyage de données", "Python", "Base de données"]
image: "/assets/img/projets/doublons.jpg"
excerpt: "Développement d'une application dédiée à l'identification et à la résolution des doublons dans les grandes bases de données de laboratoires."
---

## Contexte

Les grandes bases de données de laboratoires souffraient d'un problème récurrent de doublons, rendant les analyses peu fiables et compliquant le suivi des infrastructures. La détection manuelle était impossible face au volume de données.

## Problématique

- Des milliers d'enregistrements avec des doublons potentiels
- Différentes sources de données avec des formats variés
- Nécessité de préserver l'intégrité des données originales
- Contraintes de temps pour le nettoyage

## Solution développée

J'ai conçu et développé une **application spécialisée** qui :

1. **Identifie les doublons** grâce à des algorithmes de matching fuzzy
2. **Propose des regroupements** intelligents basés sur plusieurs critères
3. **Permet la validation** par un opérateur avant fusion
4. **Conserve un historique** des modifications

## Algorithmes utilisés

- Similarité de Levenshtein pour les chaînes de caractères
- Matching géographique pour les coordonnées proches
- Règles métier spécifiques aux laboratoires
- Apprentissage automatique pour améliorer la précision

## Résultats

- **Fiabilisation** des bases de données
- **Gain de temps** considérable pour les équipes
- **Taux de détection** > 95% des doublons
- **Processus réutilisable** pour d'autres bases

## Compétences mobilisées

`Python` `Algorithmes de matching` `Nettoyage de données` `Base de données` `Interface utilisateur`