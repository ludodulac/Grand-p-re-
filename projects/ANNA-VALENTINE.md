# Anna Valentine

Source : `annavalentineorg/annavalentine`.

## Mission
Site artistique vivant avec espaces publics et administration réelle de contenus, albums, lieux, repérage et réglages.

## Spécialité réutilisable
Référence de maturité production : administration, données réelles, non-régression, évolution sûre, infrastructure considérée comme contrat tant qu'aucune migration n'est décidée.

## Invariants durables
- Ajouter/étendre avant de supprimer.
- Sélection, déplacement, réorganisation, masquage, renommage et suppression sont des responsabilités distinctes.
- Les indications humaines de Repérage sont source de vérité ; ne pas inventer des adresses précises.
- Préserver projets multi-lieux et notes historiques.
- Une erreur de représentation ne se corrige pas par un simple patch de présentation.

## Méthode Columbo
Ne pas conclure à partir d'un seul indice de code. Distinguer : présent dans le code / probablement fonctionnel / vérifié fonctionnellement / validé en usage réel. Les tests réels admin/public peuvent invalider une lecture statique.

## Continuité IA
`AI_START_HERE.md`, `PROJECT_HANDOFF.md` et `CAHIER-DES-CHARGES.md` organisent bien la reprise. Le README historique n'est pas nécessairement canonique.

## À revérifier dans le dépôt
Infrastructure active, données Supabase/R2, déploiement, issues/PR, fonctions admin réellement vérifiées et éléments encore « à tester ».