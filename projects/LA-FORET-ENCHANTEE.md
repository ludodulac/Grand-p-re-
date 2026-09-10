# La Forêt Enchantée

Source : `ludodulac/La-foret-enchantee`.

## Mission
Bibliothèque personnelle d'histoires et de contenus audio, avec une expérience extrêmement simple, chaleureuse et adaptée notamment aux enfants.

Parcours idéal :

`OUVRIR → VOIR CE QU'ON PEUT ÉCOUTER → CHOISIR → LANCER → L'INTERFACE S'EFFACE → ÉCOUTER → REVENIR OU REPRENDRE`

Les histoires et les contenus doivent dominer l'expérience ; l'interface doit se faire oublier dès que l'écoute commence.

## Direction visuelle et produit
Préférer une ambiance chaleureuse, claire, vivante et liée à l'imaginaire de la forêt. Éviter une esthétique sombre, luxueuse ou trop adulte.

Ne pas transformer l'application en interface compliquée, en assistant vocal omniprésent, en onboarding lourd ou en système de profils qui détourne l'attention du contenu.

La simplicité enfant ne signifie pas supprimer les capacités d'administration utiles à l'adulte : séparer clairement l'expérience publique/écoute et les outils d'administration.

## Spécialité réutilisable
Gestion robuste des médias, sécurité légère mais réelle, mutations sûres et distinction navigation/écoute.

## Invariants durables
- Lecture publique, écritures réservées aux admins via RLS.
- Remplacement média sûr : upload nouveau → mise à jour SQL → suppression ancien.
- Si l'écriture SQL échoue, nettoyer le nouveau fichier plutôt que casser la référence existante.
- Le blog filtre le HTML riche et protège les surfaces publiques/admin.
- Le projet reste volontairement léger, sans framework ni build obligatoire sauf besoin réel.
- L'écoute doit devenir plus calme et se faire oublier.
- Si l'enfant ne comprend pas l'écran, simplifier l'écran avant d'ajouter une couche d'explication.

## Direction expérience jeunesse
Séparer la sélection/browsing de l'écoute. Les inspirations externes peuvent guider ergonomie, âge, navigation et explication sans copier une identité.

Le critère principal n'est pas le nombre de fonctionnalités visibles mais la facilité avec laquelle un enfant peut reconnaître un contenu, le lancer et écouter sans friction.

## Continuité IA
Le dépôt possède désormais un `AI_START_HERE.md`. Lire le routeur local puis seulement la zone concernée. La Forêt reste l'autorité sur code, Supabase, médias, sécurité et production.

## À revérifier dans le dépôt
État Supabase, migrations, stockage, CI/Pages, parcours mobile/PWA, médiathèque et blog réellement déployés, lisibilité enfant, reprise de lecture et stabilité du parcours d'écoute.