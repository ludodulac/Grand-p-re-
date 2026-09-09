# AI START HERE — Grand Père

Grand Père est une mémoire transversale. Ce fichier est un **routeur**, pas une encyclopédie à charger entièrement.

## Chemin court par défaut

1. Vérifier le vrai `main` de Grand Père.
2. Identifier le projet concerné via [`projects/_INDEX.md`](projects/_INDEX.md), puis lire **uniquement sa fiche**.
3. Ouvrir le dépôt source du projet et vérifier son `main`, ses documents canoniques, le code/tests/CI pertinents.
4. Pour un travail itératif ou autonome, appliquer [`LOOP_ENGINEERING.md`](LOOP_ENGINEERING.md) : objectif → état réel → écart borné → première couche responsable → action minimale → preuve → continue/pivot/stop.
5. Si le problème appelle un apprentissage transversal, lire la section pertinente de [`KNOWLEDGE.md`](KNOWLEDGE.md).
6. Si le problème ressemble à un échec déjà rencontré, passer par [`incidents/_INDEX.md`](incidents/_INDEX.md) puis seulement l'incident pertinent.
7. Pour une vue de l'écosystème et des relations entre projets, utiliser [`ECOSYSTEM.md`](ECOSYSTEM.md).

**Ne jamais lire tout Grand Père par défaut.**

## Hiérarchie de vérité

1. **État réel d'un projet** : dépôt projet, code, données, tests, CI/déploiement.
2. **Règles durables du projet** : principes/contrats/ADR/doc canonique du projet.
3. **Grand Père** : carte transversale, contexte, apprentissages, méthodes, liens et passations.
4. **Anciennes conversations** : contexte historique seulement si non contredit par les sources ci-dessus.

## Question obligatoire avant modification

**Est-ce que j'interviens sur la version réellement utilisée et au bon niveau du problème ?**

## À conserver ici

- mission et maturité de chaque projet ;
- spécialité architecturale ou produit ;
- invariants particulièrement importants ;
- décisions utilisateur durables ayant un impact transversal ;
- incidents et enseignements réutilisables ;
- méthodes communes ;
- relations entre projets ;
- état de réflexion produit lorsqu'il est important de ne pas le confondre avec une décision validée.

## À revérifier, pas à mémoriser comme vérité

- dernier commit ou SHA ;
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

Pour une boucle en cours, une passation doit permettre de retrouver au minimum : **objectif / dernière boucle / preuve / prochaine décision**.

## Test de qualité

Une nouvelle conversation sans historique doit pouvoir trouver son chemin avec :

**AI_START_HERE → un index → une fiche/source pertinente → dépôt projet → boucle bornée → preuve.**

Si elle doit lire tout Grand Père pour travailler sur un seul projet, ou si elle ne sait pas pourquoi elle continue à modifier le projet, l'organisation a échoué.
