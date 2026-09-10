# Célébrations des Archanges

Source : `ludodulac/Celebrations`.

## Mission
Interface publique et administration de célébrations, contenus, groupes, participants et programmes, avec personnalisation par profils visiteurs.

## Spécialité réutilisable
Séparer contenu canonique, assignation à une audience, visibilité et expérience rendue.

## Modèle conceptuel
`Content ≠ ContentAssignment ≠ ContentVisibility ≠ RenderedExperience`

## Invariants durables
- Supabase est source canonique des données métier.
- Les préférences locales ne doivent pas devenir une seconde vérité métier.
- Les profils/groupes déterminent ce qui est présenté sans dupliquer inutilement le contenu.
- L'ordre des scripts natifs fait partie de l'architecture actuelle.
- Préserver public/admin et les comportements existants lors des extensions.

## Continuité IA
Lors de l'audit du 2026-09-09, pas de `AI_START_HERE.md` à la racine. Le README est clair mais un routeur court par zone éviterait de relire trop largement le dépôt.

## À revérifier dans le dépôt
Modèle de données actuel, authentification admin, règles d'assignation, Pages, scripts réellement chargés et personnalisation vérifiée.