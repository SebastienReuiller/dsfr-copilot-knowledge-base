Fermer

# Fil d'Ariane - Breadcrumb

Le fil d’Ariane est un système de navigation secondaire qui permet à
l’utilisateur de se situer sur le site qu’il consulte.

## Fil d’Ariane

Le fil d’Ariane donne des informations sur l’architecture du site. Il indique
à l’utilisateur sa position courante et lui permet de se repérer dans
l’arborescence du site. Le fil d’Ariane est présent sur l’ensemble des pages à
l’exception de la page d'accueil. Sa position dans la page doit toujours être
la même, de préférence entre le header et le contenu principal de la page.
L’ensemble de ses éléments sont cliquables, à l’exception de la page
consultée.

### Structure

Dans l’ordre, il se compose des éléments suivants :

  * un lien menant à la racine du site (page d’accueil) - obligatoire.
  * des liens vers les pages séparant la racine du site de la page courante - obligatoire si la hiérarchie du site comporte plus d’un niveau.
  * la page courante, seul élément non cliquable - obligatoire.

Voir le fil d’Ariane

  1. Accueil
  2. Segment 1
  3. Segment 2
  4. Segment 3
  5. Segment 4
  6. Segment 5
  7. Page Actuelle

    
    
                    <nav role="navigation" class="fr-breadcrumb" aria-label="vous êtes ici :">
        <button class="fr-breadcrumb__button" aria-expanded="false" aria-controls="breadcrumb-1">Voir le fil d’Ariane</button>
        <div class="fr-collapse" id="breadcrumb-1">
            <ol class="fr-breadcrumb__list">
                <li>
                    <a class="fr-breadcrumb__link" href="#/">Accueil</a>
                </li>
                <li>
                    <a class="fr-breadcrumb__link" href="#/segment-1/">Segment 1</a>
                </li>
                <li>
                    <a class="fr-breadcrumb__link" href="#/segment-1/segment-2/">Segment 2</a>
                </li>
                <li>
                    <a class="fr-breadcrumb__link" href="#/segment-1/segment-2/segment-3/">Segment 3</a>
                </li>
                <li>
                    <a class="fr-breadcrumb__link" href="#/segment-1/segment-2/segment-3/segment-4/">Segment 4</a>
                </li>
                <li>
                    <a class="fr-breadcrumb__link" href="#/segment-1/segment-2/segment-3/segment-4/segment-5/">Segment 5</a>
                </li>
                <li>
                    <a class="fr-breadcrumb__link" aria-current="page">Page Actuelle</a>
                </li>
            </ol>
        </div>
    </nav>
                    
                  

## Responsive

Le fil d’Ariane doit être maintenu sur mobile et apparaître de la manière
suivante :

  * Afficher par défaut un bouton “Voir le fil d’Ariane”
  * Au clic, le fil d’Ariane apparaît, sur plusieurs lignes

Voir le fil d’Ariane

  1. Accueil
  2. Segment 1
  3. Segment 2
  4. Segment 3
  5. Titre de page très très très long...

## Règles d’utilisation

### Usage

**Moyen de navigation secondaire**

Le fil d'Ariane est fortement recommandé sur l’ensemble des sites,
particulièrement lorsque l’arborescence possède plus de 2 niveaux: il permet à
l’utilisateur de revenir à une page de niveau supérieur en l’utilisant à la
place du bouton «Retour» du navigateur ou de [la navigation
principale.](/elements-d-interface/composants/navigation-principale)

**Longueur et lisibilité**

Afin qu’il reste lisible, évitez que le fil d’Ariane soit trop long et passe
sur plusieurs lignes. Si les titres de page de votre site sont longs, nous
conseillons de n’afficher que les 4 premiers mots du nom de la page courante
et d’indiquer que l’élément est tronqué par l’affichage de “…”

Voir le fil d’Ariane

  1. Accueil
  2. Segment 1
  3. Segment 2
  4. Segment 3
  5. Titre de page très très très long...

Chemin du fil d’Ariane

Si plusieurs chemins sont possibles pour une page, le fil d’Ariane doit en
présenter un seul afin de conserver une hiérarchie cohérente entre les pages.
Mettez en place un fil d'Ariane basé sur la position courant dans la
hiérarchie principale du site web et non sur l'historique de navigation de
l’utilisateur, ce qui est susceptible de créer de la confusion pour
l’utilisateur.

Couleur de fond

Le fil d’Ariane ne peut être utilisé que sur les couleurs de fond de page
autorisée et définies dans la documentation
[couleur](https://gouvfr.atlassian.net/wiki/spaces/DB/pages/217186370).

Le fil d’Ariane ne doit jamais être superposé sur une image.

### Accessibilité

  * La page courante doit être clairement indiquée dans le code. Elle ne doit pas être dans un lien et sa balise doit avoir un attribut aria-current : aria-current="page” 
  * Le fil d’Ariane doit être placé dans un élément nav : <nav role="navigation" aria-label="Vous êtes ici">

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

[En-tête - Header](/composants-et-modeles/composants/en-tete)

[Gestionnaire de consentement - Consent banner](/composants-et-
modeles/composants/gestionnaire-de-consentement)

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
