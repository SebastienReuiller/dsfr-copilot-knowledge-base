Fermer

#  Pagination - Pagination

La pagination permet à l’utilisateur de naviguer entre les différentes pages
d’une liste d'éléments.

Lorsqu’une liste d'éléments est trop importante pour être affichée sur une
seule page (plus de 20 éléments) il est préférable de la diviser en plusieurs
pages. La pagination est un système de navigation entre ces différentes pages
et elle simplifie le parcours à l’utilisateur au sein de cette liste.

En fonction de la technologie utilisée pour votre site, la pagination peut
avoir des fonctionnements spécifiques. Afin de respecter cette contrainte nous
vous proposons uniquement un style de référence (UI et HTML/CSS), l’ensemble
des éléments permettant de s’approprier ce style ainsi qu’une liste de bonnes
pratiques à respecter.

  * Première page 
  * Page précédente 
  * 1 
  * 2 
  * 3 
  * … 
  * 130 
  * 131 
  * 132 
  * Page suivante 
  * Dernière page 

    
    
                    <nav role="navigation" class="fr-pagination" aria-label="Pagination">
        <ul class="fr-pagination__list">
            <li>
                <a class="fr-pagination__link fr-pagination__link--first" aria-disabled="true" role="link">
                    Première page
                </a>
            </li>
            <li>
                <a class="fr-pagination__link fr-pagination__link--prev fr-pagination__link--lg-label" aria-disabled="true" role="link">
                    Page précédente
                </a>
            </li>
            <li>
                <a class="fr-pagination__link" aria-current="page" title="Page 1">
                    1
                </a>
            </li>
            <li>
                <a class="fr-pagination__link" href="#" title="Page 2">
                    2
                </a>
            </li>
            <li>
                <a class="fr-pagination__link fr-displayed-lg" href="#" title="Page 3">
                    3
                </a>
            </li>
            <li>
                <a class="fr-pagination__link fr-displayed-lg">
                    …
                </a>
            </li>
            <li>
                <a class="fr-pagination__link fr-displayed-lg" href="#" title="Page 130">
                    130
                </a>
            </li>
            <li>
                <a class="fr-pagination__link fr-displayed-lg" href="#" title="Page 131">
                    131
                </a>
            </li>
            <li>
                <a class="fr-pagination__link" href="#" title="Page 132">
                    132
                </a>
            </li>
            <li>
                <a class="fr-pagination__link fr-pagination__link--next fr-pagination__link--lg-label" href="#">
                    Page suivante
                </a>
            </li>
            <li>
                <a class="fr-pagination__link fr-pagination__link--last" href="#">
                    Dernière page
                </a>
            </li>
        </ul>
    </nav>
                    
                  

L’implémentation de la pagination doit respecter les bonnes pratiques
suivantes :

  * La pagination est toujours placée en bas de liste
  * La page sur laquelle se trouve l'utilisateur doit être clairement mise en avant
  * Le dernier élément de la pagination est la dernière page de la liste. L’utilisateur connait ainsi le nombre total de pages. 
  * Le lien “précédent” doit être désactivé quand l’utilisateur est sur la première page, et la page “suivant” quand l’utilisateur est sur la dernière page.
  * Toujours donner un accès rapide à la première et dernière page lorsque celles-ci ne sont pas actives, soit avec les boutons “I<“ et “>I”, soit avec la page “1” et la dernière page. 
  * Il est recommandé de limiter à 5 ou 7 le nombre de page visibles et affichées par défaut dans la pagination. Au-delà les autres pages sont masquées par un système de troncature. La troncature est matérialisée par l’icône “…” : il ne s’affiche que quand le nombre de pages dépasse de la liste est supérieur à la limite fixée. 

  * Par défaut nous recommandons d’afficher la troncature “…” : après la 5ème page sur les grandes et moyennes résolutions
  * La double troncature apparait lorsque la page consultée est séparée par 5 pages ou plus de la première et de la dernière page sur les grandes et moyennes résolutions 

## Pagination sur mobile et tablette

  * Le fonctionnel doit rester le même entre mobile et desktop. 
  * Limiter le nombre de pages affichées pour pouvoir afficher dans l’idéal les éléments de la pagination sur une ligne.
  * Privilégier les icônes “<“ et “>” pour les actions “précédent” et “suivant” 
  * Réduire le nombre de page au niveau des règles d’affichage de la troncature afin d’afficher les éléments de la pagination sur une ligne. 

  * Première page 
  * Page précédente 
  * 1 
  * 2 
  * 3 
  * … 
  * 130 
  * 131 
  * 132 
  * Page suivante 
  * Dernière page 

## Règles d’utilisation

### Usage

  * Privilégier la pagination au lieu d’un rechargement automatique ou d’un bouton “voir plus” (pour faciliter le parcours et avantager le référencement de votre site).
  * Au clic sur une nouvelle page renvoyer l’utilisateur en haut de la page
  * Conserver le même fonctionnel entre les grandes et petites résolutions, en adaptant les règles d’affichage

### Accessibilité

Les règles d’accessibilité sur la pagination :

  * Identifiez clairement qu’il s’agit d’un élément de navigation. Exemple : <nav class=”ma classe” role=”navigation” aria-label=”Pagination”>
  * L’item actif doit être indiqué clairement dans le code. Par exemple : <li aria-current="page">5</li>
  * Utiliser un texte caché et un title sur les liens présentés sous forme d'icône ("page précédente" et "page suivante", “première page”, “dernière page”) 
  * Les liens désactivés n’ont pas d’attribut href, et possèdent les attributs aria-disabled="true" role="link"

### Personnalisation

Ce composant n’est pas personnalisable.

### Besoin d'aide ?

L'équipe du DSFR est là pour vous aider.

Retrouvez-la sur :

  * [la communauté slack](https://gouvfr.slack.com/ "la communauté slack - nouvelle fenêtre") pour poser vos questions, et échanger avec d’autres utilisateurs.   
Vous êtes **agent de l’État** et souhaitez accéder au slack ? [Rejoignez la
communauté](https://gouvfr.atlassian.net/servicedesk/customer/portal/1/group/1/create/9
"Rejoignez la communauté - nouvelle fenêtre") dès maintenant !

  * [ le centre de support](https://gouvfr.atlassian.net/servicedesk/customer/portals "le centre de support - nouvelle fenêtre") pour envoyer vos demandes de correctifs et d'évolution.

[Onglet - Tab](/composants-et-modeles/composants/onglet)

[Paramètre d'affichage - Display](/composants-et-modeles/composants/parametre-
d-affichage)

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
