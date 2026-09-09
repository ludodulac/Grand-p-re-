# AI START HERE — Grand Père

Grand Père est une mémoire transversale. Ce fichier est un **routeur**, pas une encyclopédie à charger entièrement.

## Avant d'agir

1. Vérifier le vrai `main` de Grand Père.
2. Identifier le ou les projets concernés.
3. Lire uniquement leurs fiches dans `projects/` et la section pertinente de `KNOWLEDGE.md`.
4. Pour toute affirmation sur l'état actuel d'un projet, ouvrir son dépôt source et vérifier `main`, ses documents canoniques, le code/tests/CI pertinents.
5. Ne jamais laisser Grand Père écraser une vérité plus fraîche du dépôt projet.
6. Après une découverte durable, mettre à jour la fiche ou la connaissance transversale concernée sans recopier inutilement la documentation source.

## Hiérarchie de vérité

1. **État réel d'un projet** : dépôt projet, code, données, tests, CI/déploiement.
2. **Règles durables du projet** : principes/contrats/ADR/doc canonique du projet.
3. **Grand Père** : carte transversale, contexte, apprentissages, liens et passations.
4. **Anciennes conversations** : contexte historique seulement si non contredit par les sources ci-dessus.

## Types d'information

### À conserver ici
- mission et maturité de chaque projet ;
- spécialité architecturale ou produit ;
- invariants particulièrement importants ;
- décisions utilisateur durables ayant un impact transversal ;
- incidents et enseignements réutilisables ;
- méthodes communes ;
- relations entre projets ;
- état de réflexion produit lorsqu'il est important de ne pas le confondre avec une décision validée.

### À revérifier, pas à mémoriser comme vérité
- dernier commit ;
- SHA ;
- PR ouverte ;
- CI du jour ;
- compteurs de tests/données ;
- URL temporaire ;
- détail d'implémentation susceptible de changer.

## Protocole de passation

Quand une conversation importante se termine :

1. distinguer **fait durable / décision / hypothèse / état éphémère / apprentissage** ;
2. écrire le durable dans le dépôt projet si cela lui appartient exclusivement ;
3. écrire dans Grand Père uniquement ce qui aide une future conversation à comprendre le projet ou plusieurs projets ;
4. pointer vers la source canonique au lieu de la recopier ;
5. signaler explicitement ce qui reste incertain ;
6. ne jamais archiver un secret.

## Test de qualité

Une nouvelle conversation sans historique doit pouvoir :
- comprendre quels projets existent ;
- savoir ce qui les distingue ;
- retrouver leurs sources de vérité ;
- connaître les grands enseignements déjà acquis ;
- éviter de répéter les erreurs importantes ;
- puis aller vérifier l'état réel du projet avant d'agir.

Si elle doit lire tout Grand Père pour travailler sur un seul projet, l'organisation a échoué.
