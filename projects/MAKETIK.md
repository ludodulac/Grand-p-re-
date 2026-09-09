# Maketik

Source : `ludodulac/Maketik`.

## Mission
Transformer des sources longues en vidéos courtes réellement publiables, avec un pipeline créatif traçable et des validations explicites.

## Spécialité réutilisable
Séparer source, transcription/faits, analyse, script, validation humaine, audio, visuel et export.

## Invariants durables
- Ne pas écraser silencieusement un script ou artefact déjà validé.
- Une régénération doit respecter les validations existantes sauf remplacement explicite.
- Ne pas prétendre qu'une transcription, génération IA, audio ou ingestion est opérationnelle sans preuve réelle.
- Les références TikTok peuvent guider structure/rythme sans être copiées ; les sources YouTube alimentent les faits, pas le texte final.

## Décision d'architecture connue
Pas de Vercel tant que l'utilisateur ne change pas explicitement cette décision ; GitHub Actions peut assurer des vérifications éphémères.

## Risque connu
Sauter trop vite vers le visuel avant de prouver une boucle éditoriale robuste de bout en bout.

## Benchmark utile
La vraie réussite n'est pas seulement un pipeline vert : c'est une vidéo que l'utilisateur aurait réellement envie de publier.

## À revérifier dans le dépôt
Pipeline actif, providers disponibles, validations humaines présentes, capacité audio réelle, sorties visuelles et export final.