# Automatisation OCR de bon de commande

Ce projet est une démonstration simple d'un workflow d'extraction de données à partir d'une image de bon de commande fictif.

L'objectif est de montrer comment un document non structuré peut être transformé en données exploitables dans un tableau CSV, avec une étape de validation humaine.

## Objectif

Le prototype permet de :

- lire une image de bon de commande ;
- améliorer la qualité de l'image avec OpenCV ;
- extraire le texte avec Tesseract OCR ;
- structurer les données avec Python et Pandas ;
- corriger certaines incohérences simples ;
- exporter le résultat final en CSV.

## Confidentialité

Prototype réalisé sur un document fictif, sans données réelles ni données client.

## Technologies utilisées

- Python
- Tesseract OCR
- OpenCV
- Pandas
- Google Colab

## Fonctionnement du workflow

1. Upload de l'image du bon de commande
2. Prétraitement de l'image :
   - niveaux de gris
   - agrandissement
   - réduction du bruit
   - amélioration du contraste
   - seuillage adaptatif
3. OCR avec Tesseract
4. Extraction des champs utiles avec regex
5. Structuration des résultats dans un tableau Pandas
6. Correction automatique simple des quantités avec la formule :
7. Ajout d'un statut de validation
8. Export du résultat en CSV


```text
quantité corrigée = total ligne / prix unitaire
