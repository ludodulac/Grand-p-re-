# Incident — corriger un symptôme au mauvais niveau

## Pattern
Un problème visible pousse facilement à corriger la présentation alors que la source du défaut est dans le modèle, l'autorité ou la représentation canonique.

## Exemples réutilisables
- multijoueur : bloquer un clic ou retourner le plateau ne corrige pas un mauvais modèle d'autorité/synchronisation ;
- contenu riche : du CSS ne répare pas une structure sémantique perdue ;
- recherche : un classement ne peut pas réparer une relation sémantique fausse ;
- LEGO : déplacer visuellement une brique ne doit pas falsifier la Scene architecturale.

## Règle durable
Avant de corriger :
1. identifier la couche qui possède la vérité ;
2. distinguer symptôme, représentation et cause ;
3. corriger au niveau propriétaire ;
4. ajouter une régression au niveau pertinent ;
5. vérifier ensuite la présentation.

## Signal d'alerte
Si plusieurs petits patchs UX/CSS/conditions locales s'accumulent autour du même problème, suspecter une frontière de modèle ou d'autorité incorrecte.