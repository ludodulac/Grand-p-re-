# Incident — autonomie longue devenue calcul long

## Observé
Sur plusieurs projets complexes, une conversation a semblé travailler pendant des heures alors que GitHub/CI ne montrait pas une progression équivalente.

## Mauvaise conclusion à éviter
« Plus longtemps ça calcule, plus le travail est approfondi. »

## Apprentissage durable
**Autonomie longue ≠ commande longue.**

Un agent autonome doit pouvoir enchaîner beaucoup de boucles courtes et vérifiables :

`inspecter → petite action → test ciblé → résultat observable → commit/trace → boucle suivante`

## Garde-fous
- préférer FAST → TARGETED → FULL lorsque possible ;
- borner les étapes lourdes ;
- afficher/consigner une progression observable ;
- poser des timeouts raisonnables aux opérations externes ;
- ne pas rejouer toute une pipeline quand seule une couche a changé ;
- en cas de durée anormale, diagnostiquer la dernière opération avant de la relancer ;
- une CI verte ou un commit utile vaut mieux qu'une session silencieuse interminable.

## Applicabilité
Boldüngo, Biblaw, Maketik, Genesis et tout futur pipeline autonome.