# Boldüngo / BrickHouse

Source : `ludodulac/lego-app`.

## Mission
Transformer des photographies d'une maison réelle en une construction LEGO fidèle et réalisable, en passant par une compréhension architecturale structurée puis une adaptation explicite aux contraintes LEGO.

Chaîne produit visée :

`photos → compréhension architecturale → reconstruction structurée → adaptation LEGO → modèle LEGO → visualisation → nomenclature/pièces → instructions réellement constructibles`

Le but n'est pas une jolie image ressemblante mais un modèle reconnaissable, cohérent et constructible.

## Ce que la compréhension doit préserver
Autant que les photos le permettent : proportions, volumes, façades, ouvertures, toitures, terrasses, escaliers, cheminées, terrain pertinent et matériaux/couleurs observables.

Une information inconnue ne doit jamais devenir artificiellement une mesure précise. Distinguer en permanence ce qui est observé, déduit, supposé ou inconnu.

## Spécialité réutilisable
Autorité des couches, provenance, inconnues explicites, validation déterministe, distinction entre vérité architecturale et adaptation LEGO.

## Invariants durables
- Survey = vérité observée/sémantique avec incertitude.
- Scene = vérité métrique/géométrique.
- L'adaptation LEGO ne doit jamais falsifier silencieusement l'architecture.
- Une approximation est une perte de fidélité explicite, pas un faux fait.
- Un inconnu reste inconnu.
- Tests et moteurs déterministes autant que possible.
- Le benchmark réel sert à améliorer des règles génériques ; ne jamais coder une exception propre à cette maison comme comportement général.

## Boucle humaine recherchée

`logiciel → résultat réel → export → contrôle visuel → corrections structurées → réinjection → nouveau résultat`

La correction humaine doit enrichir ou rectifier la représentation structurée plutôt que devenir un bricolage graphique aval.

## Supervision produit
Le progrès technique du pipeline ne suffit pas : le benchmark réel doit converger visuellement vers la maison observée sans tricher sur la vérité amont.

L'interface qui permet de fournir les photos, préparer les handoffs nécessaires, importer les résultats et atteindre la reconstruction fait partie du produit. Si ce parcours est lent, instable ou incompréhensible, il devient la première couche responsable et doit être stabilisé avant de demander à l'utilisateur de juger la reconstruction.

Les fichiers intermédiaires PDF/JSON/TXT peuvent rester nécessaires tant que l'analyse dépend d'un handoff IA externe, mais l'utilisateur ne doit pas avoir à comprendre l'architecture interne du pipeline pour les manipuler.

Le benchmark multi-vues courant et ses fixtures doivent être revérifiés dans le dépôt source plutôt que mémorisés ici comme état fixe.

## Continuité IA
Le dépôt possède un `AI_START_HERE.md` très abouti et un `PROGRESSION.md` opérationnel. Lire uniquement la zone pertinente, puis code/tests correspondants. Préférer FAST → TARGETED → FULL.

## À revérifier dans le dépôt
HEAD, CI/déploiement, benchmark réel et ses photos versionnées, parcours photo réellement chargé, stabilité mobile, génération/import des handoffs, qualité de la reconstruction, capacités d'export et preuves mécaniques.