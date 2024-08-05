Fermer

# Sélecteur de langue - Translate

Le sélecteur de langue permet à l’utilisateur de choisir la langue dans
laquelle est affichée le contenu du site, si celui-ci est disponible en
plusieurs langues.

Il prend la forme d’un bouton déclenchant l’ouverture d’une liste déroulante,
présent dans l’en-tête dans le groupe des accès rapides.

## Structure

Le composant comprend les éléments suivants :

  * un bouton tertiaire d’ouverture - obligatoire
  * une icône “langue” - obligatoire
  * la langue active - obligatoire
  * une liste déroulante des autres langues - obligatoire
  * un cadre sur le bouton - optionnel.

![](/uploads/Capture_d_ecran_2022_07_25_a_00_04_01_fbe60d1f97.png)

![](/uploads/Capture_d_ecran_2022_07_25_a_00_03_41_229117642f.png)

    
    
    <nav role="navigation" class="fr-translate fr-nav">
        <div class="fr-nav__item">
            <button class="fr-translate__btn fr-btn fr-btn--tertiary" aria-controls="translate-1177" aria-expanded="false" title="Sélectionner une langue">
                FR<span class="fr-hidden-lg"> - Français</span>
            </button>
            <div class="fr-collapse fr-translate__menu fr-menu" id="translate-1177">
                <ul class="fr-menu__list">
                    <li>
                        <a class="fr-translate__language fr-nav__link" hreflang="fr" lang="fr" href="#" aria-current="true">FR - Français</a>
                    </li>
                    <li>
                        <a class="fr-translate__language fr-nav__link" hreflang="en" lang="en" href="#">EN - English</a>
                    </li>
                    <li>
                        <a class="fr-translate__language fr-nav__link" hreflang="es" lang="es" href="#">ES - Español</a>
                    </li>
                    <li>
                        <a class="fr-translate__language fr-nav__link" hreflang="de" lang="de" href="#">DE - Deutsch</a>
                    </li>
                </ul>
            </div>
        </div>
    </nav>

### Intégration du sélecteur de langue dans l’en-tête de la page (header)

![](/uploads/Capture_d_ecran_2022_07_21_a_12_58_47_c30bebc3c4.png)

###  Extrait de code

    
    
     <header role="banner" class="fr-header">
        <div class="fr-header__body">
            <div class="fr-container">
                <div class="fr-header__body-row">
                    <div class="fr-header__brand fr-enlarge-link">
                        <div class="fr-header__brand-top">
                            <div class="fr-header__logo">
                                <p class="fr-logo">
                                    Intitulé
                                    <br>officiel
                                </p>
                            </div>
                            <div class="fr-header__navbar">
                                <button class="fr-btn--menu fr-btn" data-fr-opened="false" aria-controls="modal-517" aria-haspopup="menu" id="button-518" title="Menu">
                                    Menu
                                </button>
                            </div>
                        </div>
                        <div class="fr-header__service">
                            <a href="/" title="Accueil - [À MODIFIER - Nom du site / service] - Nom de l’entité (ministère, secrétariat d‘état, gouvernement)">
                                <p class="fr-header__service-title">
                                    Nom du site / service
                                </p>
                            </a>
                            <p class="fr-header__service-tagline">baseline - précisions sur l‘organisation</p>
                        </div>
                    </div>
                    <div class="fr-header__tools">
                        <div class="fr-header__tools-links">
                            <ul class="fr-btns-group">
                                <li>
                                    <a class="fr-btn fr-icon-add-circle-line" href="[url - à modifier]">
                                        Créer un espace
                                    </a>
                                </li>
                                <li>
                                    <a class="fr-btn fr-icon-lock-line" href="[url - à modifier]">
                                        Se connecter
                                    </a>
                                </li>
                                <li>
                                    <a class="fr-btn fr-icon-account-line" href="[url - à modifier]">
                                        S’enregistrer
                                    </a>
                                </li>
                            </ul>
                            <nav role="navigation" class="fr-translate fr-nav">
                                <div class="fr-nav__item">
                                    <button class="fr-translate__btn fr-btn fr-btn--tertiary" aria-controls="translate-516" aria-expanded="false" title="Sélectionner une langue">
                                        FR<span class="fr-hidden-lg"> - Français</span>
                                    </button>
                                    <div class="fr-collapse fr-translate__menu fr-menu" id="translate-516">
                                        <ul class="fr-menu__list">
                                            <li>
                                                <a class="fr-translate__language fr-nav__link" hreflang="fr" lang="fr" href="#" aria-current="true">FR - Français</a>
                                            </li>
                                            <li>
                                                <a class="fr-translate__language fr-nav__link" hreflang="en" lang="en" href="#">EN - English</a>
                                            </li>
                                            <li>
                                                <a class="fr-translate__language fr-nav__link" hreflang="es" lang="es" href="#">ES - Español</a>
                                            </li>
                                            <li>
                                                <a class="fr-translate__language fr-nav__link" hreflang="de" lang="de" href="#">DE - Deutsch</a>
                                            </li>
                                            <li>
                                                <a class="fr-translate__language fr-nav__link" hreflang="tr" lang="tr" href="#">TR - Türkçe</a>
                                            </li>
                                            <li>
                                                <a class="fr-translate__language fr-nav__link" hreflang="ro" lang="ro" href="#">RO - Română</a>
                                            </li>
                                        </ul>
                                    </div>
                                </div>
                            </nav>
                        </div>
                    </div>	
                </div>
            </div>
        </div>
        <div class="fr-header__menu fr-modal" id="modal-517" aria-labelledby="button-518">
            <div class="fr-container">
                <button class="fr-btn--close fr-btn" aria-controls="modal-517" title="Fermer">
                    Fermer
                </button>
                <div class="fr-header__menu-links">
                </div>
    			<nav class="fr-nav" id="navigation-498" role="navigation" aria-label="Menu principal">
    				<ul class="fr-nav__list">
    				    <li class="fr-nav__item">
    				        <a class="fr-nav__link" href="#" target="_self">accès direct</a>
    				    </li>
    				    <li class="fr-nav__item">
    				        <a class="fr-nav__link" href="#" target="_self">accès direct</a>
    				    </li>
    				</ul>
    			</nav>
            </div>
        </div>
    </header>

## Règles d’utilisation

### Usages

Le sélecteur de langue doit être présent sur un site à partir du moment où
celui-ci est disponible en trois langues (en général, il s’agira du français
et deux autres langues).

### Important

Il serait techniquement possible d’utiliser le sélecteur de langue pour un
site en deux langues. Cependant, en vertu de[ la loi n° 94-665 du 4 août 1994
relative à l'emploi de la langue
française](https://www.legifrance.gouv.fr/loda/id/JORFTEXT000000349929/2022-06-17/),
et conformément à [la politique gouvernementale constante en faveur du
plurilinguisme](https://www.legifrance.gouv.fr/jorf/id/JORFTEXT000000411109),
nous recommandons fortement de proposer une traduction en deux langues au
moins.

Il n’y a pas de nombre maximum de langues, mais les symboles dans les
librairies ne prévoient que jusqu'à huit langues.

Le sélecteur de langue prend la place d’un accès rapide, et ne s’ajoute pas à
ceux-ci. Quand il est présent, il est forcément sur l’accès rapide le plus à
droite (le dernier en mobile), à part quand un bouton tertiaire encadré y est
déjà présent (par exemple : Connexion).

### Contenus

  * Le bouton affiche la langue active, une liste déroulante propose les langues disponibles.
  * Une langue est indiquée par [son code ISO](https://fr.wikipedia.org/wiki/Liste_des_codes_ISO_639-1 "son code ISO - nouvelle fenêtre"), puis son nom en toute lettres et dans la langue cible.  
Par exemple, on écrira EN - English, et pas EN - Anglais.

  * Le composant varie selon le support : en desktop, la langue active est affichée dans le bouton sans son nom en toutes lettres (dans un souci de place), puis la liste déroulante reprend la langue active avant d’afficher les options. En mobile, la langue active est affichée en entier mais n’est pas répétée dans la liste déroulante.

### Accessibilité

L'élément actif de la liste de langue porte un attribut aria-current=”true”.  
  

### Personnalisation

Le style de ce composant n’est pas personnalisable. Cependant, certain
éléments sont facultatifs (voir la structure du composant

[Retour en haut de page - Back to top](/composants-et-
modeles/composants/retour-en-haut-de-page)

[Sommaire - Summary](/composants-et-modeles/composants/sommaire)

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
