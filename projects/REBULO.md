# Rebulo

Source : `ludodulac/Rebulo`.

## Mission
Créer des rébus riches, ludiques et intelligents avec un cœur phonétique strict, utilisables comme jeu et, avec niveaux de preuve adaptés, dans des contextes pédagogiques/orthophoniques.

## Spécialité réutilisable
Séparer clairement les niveaux de garantie : validité phonétique, plausibilité visuelle, dénomination spontanée, âge, validation clinique.

## Invariants durables
- Une image stricte représente un mot entier et sa prononciation entière.
- La concaténation stricte doit correspondre exactement à la cible.
- Une absence de solution exacte est un résultat normal.
- Toute convention non stricte future doit être explicite et testable.
- Généraliste, pédagogique et clinique sont des niveaux distincts.

## Direction corpus
Préférer une logique pilotée par vocabulaire cible utile : âge, fréquence, commonness, prononciations, décompositions, chunks manquants, candidats lexicaux, plausibilité visuelle, scoring, bibliothèque d'illustrations.

## Risque connu
Ne pas laisser un gros lexique global dicter les priorités produit. La couverture utile des mots réellement pertinents vaut plus qu'une couverture brute gonflée par des briques marginales.

## Continuité IA
Le dépôt n'avait pas encore de `AI_START_HERE.md` lors de l'audit du 2026-09-09. Le README et `docs/PRODUCT_PRINCIPLES.md` contiennent déjà une bonne partie de la constitution. Une amélioration recommandée est d'ajouter un routeur court sans recopier ces documents.

## À revérifier dans le dépôt
État du corpus, métriques de couverture, pipelines réellement actifs, tests, expérience Jouer et statut des illustrations.