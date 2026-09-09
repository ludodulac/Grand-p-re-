# Project Genesis

Source : `ludodulac/Project-Genesis`.

## Mission
Laboratoire autonome de game design pour faire émerger un jeu mobile tactile, visuel, rejouable et original à partir de règles simples et de simulation déterministe.

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

## Boucle autonome
`hypothèse → prototype minimal → test → observation → décision → conservation/abandon → expérience suivante`

## Direction
Chercher un verbe de jeu extrêmement fort et quelques systèmes simples qui le multiplient. Favoriser émergence, réactions en chaîne, compromis, anticipation, surprises compréhensibles et envie de rejouer.

## Risque connu
Prendre la vitesse de développement pour du progrès de game design. Une mécanique techniquement réussie mais faible doit pouvoir être abandonnée.

## Continuité IA
Le dépôt possède un `AI_START_HERE.md`, `CURRENT_STATE.md`, `GAMEPLAY.md`, `LAB.md`, `PARKED_IDEAS.md` et des principes explicites. Aucun EXP-XXX n'est automatiquement le jeu.

## À revérifier dans le dépôt
Expérience active, observations téléphone, décisions PROMOTE/ITERATE/PARK/DROP, état du prototype et prochaines hypothèses.