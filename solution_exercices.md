---
title: correction des exercices
author: Damien Belvèze
date: 12/09/2022
---


# Faire de la veille avec les réseaux sociaux : 

- @adgpi (Armée indienne). peu d'[informations crédibles sur le yeti](https://twitter.com/search?q=%40adgpi%20yeti&src=typed_query)  
- @oliveratlantis : chercheur ayant publié dans une revue savante un article sur le mythe du Yeti : très bon candidat  
- @HLizanne : cette chercheuse de l'université de Glasgow ne paraît pas avoir publié récemment quoique ce soit sur Twitter au sujet du Yeti : https://twitter.com/search?q=%40HLizanne%20Yeti&src=typed_query&f=top. Il s'agit bien d'une spécialiste du Folklore, mais sur Scholar non plus, [aucune publication sur le sujet](https://scholar.google.com/citations?user=bfFPJZkAAAAJ&hl=fr&inst=17849131778672153748&oi=ao), plutôt spécialisée dans le domaine des mythologies d'Angleterre et du nord de l'Europe  
- @YetiNation10 : par Yetis, ici, on entend une équipe de sport (football américain ?)  


# Flux RSS

## exercice 1

- flux du site du Réseau Sentinelles  
Le [flux](https://www.sentiweb.fr/france/fr/?page=rss) est tout en bas de la page d'accueil

- flux des actualités du site Santé Publique France sur le thème de l'alcool  
cliquer en bas de la page sur l'icone RSS et choisir dans la liste des flux, [celui correspondant aux actualités sur l'alcool](https://www.santepubliquefrance.fr/rss/themes/alcool.xml?1662988359)

## exercice 2

### Portail étudiant Rennes 1 : 

URL : https://etudiant.univ-rennes1.fr/
global search pattern : 

````html
<div class="views-field views-field-nothing">{%}
````
item repeatable search pattern : 

````html
<a class="card card-link waves-effect hoverable zoom d-flex" href="{%}" title="{%}" target="_blank">{*}<div class="card-link__content"><span class="field-content">{%}</span></div>{*}<h3 class="card-title">{%}</h3>{*} 
````

{%1} = https://soie.univ-rennes1.fr/actualites/imagine-ta-start
{%2} = Imagine ta start-up !
{%3} = Viens te tester à la création d'entreprise le mardi 27 septembre de 16h à 20h.
{%4} = Imagine ta start-up !

item Title template = {%2}
Item Link template = {%1}
Item Content template = {%3}

flux : https://feed43.com/7462500163651030.xml

### appels à projets sur le site des ARS

https://www.ars.sante.fr/liste-appels-projet-candidature-nationale

global search pattern : 

````html
<h3 class="accueil-appels-projets--item-titre"{%}
````

item repeatable search pattern :

````html
<a href="{%}" title="Voir le contenu sur la région (nouvelle fenêtre)" rel="noopener noreferer" target="_blank" >{%}</a>
````

{%1} = https://www.bourgogne-franche-comte.ars.sante.fr/parcours-de-soins-global-apres-le-traitement-cancer-2022
{%2} = Parcours de soins global après le traitement d’un cancer

item Title templace = {%2}
item Link template = {%1}

## exercice 3

utiliser Pipe Digital

- faire un filtre au flux RSS du site Libération.fr en filtrant avec le mot "ukraine"

Aller sur le site de Liberation.fr. Chercher l'icone RSS, cliquer dessus. Copier le lien obtenu. 
ouvrir [Pipes Digital](https://www.pipes.digital/editor). 
Entrer le flux dans une boîte feed, ajouter une boîte filtre. Dans la boîte filtre, ajouter le mot-clé "ukraine". Relier les boîtes entre elles et à l'output. Sauvegarder et télécharger le flux pour l'entrer ensuite dans votre agrégateur de flux.

URL du flux : 

- faire un flux RSS à partir des essais cliniques publiés sur le site Biorxiv portant sur la dépression.

Aller sur le site [Biorxiv (=serveur de preprints)](https://www.biorxiv.org). Cliquer sur [RSS/Alerts](https://www.biorxiv.org/alertsrss) dans le menu supérieur. Sélectionner le flux correspondant aux essais cliniques (= clinical trials)

ouvrir [Pipes Digital](https://www.pipes.digital/editor). 
Entrer le flux dans une boîte feed, ajouter une boîte filtre. Dans la boîte filtre, ajouter le mot-clé "depression". Relier les boîtes entre elles et à l'output. Sauvegarder et télécharger le flux pour l'entrer ensuite dans votre agrégateur de flux.

URL du flux : https://www.pipes.digital/feedpreview/7N38QxOy

