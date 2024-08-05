Fermer

# Modale - Modal

La modale permet de concentrer l’attention de l’utilisateur exclusivement sur
une tâche ou un élément d’information, sans perdre le contexte de la page en
cours. Ce composant nécessite une action de l’utilisateur afin d'être ouvert
ou fermé.

## Modale simple

La modale par défaut permet de mettre en évidence une information qui ne
nécessite pas d’action de l’utilisateur. Elle s’affiche à la suite du clic sur
un bouton.

Elle se compose des éléments suivants :

  * Le bouton Fermer, obligatoire.
  * Le titre obligatoire, avec icône, optionnelle.
  * La zone de contenu, obligatoire.  

  * Un overlay disposé à l’arrière du composant, obligatoire.  

La modale doit être placée en dehors du contenu (en dehors du main), à la fin
de la page.  
  
A partir du point de rupture MD ce composant s’affiche au centre de la page.
([Consultez la documentation Grille, pour découvrir les points de rupture.
](/elements-d-interface/fondamentaux-techniques/grille-et-points-de-rupture))

Titre de modale simple

Fermer

# Titre de la modale

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Maecenas varius
tortor nibh, sit amet tempor nibh finibus et. Aenean eu enim justo. Vestibulum
aliquam hendrerit molestie. Mauris malesuada nisi sit amet augue accumsan
tincidunt. Maecenas tincidunt, velit ac porttitor pulvinar, tortor eros
facilisis libero, vitae commodo nunc quam et ligula. Ut nec ipsum sapien.
Interdum et malesuada fames ac ante ipsum primis in faucibus. Integer id nisi
nec nulla luctus lacinia non eu turpis. Etiam in ex imperdiet justo tincidunt
egestas. Ut porttitor urna ac augue cursus tincidunt sit amet sed orci.

###  Extrait de code

    
    
                          <!--Bouton d'ouverture de la modale-->
    
    <button class="fr-btn"  data-fr-opened="false" aria-controls="fr-modal-1">
        Titre de modale simple
    </button>
    
    <!-- Modale Simple
         La balise <dialog> peut être placée n'importe où sur la page, toutefois 
         nous vous conseillons, si vous en avez la possibilité, 
         d'en faire un enfant direct de la balise <body> 
    -->
    
    <dialog aria-labelledby="fr-modal-title-modal-1" role="dialog" id="fr-modal-1" class="fr-modal">
        <div class="fr-container fr-container--fluid fr-container-md">
            <div class="fr-grid-row fr-grid-row--center">
                <div class="fr-col-12 fr-col-md-8 fr-col-lg-6">
                    <div class="fr-modal__body">
                        <div class="fr-modal__header">
                            <button class="fr-btn--close fr-btn" title="Fermer la fenêtre modale" aria-controls="fr-modal-1">Fermer</button>
                        </div>
                        <div class="fr-modal__content">
                            <h1 id="fr-modal-title-modal-1" class="fr-modal__title"><span class="fr-icon-arrow-right-line fr-icon--lg"></span>Titre de la modale</h1>
                            <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Maecenas varius tortor nibh, sit amet tempor nibh finibus et. Aenean eu enim justo. Vestibulum aliquam hendrerit molestie. Mauris malesuada nisi sit amet augue accumsan tincidunt. Maecenas tincidunt, velit ac porttitor pulvinar, tortor eros facilisis libero, vitae commodo nunc quam et ligula. Ut nec ipsum sapien. Interdum et malesuada fames ac ante ipsum primis in faucibus. Integer id nisi nec nulla luctus lacinia non eu turpis. Etiam in ex imperdiet justo tincidunt egestas. Ut porttitor urna ac augue cursus tincidunt sit amet sed orci.</p>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </dialog>
                          
                        

## Modale avec zone d’action

La modale avec une zone d’action permet de guider l’utilisateur vers des
actions attendues. Par défaut elle reprend les éléments de la modale simple
auxquels s’ajoute une zone d’action obligatoire, composée soit d’un bouton
primaire, soit d’un [groupe de boutons hiérarchisé](../composants/groupe-de-
boutons).

A noter : Pour les contenus trop longs pour s’afficher dans la surface prévue
par la modale, un scroll permet de faire défiler l’intégralité de
l'information.

Modale avec zone d'action

Fermer

#  Titre de la modale

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Maecenas varius
tortor nibh, sit amet tempor nibh finibus et. Aenean eu enim justo. Vestibulum
aliquam hendrerit molestie. Mauris malesuada nisi sit amet augue accumsan
tincidunt. Maecenas tincidunt, velit ac porttitor pulvinar, tortor eros
facilisis libero, vitae commodo nunc quam et ligula. Ut nec ipsum sapien.
Interdum et malesuada fames ac ante ipsum primis in faucibus. Integer id nisi
nec nulla luctus lacinia non eu turpis. Etiam in ex imperdiet justo tincidunt
egestas. Ut porttitor urna ac augue cursus tincidunt sit amet sed orci.

Label bouton  Label bouton

###  Extrait de code

    
    
                          <!-- Bouton d'ouverture de la modale -->
    
    <button class="fr-btn" data-fr-opened="false" aria-controls="fr-modal-2">
        Modale avec zone d'action
    </button>
    
    <!-- Modale avec zone d'action 
         La balise <dialog> peut être placée n'importe où sur la page, toutefois 
         nous vous conseillons, si vous en avez la possibilité, 
         d'en faire un enfant direct de la balise <body> 
    -->
    
    <dialog aria-labelledby="fr-modal-2-title" id="fr-modal-2" class="fr-modal" role="dialog" >
        <div class="fr-container fr-container--fluid fr-container-md">
            <div class="fr-grid-row fr-grid-row--center">
                <div class="fr-col-12 fr-col-md-8 fr-col-lg-6">
                    <div class="fr-modal__body">
                        <div class="fr-modal__header">
                            <button class="fr-btn--close fr-btn" aria-controls="fr-modal-2">Fermer</button>
                        </div>
                        <div class="fr-modal__content">
                            <h1 id="fr-modal-2-title" class="fr-modal__title">
                                <span class="fr-icon-arrow-right-line fr-icon--lg"></span>
                                Titre de la modale
                            </h1>
                            <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Maecenas varius tortor nibh, sit amet tempor nibh finibus et. Aenean eu enim justo. Vestibulum aliquam hendrerit molestie. Mauris malesuada nisi sit amet augue accumsan tincidunt. Maecenas tincidunt, velit ac porttitor pulvinar, tortor eros facilisis libero, vitae commodo nunc quam et ligula. Ut nec ipsum sapien. Interdum et malesuada fames ac ante ipsum primis in faucibus. Integer id nisi nec nulla luctus lacinia non eu turpis. Etiam in ex imperdiet justo tincidunt egestas. Ut porttitor urna ac augue cursus tincidunt sit amet sed orci.</p>
                        </div>
                        <div class="fr-modal__footer">
                            <div class="fr-btns-group fr-btns-group--right fr-btns-group--inline-reverse fr-btns-group--inline-lg fr-btns-group--icon-left">
                                <button class="fr-btn fr-icon-checkbox-circle-line fr-btn--icon-left">
                                    Label bouton
                                </button>
                                <button class="fr-btn fr-icon-checkbox-circle-line fr-btn--icon-left fr-btn--secondary">
                                    Label bouton
                                </button>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </dialog>
     
                          
                        

## Tailles

La modale est disponible en trois tailles afin d’adapter sa largeur au volume
de votre contenu.

  * SM pour Small, MD pour Medium, LG pour large
  * La taille medium (MD) est la taille de modale par défaut

![](/uploads/Capture_d_ecran_2021_02_02_a_18_27_20_0aa7faee64.png)

La hauteur maximum des modales est fixée à 80% de la hauteur de l'écran en
desktop.

Si le contenu est plus long que la hauteur maximale, la barre de scroll du
navigateur s’affiche à l’intérieur de la modale afin de pouvoir faire défiler
le contenu.

La largeur de la modale est gérée via la grille. La modale LG utilise la
classe `.fr-col-md-8` .La modale SM utilise la classe `.fr-col-md-4` .

Modale SM avec zone d'action

Fermer

# Titre de la modale SM

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Maecenas varius
tortor nibh, sit amet tempor nibh finibus et. Aenean eu enim justo. Vestibulum
aliquam hendrerit molestie. Mauris malesuada nisi sit amet augue accumsan
tincidunt. Maecenas tincidunt, velit ac porttitor pulvinar, tortor eros
facilisis libero, vitae commodo nunc quam et ligula. Ut nec ipsum sapien.
Interdum et malesuada fames ac ante ipsum primis in faucibus. Integer id nisi
nec nulla luctus lacinia non eu turpis. Etiam in ex imperdiet justo tincidunt
egestas. Ut porttitor urna ac augue cursus tincidunt sit amet sed orci.

###  Extrait de code

    
    
                          <!-- Modale SM -->
    <button class="fr-btn"  data-fr-opened="false" aria-controls="fr-modal-3">
        Modale SM avec zone d'action
    </button>
    <dialog aria-labelledby="fr-modal-title-modal-3" role="dialog" id="fr-modal-3" class="fr-modal">
        <div class="fr-container fr-container--fluid fr-container-md">
            <div class="fr-grid-row fr-grid-row--center">
                <div class="fr-col-12 fr-col-md-4">
                    <div class="fr-modal__body">
                        <div class="fr-modal__header">
                            <button class="fr-btn--close fr-btn" title="Fermer la fenêtre modale" aria-controls="fr-modal-3">Fermer</button>
                        </div>
                        <div class="fr-modal__content">
                            <h1 id="fr-modal-title-modal-3" class="fr-modal__title"><span class="fr-icon-arrow-right-line fr-icon--lg"></span>Titre de la modale SM</h1>
                            <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Maecenas varius tortor nibh, sit amet tempor nibh finibus et. Aenean eu enim justo. Vestibulum aliquam hendrerit molestie. Mauris malesuada nisi sit amet augue accumsan tincidunt. Maecenas tincidunt, velit ac porttitor pulvinar, tortor eros facilisis libero, vitae commodo nunc quam et ligula. Ut nec ipsum sapien. Interdum et malesuada fames ac ante ipsum primis in faucibus. Integer id nisi nec nulla luctus lacinia non eu turpis. Etiam in ex imperdiet justo tincidunt egestas. Ut porttitor urna ac augue cursus tincidunt sit amet sed orci.</p>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </dialog>
                          
                        

Modale LG avec zone d'action

Fermer

# Titre de la modale

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Maecenas varius
tortor nibh, sit amet tempor nibh finibus et. Aenean eu enim justo. Vestibulum
aliquam hendrerit molestie. Mauris malesuada nisi sit amet augue accumsan
tincidunt. Maecenas tincidunt, velit ac porttitor pulvinar, tortor eros
facilisis libero, vitae commodo nunc quam et ligula. Ut nec ipsum sapien.
Interdum et malesuada fames ac ante ipsum primis in faucibus. Integer id nisi
nec nulla luctus lacinia non eu turpis. Etiam in ex imperdiet justo tincidunt
egestas. Ut porttitor urna ac augue cursus tincidunt sit amet sed orci.

###  Extrait de code

    
    
                          <!-- Modale LG -->
    <button class="fr-btn"  data-fr-opened="false" aria-controls="fr-modal-4" title="Modal LG (ouvre une fenêtre modale)">
        Modale LG avec zone d'action
    </button>
    <dialog aria-labelledby="fr-modal-title-modal-4" role="dialog" id="fr-modal-4" class="fr-modal">
        <div class="fr-container fr-container--fluid fr-container-md">
            <div class="fr-grid-row fr-grid-row--center">
                <div class="fr-col-12 fr-col-md-8">
                    <div class="fr-modal__body">
                        <div class="fr-modal__header">
                            <button class="fr-btn--close fr-btn" title="Fermer la fenêtre modale" aria-controls="fr-modal-4" target="_self">Fermer</button>
                        </div>
                        <div class="fr-modal__content">
                            <h1 id="fr-modal-title-modal-4" class="fr-modal__title"><span class="fr-icon-arrow-right-line fr-icon--lg"></span>Titre de la modale</h1>
                            <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Maecenas varius tortor nibh, sit amet tempor nibh finibus et. Aenean eu enim justo. Vestibulum aliquam hendrerit molestie. Mauris malesuada nisi sit amet augue accumsan tincidunt. Maecenas tincidunt, velit ac porttitor pulvinar, tortor eros facilisis libero, vitae commodo nunc quam et ligula. Ut nec ipsum sapien. Interdum et malesuada fames ac ante ipsum primis in faucibus. Integer id nisi nec nulla luctus lacinia non eu turpis. Etiam in ex imperdiet justo tincidunt egestas. Ut porttitor urna ac augue cursus tincidunt sit amet sed orci.</p>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </dialog>
                          
                        

## Responsive

En mobile la modale s’affiche sur la quasi totalité de l'écran : 100% - 4W de
marge laissée en haut de l'écran.

**Cas d’une modale simple**

![](/uploads/test_modale_simple_4_a7eaef18f6.jpg)

**Cas d’une modale avec zone d’action**

![](/uploads/modale_action_48c52c339e.jpg)

## Règles d’utilisation

### Usages

  * Utilisez les modales pour afficher des informations importantes. Attention toutefois à les utiliser avec parcimonie car elles sont invasives.
  * La fermeture de la modale doit permettre à l’utilisateur de reprendre sa navigation à l’endroit où il se trouvait auparavant dans la page.  

  * Lorsqu’une modale est ouverte, la page en arrière plan se fige, il devient alors impossible de scroller le contenu d’arrière plan avant de l’avoir clôturée.
  * Limitez le nombre d'interactions dans une modale.
  * Exemples de cas d’usage de modale : gestionnaire de consentement, paramètre d’affichage, formulaire simple, demande d’un choix à l’utilisateur, affichage d’un média, ou tout autre contenu qui pourrait faire l’objet d’une page dédiée.
  * S’il s’agit d’un complément de contenu (ex: en savoir plus), il est préférable d’utiliser un accordéon.   
  

### Hiérarchie de l'information

  * La modale doit être utilisée pour afficher un contenu à part, elle doit être placée en dehors du contenu (main), à la fin de la page. La dialog doit être enfant du body : nous ne pouvons pas garantir le bon fonctionnement si elle est placée à un autre niveau dans le dom.
  *  **Privilégiez le niveau d’entête <h1> pour le titre de la modale **: nous avons fait le choix d’utiliser <h1> car nous préconisons l’utilisation de modale uniquement dans le cas d’ouverture d’un contenu annexe, qui pourrait-être une page à part. Mais le niveau d’entête du titre des modales est un sujet qui fait débat (voir ci-dessous)  

  * Les <dialog> sont considérés comme des sectioning root, permettant techniquement le reset du niveau d’entête (néanmoins le document outline algorithm n’a jamais vraiment été implémenté par les navigateurs et lecteurs d'écran).   

  * Il est possible dans certains cas d’utiliser un niveau d’entête correspondant au niveau d’entête courant dans le DOM (notamment <h2>). 
  * Voici quelques ressources sur lesquelles s’appuyer :   

Github - DialogTitle should use h1 instead of h2 (en anglais)

UX StackExchange - Heading levels in an accessible modal window (en anglais)

Stackoverflow - Is it semantically correct to use H1 in a dialog? (en anglais)

Medium - Which heading level should dialog modals have (en anglais)

### Accessibilité

  * Pour fermer la modale l’utilisateur peut cliquer sur le bouton fermer, à l’extérieur de la modale ou appuyer sur la touche “escape” du clavier. 
  * Lors de la navigation clavier, le focus ne doit pas sortir de la modale. Cette dernière doit être fermée afin de reprendre la navigation dans la page courante (Le focus se place sur le bouton d’ouverture de la modale). À cet effet, le focus est repositionné sur le bouton qui a permis d'ouvrir la modale.
  * La balise dialog et son titre sont relié par les attributs aria-labelledby et id .

### Contenus

  * Tout type de contenu est autorisé dans la modale. Il est toutefois conseillé d’y limiter nombre d'interactions et d'éviter de présenter des décisions complexes qui nécessitent des sources d'informations supplémentaires non disponibles.
  * Lorsqu’une modale intègre des éléments de formulaire requis non renseignés, un message d’erreur s’affiche au niveau du ‘chapô' pour le signaler.

### Personnalisation

Ce composant n’est pas personnalisable. Toutefois, certains éléments sont
optionnels et les icônes peuvent être changées.

### Besoin d'aide ?

L'équipe du DSFR est là pour vous aider.

Retrouvez-la sur :

  * [la communauté slack](https://gouvfr.slack.com/ "la communauté slack - nouvelle fenêtre") pour poser vos questions, et échanger avec d’autres utilisateurs.   
Vous êtes **agent de l’État** et souhaitez accéder au slack ? [Rejoignez la
communauté](https://gouvfr.atlassian.net/servicedesk/customer/portal/1/group/1/create/9
"Rejoignez la communauté - nouvelle fenêtre") dès maintenant !

  * [ le centre de support](https://gouvfr.atlassian.net/servicedesk/customer/portals "le centre de support - nouvelle fenêtre") pour envoyer vos demandes de correctifs et d'évolution.

[Mise en exergue - Highlight](/composants-et-modeles/composants/mise-en-
exergue)

[Mot de passe - Password](/composants-et-modeles/composants/mot-de-passe)

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
