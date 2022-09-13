---
title: Cours Veille master MEQS
author: Damien Belvèze
date: 20220907
---

La réponse aux exercices ci-dessous se trouve dans le document "solution_exercices"
Sur le contexte du déroulé de la séance et ses objectifs, voir le fichier README.

# transition avec le cours précédent. 

Avec le matériel listé ci-dessous :

- 8 fiches vertes sur chacune un texte décrivant l'utilité d'un outil (le nom de l'outil est absent de ce descriptif)  
- 8 fiches jaunes sur chacune une URL écrit à la main ou un QR code imprimé (plus rapide à utiliser)  
- 8 fiches roses sur chacune une ou des conditions pour accéder à l'information (authentifié, accessible à tous, accessible depuis le campus, etc.)  

Reconstituez les triplets (service / lien / type d'accès)

# Recherche d'informations à partir d'une image

Comment vous serait-il possible d'identifier l'image suivante : qui est sur la photo ? où se trouve t-on ? De quand date la photo ?  

![](images/nurse.jpg)

Confirmer les informations sur l'image en faisant des recherches complémentaires 

trouver un autre site, de préférence crédible, qui met en relation la personne sur la photo et le nom trouvé.

# Faire de la veille sur les réseaux sociaux

## Présence sur Twitter

Quelle présence sur Twitter : cette personne a t-elle un compte personnel ? Son institution a t-elle un compte ? 

## choix du réseau social

Sur quel réseau social chercher à suivre une personne ? Cela dépend de l'occupation de la personne. 

- Twitter : hommes et femmes politique, chercheurs, journalistes, professionnels de l'information, militants. Profils très majoritairement ouverts
- Facebook : Les personnes arrivées sur Facebook entre 2015 et aujourd'hui ont souvent fait fuir les plus jeunes ou les plus geeks vers d'autres réseaux. Facebook a d'abord attiré des ados et de jeunes adultes, aujourd'hui, on va plus facilement trouver leurs parents. 
- Instagram : influenceurs, photographes, artistes, mais aussi toute une partie du grand public qui préfère Instagram à Twitter rebuté par la violence des échanges sur le réseau de l'oiseau bleu. Profils tantôt ouverts, tantôt privés
- ResearchGate : chercheurs (au départ en sciences exactes, mais de plus en plus de chercheurs en Sciences Humaines rebutés par le modèle économique d'Academia.edu ont tendance à s'y retrouver)

On peut librement chercher des profils dans [Twitter](https://www.twitter.com) sans avoir de compte. 
En revanche, Instagram vous force la main pour obtenir des informations sur ses abonnés : il faut que vous fassiez vous-même partie des abonnés. Il existe une alternative pour sonder Instagram sans se créer de compte : le site [Dumpor](https://dumpor.com) qui donne accès aux comptes publics sur Instagram. Evidemment, pour suivre ce qu'écrivent ces abonnés au réseau, il vous faudra vous y abonner vous-même. 

Y a t-il quelque chose sur Instagram, pour ce que vous pouvez en voir- qui concerne la clinique en question ? 


## Choisir avec discernement les sources à suivre. 

L'exercice suivant est proposé aux doctorants de Rennes, dans le cadre d'un exercice sur la veille.
Supposons que vous soyez un chercheur dans le domaine du folklore. Quel compte Twitter vous semble le plus intéressant à suivre sur le folklore relatif au Yeti. 

- @adgpi  
- @oliveratlantis 
- @HLizanne  
- @YetiNation10  

# Les agrégateurs de flux

## Qu'est ce que le RSS ?

Le RSS donne la possibilité d'automatiser la collecte de renseignements.
flux = fichier en xml qui permet d'envoyer de l'information qui paraît sur une page ou un site vers une autre page (agrégateur de flux)
RSS : premier protocole pour la mise en oeuvre de cette fonctionnalité (il y a aussi atom). RSS est devenu en quelque sorte générique : un flux RSS (Really Simple Syndication) désigne à la fois les flux RSS, les flux Atom et les autres fichiers de ce type.
Assez-souvent une [icone orange](https://www.google.com/search?tbm=isch&q=RSS&tbs=imgo:1) permet de faciliter la capture d'un flux.

Le RSS est un protocole aussi massif qu'il est invisible : tous les abonnements aux podcasts fonctionnent au moyen de ce protocole.
Une grande partie des sites, conçus avec Wordpress, disposent d'un flux RSS par défaut qui n'est pas forcément visible sur la page d'accueil du site (pas d'icone)

Le RSS permet une syndication (=abonnement) **loyale**, au sens où toutes les nouveautés du site vous parviennent. Il n'y a pas de tri opéré en amont par un algorithme qui vous sert uniquement ce qu'il estime plus pertinent pour vous (Sur les réseaux sociaux, vous ne voyez plus forcément tous les nouveaux posts des personnes que vous suivez).
Comparé à la newsletter ou à l'usage du mail, le RSS a l'avantage de ne laisser aucune donnée personnelle à une plateforme. La plupart des réseaux sociaux sont gourmands en données personnelles (mails, centres d'intérêts) que leurs ingénieurs convertissent en profils publicitaires. Le RSS ne participe pas de cette logique, il est compréhensible que la plupart de ces plateformes ne proposent pas de flux et qu'ils faillent trouver des solutions de contournement.

## utiliser un agrégateur

Feedbro (si on ne change pas souvent de machine et de navigateur)
Feedly (si on préfère le cloud)

pour reprérer un flux dans un site dépourvu d'icone, télécharger l'URL du site ou dans Feedbro, cliquer sur le lien "find feeds in open tab"

## Gérer de façon fine les flux RSS

### créer, filtrer

Possibilité de construire un flux RSS à partir d'une page avec Feed43 (voir https://youtu.be/DcEbjeMciOQ)

Possibilité de filtrer un flux avec [Pipes Digital](https://pipes.digital). Voir par exemple [ce flux](https://www.pipes.digital/pipe/MOQ7k19e) qui ajoute un filtre "numérique" appliqué sur le flux RSS de la rubrique Santé du site Lemonde.fr

Possibilité de convertir un compte Twitter en flux RSS. Utiliser pour ce faire le site [Nitter (instance FDN)](https://nitter.fdn.fr) Ce service permettra de sauvegarder un flux RSS en lien avec sa recherche sur Twitter
chercher dans Nitter @theotherclinic et cliquer dans Feedbro (Find Feeds in Current tab)

### Faites l'un des exercices suivants : 

Les exercices qui suivent sont d'une difficulté croissante, n'hésitez pas à demander l'aide de vos formateurs.

#### exercice 1 : importer un flux

Importer dans l'agrégateur de votre choix les flux RSS des sites suivants :
- Site du Réseau Sentinelles    
- Actualités du site Santé Publique France sur le thème de l'alcool    

#### exercice 2 : filtrer un flux

- faire un filtre au flux RSS du site Libération.fr en filtrant avec le mot "ukraine"
- faire un flux RSS à partir des essais cliniques publiés sur le site Biorxiv portant sur la dépression.

#### exercice 3 : construire un flux 

construire un flux avec [Feed43](https://feed43.com/) pour le [portail étudiant de Rennes 1](https://etudiant.univ-rennes1.fr) ou pour la page des appels à projet du site de l'ARS


## Twitter en mode RSS

on peut faire une recherche sur Twitter sans avoir de compte avec Twitter search ou bien avec https://nitter.fdn.fr Ce service permettra de sauvegarder un flux RSS en lien avec sa recherche sur Twitter entrer le flux dans la bibliothèque de flux de Zotero

Rélaiser avec Nitter et avec le compte Twitter @theotherclinic un flux RSS et l'intégrer dans Feedbro (Find Feeds in Current tab)

# faire de la veille avec Pubmed

A partir de ce que vous avez vu dans la première séance. 
Faites une requête pour obtenir des résultats sur l'évaluation des soins apportés aux personnes transgenres.

Trouver des requêtes qui génèrent un nombre compris entre 50 et 10 résultats (possibilité de mixer des mots MESH et des mots du langage naturel)

Sauvegardez dans Feedbro (ou Feedly) le flux issu de la requête.