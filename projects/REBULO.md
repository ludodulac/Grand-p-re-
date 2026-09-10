# Rebulo

Source : `ludodulac/Rebulo`.

## Mission
Créer des rébus phonétiques riches, ludiques et intelligents, avec un cœur phonétique strict mais capable d'explorer plusieurs conventions explicites, et avec des usages possibles en orthophonie lorsque le niveau de preuve le permet.

Chaîne produit visée :

`mot/phrase → chaîne phonétique continue → segmentations concurrentes → SON → MOT(S) POSSIBLE(S) → IMAGE / LETTRE / CHIFFRE / AUTRE REPRÉSENTATION → qualité phonétique → évidence humaine → composition du rébus`

## Objectif actuel important
Cartographier largement les sons correspondant surtout à environ une ou deux syllabes et déterminer lesquels peuvent être représentés clairement. Constituer progressivement une grande banque de représentations simples, lisibles et immédiatement nommables.

La priorité actuelle n'est pas de fabriquer de magnifiques planches finales mais d'améliorer conjointement :

`couverture des sons + qualité phonétique + évidence des mots + nommabilité des images + capacité à composer de bons rébus`

Une représentation de deux syllabes très évidente peut être préférable à deux représentations d'une syllabe plus ambiguës.

## Spécialité réutilisable
Séparer clairement les niveaux de garantie : validité phonétique, approximation ludique, évidence lexicale, plausibilité visuelle, dénomination spontanée, âge, validation clinique.

## Invariants durables
- Une image stricte représente un mot entier et sa prononciation entière.
- La concaténation stricte doit correspondre exactement à la cible.
- Une absence de solution exacte est un résultat normal.
- Une phrase peut être explorée comme chaîne phonétique continue ; les frontières lexicales écrites ne doivent pas limiter les segmentations possibles.
- Toute convention non stricte future doit être explicite et testable.
- Une approximation ludique ne doit jamais être présentée comme exacte.
- Ce qui est acceptable dans un rébus ludique n'est pas automatiquement acceptable en orthophonie.
- Généraliste, pédagogique et clinique sont des niveaux distincts.

## Direction corpus
Préférer une logique pilotée par vocabulaire cible utile : âge, fréquence, commonness, prononciations, décompositions, chunks manquants, candidats lexicaux, dessinabilité, plausibilité visuelle, risque de dénomination, scoring, bibliothèque d'illustrations.

Les prototypes visuels servent aussi à apprendre quelles propriétés prédisent une représentation humainement bonne ; ne pas confondre un homophone lexical exact avec un asset immédiatement utilisable.

## Risque connu
Ne pas laisser un gros lexique global dicter les priorités produit. La couverture utile des sons réellement pertinents vaut plus qu'une couverture brute gonflée par des briques marginales.

Inversement, ne pas pousser trop tôt tout le chantier vers seulement quelques rébus complets : la construction de la banque et la cartographie 1–2 syllabes sont elles-mêmes des objectifs actuels explicites. Tester périodiquement des phrases réelles permet de vérifier que la couverture théorique devient effectivement exploitable.

## Continuité IA
Le dépôt possède désormais un `AI_START_HERE.md`. Lire le routeur local, les principes produit et seulement la documentation pertinente à la zone, puis vérifier l'état réel du corpus, des illustrations et du moteur.

## À revérifier dans le dépôt
État du corpus, métriques de couverture utile, pipelines réellement actifs, banque SON/MOT/IMAGE/SYMBOLE, tests, expérience Jouer, statut de preuve des illustrations et résultats de composition sur phrases réelles.