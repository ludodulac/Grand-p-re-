# IN-SECT

Source : `ludodulac/In-sect`.

## Mission
Jeu de stratégie 9×9 à colonies, règles spécifiques et IA, avec ambition multijoueur robuste et expérience produit lisible.

## Spécialité réutilisable
Règles, actions légales, autorité serveur, synchronisation d'état et distinction logique/perspective visuelle.

## Invariants durables
- Le multijoueur ne doit pas affaiblir les règles/IA/solo existants.
- Le serveur doit être autoritaire sur les actions réelles.
- Perspective d'affichage et coordonnées logiques sont des responsabilités distinctes.
- Snapshots pour initialisation/reconnexion/récupération ; événements acceptés pour le flux de jeu lorsque pertinent.

## Modèle professionnel visé
`intention locale → validation serveur → événement accepté → application sur les deux clients → animation → snapshot résultant`

## Risque connu
Les symptômes UX du multijoueur peuvent masquer un problème de frontière d'autorité. Ne pas traiter seulement les clics/rotations si le modèle d'état est mauvais.

## Particularité dépôt
Le dépôt contient historiquement un sous-projet DROP-Service. Ne pas inférer les priorités IN-SECT depuis des commits DROP ni nettoyer sans besoin explicite.

## Validation utile
Distinguer technique, interaction et expérience réelle. Une fonction multijoueur n'est pas considérée robuste uniquement parce qu'elle marche dans un navigateur isolé.

## À revérifier dans le dépôt
État du backend, Edge Function, Realtime/polling, reprise de session, tests réels à deux appareils et direction produit.