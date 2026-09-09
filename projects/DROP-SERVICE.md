# DROP-Service

Source : `ludodulac/DROP-Service`.

## Mission
Micro-SaaS pour artisans : réception, qualification et suivi simple des demandes clients jusqu'au pipeline Nouveau → Contacté → Devis → Gagné/Perdu.

## Spécialité réutilisable
Multi-tenant simple, workflow métier clair, validation marché avant sophistication technique.

## Invariants durables
- Une seule base de code multi-clients.
- Isolation stricte des données par artisan.
- Pas d'IA, WhatsApp, SMS payants ou CRM obligatoire dans le cœur V1.
- Ne pas payer des outils « au cas où ».
- Arrêter d'ajouter dès que la V1 est montrable et aller parler aux artisans.

## Validation produit
Les conversations réelles, démonstrations et pilotes payants valent plus qu'un produit techniquement « complet » construit sans preuve de besoin.

## Continuité IA
Lors de l'audit du 2026-09-09, aucun `AI_START_HERE.md` n'était présent à la racine. README + `docs/PRODUCT.md`, `docs/ARCHITECTURE.md`, `docs/ROADMAP.md` constituent déjà une bonne base ; un routeur court serait utile sans recopier ces documents.

## À revérifier dans le dépôt
État de la V1, authentification/RLS, pipeline réel, déploiement, retours artisans et pilotes.