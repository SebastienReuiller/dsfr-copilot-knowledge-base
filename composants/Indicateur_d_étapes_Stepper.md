Fermer

# Indicateur d'étapes - Stepper

L’indicateur d'étapes permet d’indiquer à l’utilisateur où il se trouve dans
un formulaire ou dans une démarche.

Cet indicateur d'étapes est utilisable dans le cas d’un processus linéaire, le
composant ne permet pas de naviguer d’une étape à une autre (pour cela, il
faudra utiliser des boutons).

## Structure

L’indicateur d'étapes est constitué des éléments suivants :

  * Le numéro de l'étape et le nombre d'étapes total - obligatoire
  * le titre de l'étape en cours - obligatoire
  * la barre de progression - obligatoire
  * le titre de l'étape suivante - obligatoire.

La barre de progression contient autant de sections qu’il y a d'étapes, les
étapes validées et l'étape en cours sont en bleu.

Aucun des éléments de l’indicateur d'étapes n’est cliquable.

##  Titre de l'étape en cours Étape 1 sur 3

Étape suivante : Titre de la prochaine étape

###  Extrait de code

    
    
                          <div class="fr-stepper">
        <h2 class="fr-stepper__title">
            Titre de l'étape en cours
            <span class="fr-stepper__state">Étape 1 sur 3</span>
        </h2>
        <div class="fr-stepper__steps" data-fr-current-step="1" data-fr-steps="3"></div>
        <p class="fr-stepper__details">
            <span class="fr-text--bold">Étape suivante :</span> Titre de la prochaine étape
        </p>
    </div>
                          
                        

##  Titre de la dernière étape en cours Étape 4 sur 4

###  Extrait de code

    
    
                          <div class="fr-stepper">
        <h2 class="fr-stepper__title">
            Titre de la dernière étape en cours
            <span class="fr-stepper__state">Étape 4 sur 4</span>
        </h2>
        <div class="fr-stepper__steps" data-fr-current-step="4" data-fr-steps="4"></div>
    </div>
    
                          
                        

## Règles d’utilisation

### Usages

L’indicateur d'étapes ne sert pas à naviguer d’une étape à l’autre, pour cela
utiliser des boutons en bas des champs de l'étape.

Il est conseillé de finir par une étape de confirmation. Il est aussi
conseillé de créer une page d’introduction à la démarche, avant de commencer
cette dernière pour présenter les différentes étapes, sur laquelle ne figure
pas cet indicateur d’étapes.  

Le nombre maximal d’étapes proposées dans le composant est limité à 8. En
effet, plus le parcours du formulaire est long, plus le risque d’abandon est
élevé. De ce fait, il est nécessaire d’identifier avec soin les champs
demandés aux utilisateurs et les rassembler au maximum dans des sections
similaires.

### Contenus

  * Chaque étape doit avoir un titre clair, unique et ne comprenant pas le numéro de l'étape (car on l’a déjà dans le champ numéro de l'étape).
  * À la dernière étape, le titre de l'étape suivante n’est pas à afficher.

### Accessibilité

  * Le titre de l’étape est bien dans un élément <hx>
  * Le numéro de l’étape et le nom de l'étape suivante sont dans des éléments <p>
  * La barre de progression ne nécessite aucune alternative ni attribut aria (car purement illustrative).

### Personnalisation

Le style de ce composant n’est pas personnalisable.

### Besoin d'aide ?

L'équipe du DSFR est là pour vous aider.

Retrouvez-la sur :

  * [la communauté slack](https://gouvfr.slack.com/ "la communauté slack - nouvelle fenêtre") pour poser vos questions, et échanger avec d’autres utilisateurs.   
Vous êtes **agent de l’État** et souhaitez accéder au slack ? [Rejoignez la
communauté](https://gouvfr.atlassian.net/servicedesk/customer/portal/1/group/1/create/9
"Rejoignez la communauté - nouvelle fenêtre") dès maintenant !

  * [ le centre de support](https://gouvfr.atlassian.net/servicedesk/customer/portals "le centre de support - nouvelle fenêtre") pour envoyer vos demandes de correctifs et d'évolution.

[Gestionnaire de consentement - Consent banner](/composants-et-
modeles/composants/gestionnaire-de-consentement)

[Infobulle - Tooltip](/composants-et-modeles/composants/infobulle)

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
