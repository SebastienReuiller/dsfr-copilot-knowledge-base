Fermer

# Mise en avant - Callout

La mise en avant permet à l’utilisateur de distinguer rapidement une
information qui vient compléter le contenu consulté.

## Mise en avant

La mise en avant est une proposition de mise en page du contenu éditorial pour
mettre en évidence une information complémentaire.

### Structure

Elle se compose des éléments suivants :

  * Une icône - optionnellepour aider à la compréhension du message. L’icône est facilement modifiable : la classe correspondante à l’icône voulue doit être placée dans l’attribut class de l'élément .fr-callout.  
[Voir les icônes disponibles](/elements-d-interface/fondamentaux-
techniques/icone).

  * pour aider à la compréhension du message. L’icône est facilement modifiable : la classe correspondante à l’icône voulue doit être placée dans l’attribut class de l'élément .fr-callout.  
[Voir les icônes disponibles. ](/elements-d-interface/fondamentaux-
techniques/icone)

  * Un titre - optionnel 
  * Une description - obligatoire 
  * Un bouton - optionnel qui permet d’inciter à l’action, ou un lien pour naviguer vers un autre contenu. 
  * qui permet d’inciter à l’action, ou un lien pour naviguer vers un autre contenu. 
  * Une bordure de couleur (voir la personnalisation possible décrite dans cette page)- obligatoire. 

### Titre mise en avant

Les parents d’enfants de 11 à 14 ans n’ont aucune démarche à accomplir : les
CAF versent automatiquement l’ARS aux familles déjà allocataires qui
remplissent les conditions.

Label bouton MD

    
    
                    <div class="fr-callout fr-icon-information-line">
        <h3 class="fr-callout__title">Titre mise en avant</h3>
        <p class="fr-callout__text">
            Les parents d’enfants de 11 à 14 ans n’ont aucune démarche à accomplir : les CAF versent automatiquement l’ARS aux familles déjà allocataires qui remplissent les conditions.
        </p>
        <button class="fr-btn">
            Label bouton MD
        </button>
    </div>
                    
                  

Hiérarchisez et sélectionnez votre contenu, afin d’utiliser une ou deux mises
en avant maximum par page, sinon elles attireront moins l’œil de
l’utilisateur.

### Pour les développeurs

Le titre, matérialisé par la classe fr-callout__title peut être :  
\- une balise <h3> (défaut) : <h3 class="fr-callout__title"> , ou  
\- une autre balise de titre : <h2 class="fr-callout__title"> à <h6>  
\- une balise <p> si jamais vous estimez qu'il ne s'agit pas d'un titre..  
Vous pouvez ainsi adapter le titre du bloc à la structure et l’architecture de
votre contenu.  

## Règles d’utilisation

### Usages

Les messages d’erreur, d’alerte ou de confirmation, ne sont pas des mises en
avant. Pour utiliser ces blocs, rendez-vous dans la section
"[Alertes](/elements-d-interface/composants/alerte)".

### Accessibilité

  * Le niveau de titre dépend du contexte (et ne sera pas toujours un <h3>).

### Contenus

Les informations mises en avant doivent être synthétiques.

## Personnalisation

Certains éléments sont optionnels et les icônes peuvent être changées:

#### Couleurs d’accent

Les éléments fond et bordure peuvent utiliser les couleurs illustratives :

Élément  
| Valeur par défaut  
| Valeur(s) autorisée(s)  
  
---|---|---  
|  | Token | Classe css  
Bordure | $border-default-blue-france  
Correspondances :  
Thème clair et sombre =  
$blue-france-main-525  
| $[couleur]-main (thèmes clair / sombre)  
exemples :  
$green-emeraude-main-632  
$brown-caramel-main-648  
  
  
|  
  
.fr-callout--[couleur]  
.fr-callout--green-emeraude  
.fr-callout--brown-caramel  
Fond | $background-contrast-neutral  
Correspondances :  
Thème clair = $grey-950  
Thème sombre = $grey-100  
| $[couleur]-950 (thème clair)  
$[couleur]-100 (thème sombre)  
exemples:  
thème clair = green-emeraude-950  
thème sombre = green-emeraude-100  
  
thème clair = brown-caramel-950  
thème sombre = brown-caramel-100  
  
  
### Titre mise en avant

Les parents d’enfants de 11 à 14 ans n’ont aucune démarche à accomplir : les
CAF versent automatiquement l’ARS aux familles déjà allocataires qui
remplissent les conditions.

Label bouton MD

### Titre mise en avant

Les parents d’enfants de 11 à 14 ans n’ont aucune démarche à accomplir : les
CAF versent automatiquement l’ARS aux familles déjà allocataires qui
remplissent les conditions.

Label bouton MD

### Besoin d'aide ?

L'équipe du DSFR est là pour vous aider.

Retrouvez-la sur :

  * [la communauté slack](https://gouvfr.slack.com/ "la communauté slack - nouvelle fenêtre") pour poser vos questions, et échanger avec d’autres utilisateurs.   
Vous êtes **agent de l’État** et souhaitez accéder au slack ? [Rejoignez la
communauté](https://gouvfr.atlassian.net/servicedesk/customer/portal/1/group/1/create/9
"Rejoignez la communauté - nouvelle fenêtre") dès maintenant !

  * [ le centre de support](https://gouvfr.atlassian.net/servicedesk/customer/portals "le centre de support - nouvelle fenêtre") pour envoyer vos demandes de correctifs et d'évolution.

[Menu latéral - Sidemenu](/composants-et-modeles/composants/menu-lateral)

[Mise en exergue - Highlight](/composants-et-modeles/composants/mise-en-
exergue)

### Le DSFR

  * [ Nous contacter ](https://gouvfr.atlassian.net/servicedesk/customer/portals "Nous contacter - nouvelle fenêtre")
  * [Support](/centre-de-support)
  * [Communauté](/communaute)

### Liens utiles

  * [Charte de l'État](https://www.info.gouv.fr/marque-Etat "Charte de l'État - nouvelle fenêtre")
  * [Obtenir l'agrément](/utilisation-et-organisation/procedure-des-agrements)
  * [Notes de version](/a-propos/versions/version-courante)

[ république  
française

](/ "Retour à l’accueil du site - République Française")

Ce site est géré par le Service d’Information du Gouvernement (SIG)

  * [info.gouv.fr](https://info.gouv.fr "info.gouv.fr - nouvelle fenêtre")
  * [service-public.fr](https://service-public.fr "service-public.fr - nouvelle fenêtre")
  * [legifrance.gouv.fr](https://legifrance.gouv.fr "legifrance.gouv.fr - nouvelle fenêtre")
  * [data.gouv.fr](https://data.gouv.fr "data.gouv.fr - nouvelle fenêtre")

  * [Accessibilité : totalement conforme](/accessibilite)
  * [Conditions générales d’utilisation](/a-propos/conditions-generales-d-utilisation)
  * [Mentions légales](/mentions-legales)
  * [Plan du site](/plan-du-site)
  * Gestion des cookies 
  * Paramètres d'affichage 

Sauf mention contraire, tous les contenus de ce site sont sous [licence
etalab-2.0](https://github.com/etalab/licence-ouverte/blob/master/LO.md
"licence etalab-2.0 - nouvelle fenêtre")

Fermer
