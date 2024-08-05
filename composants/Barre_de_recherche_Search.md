Fermer

# Barre de recherche - Search

La barre de recherche est un système de navigation qui permet à l'utilisateur
d’accéder rapidement à un contenu en lançant une recherche sur un mot clé ou
une expression.

## Barre de recherche

### Structure

La barre de recherche se compose des éléments suivants :

  * un champs de saisie - obligatoire.
  * un bouton primaire - obligatoire. 

### Barre de recherche MD

Choisissez la barre de recherche MD lorsqu'il y a des contraintes d'espace
dans vos interfaces. Le cas d’usage principal est l’accès à la recherche
globale depuis l’en-tête.

Il peut également être spécifique à certains composants dans le cas de
recherche contextuelle (exemple : recherche pour filtrer des listes ou un
tableau de données).

Recherche  Rechercher

    
    
                    <div class="fr-search-bar" id="header-search" role="search">
       <label class="fr-label" for="search-784-input">
           Recherche
       </label>
       <input class="fr-input" placeholder="Rechercher" type="search" id="search-784-input" name="search-784-input">
       <button class="fr-btn" title="Rechercher">
           Rechercher
       </button>
    </div>
                    
                  

### Barre de recherche LG

Choisissez la barre de recherche LG pour présenter un moteur de recherche
global à l’intérieur d'une page (exemple : mise en avant de la recherche
depuis la home page, moteur de recherche sur la liste de résultats de
recherche).

Recherche  Rechercher

    
    
                    <div class="fr-search-bar fr-search-bar--lg" id="search-2" role="search">
       <label class="fr-label" for="search-787-input">
           Recherche
       </label>
       <input class="fr-input" placeholder="Rechercher" type="search" id="search-787-input" name="search-787-input">
       <button class="fr-btn">
           Rechercher
       </button>
    </div>
                    
                  

## Responsive

Pour l’affichage mobile/tablette, il est obligatoire d’utiliser le format MD
qui est le plus adapté.

Si vous utilisez le format LG en desktop, le composant sera automatiquement
redimensionné au format MD

![](/uploads/Capture_d_ecran_2020_07_24_a_15_18_53_8ffffd36b4.png)

![](/uploads/Capture_d_ecran_2020_07_24_a_15_19_18_b7767098da.png)

## Règles d’utilisation

### Usage

La barre de recherche doit être assez LG, pour afficher 27 caractères minimum.
Cela doit permettre aux utilisateurs de saisir plusieurs termes et qu’ils
restent tous visibles. Si les termes de la recherche restent visibles,
l’utilisateur peut plus facilement vérifier sa requête avant de la soumettre.

Quand un site propose une recherche globale :

  * celle-ci doit être intégrée dans l’en-tête (cf le composant [En-tête](/elements-d-interface/composants/en-tete) ) et accessible depuis l’ensemble des pages de votre site.
  * si elle constitue le point de départ de la navigation pour l’utilisateur, la barre de recherche LG doit être présentée comme l'élément le plus important sur la page d’accueil. 

La largeur du composant s’adapte à son contenant.

### Accessibilité

Les règles d’accessibilité sur la barre de recherche :

  * Le champ de recherche doit avoir une étiquette (visible ou non) permettant de comprendre la nature de la saisie attendue
  * Le bouton de validation de recherche doit avoir un attribut title et un libellé (éventuellement masqué avec la classe sr-only)

### Contenu

Pour le libellé du champ de saisie, utiliser un texte clair et concis qui
définit le contexte de recherche à l'utilisateur (recherche globale ?
recherche d’un type de contenu spécifiques ?…).

Pour le libellé du bouton de recherche, nous préconisons par défaut d’utiliser
le texte “Rechercher” qui est le plus clair pour l’utilisateur et respecte
l[es règles d'écriture pour le contenu des boutons](/elements-d-
interface/composants/bouton).

### Personnalisation

Le style de ce composant n’est pas personnalisable.Toutefois, certains
éléments sont optionnels - voir la structure du composant.

### Besoin d'aide ?

L'équipe du DSFR est là pour vous aider.

Retrouvez-la sur :

  * [la communauté slack](https://gouvfr.slack.com/ "la communauté slack - nouvelle fenêtre") pour poser vos questions, et échanger avec d’autres utilisateurs.   
Vous êtes **agent de l’État** et souhaitez accéder au slack ? [Rejoignez la
communauté](https://gouvfr.atlassian.net/servicedesk/customer/portal/1/group/1/create/9
"Rejoignez la communauté - nouvelle fenêtre") dès maintenant !

  * [ le centre de support](https://gouvfr.atlassian.net/servicedesk/customer/portals "le centre de support - nouvelle fenêtre") pour envoyer vos demandes de correctifs et d'évolution.

[Bandeau d'information importante - Notice 🆕](/composants-et-
modeles/composants/bandeau-d-information-importante)

[Bouton - Button](/composants-et-modeles/composants/bouton)

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
