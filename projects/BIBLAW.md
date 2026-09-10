# Biblaw

Source : `ludodulac/Biblaw`.

## Mission
Transformer un corpus biblique/essénien en compréhension thématique traçable : permettre de demander « qu'est-ce que cette Bible dit de ce concept ? », d'en comprendre les grandes facettes, de lire les textes essentiels puis l'ensemble des textes pertinents, et de vérifier chaque synthèse sur les sources.

Chaîne produit visée :

`CORPUS → analyses fondées → concepts → relations validées → synthèse traçable → présentation`

Expérience cible :

`COMPRENDRE UN CONCEPT → APPROFONDIR SES FACETTES → LIRE LES TEXTES ESSENTIELS → EXPLORER TOUS LES TEXTES → VÉRIFIER LES SOURCES`

## Résultat attendu pour une recherche thématique
Pour une requête comme « Assemblée », Biblaw doit progressivement pouvoir fournir :

1. une synthèse globale de ce que le corpus dit principalement du thème ;
2. les grandes facettes sous lesquelles le concept apparaît ;
3. les psaumes/textes essentiels pour le comprendre ;
4. tous les textes pertinents avec une explication orientée vers ce thème ;
5. la possibilité de remonter aux passages qui justifient les affirmations de Biblaw.

Biblaw ne doit jamais devenir une IA qui invente une doctrine religieuse plausible au-delà du corpus.

## Spécialité réutilisable
Canonicalisation, indexation, ambiguïté, audits reproductibles, synthèse avec provenance et relations sémantiques typées.

## Invariants durables
- Occurrence ≠ thème.
- Cooccurrence ≠ synonymie ni relation doctrinale.
- Similarité lexicale ≠ équivalence.
- Un alias ambigu reste ambigu tant qu'il n'est pas résolu.
- Un mot présent dans le nom d'un concept n'est pas automatiquement une composante de ce concept.
- Un composant d'un thème composé ne devient pas automatiquement un thème autonome du psaume.
- Toute affirmation de synthèse importante doit rester reliée aux textes qui la fondent.
- Les artefacts générés doivent rester reproductibles/auditables.

## Direction sémantique
Distinguer explicitement SAME/EQUIVALENT, VARIANT, MORE GENERAL/MORE SPECIFIC, COMPONENT et RELATED. Construire des candidats puis les valider, plutôt que fusionner naïvement par similarité de chaînes.

Le graphe sémantique est un moyen d'aider à comprendre les concepts, pas une fin quantitative. Un graphe plus pauvre mais juste vaut mieux qu'un réseau riche de relations fabriquées.

## Objectif de couverture
Un chantier important est de vérifier si tous les thèmes utiles du corpus ont réellement été cartographiés et si tous les psaumes/textes ont été analysés avec une profondeur suffisante pour soutenir les synthèses futures. Ne pas confondre nombre de thèmes détectés et couverture sémantique réelle.

## Risque connu
L'infrastructure de validation peut devenir un refuge confortable. Après stabilisation des guardrails, reprendre le progrès sémantique réel et prouver les relations/synthèses sur des cas concrets avant de généraliser.

Une interface de recherche qui retourne des résultats pertinents ne prouve pas encore que Biblaw sait expliquer fidèlement ce que le corpus dit d'un concept.

## Continuité IA
`AI_START_HERE.md` sert de routeur. Les rapports générés fournissent les compteurs actuels ; Grand Père ne doit pas les recopier comme vérités durables.

## À revérifier dans le dépôt
État de la cartographie sémantique, couverture réelle des psaumes/textes, relations validées, capacité de synthèse thématique avec provenance, métriques actuelles, validations éditoriales et Pages.