# Grand Père — mémoire transversale des projets

Grand Père est le dépôt de **mémoire et de passation inter-projets** de l'écosystème `ludodulac` et des projets associés.

Il ne remplace jamais les dépôts projets. Son rôle est de conserver ce qui risquerait autrement de rester uniquement dans une conversation : compréhension globale, liens entre projets, méthodes éprouvées, décisions transversales, enseignements, incidents et règles de passation.

## Règle fondamentale

**Le dépôt projet reste la source de vérité de son propre état. Grand Père conserve la connaissance transversale et les pointeurs permettant de la retrouver.**

Une information changeante (SHA, CI, nombre de tests, état d'une PR, fonctionnalité en cours) doit être revérifiée dans le dépôt concerné avant d'être utilisée.

## Démarrage IA

Toute nouvelle conversation qui travaille sur Grand Père commence par `AI_START_HERE.md`.

## Carte

- `AI_START_HERE.md` — routeur de reprise.
- `ECOSYSTEM.md` — carte des projets, maturité et spécialités.
- `KNOWLEDGE.md` — principes et enseignements transversaux.
- `projects/` — une fiche compacte par projet.
- `incidents/` — enseignements réutilisables issus d'incidents importants.

## Ce qui ne doit pas être stocké ici

- secrets, clés API, mots de passe, tokens ;
- copie complète du code des autres dépôts ;
- états techniques éphémères présentés comme vérités durables ;
- duplications massives de documentation déjà canonique ailleurs ;
- souvenirs de conversation sans valeur durable.

Grand Père doit rester une **carte de connaissance**, pas devenir une seconde copie de tous les projets.
