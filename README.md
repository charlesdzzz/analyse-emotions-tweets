# Analyse des Émotions dans les Tweets

## Description du projet

L'objectif est d'analyser et de classifier des tweets selon cinq émotions principales : **tristesse, joie, amour, colère et peur**.

Le projet couvre l'ensemble du pipeline de traitement de données textuelles : du nettoyage des données à l'évaluation des modèles, en passant par l'apprentissage non supervisé et supervisé.

##️ Outils et Technologies \* **Orange Data Mining** : Création des workflows, prétraitement, clustering et modélisation. \* **NLP (Traitement du Langage Naturel)** : Tokenisation, n-grammes (1-2), filtrage par lexiques.

## Contenu du dépôt

-   `DESTRADE_Charles_GRAVES_Sacha.pdf` : Rapport complet détaillant la méthodologie, les tests et les résultats.
-   `GRAVES_Sacha_data1.csv` : Workflow Orange (format XML) illustrant le pipeline de traitement.
-   `DESTRADE_Charles_data2.csv` : Jeu de données principal (textes et émotions associées).
-   `emotions_donnee_non_etiquetee_apprentisage_supervisee.csv` : Jeu de données de test sans étiquettes pour la prédiction finale.
-   `blockwords.txt` / `destrade_charles_stopwords2.txt` : Lexiques de "stop words" utilisés pour nettoyer le bruit dans les textes.

## Méthodologie

1.  **Prétraitement du texte** : Mise en minuscules, suppression des URLs et caractères spéciaux, filtrage des mots vides via des listes personnalisées, tokénisation et vectorisation (Bag of Words avec TF-IDF).
2.  **Apprentissage Non Supervisé** : Utilisation du clustering hiérarchique avec la distance cosinus pour observer les regroupements naturels des données.
3.  **Apprentissage Supervisé** : Entraînement et comparaison de plusieurs modèles de classification (Régression Logistique, kNN, Random Forest, etc.) pour prédire l'émotion d'un tweet.

## Comment utiliser ce projet

1.  Téléchargez et installez le logiciel [Orange](https://orangedatamining.com/).
2.  Chargez les fichiers `.csv` correspondants au workflow et aux données.
3.  Observez le pipeline et testez les différents modèles de prédiction de texte.
