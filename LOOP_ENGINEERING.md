# Loop Engineering — méthode transversale

Cette méthode décrit **comment progresser**, pas ce que chaque projet doit construire. Le dépôt projet reste la source de vérité.

## Boucle canonique

`objectif utilisateur → état réel → plus petit écart important → première couche responsable → modification/expérience minimale → preuve → décision : continuer / pivoter / arrêter`

## 1. Observer avant d'agir

Avant une modification :
- reformuler l'objectif fonctionnel sans confondre le besoin avec une ancienne solution technique ;
- vérifier le vrai `main`, le chemin réellement utilisé et les preuves disponibles ;
- distinguer présent dans le code / probablement fonctionnel / vérifié / validé en usage réel.

Question obligatoire : **Est-ce que j'interviens sur la version réellement utilisée et au bon niveau du problème ?**

## 2. Choisir un écart borné

Une boucle traite le plus petit écart important qui rapproche réellement de l'objectif. Éviter les grappes de refactors, documentation, nouvelles fonctions et optimisations sans rapport direct.

Une autonomie longue doit être composée de **petites boucles observables**, jamais d'une commande opaque qui calcule pendant des heures.

## 3. Corriger la première frontière responsable

Suivre le flux du projet jusqu'au premier endroit où la vérité devient fausse, ambiguë ou disparaît. Corriger cette frontière plutôt que maquiller le symptôme dans une couche plus basse.

Ne pas perfectionner une solution si elle répond au mauvais niveau du problème.

## 4. Produire une preuve adaptée

Chaque boucle doit se terminer par une preuve proportionnée :
- test déterministe ou invariant ;
- CI/build ;
- donnée ou artefact reconstruit ;
- rendu comparé à la référence ;
- parcours réel ;
- observation humaine quand la question porte sur compréhension, usage ou plaisir.

Un test technique ne prouve pas automatiquement une validation humaine.

## 5. Décider explicitement

Après la preuve :
- **CONTINUE** : l'écart est réduit et un nouvel écart important est clairement identifié ;
- **PIVOT** : l'hypothèse était fausse ou la couche choisie n'était pas responsable ;
- **STOP** : le critère de sortie est atteint ou poursuivre produirait surtout de la sophistication.

Ne jamais continuer uniquement parce qu'il reste des améliorations possibles.

## 6. Garde-fous

- préserver ce qui fonctionne ; ajouter avant de supprimer quand c'est raisonnable ;
- indisponible ≠ supprimé ≠ remplacé silencieusement ;
- ne jamais affaiblir la vérité mesurée pour faire monter un indicateur ;
- pas de logique spécifique au benchmark dans une correction censée être générale ;
- timeout/progrès visibles pour les validations coûteuses ;
- si une approche échoue, analyser l'échec avant de répéter la même approche ;
- les états éphémères restent dans le projet, les apprentissages durables et transversaux peuvent remonter dans Grand Père.

## Boucles spécialisées connues

Ces exemples sont des patrons, pas des contrats figés.

### Boldüngo
`rendu réel → comparaison photos → 1–3 écarts visibles → première frontière Survey/Scene/build/export/viewer responsable → correction générique minimale → tests → nouveau rendu`

### Biblaw
`relation proposée → cas adversarial → relation concurrente → reformulation sans vocabulaire commun → preuve/argument → valider, reclasser ou marquer frontière`

### Rebulo
`stimulus → réponse humaine → phonologie → clarté lexicale → nommabilité/représentation → correction minimale → nouveau test humain`

### Project Genesis
`observation → prédiction de l'utilisateur → geste → résultat → divergence du modèle mental → plus petite expérience suivante`

### IN-SECT multijoueur
`intention locale → validation serveur → événement autoritaire → application clients → animation → snapshot → comparaison des deux états`

### La Forêt Enchantée
`écran réel → geste attendu enfant → friction observée → couche responsable → simplification minimale → test mobile réel`

## Critère de bonne autonomie

À tout moment, une autre conversation doit pouvoir répondre rapidement à :
1. quel objectif est poursuivi ?
2. quelle boucle vient d'être exécutée ?
3. quelle preuve a été obtenue ?
4. pourquoi continue-t-on, pivote-t-on ou s'arrête-t-on ?

Si ces quatre réponses deviennent floues, arrêter l'expansion et reconstruire l'état réel avant de poursuivre.
