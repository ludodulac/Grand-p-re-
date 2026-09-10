# La Forêt Enchantée

Source : `ludodulac/La-foret-enchantee`.

## Mission
Médiathèque personnelle audio jeunesse avec lecture publique, fiches audio, blog et administration.

## Spécialité réutilisable
Gestion robuste des médias, sécurité légère mais réelle, mutations sûres et distinction navigation/écoute.

## Invariants durables
- Lecture publique, écritures réservées aux admins via RLS.
- Remplacement média sûr : upload nouveau → mise à jour SQL → suppression ancien.
- Si l'écriture SQL échoue, nettoyer le nouveau fichier plutôt que casser la référence existante.
- Le blog filtre le HTML riche et protège les surfaces publiques/admin.
- Le projet reste volontairement léger, sans framework ni build obligatoire.

## Direction expérience jeunesse
Séparer la sélection/browsing de l'écoute. L'écoute doit devenir plus calme et se faire oublier. Les inspirations externes peuvent guider ergonomie, âge, navigation et explication sans copier une identité.

## Continuité IA
Lors de l'audit du 2026-09-09, pas de `AI_START_HERE.md` à la racine. Le README documente bien architecture, sécurité et surfaces ; un routeur court vers les zones concernées serait utile.

## À revérifier dans le dépôt
État Supabase, migrations, stockage, CI, parcours mobile/PWA, médiathèque et blog réellement déployés.