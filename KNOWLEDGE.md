# Connaissance transversale

## 1. Grammaire commune

De nombreux projets convergent vers la même architecture conceptuelle :

`Evidence / Source → Canonical Model → Derived / Relations → Audience / Context → Capabilities / Permissions → Valid Actions → Ranking / Next Action → Safe Mutation → Runtime / Presentation → Outcome → Verification in real use → Measurement / Learning`

Propriétés transversales :

`provenance · confidence · ambiguity · version · visibility · validation status · limitations · reversibility`

Cette grammaire est une méthode de raisonnement, pas un framework à imposer à tous les dépôts.

## 2. Canonique et dérivé

Toujours distinguer la vérité canonique de ses représentations pratiques.

- Une couche aval ne doit pas réécrire silencieusement une vérité amont pour rendre son travail plus facile.
- Une approximation doit rester identifiable comme approximation.
- Un inconnu ne doit pas devenir une certitude pour faire passer un pipeline.
- Les artefacts générés doivent pouvoir être reconstruits depuis leurs sources lorsque le projet l'exige.

## 3. Validité, qualité et vérification réelle

Ne pas confondre :

`présent dans le code → probablement fonctionnel → testé techniquement → vérifié fonctionnellement → validé en usage réel`

Une CI verte ne prouve pas qu'une expérience est bonne, qu'une UX est comprise ou qu'un produit répond à son marché.

## 4. Préservation et mutation sûre

Principe général : **ajouter/étendre avant de supprimer ou réécrire**, sauf lorsque le retrait est réellement l'objectif.

Avant une mutation destructive, préférer lorsque possible :

`créer le nouvel état valide → basculer la référence → vérifier → supprimer/nettoyer l'ancien`

Une restauration ou migration ne doit pas automatiquement rendre public/actif un élément lorsque cela pourrait provoquer une publication accidentelle.

## 5. Ne jamais réparer le mauvais niveau

Un problème de représentation ou de modèle ne doit pas être masqué par du CSS ou une présentation trompeuse. Une erreur sémantique ne se corrige pas dans la barre de recherche. Une faiblesse d'autorité multijoueur ne se corrige pas uniquement en bloquant un bouton.

Chercher la couche qui possède réellement la vérité concernée.

## 6. IA comme enrichissement

Lorsque l'IA enrichit une donnée canonique :

- l'enrichissement doit rester dérivé et identifiable ;
- son échec ne doit pas bloquer le cœur du produit sauf si l'IA est réellement le cœur contractuel ;
- les sorties validées humainement doivent être préservées lors des régénérations ;
- ne jamais prétendre qu'une capacité externe est opérationnelle sans l'avoir vérifiée.

## 7. Autonomie longue ≠ commande longue

Un agent autonome peut travailler longtemps, mais doit préférer de nombreuses boucles courtes :

`inspecter → modifier → test ciblé → mesurer → commit → continuer`

Une commande potentiellement lourde doit avoir un but explicite, progression observable, timeout raisonnable et possibilité de reprise. Préférer `FAST → TARGETED → FULL` lorsque le projet s'y prête.

Cette règle vient notamment des blocages observés sur Biblaw et Boldüngo : une conversation qui tourne des heures n'est pas une preuve de travail utile.

## 8. Mémoire documentaire efficace

Un bon dépôt IA ne possède pas nécessairement beaucoup de Markdown.

Préférer :

`AI_START_HERE → état courant → zone concernée → source canonique / code / tests`

Le routeur doit indiquer **quoi ne pas lire** autant que quoi lire. Éviter les documents qui se recopient et les passations concurrentes.

Le dépôt réel reste supérieur à un handoff périmé pour les faits changeants.

## 9. Maturité

Évaluer séparément :

- **maturité produit** : idée → prototype → utilisable → production → produit vivant mature ;
- **maturité ingénierie** : ad hoc → structuré → contrats/tests/audits → fortement gouverné ;
- **validation réelle** : hypothèse → test interne → pilote → usage répété.

Une architecture sophistiquée ne rend pas automatiquement un produit mature.

## 10. Principes spécifiques réutilisables

### Anna Valentine — méthode Columbo
Ne pas conclure depuis un seul indice de code. Vérifier frontend, backend, styles/interactions bloquantes, fonctions voisines, limites implicites et usage réel. Le test réel de l'administration peut invalider une conclusion statique.

### Biblaw — rigueur sémantique
Occurrence ≠ thème. Cooccurrence ≠ synonymie. Proximité ≠ causalité. Similarité lexicale ≠ équivalence. Alias ambigu ≠ résolution arbitraire. Thème lié ≠ même thème. Composante ≠ tout.

### Boldüngo — autorité des couches
Les preuves et représentations architecturales amont ne doivent pas être falsifiées pour faciliter l'adaptation LEGO. Les pertes de fidélité restent explicites.

### IN-SECT — multijoueur
Le serveur doit être autoritaire sur les actions réelles. Distinguer intention locale, action validée, événement accepté, animation locale et snapshot de récupération. Séparer perspective d'affichage et coordonnées logiques.

### Genesis — laboratoire autonome
`hypothèse → prototype minimal → test → observation → décision → conservation/abandon → expérience suivante`.
La vitesse de développement n'est pas le progrès de game design. Une mécanique doit gagner son droit de rester.

### Maketik — pipeline créatif
Séparer sources, faits/transcriptions, analyses, scripts, validations, audio, visuels et exports. Une sortie validée ne doit pas être écrasée silencieusement. Le benchmark final devient une vidéo que l'utilisateur aurait réellement envie de publier.

### Rebulo — garanties distinctes
Validité phonétique, dénomination visuelle spontanée, adéquation à l'âge et validation clinique sont des axes différents. Une solution stricte peut légitimement ne pas exister.

### DROP-Service — produit avant sophistication
Une V1 montrable et des conversations/pilotes réels valent plus qu'un SaaS complet construit sans validation terrain.

## 11. Règle de mesure

**Ne jamais améliorer artificiellement un indicateur en affaiblissant la vérité qu'il est censé mesurer.**

Exemples : réduire les erreurs en supprimant des validations, augmenter la couverture en acceptant des rapprochements faux, déclarer une fonction vérifiée parce qu'elle existe dans le code, rendre un modèle LEGO constructible en falsifiant l'architecture observée.
