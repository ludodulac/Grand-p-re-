# Boldüngo / BrickHouse

Source : `ludodulac/lego-app`.

## Mission
Transformer des preuves architecturales, notamment des photos multi-vues, en représentation structurée puis en approximation LEGO fidèle, traçable, déterministe et exportable.

## Spécialité réutilisable
Autorité des couches, provenance, inconnues explicites, validation déterministe, distinction entre vérité architecturale et adaptation LEGO.

## Invariants durables
- Survey = vérité observée/sémantique avec incertitude.
- Scene = vérité métrique/géométrique.
- L'adaptation LEGO ne doit jamais falsifier silencieusement l'architecture.
- Une approximation est une perte de fidélité explicite, pas un faux fait.
- Un inconnu reste inconnu.
- Tests et moteurs déterministes autant que possible.

## Continuité IA
Le dépôt possède un `AI_START_HERE.md` très abouti et un `PROGRESSION.md` opérationnel. Lire uniquement la zone pertinente, puis code/tests correspondants. Préférer FAST → TARGETED → FULL.

## Apprentissage important
Le progrès technique du pipeline ne suffit pas : le benchmark réel doit converger visuellement vers la maison observée sans tricher sur la vérité amont.

## À revérifier dans le dépôt
HEAD, CI, benchmark réel, métriques, prochaines priorités, capacités d'export et preuves mécaniques.