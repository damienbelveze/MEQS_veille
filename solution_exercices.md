---
title: Solutions aux exercices
author: Damien Belvèze
date: 12/09/2022
---

# transition avec le cours précédent

| Numéro | fiche verte | fiche jaune | fiche rose |
|:---:|:---:|:---:|:---:|
| 1 | une série de rencontres balladodiffusées | https://theconversation.com/au/podcasts/politics-with-michelle-grattan.rss | disposer d'un lecteur de flux |
| 2 | un article trouvé sur une bibliothèque pirate | https://sci-hub.se/10.1016/j.amepre.2019.12.005 | Site indisponible en passant par les principaux fournisseurs d'information à Internet |
| 3 | un article scientifique diffusé sur un site d'archives | https://www-jstor-org.passerelle.univ-rennes1.fr/stable/44001212#metadata_info_tab_contents | accessible aux abonnés de Rennes 1 mais pas à tous les internautes
| 4 | un article scientifique en open access | https://doi-org.passerelle.univ-rennes1.fr/10.1177/0141076817696054 | accessible à tous les internautes |
| 5 | un moteur de recherche inverse d'images permettant de classer les résultats par date | https://www.tineye.com | accessible à tous les internautes |
| 6 | un site permettant de repérer des ouvrages présents dans une autre bibliothèque pour les faire venir | https://www.sudoc.abes.fr | accessible à tous les internautes |
| 7 | un logiciel permettant de gérer des références bibliographiques | https://www.zotero.org | librement téléchargeable |
| 8 | un jeu de données relatif à un article à paraître | https://zenodo.org/record/6868945 | accessible après embargo |

Certains triplets introduisent des formats, notions pas encore connues (flux, gestion de références bibliographiques)
A ce stade, il ne s'agit pas encore de définir ce dont il s'agit, mais de susciter la curiosité des étudiants.


# Recherche d'informations à partir d'une image

Identifier l'image proposée
Réponse : avec un moteur de recherche inverse d'images.
une recherche avec Tineye permet d'accéder à [un site](https://www.alamy.com/stacie-pace-a-nurse-practitioner-who-opened-spectrum-the-other-clinic-offers-trans-individuals-hormone-therapy-in-south-mississippi-pictured-here-in-her-office-in-hattiesburg-miss-july-17-2020-she-centers-her-care-on-meeting-trans-and-non-binary-indiviuals-needs-to-transition-through-hormone-therapy-hat-4389-photo-by-cam-bonellihattiesburg-americanusa-today-networksipa-usa-image407746601.html?irclickid=xJG3Gl2%3AKxyNT0H2N%3ASXpxqkUkDR%3AL1%3AxxkHw00&utm_source=77643&utm_campaign=Shop%20Royalty%20Free%20at%20Alamy&utm_medium=impact&irgwc=1) qui donne des informations sur l'image. 

# Faire de la veille avec les réseaux sociaux

## Présence sur Twitter

Stacie Pace a t-elle un compte sur Twitter ? 
Réponse : @staciepace est un homonyme, en revanche la clinique *Spectrum : the other clinic* a un compte sur Twitter (@otherclinic)

## choisir avec discernement les sources à suivre

- @adgpi (Armée indienne). peu d'[informations crédibles sur le yeti](https://twitter.com/search?q=%40adgpi%20yeti&src=typed_query)  
- @oliveratlantis : chercheur ayant publié dans une revue savante un article sur le mythe du Yeti : très bon candidat  
- @HLizanne : cette chercheuse de l'université de Glasgow ne paraît pas avoir publié récemment quoique ce soit sur Twitter au sujet du Yeti : https://twitter.com/search?q=%40HLizanne%20Yeti&src=typed_query&f=top. Il s'agit bien d'une spécialiste du Folklore, mais sur Scholar non plus, [aucune publication sur le sujet](https://scholar.google.com/citations?user=bfFPJZkAAAAJ&hl=fr&inst=17849131778672153748&oi=ao), plutôt spécialisée dans le domaine des mythologies d'Angleterre et du nord de l'Europe  
- @YetiNation10 : par Yetis, ici, on entend une équipe de sport (football américain ?)  

Question : y a t-il quelque chose sur Instagram, pour ce que vous pouvez en voir- qui concerne la clinique Spectrum ?
Réponse (avec Dumpor) : https://dumpor.com/v/the_other_clinic

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

# Faire de la veille avec Pubmed

Requêtes possibles : 
- Quality AND "Health Services for Transgender Persons"[Mesh] : 27 résultats
- ("Quality Indicators, Health Care"[Mesh]) AND "Transgender Persons"[Mesh] : 25 résultats
- ("Health Services Needs and Demand"[Mesh]) AND "Transgender Persons"[Mesh] AND Quality : 14 résultats

