Fermer

# Gestionnaire de consentement - Consent banner

Le gestionnaire de consentement permet à l'utilisateur de définir ses
préférences sur l'utilisation de ses données personnelles, notamment le dépôt
de cookies non fonctionnels dans son navigateur).

## Structure

Le gestionnaire de consentement se compose plusieurs éléments :

  1. Le bandeau
  2. La modale de gestion du consentement  

  3. Le bouton d’accès rapide à la modale de gestion du consentement  

  4. L’affichage des services désactivés 

## 1\. Le bandeau

Le bandeau permet le recueil du consentement des utilisateurs à l’arrivée sur
le site. Il est composé de :

  * Un titre - optionnel.
  * Une description, contenant un texte explicatif - obligatoire.
  * 3 boutons - obligatoires.  

    * « Accepter tout » > ferme le bandeau et enregistre le choix de l’utilisateur.
    * « Refuser tout » > ferme le bandeau et enregistre le choix de l’utilisateur.
    * « Personnaliser » > ouvre la modale de gestion du consentement.

Ce doit être le premier élément sélectionné lors de la navigation au clavier .
Il est faut donc le placer en première position dans le DOM, juste après la
balise `<body>` (et avant les liens d'évitement).

## À propos des cookies sur nomdusite.fr

Bienvenue ! Nous utilisons des cookies pour améliorer votre expérience et les
services disponibles sur ce site. Pour en savoir plus, visitez la page
[Données personnelles et cookies](). Vous pouvez, à tout moment, avoir le
contrôle sur les cookies que vous souhaitez activer.

  * Tout accepter 
  * Tout refuser 
  * Personnaliser 

###  Extrait de code

    
    
    <div class="fr-consent-banner">
        <h2 class="fr-h6">À propos des cookies sur nomdusite.fr</h2>
        <div class="fr-consent-banner__content">
            <p class="fr-text--sm">Bienvenue ! Nous utilisons des cookies pour améliorer votre expérience et les services disponibles sur ce site. Pour en savoir plus, visitez la page <a href="">Données personnelles et cookies</a>. Vous pouvez, à tout moment, avoir le contrôle sur les cookies que vous souhaitez activer.</p>
        </div>
        <ul class="fr-consent-banner__buttons fr-btns-group fr-btns-group--right fr-btns-group--inline-reverse fr-btns-group--inline-sm">
            <li>
                <button class="fr-btn" title="Autoriser tous les cookies">
                    Tout accepter
                </button>
            </li>
            <li>
                <button class="fr-btn" title="Refuser tous les cookies">
                    Tout refuser
                </button>
            </li>
            <li>
                <button class="fr-btn fr-btn--secondary" data-fr-opened="false" aria-controls="fr-consent-modal" title="Personnaliser les cookies">
                    Personnaliser
                </button>
            </li>
        </ul>
    </div>

**En desktop** , le bandeau est ferré en bas à gauche de la fenêtre du
navigateur.

![](/uploads/Capture_d_ecran_2022_07_28_a_00_33_45_a2bdc7f377.png)

**En mobile** , il est ferré en bas. Lorsque la hauteur maximum du bandeau est
atteinte , dans le cas d’un texte explicatif long, un scroll vertical apparait
sur l’ensemble du bandeau permettant à l’utilsateur de prendre connaissance de
la totalité du message avant de faire son choix.

![](/uploads/Capture_d_u2019ecran_2022_07_28_a_00_29_53_18dd71653f.png)

## 2\. La modale de gestion du consentement

La modale de gestion du consentement permet de lister les cookies par finalité
et de gérer le consentement de façon granulaire.

La modale liste les finalités de cookies. Chaque finalité se compose d'un
titre, d’une description et d'un bouton “voir plus de détails” permettant
d’afficher les sous-finalités associées. Les sous-finalités servent à
présenter le détail des partenaires associés à la finalité.

Le consentement est obtenu de manière globale (“tout accepter” / “tout
refuser”) ou par finalité et sous finalité (“accepter”/”tout refuser”).

Pour les éléments de contenus obligatoires à afficher sur ce premier, et la
présentation des finalités, [consultez les directives
CNIL](https://www.cnil.fr/fr/questions-reponses-lignes-directrices-
modificatives-et-recommandation-cookies-traceurs "consultez les directives
CNIL - nouvelle fenêtre").

Personnaliser

Fermer

###  Extrait de code

    
    
    <dialog id="fr-consent-modal" class="fr-modal" role="dialog" aria-labelledby="fr-consent-modal-title">
        <div class="fr-container fr-container--fluid fr-container-md">
            <div class="fr-grid-row fr-grid-row--center">
                <div class="fr-col-12 fr-col-md-10 fr-col-lg-8">
                    <div class="fr-modal__body">
                        <div class="fr-modal__header">
                            <button class="fr-btn--close fr-btn" aria-controls="fr-consent-modal" title="Fermer">
                                Fermer
                            </button>
                        </div>
                        <div class="fr-modal__content">
                            <h1 id="fr-consent-modal-title" class="fr-modal__title">
                                Panneau de gestion des cookies
                            </h1>
                            <div class="fr-consent-manager">
                                <!-- Finalités -->
                                <div class="fr-consent-service fr-consent-manager__header">
                                    <fieldset class="fr-fieldset fr-fieldset--inline">
                                        <legend id="finality-legend" class="fr-consent-service__title">Préférences pour tous les services. <a href="">Données personnelles et cookies</a>
                                        </legend>
                                        <div class="fr-consent-service__radios">
                                            <div class="fr-radio-group">
                                                <input type="radio" id="consent-all-accept" name="consent-all">
                                                <label class="fr-label" for="consent-all-accept">
                                                    Tout accepter
                                                </label>
                                            </div>
                                            <div class="fr-radio-group">
                                                <input type="radio" id="consent-all-refuse" name="consent-all">
                                                <label class="fr-label" for="consent-all-refuse">
                                                    Tout refuser
                                                </label>
                                            </div>
                                        </div>
                                    </fieldset>
                                </div>
                                <div class="fr-consent-service">
                                    <fieldset aria-labelledby="finality-0-legend finality-0-desc" role="group" class="fr-fieldset fr-fieldset--inline">
                                        <legend id="finality-0-legend" class="fr-consent-service__title">Cookies obligatoires</legend>
                                        <div class="fr-consent-service__radios">
                                            <div class="fr-radio-group">
                                                <input type="radio" id="consent-finality-0-accept" name="consent-finality-0">
                                                <label class="fr-label" for="consent-finality-0-accept">
                                                    Accepter
                                                </label>
                                            </div>
                                            <div class="fr-radio-group">
                                                <input disabled type="radio" id="consent-finality-0-refuse" name="consent-finality-0">
                                                <label class="fr-label" for="consent-finality-0-refuse">
                                                    Refuser
                                                </label>
                                            </div>
                                        </div>
                                        <p id="finality-0-desc" class="fr-consent-service__desc">Ce site utilise des cookies nécessaires à son bon fonctionnement qui ne peuvent pas être désactivés.</p>
                                    </fieldset>
                                </div>
                                <div class="fr-consent-service">
                                    <fieldset aria-labelledby="finality-1-legend finality-1-desc" role="group" class="fr-fieldset fr-fieldset--inline">
                                        <legend id="finality-1-legend" class="fr-consent-service__title">Nom de la finalité</legend>
                                        <div class="fr-consent-service__radios">
                                            <div class="fr-radio-group">
                                                <input type="radio" id="consent-finality-1-accept" name="consent-finality-1">
                                                <label class="fr-label" for="consent-finality-1-accept">
                                                    Accepter
                                                </label>
                                            </div>
                                            <div class="fr-radio-group">
                                                <input type="radio" id="consent-finality-1-refuse" name="consent-finality-1">
                                                <label class="fr-label" for="consent-finality-1-refuse">
                                                    Refuser
                                                </label>
                                            </div>
                                        </div>
                                        <p id="finality-1-desc" class="fr-consent-service__desc">Description optionnelle de la finalité, lorem ipsum dolor sit amet, consectetur adipiscing elit. Morbi in suscipit nulla, et pulvinar velit.</p>
                                        <div class="fr-consent-service__collapse">
                                            <button class="fr-consent-service__collapse-btn" aria-expanded="false" aria-describedby="finality-1-legend" aria-controls="finality-1-collapse"> Voir plus de détails</button>
                                        </div>
                                        <div class="fr-consent-services fr-collapse" id="finality-1-collapse">
                                            <!-- Sous finalités -->
                                            <div class="fr-consent-service">
                                                <fieldset class="fr-fieldset fr-fieldset--inline">
                                                    <legend id="finality-1-service-1-legend" class="fr-consent-service__title">Sous finalité 1</legend>
                                                    <div class="fr-consent-service__radios fr-fieldset--inline">
                                                        <div class="fr-radio-group">
                                                            <input type="radio" id="consent-finality-1-service-1-accept" name="consent-finality-1-service-1">
                                                            <label class="fr-label" for="consent-finality-1-service-1-accept">
                                                                Accepter
                                                            </label>
                                                        </div>
                                                        <div class="fr-radio-group">
                                                            <input type="radio" id="consent-finality-1-service-1-refuse" name="consent-finality-1-service-1">
                                                            <label class="fr-label" for="consent-finality-1-service-1-refuse">
                                                                Refuser
                                                            </label>
                                                        </div>
                                                    </div>
                                                </fieldset>
                                            </div>
                                            <div class="fr-consent-service">
                                                <fieldset aria-labelledby="finality-1-service-2-legend finality-1-service-2-desc" role="group" class="fr-fieldset fr-fieldset--inline">
                                                    <legend id="finality-1-service-2-legend" class="fr-consent-service__title" aria-describedby="finality-1-service-2-desc">Sous finalité 2</legend>
                                                    <div class="fr-consent-service__radios fr-fieldset--inline">
                                                        <div class="fr-radio-group">
                                                            <input type="radio" id="consent-finality-1-service-2-accept" name="consent-finality-1-service-2">
                                                            <label class="fr-label" for="consent-finality-1-service-2-accept">
                                                                Accepter
                                                            </label>
                                                        </div>
                                                        <div class="fr-radio-group">
                                                            <input type="radio" id="consent-finality-1-service-2-refuse" name="consent-finality-1-service-2">
                                                            <label class="fr-label" for="consent-finality-1-service-2-refuse">
                                                                Refuser
                                                            </label>
                                                        </div>
                                                    </div>
                                                    <p id="finality-1-service-2-desc" class="fr-consent-service__desc">Ce service utilise 3 cookies.</p>
                                                </fieldset>
                                            </div>
                                            <div class="fr-consent-service">
                                                <fieldset class="fr-fieldset fr-fieldset--inline">
                                                    <legend id="finality-1-service-3-legend" class="fr-consent-service__title">Sous finalité 3</legend>
                                                    <div class="fr-consent-service__radios fr-fieldset--inline">
                                                        <div class="fr-radio-group">
                                                            <input type="radio" id="consent-finality-1-service-3-accept" name="consent-finality-1-service-3">
                                                            <label class="fr-label" for="consent-finality-1-service-3-accept">
                                                                Accepter
                                                            </label>
                                                        </div>
                                                        <div class="fr-radio-group">
                                                            <input type="radio" id="consent-finality-1-service-3-refuse" name="consent-finality-1-service-3">
                                                            <label class="fr-label" for="consent-finality-1-service-3-refuse">
                                                                Refuser
                                                            </label>
                                                        </div>
                                                    </div>
                                                </fieldset>
                                            </div>
                                        </div>
                                    </fieldset>
                                </div>
                                <div class="fr-consent-service">
                                    <fieldset aria-labelledby="finality-2-legend finality-2-desc" role="group" class="fr-fieldset fr-fieldset--inline">
                                        <legend id="finality-2-legend" class="fr-consent-service__title">Nom de la finalité</legend>
                                        <div class="fr-consent-service__radios">
                                            <div class="fr-radio-group">
                                                <input type="radio" id="consent-finality-2-accept" name="consent-finality-2">
                                                <label class="fr-label" for="consent-finality-2-accept">
                                                    Accepter
                                                </label>
                                            </div>
                                            <div class="fr-radio-group">
                                                <input type="radio" id="consent-finality-2-refuse" name="consent-finality-2">
                                                <label class="fr-label" for="consent-finality-2-refuse">
                                                    Refuser
                                                </label>
                                            </div>
                                        </div>
                                        <p id="finality-2-desc" class="fr-consent-service__desc">Description optionnelle de la finalité, lorem ipsum dolor sit amet, consectetur adipiscing elit. Morbi in suscipit nulla, et pulvinar velit.</p>
                                        <div class="fr-consent-service__collapse">
                                            <button class="fr-consent-service__collapse-btn" aria-expanded="false" aria-describedby="finality-2-legend" aria-controls="finality-2-collapse"> Voir plus de détails</button>
                                        </div>
                                        <div class="fr-consent-services fr-collapse" id="finality-2-collapse">
                                            <!-- Sous finalités -->
                                            <div class="fr-consent-service">
                                                <fieldset class="fr-fieldset fr-fieldset--inline">
                                                    <legend id="finality-2-service-1-legend" class="fr-consent-service__title">Sous finalité 1</legend>
                                                    <div class="fr-consent-service__radios fr-fieldset--inline">
                                                        <div class="fr-radio-group">
                                                            <input type="radio" id="consent-finality-2-service-1-accept" name="consent-finality-2-service-1">
                                                            <label class="fr-label" for="consent-finality-2-service-1-accept">
                                                                Accepter
                                                            </label>
                                                        </div>
                                                        <div class="fr-radio-group">
                                                            <input type="radio" id="consent-finality-2-service-1-refuse" name="consent-finality-2-service-1">
                                                            <label class="fr-label" for="consent-finality-2-service-1-refuse">
                                                                Refuser
                                                            </label>
                                                        </div>
                                                    </div>
                                                </fieldset>
                                            </div>
                                            <div class="fr-consent-service">
                                                <fieldset aria-labelledby="finality-2-service-2-legend finality-2-service-2-desc" role="group" class="fr-fieldset fr-fieldset--inline">
                                                    <legend id="finality-2-service-2-legend" class="fr-consent-service__title" aria-describedby="finality-2-service-2-desc">Sous finalité 2</legend>
                                                    <div class="fr-consent-service__radios fr-fieldset--inline">
                                                        <div class="fr-radio-group">
                                                            <input type="radio" id="consent-finality-2-service-2-accept" name="consent-finality-2-service-2">
                                                            <label class="fr-label" for="consent-finality-2-service-2-accept">
                                                                Accepter
                                                            </label>
                                                        </div>
                                                        <div class="fr-radio-group">
                                                            <input type="radio" id="consent-finality-2-service-2-refuse" name="consent-finality-2-service-2">
                                                            <label class="fr-label" for="consent-finality-2-service-2-refuse">
                                                                Refuser
                                                            </label>
                                                        </div>
                                                    </div>
                                                    <p id="finality-2-service-2-desc" class="fr-consent-service__desc">Ce service utilise 3 cookies.</p>
                                                </fieldset>
                                            </div>
                                            <div class="fr-consent-service">
                                                <fieldset class="fr-fieldset fr-fieldset--inline">
                                                    <legend id="finality-2-service-3-legend" class="fr-consent-service__title">Sous finalité 3</legend>
                                                    <div class="fr-consent-service__radios fr-fieldset--inline">
                                                        <div class="fr-radio-group">
                                                            <input type="radio" id="consent-finality-2-service-3-accept" name="consent-finality-2-service-3">
                                                            <label class="fr-label" for="consent-finality-2-service-3-accept">
                                                                Accepter
                                                            </label>
                                                        </div>
                                                        <div class="fr-radio-group">
                                                            <input type="radio" id="consent-finality-2-service-3-refuse" name="consent-finality-2-service-3">
                                                            <label class="fr-label" for="consent-finality-2-service-3-refuse">
                                                                Refuser
                                                            </label>
                                                        </div>
                                                    </div>
                                                </fieldset>
                                            </div>
                                        </div>
                                    </fieldset>
                                </div>
                                <!-- Bouton de confirmation/fermeture -->
                                <ul class="fr-consent-manager__buttons fr-btns-group fr-btns-group--right fr-btns-group--inline-sm">
                                    <li>
                                        <button class="fr-btn">
                                            Confirmer mes choix
                                        </button>
                                    </li>
                                </ul>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </dialog>

Exemple de présentation des finalités et sous finalités :

![](/uploads/Capture_d_ecran_2021_03_24_a_17_45_33_8ba8e1fabb_1_1dd3309589.png)

![](/uploads/Capture_d_ecran_2021_03_24_a_17_45_39_cd1072075f_1_4488004fa6.png)

**Pour les développeurs:**  
Sur les balises fieldset , les attribut aria-labelledby et role(=”group”) sont
présents lorsqu’il y a une balise legend et un paragraphe de description. Si
le legend est seul, il ne faut pas mettre ces attributs sur le fieldset.  
  

## 3\. Le bouton d’accès rapide à la gestion du consentement

La modale de gestion du consentement doit toujours être accessible à n’importe
quel moment de la navigation de l’utilisateur. Un lien permettant d’afficher
la modale devra donc être toujours présent dans le pied de page (Footer) dans
la liste `fr-footer__bottom-list`.

  * Données personnelles
  * Gestion des cookies

Sauf mention contraire, tous les textes de ce site sont sous [licence
etalab-2.0](https://github.com/etalab/licence-ouverte/blob/master/LO.md)

    
    
    <!-- Le bouton d'ouverture est placé dans le footer, au sein de 
    la liste .fr-footer__bottom-list --> 
    
    <li class="fr-footer__bottom-item">
      <button class="fr-footer__bottom-link" data-fr-opened="false" aria-controls="fr-consent-modal">Gestion des cookies</button>
    </li> 
    

## 4\. L’affichage des services désactivés

Le refus sur certains cookies peuvent amener le blocage de certaines
fonctionnalités, notamment les services tiers affichés dans les pages du site
via une iframe comme par ex les players vidéo… il faut alors désactiver le
service et afficher un texte d’information et d’un lien permettant le
consentement au service.

#### **Nom du service** est désactivé

Autorisez le dépôt de cookies pour accéder à cette fonctionnalité.

Autoriser

###  Extrait de code

    
    
    <div class="fr-consent-placeholder">
        <h4 class="fr-h6 fr-mb-2v">**Nom du service** est désactivé</h4>
        <p class="fr-mb-6v">Autorisez le dépôt de cookies pour accéder à cette fonctionnalité.</p>
        <button class="fr-btn" title="Autorisez le dépôt de cookies pour accéder au service **Nom du service**">
            Autoriser
        </button>
    </div>

**Exemple vidéo petit format**

#### **Nom du service** est désactivé

Autorisez le dépôt de cookies pour accèder à cette fonctionnalité.

Autoriser

© Légende de la vidéo

Label du bouton de la transcription

###  Extrait de code

    
    
    <div class="fr-content-media fr-content-media--sm">
        <div class="fr-responsive-vid">
            <div class="fr-consent-placeholder">
                <h4 class="fr-h6">**Nom du service** est désactivé</h4>
                <p>Autorisez le dépôt de cookies pour accèder à cette fonctionnalité.</p>
                <button class="fr-btn">
                    Autoriser
                </button>
            </div>
        </div>
        <div class="fr-content-media__caption">© Légende de la vidéo</div>
        <div class="fr-content-media__transcription">
            <button class="fr-btn">
                Label du bouton de la transcription
            </button>
        </div>
    </div>

### Thème DSFR pour Tarteaucitron

Le DSFR propose une adaptation du composant pour le gestionnaire de
consentement Tarte au citron que vous pouvez ré-utiliser sur vos projets via
le dépôt GIT: [GitHub - GouvernementFR/dsfr-theme-
tarteaucitron](https://github.com/GouvernementFR/dsfr-theme-tarteaucitron)

### Information

Il n’y a aucune dépendance au DSFR - le thème propose sa propre css.  
Le code html et js sont ceux de tarteaucitron.  
Le thème a été testé sur les versions 1.9.1, 1.8.4 et 1.8.3 de tarteaucitron,
avec les label de boutons présent dans le bandeaux de consentement ci-dessus
('Personnaliser', ‘Tout refuser’, ‘Tout accepter’).  

## Règles d’utilisation

### Usage

La place du bandeau, les styles et l’ordre des boutons ne peuvent pas être
modifié. Seul le texte est à adapté en fonction du contexte.

### Accessibilité

  * Le bandeau de consentement doit être le premier élément sélectionné lors de la navigation au clavier (avant les liens d’évitement) ou au lecteur d’écran. Il faut le placer en première position dans le DOM, juste après la balise <body> (et avant les liens d’évitement).
  * Gestion du focus : lorsque l’utilisateur confirme ses choix de cookies, repositionner l’utilisateur en haut de la page.
  * La fenêtre de finalité étant une modale, elle suit les mêmes recommandations que cette dernière. Il en est de même pour les boutons radios permettant de choisir l'état des finalités.

### Besoin d'aide ?

L'équipe du DSFR est là pour vous aider.

Retrouvez-la sur :

  * [la communauté slack](https://gouvfr.slack.com/ "la communauté slack - nouvelle fenêtre") pour poser vos questions, et échanger avec d’autres utilisateurs.   
Vous êtes **agent de l’État** et souhaitez accéder au slack ? [Rejoignez la
communauté](https://gouvfr.atlassian.net/servicedesk/customer/portal/1/group/1/create/9
"Rejoignez la communauté - nouvelle fenêtre") dès maintenant !

  * [ le centre de support](https://gouvfr.atlassian.net/servicedesk/customer/portals "le centre de support - nouvelle fenêtre") pour envoyer vos demandes de correctifs et d'évolution.

[Fil d'Ariane - Breadcrumb](/composants-et-modeles/composants/fil-d-ariane)

[Indicateur d'étapes - Stepper](/composants-et-modeles/composants/indicateur-
d-etapes)

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
