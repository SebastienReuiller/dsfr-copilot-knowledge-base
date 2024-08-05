Fermer

# En-tête - Header

L’en-tête permet aux utilisateurs d’identifier sur quel site ils se trouvent.
Il peut donner accès à la recherche et à certaines pages ou fonctionnalités
clés.

## Structure

L’en-tête est composé :

  * du bloc Marque (dont [les règles de composition sont disponibles ici](https://www.gouvernement.fr/marque-Etat)) - obligatoire.
  * du nom de site - optionnel.
  * d’une ‘baseline’, sous le nom de site - optionnelle.
  * d’une partie fonctionnelle - proposant des accès rapide et/ou le moteur de recherche - adaptée aux besoins particuliers de chaque site - optionnelle.

L’en-tête est sur fond blanc en thème clair et sur fond G800 en thème sombre.

## En-tête simple

L’en-tête simple doit être utilisé pour les sites ne comprenant ni moteur de
recherche, ni accès rapides.

Il est composé ici :

  * du bloc marque - obligatoire.
  * du nom de site - optionnel.
  * d’une phrase descriptive - optionnelle.

Un lien, dont la place peut changer selon les éléments présents dans l’en-
tête, pointe vers la page d’accueil du site. Le lien est étendu à l’ensemble
du bloc grâce à la classe .`fr-enlarge-link`.

[

Intitulé  
officiel

](/ "Accueil - Nom de l’entité \(ministère, secrétariat d‘état,
gouvernement\)")

Menu

Fermer

  * accès direct
  * accès direct
  * accès direct
  * accès direct

###  Extrait de code

    
    
                          <header role="banner" class="fr-header">
        <div class="fr-header__body">
            <div class="fr-container">
                <div class="fr-header__body-row">
                    <div class="fr-header__brand fr-enlarge-link">
                        <div class="fr-header__brand-top">
                            <div class="fr-header__logo">
                                <a href="/" title="Accueil - Nom de l’entité (ministère, secrétariat d‘état, gouvernement)">
                                    <p class="fr-logo">
                                        Intitulé
                                        <br>officiel
                                    </p>
                                </a>
                            </div>
                            <div class="fr-header__navbar">
                                <button class="fr-btn--menu fr-btn" data-fr-opened="false" aria-controls="modal-491"  id="button-492" title="Menu">
                                    Menu
                                </button>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
        <div class="fr-header__menu fr-modal" id="modal-491" aria-labelledby="button-492">
            <div class="fr-container">
                <button class="fr-btn--close fr-btn" aria-controls="modal-491" title="Fermer">
                    Fermer
                </button>
                <div class="fr-header__menu-links">
                </div>
                <nav class="fr-nav" id="navigation-494" role="navigation" aria-label="Menu principal">
                    <ul class="fr-nav__list">
                        <li class="fr-nav__item">
                            <a class="fr-nav__link" href="#" target="_self">accès direct</a>
                        </li>
                        <li class="fr-nav__item">
                            <a class="fr-nav__link" href="#" target="_self">accès direct</a>
                        </li>
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
                          
                        

Le lien est placé sur le bloc marque et peut-être étendu à l’ensemble du bloc
.fr-header__brand (via la classe .fr-enlarge-link).

### En-tête simple avec nom de service et description

Intitulé  
officiel

[

Nom du site / service

](/ "Accueil - \[À MODIFIER - Nom du site / service\] - Nom de l’entité
\(ministère, secrétariat d‘état, gouvernement\)")

baseline - précisions sur l‘organisation

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
                </div>
            </div>
        </div>
    </header>
                          
                        

Le lien est placé sur le “nom de service” et est étendu à l’ensemble du bloc
.fr-header__brand (via la classe .fr-enlarge-link.).

## En-tête avec accès rapides

L’en-tête avec accès rapides doit être utilisé pour les sites souhaitant
mettre en avant certaines pages/fonctionnalités clés de leur site, comme par
exemple la connexion à un espace sécurisé.

Il est composé ici des éléments du haut de page simple et de liens accès
rapides. Il est possible d’afficher jusqu'à 3 accès rapides maximum.

![](/uploads/entete_quicklinks_3838fabb52.png)

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
                                <button class="fr-btn--menu fr-btn" data-fr-opened="false" aria-controls="modal-499" id="button-500" title="Menu">
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
                        </div>
                    </div>
                </div>
            </div>
        </div>
        <div class="fr-header__menu fr-modal" id="modal-499" aria-labelledby="button-500">
            <div class="fr-container">
                <button class="fr-btn--close fr-btn" aria-controls="modal-499" title="Fermer">
                    Fermer
                </button>
                <div class="fr-header__menu-links">
                </div>
            </div>
        </div>
    </header>

## En-tête avec moteur de recherche

L’en-tête avec moteur de recherche doit être utilisé pour les sites souhaitant
rendre facilement accessible le moteur de recherche. Il est composé ici des
éléments du haut de page simple et de [la barre de recherche
medium](/elements-d-interface/composants/barre-de-recherche).

![](/uploads/Capture_d_ecran_2022_01_07_a_11_48_44_82b48bdd38.png)

![](/uploads/entete_recherche_dm_3fd880531e.png)

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
                                <button class="fr-btn--search fr-btn" data-fr-opened="false" aria-controls="modal-541" id="button-542" title="Rechercher">
                                    Rechercher
                                </button>
                                <button class="fr-btn--menu fr-btn" data-fr-opened="false" aria-controls="modal-543" id="button-544" title="Menu">
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
                        <div class="fr-header__search fr-modal" id="modal-541">
                            <div class="fr-container fr-container-lg--fluid">
                                <button class="fr-btn--close fr-btn" aria-controls="modal-541" title="Fermer">
                                    Fermer
                                </button>
                                <div class="fr-search-bar" id="search-540" role="search">
                                    <label class="fr-label" for="search-540-input">
                                        Rechercher
                                    </label>
                                    <input class="fr-input" placeholder="Rechercher" type="search" id="search-540-input" name="search-540-input">
                                    <button class="fr-btn" title="Rechercher">
                                        Rechercher
                                    </button>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
        <div class="fr-header__menu fr-modal" id="modal-543" aria-labelledby="button-544">
            <div class="fr-container">
                <button class="fr-btn--close fr-btn" aria-controls="modal-543" title="Fermer">
                    Fermer
                </button>
                <div class="fr-header__menu-links">
                </div>
                <nav class="fr-nav" id="navigation-547" role="navigation" aria-label="Menu principal">
                    <ul class="fr-nav__list">
                        <li class="fr-nav__item">
                            <a class="fr-nav__link" href="#" target="_self">accès direct</a>
                        </li>
                        <li class="fr-nav__item">
                            <a class="fr-nav__link" href="#" target="_self">accès direct</a>
                        </li>
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

## En-tête avec accès rapides et moteur de recherche

Il s’agit de la version complète pour les sites souhaitant à la fois mettre en
avant certaines pages/fonctionnalités clés de leur site et rendre facilement
accessible le moteur de recherche.  
Il peut également être accompagné d’un logo opérateur (voir exemples ci-
après).  

![](/uploads/entete_recherche_quicklinks_c84921f737.png)

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
                                <button class="fr-btn--search fr-btn" data-fr-opened="false" aria-controls="modal-474" id="button-475" title="Rechercher">
                                    Rechercher
                                </button>
                                <button class="fr-btn--menu fr-btn" data-fr-opened="false" aria-controls="modal-476"  id="button-477" title="Menu">
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
                        </div>
                        <div class="fr-header__search fr-modal" id="modal-474">
                            <div class="fr-container fr-container-lg--fluid">
                                <button class="fr-btn--close fr-btn" aria-controls="modal-474" title="Fermer">
                                    Fermer
                                </button>
                                <div class="fr-search-bar" id="search-473" role="search">
                                    <label class="fr-label" for="search-473-input">
                                        Rechercher
                                    </label>
                                    <input class="fr-input" placeholder="Rechercher" type="search" id="search-473-input" name="search-473-input">
                                    <button class="fr-btn" title="Rechercher">
                                        Rechercher
                                    </button>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
        <div class="fr-header__menu fr-modal" id="modal-476" aria-labelledby="button-477">
            <div class="fr-container">
                <button class="fr-btn--close fr-btn" aria-controls="modal-476" title="Fermer">
                    Fermer
                </button>
                <div class="fr-header__menu-links">
                </div>
                <nav class="fr-nav" id="navigation-478" role="navigation" aria-label="Menu principal">
                    <ul class="fr-nav__list">
                        <li class="fr-nav__item">
                            <a class="fr-nav__link" href="#" target="_self">accès direct</a>
                        </li>
                        <li class="fr-nav__item">
                            <a class="fr-nav__link" href="#" target="_self">accès direct</a>
                        </li>
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

## Avec logo opérateur vertical

![](/uploads/entete_operateur_vertical_07073bebae.png)

###  Extrait de code

    
    
    <header role="banner" class="fr-header">
        <div class="fr-header__body">
            <div class="fr-container">
                <div class="fr-header__body-row">
                    <div class="fr-header__brand fr-enlarge-link">
                        <div class="fr-header__brand-top">
                            <div class="fr-header__logo">
                                <p class="fr-logo">
                                    République
                                    <br>Française
                                </p>
                            </div>
                            <div class="fr-header__operator">
                                <a href="/" title="Accueil - [À MODIFIER - texte alternatif de l’image : nom de l'opérateur ou du site serviciel] - République Française">
                                    <img class="fr-responsive-img" style="width:3.5rem;" src="../../../example/img/placeholder.9x16.png" alt="[À MODIFIER - texte alternatif de l’image]" />
                                    <!-- L’alternative de l’image (attribut alt) doit impérativement être renseignée et reprendre le texte visible dans l’image -->
                                </a>
                            </div>
                            <div class="fr-header__navbar">
                                <button class="fr-btn--search fr-btn" data-fr-opened="false" aria-controls="modal-558" id="button-559" title="Rechercher">
                                    Rechercher
                                </button>
                                <button class="fr-btn--menu fr-btn" data-fr-opened="false" aria-controls="modal-560" id="button-561" title="Menu">
                                    Menu
                                </button>
                            </div>
                        </div>
                    </div>
                    <div class="fr-header__tools">
                        <div class="fr-header__search fr-modal" id="modal-558">
                            <div class="fr-container fr-container-lg--fluid">
                                <button class="fr-btn--close fr-btn" aria-controls="modal-558" title="Fermer">
                                    Fermer
                                </button>
                                <div class="fr-search-bar" id="search-557" role="search">
                                    <label class="fr-label" for="search-557-input">
                                        Rechercher
                                    </label>
                                    <input class="fr-input" placeholder="Rechercher" type="search" id="search-557-input" name="search-557-input">
                                    <button class="fr-btn" title="Rechercher">
                                        Rechercher
                                    </button>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
        <div class="fr-header__menu fr-modal" id="modal-560" aria-labelledby="button-561">
            <div class="fr-container">
                <button class="fr-btn--close fr-btn" aria-controls="modal-560" title="Fermer">
                    Fermer
                </button>
                <div class="fr-header__menu-links">
                </div>
                <nav class="fr-nav" id="navigation-564" role="navigation" aria-label="Menu principal">
                    <ul class="fr-nav__list">
                        <li class="fr-nav__item">
                            <a class="fr-nav__link" href="#" target="_self">accès direct</a>
                        </li>
                        <li class="fr-nav__item">
                            <a class="fr-nav__link" href="#" target="_self">accès direct</a>
                        </li>
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

**Pour les développeurs** : L’alternative textuelle du logo (attribut alt)
doit impérativement contenir le texte présent dans l’image.  

## Avec logo opérateur horizontal

![](/uploads/entete_operateur_horizontal_ac21ee1b70.png)

###  Extrait de code

    
    
    <header role="banner" class="fr-header">
        <div class="fr-header__body">
            <div class="fr-container">
                <div class="fr-header__body-row">
                    <div class="fr-header__brand fr-enlarge-link">
                        <div class="fr-header__brand-top">
                            <div class="fr-header__logo">
                                <p class="fr-logo">
                                    République
                                    <br>Française
                                </p>
                            </div>
                            <div class="fr-header__operator">
                                <img class="fr-responsive-img" style="max-width:9.0625rem;" src="../../../example/img/placeholder.16x9.png" alt="[À MODIFIER - texte alternatif de l’image]" >
                                <!-- L’alternative de l’image (attribut alt) doit impérativement être renseignée et reprendre le texte visible dans l’image -->
                            </div>
                            <div class="fr-header__navbar">
                                <button class="fr-btn--search fr-btn" data-fr-opened="false" aria-controls="modal-575" id="button-576" title="Rechercher">
                                    Rechercher
                                </button>
                                <button class="fr-btn--menu fr-btn" data-fr-opened="false" aria-controls="modal-577" id="button-578" title="Menu">
                                    Menu
                                </button>
                            </div>
                        </div>
                        <div class="fr-header__service">
                            <a href="/" title="Accueil - [À MODIFIER - Nom du site / service] - [À MODIFIER - texte alternatif de l’image : nom de l'opérateur ou du site serviciel] - République Française">
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
                        </div>
                        <div class="fr-header__search fr-modal" id="modal-575">
                            <div class="fr-container fr-container-lg--fluid">
                                <button class="fr-btn--close fr-btn" aria-controls="modal-575" title="Fermer">
                                    Fermer
                                </button>
                                <div class="fr-search-bar" id="search-574" role="search">
                                    <label class="fr-label" for="search-574-input">
                                        Rechercher
                                    </label>
                                    <input class="fr-input" placeholder="Rechercher" type="search" id="search-574-input" name="search-574-input">
                                    <button class="fr-btn" title="Rechercher">
                                        Rechercher
                                    </button>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
        <div class="fr-header__menu fr-modal" id="modal-577" aria-labelledby="button-578">
            <div class="fr-container">
                <button class="fr-btn--close fr-btn" aria-controls="modal-577" title="Fermer">
                    Fermer
                </button>
                <div class="fr-header__menu-links">
                </div>
                <nav class="fr-nav" id="navigation-581" role="navigation" aria-label="Menu principal">
                    <ul class="fr-nav__list">
                        <li class="fr-nav__item">
                            <a class="fr-nav__link" href="#" target="_self">accès direct</a>
                        </li>
                        <li class="fr-nav__item">
                            <a class="fr-nav__link" href="#" target="_self">accès direct</a>
                        </li>
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

**Pour les développeurs** : L’alternative textuelle du logo (attribut alt)
doit impérativement contenir le texte présent dans l’image.  

## Déclinaison avec badge "Bêta"

![](/uploads/entete_beta_ope_7d329bbd65.png)

![](/uploads/entete_beta_bm_28f9fd3462.png)

## Responsive

En version mobile l’en-tête se compose d’une zone haute intégrant les éléments
obligatoires liés au bloc marque. Une zone basse complète l’en-tête mobile
avec :

  * le nom site (si présent),
  * le picto loupe pour accéder à la recherche (si présente),
  * le picto burger pour accéder au menu principal.

![](/uploads/Capture_d_ecran_2022_01_07_a_11_54_15_4e910e54e5.png)

![](/uploads/Capture_d_ecran_2022_01_07_a_11_54_53_6e9f132d95.png)

### Bloc marque mobile

Le bloc marque suit les mêmes règle de composition que pour le desktop et doit
respecter [la charte de marque de l'État](https://www.gouvernement.fr/marque-
Etat).

### Recherche

Le picto “loupe” permet l'affichage de la barre de recherche dans un ‘overlay’
dédié.

Un badge comportant la mention "Bêta" peut être ajouté à l’en-tête afin de
notifier que le site ou l’applicatif n’est pas en version stable.

![](/uploads/Capture_d_ecran_2020_09_14_a_16_51_18_bc544c5a0b.png)

Le picto “loupe” ne doit être affiché que si la fonctionnalité de recherche
est présente dans le header desktop. Il doit être positionné dans le bloc .fr-
header__navbar.

### Menu burger

Le picto burger permet l’affichage du menu dans un overlay présentant :

  * la navigation principale (si présente). [Voir en détail la navigation mobile](/elements-d-interface/composants/navigation-principale),
  * les accès rapides (si présents).

Le picto “burger” ne doit être présent que si des accès rapides sont presents
en version desktop et/ou la navigation principale est présente en version
desktop.Il doit être positionné dans le bloc .fr-header__navbar.

## Règles d’utilisation

### Usage

L’en-tête doit être utilisé sur l’ensemble des sites de la sphère
gouvernementale. Sur chaque site, l’en-tête doit être affiché en haut de
chaque page.

L’en-tête peut être utilisé seul sans système de navigation principale (one
page, site outil…). [La navigation principale](/elements-d-
interface/composants/navigation-principale) est donc un composant dissocié de
l’en-tête.

Lors des périodes de deuil national, il est possible d’utiliser la version en
berne du header, en ajoutant à la balise <html> l’attribut data-fr-mourning.
La Marianne s’affichera alors dans sa version en berne.

    
    
    <html lang="fr" data-fr-mourning>

![](/uploads/entete_deuil_5124993876.png)

![](/uploads/entete_deuil_dm_f8b8b4de36.png)

#### Pour les designers

Le composant étant complexe, les symboles ne sont pas totalement dynamiques.
Si vous devez utiliser les éléments “logo” ou le bloc “nom de site - baseline”
il est nécessaire de détacher le symbole pour l’adapter, car ces éléments ne
prennent pas automatiquement les espacements prévus de 5w entre eux.

### Accessibilité

Les liens d'évitement (masqués ou non) sont placés juste avant le header.

#### Gestion du lien “retour à l’accueil”

  * Le lien vers l’accueil du site est placé sur le nom du site (qu’il soit dans le bloc-marque, le nom du site et sa baseline ou le logo).
  * Le lien est étendu à l’ensemble du bloc-marque en css par le bias de la classe fr-enlarge-link.
  * Le title du lien doit contenir le terme Accueil, suivi du nom du site. title="Accueil - [À MODIFIER | Nom du site / service]”.
  * Si le header est complexe et que le bloc marque n’est pas République Française, mais une autre entité, cette dernière doit également être ajoutée (voir les exemples dans les extraits de code).  

#### Menu burger

Le menu est utilisable au clavier.

### Contenu

Pour les libellés des lien accès rapides, utiliser des formulations claires et
concises.

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

### Voir aussi

#### [En-tête - Header](/composants-et-modeles/composants/en-tete)

L’en-tête permet aux utilisateurs d’identifier sur quel site ils se trouvent.

![](/uploads/thumbnail_composants_en_tete_187c5b71fc.png)

[Curseur - Range](/composants-et-modeles/composants/curseur-range)

[Fil d'Ariane - Breadcrumb](/composants-et-modeles/composants/fil-d-ariane)

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
