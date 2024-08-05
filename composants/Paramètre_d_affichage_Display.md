Fermer

# Paramètre d'affichage - Display

Le parcours “Paramètres d’affichage” permet à l’utilisateur de choisir
d'afficher le site en thème clair ou en thème sombre (pour en savoir plus sur
ces deux thèmes, consultez [la page Couleurs](https://www.systeme-de-
design.gouv.fr/elements-d-interface/fondamentaux-de-l-identite-de-l-
etat/couleurs-palette)).

## Paramètres d’affichage

Le parcours “Paramètres d’affichage” peut s’intégrer dans l’en-tête ou le pied
de page de votre site.

### Structure

Le parcours se compose des éléments suivants :

  1. d’un attribut sur la balise html - obligatoire.
  2. d’un lien pouvant s’intégrer dans l’en-tête ou le pied de page de votre site - obligatoire.
  3. d’une modale comportant un titre, un texte de description, et deux boutons radios riches - obligatoire.

### 1\. Activation de la gestion du thème

Afin d’activer la gestion du thème, il est nécessaire d’ajouter l’attribut
data-fr-scheme sur la balise html.

  * Si l’attribut n’est pas présent, le site s’affichera en mode clair (thème par défaut).
  * Si l’attribut est présent, le site affichera le thème adapté selon les règles suivantes: data-fr-theme=”system” (par défaut) : les préférences par défaut du navigateur/os sont prises en compte (en se basant sur la média query prefers-color-scheme)

    
    
    <html lang="fr" data-fr-scheme="system">

  * data-fr-theme=”light” : le site s’affiche en thème clair.

    
    
    <html lang="fr" data-fr-scheme="light">

  * data-fr-theme=”dark” : le site s’affiche en thème sombre.   

    
    
    <html lang="fr" data-fr-scheme="dark"> 

  * Si l’utilisateur effectue une modification, son choix est conservé (dans le local storage) pour les visites ultérieures. 

#### À noter

L’attribut data-fr-theme n’est plus utilisable directement , il faut utiliser
data-fr-scheme à la place

### 2\. Le lien

**Intégré dans l’en-tête du site**

Lorsque le lien paramètres d’affichage est mis en avant dans l’en-tête de la
page, il prend la forme d’un lien accès rapide. (voir le snippet de l'en-tête
avec accès rapide)

###  Extrait de code

    
    
    <!-- bouton à insérer dans le bloc tools-links du header -->
    <div class="fr-header__tools-links">
        <ul class="fr-btns-group">
            <li>
                <button class="fr-btn fr-icon-theme-fill" aria-controls="fr-theme-modal" data-fr-opened="false">Paramètres d'affichage</button>
            </li>
        </ul>
    </div>

**Intégré dans le pied de page**

Lorsque le lien paramètres d’affichage est mis en avant dans le pied de page,
il est intégré au niveau des mentions légales (voir le snippet du footer)

* Paramètres d'affichage

###  Extrait de code

    
    
                          <!-- bouton à insérer dans le bloc bottom list du footer -->
    
    <li class="fr-footer__bottom-item">
      <button class="fr-footer__bottom-link fr-icon-theme-fill fr-btn--icon-left" aria-controls="fr-theme-modal" data-fr-opened="false">Paramètres d'affichage</button>
    </li>
    
                          
                        

### 3\. La modale

Une fois la modale affichée, la modification du thème s’effectue immédiatement
lorsque l’utilisateur effectue son choix.

### Attention

Bien adapter le chemin des images de pictogrammes illustratifs à votre
architecture de site !

    
    
    <dialog id="fr-theme-modal" class="fr-modal" role="dialog" aria-labelledby="fr-theme-modal-title">
        <div class="fr-container fr-container--fluid fr-container-md">
            <div class="fr-grid-row fr-grid-row--center">
                <div class="fr-col-12 fr-col-md-6 fr-col-lg-4">
                    <div class="fr-modal__body">
                        <div class="fr-modal__header">
                            <button class="fr-btn--close fr-btn" aria-controls="fr-theme-modal" id="button-5622" title="Fermer">
                                Fermer
                            </button>
                        </div>
                        <div class="fr-modal__content">
                            <h1 id="fr-theme-modal-title" class="fr-modal__title">
                                Paramètres d’affichage
                            </h1>
                            <div id="fr-display" class="fr-display">
                                <fieldset class="fr-fieldset" id="display-fieldset">
                                    <legend class="fr-fieldset__legend--regular fr-fieldset__legend" id="display-fieldset-legend">
                                        Choisissez un thème pour personnaliser l’apparence du site.
                                    </legend>
                                    <div class="fr-fieldset__element">
                                        <div class="fr-radio-group fr-radio-rich">
                                            <input value="light" type="radio" id="fr-radios-theme-light" name="fr-radios-theme">
                                            <label class="fr-label" for="fr-radios-theme-light">
                                                Thème clair
                                            </label>
                                            <div class="fr-radio-rich__img">
                                                <svg aria-hidden="true" class="fr-artwork" viewBox="0 0 80 80" width="80px" height="80px">
                                                    <use class="fr-artwork-decorative" href="/img/artwork/pictograms/environment/sun.svg#artwork-decorative"></use>
                                                    <use class="fr-artwork-minor" href="/img/artwork/pictograms/environment/sun.svg#artwork-minor"></use>
                                                    <use class="fr-artwork-major" href="/img/artwork/pictograms/environment/sun.svg#artwork-major"></use>
                                                </svg>
                                            </div>
                                        </div>
                                    </div>
                                    <div class="fr-fieldset__element">
                                        <div class="fr-radio-group fr-radio-rich">
                                            <input value="dark" type="radio" id="fr-radios-theme-dark" name="fr-radios-theme">
                                            <label class="fr-label" for="fr-radios-theme-dark">
                                                Thème sombre
                                            </label>
                                            <div class="fr-radio-rich__img">
                                                <svg aria-hidden="true" class="fr-artwork" viewBox="0 0 80 80" width="80px" height="80px">
                                                    <use class="fr-artwork-decorative" href="/img/artwork/pictograms/environment/moon.svg#artwork-decorative"></use>
                                                    <use class="fr-artwork-minor" href="/img/artwork/pictograms/environment/moon.svg#artwork-minor"></use>
                                                    <use class="fr-artwork-major" href="/img/artwork/pictograms/environment/moon.svg#artwork-major"></use>
                                                </svg>
                                            </div>
                                        </div>
                                    </div>
                                    <div class="fr-fieldset__element">
                                        <div class="fr-radio-group fr-radio-rich">
                                            <input value="system" type="radio" id="fr-radios-theme-system" name="fr-radios-theme">
                                            <label class="fr-label" for="fr-radios-theme-system">
                                                Système
                                                <span class="fr-hint-text">Utilise les paramètres système</span>
                                            </label>
                                            <div class="fr-radio-rich__img">
                                                <svg aria-hidden="true" class="fr-artwork" viewBox="0 0 80 80" width="80px" height="80px">
                                                    <use class="fr-artwork-decorative" href="/img/artwork/pictograms/system/system.svg#artwork-decorative"></use>
                                                    <use class="fr-artwork-minor" href="/img/artwork/pictograms/system/system.svg#artwork-minor"></use>
                                                    <use class="fr-artwork-major" href="/img/artwork/pictograms/system/system.svg#artwork-major"></use>
                                                </svg>
                                            </div>
                                        </div>
                                    </div>
                                </fieldset>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </dialog>

### Responsive

En version mobile, les éléments du parcours paramètres d’affichage se
réorganisent automatiquement afin d’afficher les versions mobiles des
composants :

  * En-tête avec accès rapide
  * Modale

#### Le lien

**Intégré dans l’en-tête du site**

Comme dans la version mobile du header, l’accès rapide au lien “paramètres
d’affichage” se trouve dans le menu mobile.

![](/uploads/Capture_d_ecran_2021_03_23_a_17_46_13_336ec0652b.png)

![](/uploads/Capture_d_ecran_2021_04_06_a_22_04_10_e10ad2b3f5.png)

**Intégré dans le footer du site**

![](/uploads/Capture_d_ecran_2021_04_06_a_22_07_50_058982cd40.png)

#### La modale

![](/uploads/Capture_d_ecran_2021_11_15_a_15_51_32_8eae1e3fc2.png)

### Règles d’utilisation

### Usage

La fermeture de la modale permet à l’utilisateur de reprendre sa navigation à
l’endroit où il se trouvait auparavant dans la page.

Lorsque la modale de paramètre est ouverte, la page en arrière plan se fige,
il devient alors impossible de scroller le contenu d’arrière plan avant de
l’avoir clôturée.

### Accessibilité

Pour ce parcours veillez à respecter les règles d’accessibilité des composants
:

  * Modale
  * Boutons radio riches

### Personnalisation

Il est possible de personnaliser le texte de description de la modale
Paramètres d’affichage.

### Besoin d'aide ?

L'équipe du DSFR est là pour vous aider.

Retrouvez-la sur :

  * [la communauté slack](https://gouvfr.slack.com/ "la communauté slack - nouvelle fenêtre") pour poser vos questions, et échanger avec d’autres utilisateurs.   
Vous êtes **agent de l’État** et souhaitez accéder au slack ? [Rejoignez la
communauté](https://gouvfr.atlassian.net/servicedesk/customer/portal/1/group/1/create/9
"Rejoignez la communauté - nouvelle fenêtre") dès maintenant !

  * [ le centre de support](https://gouvfr.atlassian.net/servicedesk/customer/portals "le centre de support - nouvelle fenêtre") pour envoyer vos demandes de correctifs et d'évolution.

[Pagination - Pagination](/composants-et-modeles/composants/pagination)

[Partage - Share](/composants-et-modeles/composants/partage)

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
