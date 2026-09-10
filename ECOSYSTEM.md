# Écosystème — carte compacte

Cette carte décrit les projets connus et leur rôle. Les états techniques doivent être revérifiés dans les dépôts sources.

| Projet | Dépôt | Rôle / spécialité | Maturité à garder en tête |
|---|---|---|---|
| Boldüngo / BrickHouse | `ludodulac/lego-app` | Vérité architecturale, provenance, couches d'autorité, validation déterministe, LEGO fidèle et vérifiable | Projet complexe et fortement gouverné ; convergence visuelle du benchmark réel importante |
| Rebulo | `ludodulac/Rebulo` | Rébus phonétiques, niveaux de garantie, corpus phonétique/visuel, UX enfant/pro | En développement ; rigueur phonétique forte, validation visuelle/âge/clinique distincte |
| Biblaw | `ludodulac/Biblaw` | Corpus structuré, indexation thématique, ambiguïté, audits reproductibles, cartographie sémantique | Fondation canonique solide ; enrichissement sémantique doit préserver les distinctions |
| La Forêt Enchantée | `ludodulac/La-foret-enchantee` | Médiathèque audio jeunesse, médias, sécurité, mutations robustes, expérience d'écoute | Produit léger en évolution |
| DROP-Service | `ludodulac/DROP-Service` | Micro-SaaS artisans, workflow commercial, multi-tenant, validation terrain | V1/pilote : éviter la surconstruction avant validation commerciale |
| IN-SECT | `ludodulac/In-sect` | Jeu de stratégie, règles/état/actions légales, multijoueur, UX de jeu, marketing | Jeu existant ; multijoueur doit devenir une vraie couche produit autoritaire sans casser solo/IA |
| Célébrations des Archanges | `ludodulac/Celebrations` | Contenu canonique, profils/groupes, assignation et expérience personnalisée | Produit fonctionnel en évolution |
| Calis | `ludodulac/Calis` | Callisthénie, progression, contenu/SEO, hypothèse commerce contextuel | **Exploratoire** : domaine et direction produit encore à étudier ; ne pas le traiter comme référence mature |
| Anna Valentine | `annavalentineorg/annavalentine` | Produit vivant mature, administration, données réelles, non-régression, évolution sûre | Référence de maturité production ; certaines zones restent expérimentales/non vérifiées |
| Maketik | `ludodulac/Maketik` | Pipeline créatif source → faits → scripts → validation → audio/visuel/export | Doit maintenant prouver la boucle complète par des vidéos réellement publiables |
| Project Genesis | `ludodulac/Project-Genesis` | Laboratoire autonome de game design, simulation déterministe, émergence | Très jeune ; aucune mécanique n'est sacrée tant qu'elle n'a pas gagné le droit de rester |
| Wikignose | dépôt à confirmer | Fonds documentaire, provenance, originaux vs dérivés, futur traitement de PDF | Projet/architecture émergente ; stockage documentaire brut ne vaut pas connaissance validée |

## Lecture par spécialité

- **Vérité / provenance / contrats** : Boldüngo.
- **Canon / index / ambiguïté** : Biblaw.
- **Garanties linguistiques / corpus** : Rebulo.
- **Production vivante / non-régression** : Anna Valentine.
- **Règles / actions / synchronisation de jeu** : IN-SECT.
- **Laboratoire de game design** : Genesis.
- **Pipeline créatif vertical** : Maketik.
- **Workflow business / validation marché** : DROP-Service.
- **Personnalisation par profils** : Célébrations.
- **Médias / mutations sûres / écoute** : La Forêt Enchantée.
- **Exploration contenu-produit-commerce** : Calis.
- **Fonds documentaire / provenance** : Wikignose.
