# Wikignose

Source : dépôt standalone à confirmer.

## Mission
Construire un fonds documentaire durable à partir de centaines de PDF, avec provenance, originaux immuables et futurs dérivés exploitables.

## Spécialité réutilisable
Séparer document source, extraction, analyse, indexation et contenu utilisable.

## Modèle conceptuel
`PDF raw → text extraction → analysis → indexing → usable content`

## Invariants durables
- Les originaux doivent rester identifiables et idéalement immuables.
- Stocker provenance, source/URL, date d'import, auteur/date/type/status lorsqu'ils sont connus.
- Utiliser un identifiant stable et un hash pour déduplication/provenance.
- Distinguer duplicate exact, version différente et document seulement similaire.
- Ne pas confondre stockage documentaire avec connaissance validée.
- Ne jamais mettre de secrets dans GitHub ou le frontend.

## Direction stockage
Cloudflare R2 avait été envisagé comme fonds documentaire brut, privé par défaut, avec structure stable des clés. Toujours revérifier accès, coûts et contraintes actuelles avant opération réelle.

## À revérifier
Dépôt réel, stockage actif, permissions, statut des imports et règles juridiques/licences des documents.