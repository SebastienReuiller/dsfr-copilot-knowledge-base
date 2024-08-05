Fermer

# Onglet - Tab

Le composant onglet permet aux utilisateurs de naviguer dans différentes
sections de contenu au sein d’une même page.

Le système d'onglet aide à regrouper différents contenus dans un espace limité
et permet de diviser un contenu dense en sections accessibles individuellement
afin de faciliter la lecture pour l'utilisateur.

## Structure

Chaque onglet se compose des éléments suivants :

  * un icône à gauche du titre - optionnel.
  * un titre cliquable - obligatoire ( permet d’afficher la zone de contenu qui lui est associée). 

Si le nombre d’onglets dépasse la largeur du container, un scroll horizontal
permet de naviguer entre les différents onglets.

  * Label Tab 1
  * Label Tab 2
  * Label Tab 2

Contenu 1

Contenu 2

Contenu 3

    
    
                    <div class="fr-tabs">
        <ul class="fr-tabs__list" role="tablist" aria-label="[A modifier | nom du système d'onglet]">
            <li role="presentation">
                <button id="tabpanel-404" class="fr-tabs__tab fr-icon-checkbox-line fr-tabs__tab--icon-left" tabindex="0" role="tab" aria-selected="true" aria-controls="tabpanel-404-panel">Label Tab 1</button>
            </li>
            <li role="presentation">
                <button id="tabpanel-405" class="fr-tabs__tab fr-icon-checkbox-line fr-tabs__tab--icon-left" tabindex="-1" role="tab" aria-selected="false" aria-controls="tabpanel-405-panel">Label Tab 2</button>
            </li>
            <li role="presentation">
                <button id="tabpanel-406" class="fr-tabs__tab fr-icon-checkbox-line fr-tabs__tab--icon-left" tabindex="-1" role="tab" aria-selected="false" aria-controls="tabpanel-406-panel">Label Tab 2</button>
            </li>
        </ul>
        <div id="tabpanel-404-panel" class="fr-tabs__panel fr-tabs__panel--selected" role="tabpanel" aria-labelledby="tabpanel-404" tabindex="0">
            <!-- données de test -->
           <p>Contenu 1</p>
        </div>
        <div id="tabpanel-405-panel" class="fr-tabs__panel" role="tabpanel" aria-labelledby="tabpanel-405" tabindex="0">
            <!-- données de test -->
            <p>Contenu 2</p>
        </div>
        <div id="tabpanel-406-panel" class="fr-tabs__panel" role="tabpanel" aria-labelledby="tabpanel-406" tabindex="0">
            <!-- données de test -->
            <p>Contenu 3</p>
        </div>
    </div>
                    
                  

**Pour les designers**

Pour ajouter du contenu, vous pouvez utiliser la “zone de contenu” afin de
respecter les espacements prévus, puis la masquer en modifiant le style de
calque par “aucun”

![](/uploads/Capture_d_ecran_2020_12_15_a_19_09_59_27b6343035.png)

![](/uploads/Capture_d_ecran_2020_12_15_a_19_09_59_27b6343035.png)

**Pour les développeurs**

Il est possible de forcer le passage sur 2 lignes d’un onglet, pour éviter
d’activer le scroll automatique des onglets qui dépasse la zone de contenu
définie.

Pour cela il suffit :

  * D’ajouter un <br> dans le bouton pour forcer un passage à la ligne dans tous les cas.
  * D’ajouter le style CSS max-width: n% sur l'élément <li> contenant l'onglet (fr-tabs__tab) pour forcer le passage sur 2 lignes que lorsque l’onglet fait plus de n% de la largeur. <li style=”max-width:xx%”>

Attention lorsque vous utilisez cet ajustement, le titre de l’onglet, ne doit
jamais passer sur 3 lignes quel que soit le support utilisé.

Depuis la version 1.10, il est possible de faire un lien depuis une autre page
vers un onglet qui n'est pas le premier en mettant l'ID de l'onglet
correspondant en ancre dans l'URL tel que : #tad-id  

## Responsive

En mobile, l’onglet affiche un scroll horizontal qui permet d’accéder à
l’ensemble des onglets.

![](/uploads/Capture_d_ecran_2022_01_18_a_15_39_39_a6484550bb.png)

## Règles d’utilisation

### Usages

  * Trier les onglets en fonction des besoins des utilisateurs, en plaçant le plus important en premier.
  * Utilisez des onglets si vous avez moins de 5 sections. Si vous avez plus de 5 sections, utilisez plutôt des accordéons. 
  * Les onglets sont pertinents si le contenu peut être utilement séparé en sections clairement nommées. 
  * Ne pas utiliser les onglets si les utilisateurs ont besoin de lire le contenu de l’ensemble des sections.
  * Ne pas utiliser pour un contenu trop long où les onglets sont difficiles à retrouver après lecture..

### Accessibilité

Le composant onglet est basé sur le design pattern aria tabpanel [WAI-ARIA
Authoring Practices 1.2](https://www.w3.org/TR/wai-aria-practices/#tabpanel
"WAI-ARIA Authoring Practices 1.2 - nouvelle fenêtre") ce qui implique
l’implémentation des attributs suivants :

  * Attribut role="tablist" sur l'élément contenant les onglets.
  * Chaque onglet a un attribut role="tab"
  * Chaque panneau a les attributs role="tabpanel" et tabindex="0" 
  * Chaque onglet est associé à son panneau avec le couple d’attributs aria-controls/id
  * Chaque panneau est associé à son onglet aria-labelledby/id
  * Suivant l'état de l’onglet (sélectionné ou non), les attributs suivants changent de valeursaria-selected = true ou false tabindex = 0 ou -1
  * aria-selected = true ou false 
  * tabindex = 0 ou -1
  * Les panneaux non affichés à l’écran sont masqués avec display: none et/ou visibility: hidden

La navigation des onglets au clavier suit [ce fonctionnement
](https://www.w3.org/WAI/ARIA/apg/patterns/tabs/#keyboardinteraction "ce
fonctionnement  - nouvelle fenêtre").  

### Contenus

Utiliser des intitulés clairs et courts.

### Personnalisation

Le style de ce composant n’est pas personnalisable.Toutefois, certains
éléments sont optionnels et les icônes peuvent être changées - voir la
structure du composant.

### Besoin d'aide ?

L'équipe du DSFR est là pour vous aider.

Retrouvez-la sur :

  * [la communauté slack](https://gouvfr.slack.com/ "la communauté slack - nouvelle fenêtre") pour poser vos questions, et échanger avec d’autres utilisateurs.   
Vous êtes **agent de l’État** et souhaitez accéder au slack ? [Rejoignez la
communauté](https://gouvfr.atlassian.net/servicedesk/customer/portal/1/group/1/create/9
"Rejoignez la communauté - nouvelle fenêtre") dès maintenant !

  * [ le centre de support](https://gouvfr.atlassian.net/servicedesk/customer/portals "le centre de support - nouvelle fenêtre") pour envoyer vos demandes de correctifs et d'évolution.

[Navigation principale - Navigation](/composants-et-
modeles/composants/navigation-principale)

[Pagination - Pagination](/composants-et-modeles/composants/pagination)

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
