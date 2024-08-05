Fermer

# Lien d'évitement - Skiplink

Les liens d’évitement permettent aux utilisateurs naviguant au clavier, ou
équipés de lecteurs d'écran, d’accéder plus rapidement à des zones précises de
la page.

## Liens d'évitement par défaut

**_Toujours placé en haut de la pag_** e, le composant est masqué par défaut.
Il apparait en haut de page lorsqu’un de ses liens reçoit le focus (navigation
clavier). Une fois affichée, la zone de liens d’évitement permet de fournir
plusieurs liens pour aider les utilisateurs à naviguer rapidement vers des
fonctionnalités importantes :

  * Contenu
  * Menu
  * Recherche
  * Pied de page
  * etc

Le composant est composé de liens simples.

  * Contenu
  * Menu
  * Recherche
  * Pied de page

    
    
    <div class="fr-skiplinks">
        <nav class="fr-container" role="navigation" aria-label="Accès rapide">
            <ul class="fr-skiplinks__list">
                <li>
                    <a class="fr-link" href="#contenu">Contenu</a>
                </li>
                <li>
                    <a class="fr-link" href="#header-navigation">Menu</a>
                </li>
                <li>
                    <a class="fr-link" href="#header-search">Recherche</a>
                </li>
                <li>
                    <a class="fr-link" href="#footer">Pied de page</a>
                </li>
            </ul>
        </nav>
    </div>

### À noter

Les liens d'évitement pointent vers des ancres (#intitulé), qui doivent être
présentes dans la page.  
Par exemple, Le lien <a class="fr-link" href="#contenu">Contenu</a> ne peut
fonctionner que si un élément avec l’id “contenu” est présent dans la page
(comme <main id=”contenu”), à l’endroit souhaité.

Ils doivent figurer parmi les premiers éléments accessibles au clavier et
avoir toujours le même contenu, la même position et la même forme sur
l’ensemble du site.

![](/uploads/Capture_d_ecran_2021_03_08_a_09_25_19_142687d7f2.png)

## Règles d’utilisation

### Usages

  * L’intégration des liens d’évitement est une obligation pour l’ensemble des sites.
  * Le composant doit toujours être placé au tout début de la page.
  * Le choix des liens à afficher dépend des éléments clés présents dans le site. Le lien minimum est “Accéder au contenu”, les autres liens doivent être choisis en fonction des fonctionnalité/zone clés.
  * Pour que les liens d'évitement soient efficaces, il faut en limiter le nombre.

### Accessibilité

  * Les liens d’accès rapide doivent être entourés par une balise <nav>.
  * Les liens d’accès rapide doivent être structurés avec une liste <ul><li>.
  * Le lien d’accès au contenu devrait toujours être le premier dans la liste.

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

[Lien - Link](/composants-et-modeles/composants/lien)

[Liste déroulante - Select](/composants-et-modeles/composants/liste-
deroulante)

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
