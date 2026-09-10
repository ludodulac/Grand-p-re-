# Project Genesis

Source : `ludodulac/Project-Genesis`.

## Mission
Laboratoire de game design destiné à **découvrir quel jeu mérite d'être construit**, puis à le faire émerger progressivement comme expérience mobile tactile, visuelle, colorée, immédiatement manipulable, compréhensible, surprenante, rejouable et assez profonde pour devenir un vrai produit.

Genesis n'est pas un jeu déjà défini. Il explore l'espace des possibles avec les moyens disponibles, notamment web/HTML/JS, GitHub, ChatGPT et éventuellement Supabase lorsque le besoin est réel.

Progression visée :

`FONDATION → JOUET → DÉCOUVERTE → JEU → PROFONDEUR → PRODUIT`

## Inspiration et non-spécification
Clash Royale est une référence d'efficacité d'interface, de manipulation tactile et de lisibilité du gameplay, pas une demande de clone ni une spécification de cartes, tours ou combat.

L'exploration externe peut regarder jeux mobiles/web, indépendants, game jams, prototypes, postmortems, forums et retours joueurs afin d'identifier des **sources élémentaires de plaisir** : envie de toucher, anticipation, retry, réaction en chaîne, surprise compréhensible, maîtrise progressive, profondeur à peu de règles, manipulation directe et génération de situations sans gros volume d'assets.

## Spécialité réutilisable
Séparation expérience/gameplay retenu, simulation/rendu, reproductibilité, apprentissage par expérimentation et promotion explicite des mécaniques.

## Invariants durables
- Le monde canonique est une donnée sérialisable.
- La simulation décide ; la présentation montre.
- Le joueur émet des intentions ; seule la simulation mute l'état canonique.
- Même état + même action doit produire le même résultat autant que possible.
- Animation ≠ règle.
- Expériences jetables ; fondations non jetables.
- Implemented ≠ verified ≠ fun.
- Une règle déterministe peut rester incompréhensible pour un humain.
- Aucun EXP-XXX, même réussi, ne devient automatiquement « le jeu Genesis ».

## Cycle humain recherché

`J'OBSERVE → JE PRÉDIS → J'AGIS → JE CONSTATE → JE COMPRENDS UN PEU MIEUX`

Une mécanique fondamentale doit être testée non seulement par reproduction mais par **prédiction sur des situations nouvelles**. Les formulations spontanées imparfaites de l'utilisateur sont des données utiles sur son modèle mental.

## Boucle de laboratoire

`explorer largement → sélectionner un pari → prototype minimal → test humain → apprendre → KEEP/PROMOTE-PARTIAL/PARK/DROP → rouvrir l'espace → éventuellement combiner les meilleures primitives`

Préférer beaucoup de petits paris réversibles à la construction progressive d'un jeu moyen simplement parce que la première mécanique fonctionnait.

Une primitive validée doit être conservée comme ressource disponible sans enfermer le projet dans cette famille. Après une séquence d'approfondissement, demander explicitement si l'incertitude la plus importante est encore dans cette piste ou s'il faut rouvrir l'exploration.

## Direction
Chercher des verbes et langages de jeu extrêmement forts et quelques systèmes simples qui les multiplient. Favoriser émergence, réactions en chaîne, compromis, anticipation, surprises compréhensibles et envie de rejouer.

Le relief, le déplacement d'un acteur ou toute autre primitive expérimentale actuelle peuvent devenir un morceau du futur jeu, une mécanique parmi d'autres ou seulement un apprentissage de design. Ne jamais confondre une piste prometteuse avec la destination finale.

## Risque connu
Prendre la vitesse de développement pour du progrès de game design, ou laisser l'approfondissement rigoureux d'une famille réduire silencieusement l'espace de recherche. Une mécanique techniquement réussie mais faible doit pouvoir être abandonnée ; une mécanique comprise et intéressante doit pouvoir être conservée sans devenir automatiquement le jeu entier.

## Continuité IA
Le dépôt possède un `AI_START_HERE.md`, `CURRENT_STATE.md`, `GAMEPLAY.md`, `LAB.md`, `PARKED_IDEAS.md` et des principes explicites. L'historique durable doit permettre de retrouver ce qui a été testé, appris, abandonné, promu et la prochaine hypothèse.

## À revérifier dans le dépôt
Expérience active, observations téléphone, prédictions humaines, décisions PROMOTE/ITERATE/PARK/DROP, primitives retenues, état du prototype, dernières recherches externes et prochaine décision explorer/approfondir.