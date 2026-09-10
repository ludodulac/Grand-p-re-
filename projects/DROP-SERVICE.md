# DROP-Service

Source : `ludodulac/DROP-Service`.

## Mission
Micro-SaaS destiné notamment aux artisans pour faciliter la réception et le traitement des demandes clients sans imposer un CRM lourd.

Chaîne produit visée :

`CLIENT → DEMANDE → INFORMATIONS UTILES → TRAITEMENT PAR L'ARTISAN → SUIVI`

Le produit doit d'abord résoudre simplement et correctement un problème quotidien : ne pas perdre les demandes, savoir quoi faire ensuite et suivre leur avancement.

## Spécialité réutilisable
Multi-tenant simple, workflow métier clair, isolation des données et validation marché avant sophistication technique.

## Invariants durables
- Une seule base de code multi-clients.
- Isolation stricte des données par artisan.
- Chaque demande doit rester rattachée au bon artisan et visible uniquement dans le bon contexte.
- Pas d'IA, WhatsApp, SMS payants ou CRM complexe obligatoires dans le cœur V1.
- Ne pas payer ni ajouter des outils « au cas où ».
- Préserver un parcours simple : recevoir → comprendre → traiter → suivre.
- Arrêter d'ajouter lorsque la V1 est suffisamment démontrable pour être confrontée à des artisans réels.

## Validation produit
Les conversations réelles, démonstrations et pilotes valent plus qu'un produit techniquement « complet » construit sans preuve de besoin.

Ne pas confondre :

`fonction présente → parcours réellement simple → artisan qui comprend → artisan qui l'utilise → problème quotidien réellement réduit`

La sophistication commerciale ou automatisée doit venir après preuve qu'elle enlève une friction réelle.

## Risque connu
Transformer trop tôt le produit en gros CRM ou en démonstration d'IA. Une architecture techniquement élégante n'est pas un progrès si elle augmente la charge mentale de l'artisan ou retarde la validation terrain.

## Continuité IA
Le dépôt possède désormais un `AI_START_HERE.md` ainsi que des documents produit/architecture. Lire le routeur local puis seulement la zone pertinente. Vérifier l'état réel du code, du schéma Supabase/RLS et du parcours avant d'agir.

## À revérifier dans le dépôt
État de la V1, authentification/RLS, isolation réelle multi-client, pipeline de demandes, déploiement, simplicité du parcours, retours artisans, démonstrations et pilotes.