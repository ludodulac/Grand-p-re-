# Biblaw

Source : `ludodulac/Biblaw`.

## Mission
Structurer, indexer et relier un corpus biblique/essénien avec des analyses thématiques traçables et reproductibles.

## Spécialité réutilisable
Canonicalisation, indexation, ambiguïté, audits reproductibles et relations sémantiques typées.

## Invariants durables
- Occurrence ≠ thème.
- Cooccurrence ≠ synonymie ni causalité.
- Similarité lexicale ≠ équivalence.
- Un alias ambigu reste ambigu tant qu'il n'est pas résolu.
- Un composant d'un thème composé ne devient pas automatiquement un thème autonome du psaume.
- Les artefacts générés doivent rester reproductibles/auditables.

## Direction sémantique
Distinguer explicitement SAME/EQUIVALENT, VARIANT, MORE GENERAL/MORE SPECIFIC, COMPONENT et RELATED. Construire des candidats puis les valider, plutôt que fusionner naïvement par similarité de chaînes.

## Risque connu
L'infrastructure de validation peut devenir un refuge confortable. Après stabilisation des guardrails, reprendre le progrès sémantique réel et prouver les relations sur quelques cas concrets avant de généraliser.

## Continuité IA
`AI_START_HERE.md` sert de routeur et encourage FAST/TARGETED/FULL. Les rapports générés fournissent les compteurs actuels ; Grand Père ne doit pas les recopier comme vérités durables.

## À revérifier dans le dépôt
État de la cartographie sémantique, cas `licorne`, métriques de thèmes/aliases, validations et Pages.