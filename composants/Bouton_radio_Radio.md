Fermer

# Bouton radio - Radio button

Les boutons radio permettent à l’utilisateur de sélectionner une seule option
dans une liste.

Le bouton radio ne peut pas être utilisé seul : il faut au minimum 2 options.
Il est préférable de ne pas sélectionner d’option par défaut pour que le choix
de l’utilisateur soit conscient (en particulier si le choix est obligatoire).

## Structure

Les boutons radios sont composés des éléments suivants :

  * des boutons - obligatoires.
  * des labels, associés aux boutons - obligatoires.
  * un texte additionnel pour les boutons / labels - optionnel.
  * une légende, décrivant le contexte du groupe de bouton - obligatoire.
  * une description additionnelle pour la légende - optionnelle.
  * un message d’erreur ou de succès - obligatoire si un changement d'état doit être notifié à l’utilisateur.

## Liste horizontale (radio buttons inline)

Il faut privilégier les listes verticales aux listes horizontales, plus
difficile à lire pour l’utilisateur. Cette organisation est donc à utiliser
uniquement lorsqu'il n’y a que 2 options ou que les libellés sont courts.

Légende pour l’ensemble des éléments

Libellé bouton radio

Libellé bouton radio

Libellé bouton radio

###  Extrait de code

    
    
                          <fieldset class="fr-fieldset" id="radio-inline" aria-labelledby="radio-inline-legend radio-inline-messages">
        <legend class="fr-fieldset__legend--regular fr-fieldset__legend" id="radio-inline-legend">
            Légende pour l’ensemble des éléments
        </legend>
        <div class="fr-fieldset__element fr-fieldset__element--inline">
            <div class="fr-radio-group">
                <input type="radio" id="radio-inline-1" name="radio-inline">
                <label class="fr-label" for="radio-inline-1">
                    Libellé bouton radio
                </label>
            </div>
        </div>
        <div class="fr-fieldset__element fr-fieldset__element--inline">
            <div class="fr-radio-group">
                <input type="radio" id="radio-inline-2" name="radio-inline">
                <label class="fr-label" for="radio-inline-2">
                    Libellé bouton radio
                </label>
            </div>
        </div>
        <div class="fr-fieldset__element fr-fieldset__element--inline">
            <div class="fr-radio-group">
                <input type="radio" id="radio-inline-3" name="radio-inline">
                <label class="fr-label" for="radio-inline-3">
                    Libellé bouton radio
                </label>
            </div>
        </div>
        <div class="fr-messages-group" id="radio-inline-messages" aria-live="assertive">
        </div>
    </fieldset>
                          
                        

## Liste avec texte d’aide

Il est recommandé d’ajouter un texte d’aide afin de faciliter le choix de
l’utilisateur. Ces précisions peuvent être apportées de 2 façons :

  * via un texte sous le titre de la liste

Légende pour l’ensemble des éléments Texte de description additionnel

Libellé bouton radio

Libellé bouton radio

Libellé bouton radio

###  Extrait de code

    
    
                          <fieldset class="fr-fieldset" id="radio-hint" aria-labelledby="radio-hint-legend radio-hint-messages">
        <legend class="fr-fieldset__legend--regular fr-fieldset__legend" id="radio-hint-legend">
            Légende pour l’ensemble des éléments
            <span class="fr-hint-text">Texte de description additionnel</span>
        </legend>
        <div class="fr-fieldset__element">
            <div class="fr-radio-group">
                <input type="radio" id="radio-hint-1" name="radio-hint">
                <label class="fr-label" for="radio-hint-1">
                    Libellé bouton radio
                </label>
            </div>
        </div>
        <div class="fr-fieldset__element">
            <div class="fr-radio-group">
                <input type="radio" id="radio-hint-2" name="radio-hint">
                <label class="fr-label" for="radio-hint-2">
                    Libellé bouton radio
                </label>
            </div>
        </div>
        <div class="fr-fieldset__element">
            <div class="fr-radio-group">
                <input type="radio" id="radio-hint-3" name="radio-hint">
                <label class="fr-label" for="radio-hint-3">
                    Libellé bouton radio
                </label>
            </div>
        </div>
        <div class="fr-messages-group" id="radio-hint-messages" aria-live="assertive">
        </div>
    </fieldset>
                          
                        

  * via un texte sous le libellé de chaque bouton radio

Légende pour l’ensemble des éléments

Libellé bouton radio Texte de description additionnel

Libellé bouton radio Texte de description additionnel

Libellé bouton radio Texte de description additionnel

###  Extrait de code

    
    
                          <fieldset class="fr-fieldset" id="radio-hint-element" aria-labelledby="radio-hint-element-legend radio-hint-element-messages">
        <legend class="fr-fieldset__legend--regular fr-fieldset__legend" id="radio-hint-element-legend">
            Légende pour l’ensemble des éléments
        </legend>
        <div class="fr-fieldset__element">
            <div class="fr-radio-group">
                <input type="radio" id="radio-hint-element-1" name="radio-hint-element">
                <label class="fr-label" for="radio-hint-element-1">
                    Libellé bouton radio
                    <span class="fr-hint-text">Texte de description additionnel</span>
                </label>
            </div>
        </div>
        <div class="fr-fieldset__element">
            <div class="fr-radio-group">
                <input type="radio" id="radio-hint-element-2" name="radio-hint-element">
                <label class="fr-label" for="radio-hint-element-2">
                    Libellé bouton radio
                    <span class="fr-hint-text">Texte de description additionnel</span>
                </label>
            </div>
        </div>
        <div class="fr-fieldset__element">
            <div class="fr-radio-group">
                <input type="radio" id="radio-hint-element-3" name="radio-hint-element">
                <label class="fr-label" for="radio-hint-element-3">
                    Libellé bouton radio
                    <span class="fr-hint-text">Texte de description additionnel</span>
                </label>
            </div>
        </div>
        <div class="fr-messages-group" id="radio-hint-element-messages" aria-live="assertive">
        </div>
    </fieldset>
                          
                        

## État d'erreur

L'état d’erreur est signalé par l’affichage d’une ligne rouge et d'un message
d’erreur en-dessous du composant (cf. couleurs fonctionnelles :link: : le
rouge est la couleur de l’état erreur).

### Pour les développeurs

Pour l'état d’erreur, il est nécessaire d’ajouter un `role=”group”` à la
balise fieldset. De plus, le message d’erreur et la balise legend sont liés au
fieldset via l’attribut `aria-labelledby`.

Légende pour l’ensemble des éléments

Libellé bouton radio

Libellé bouton radio

Libellé bouton radio

Texte d’erreur obligatoire

###  Extrait de code

    
    
                          <fieldset class="fr-fieldset fr-fieldset--error" id="radio-error" role="group" aria-labelledby="radio-error-legend radio-error-messages">
        <legend class="fr-fieldset__legend--regular fr-fieldset__legend" id="radio-error-legend">
            Légende pour l’ensemble des éléments
        </legend>
        <div class="fr-fieldset__element">
            <div class="fr-radio-group">
                <input type="radio" id="radio-error-1" name="radio-error">
                <label class="fr-label" for="radio-error-1">
                    Libellé bouton radio
                </label>
            </div>
        </div>
        <div class="fr-fieldset__element">
            <div class="fr-radio-group">
                <input type="radio" id="radio-error-2" name="radio-error">
                <label class="fr-label" for="radio-error-2">
                    Libellé bouton radio
                </label>
            </div>
        </div>
        <div class="fr-fieldset__element">
            <div class="fr-radio-group">
                <input type="radio" id="radio-error-3" name="radio-error">
                <label class="fr-label" for="radio-error-3">
                    Libellé bouton radio
                </label>
            </div>
        </div>
        <div class="fr-messages-group" id="radio-error-messages" aria-live="assertive">
            <p class="fr-message fr-message--error" id="radio-error-message-error">Texte d’erreur obligatoire</p>
        </div>
    </fieldset>
                          
                        

Pour les liste de boutons radio en ligne :

Légende pour l’ensemble des éléments

Libellé bouton radio

Libellé bouton radio

Libellé bouton radio

Texte d’erreur obligatoire

###  Extrait de code

    
    
                          <fieldset class="fr-fieldset fr-fieldset--error" id="radio-error-inline" role="group" aria-labelledby="radio-error-inline-legend radio-error-inline-messages">
        <legend class="fr-fieldset__legend--regular fr-fieldset__legend" id="radio-error-inline-legend">
            Légende pour l’ensemble des éléments
        </legend>
        <div class="fr-fieldset__element fr-fieldset__element--inline">
            <div class="fr-radio-group">
                <input type="radio" id="radio-error-inline-1" name="radio-error-inline">
                <label class="fr-label" for="radio-error-inline-1">
                    Libellé bouton radio
                </label>
            </div>
        </div>
        <div class="fr-fieldset__element fr-fieldset__element--inline">
            <div class="fr-radio-group">
                <input type="radio" id="radio-error-inline-2" name="radio-error-inline">
                <label class="fr-label" for="radio-error-inline-2">
                    Libellé bouton radio
                </label>
            </div>
        </div>
        <div class="fr-fieldset__element fr-fieldset__element--inline">
            <div class="fr-radio-group">
                <input type="radio" id="radio-error-inline-3" name="radio-error-inline">
                <label class="fr-label" for="radio-error-inline-3">
                    Libellé bouton radio
                </label>
            </div>
        </div>
        <div class="fr-messages-group" id="radio-error-inline-messages" aria-live="assertive">
            <p class="fr-message fr-message--error" id="radio-error-inline-message-error">Texte d’erreur obligatoire</p>
        </div>
    </fieldset>
                          
                        

## État de succès

L'état de succès est signalé par l’affichage d’une ligne verte et d'un message
de succès en-dessous du composant (cf. couleurs fonctionnelles :link: : le
vert est la couleur de l’état succès).

#### Pour les développeurs

Pour l'état de success, il est nécessaire d’ajouter un `role=”group”` à la
balise fieldset. De plus, le message de validation et la balise legend sont
liés au fieldset via l’attribut `aria-labelledby`.

Légende pour l’ensemble des éléments

Libellé bouton radio

Libellé bouton radio

Libellé bouton radio

Texte de validation

###  Extrait de code

    
    
                          <fieldset class="fr-fieldset fr-fieldset--valid" id="radio-valid" role="group" aria-labelledby="radio-valid-legend radio-valid-messages">
        <legend class="fr-fieldset__legend--regular fr-fieldset__legend" id="radio-valid-legend">
            Légende pour l’ensemble des éléments
        </legend>
        <div class="fr-fieldset__element">
            <div class="fr-radio-group">
                <input type="radio" id="radio-valid-1" name="radio-valid">
                <label class="fr-label" for="radio-valid-1">
                    Libellé bouton radio
                </label>
            </div>
        </div>
        <div class="fr-fieldset__element">
            <div class="fr-radio-group">
                <input type="radio" id="radio-valid-2" name="radio-valid">
                <label class="fr-label" for="radio-valid-2">
                    Libellé bouton radio
                </label>
            </div>
        </div>
        <div class="fr-fieldset__element">
            <div class="fr-radio-group">
                <input type="radio" id="radio-valid-3" name="radio-valid">
                <label class="fr-label" for="radio-valid-3">
                    Libellé bouton radio
                </label>
            </div>
        </div>
        <div class="fr-messages-group" id="radio-valid-messages" aria-live="assertive">
            <p class="fr-message fr-message--valid" id="radio-valid-message-valid">Texte de validation</p>
        </div>
    </fieldset>
                          
                        

Légende pour l’ensemble des éléments

Libellé bouton radio

Libellé bouton radio

Libellé bouton radio

Texte de validation

###  Extrait de code

    
    
                          <fieldset class="fr-fieldset fr-fieldset--valid" id="radio-valid-inline" role="group" aria-labelledby="radio-valid-inline-legend radio-valid-inline-messages">
        <legend class="fr-fieldset__legend--regular fr-fieldset__legend" id="radio-valid-inline-legend">
            Légende pour l’ensemble des éléments
        </legend>
        <div class="fr-fieldset__element fr-fieldset__element--inline">
            <div class="fr-radio-group">
                <input type="radio" id="radio-valid-inline-1" name="radio-valid-inline">
                <label class="fr-label" for="radio-valid-inline-1">
                    Libellé bouton radio
                </label>
            </div>
        </div>
        <div class="fr-fieldset__element fr-fieldset__element--inline">
            <div class="fr-radio-group">
                <input type="radio" id="radio-valid-inline-2" name="radio-valid-inline">
                <label class="fr-label" for="radio-valid-inline-2">
                    Libellé bouton radio
                </label>
            </div>
        </div>
        <div class="fr-fieldset__element fr-fieldset__element--inline">
            <div class="fr-radio-group">
                <input type="radio" id="radio-valid-inline-3" name="radio-valid-inline">
                <label class="fr-label" for="radio-valid-inline-3">
                    Libellé bouton radio
                </label>
            </div>
        </div>
        <div class="fr-messages-group" id="radio-valid-inline-messages" aria-live="assertive">
            <p class="fr-message fr-message--valid" id="radio-valid-inline-message-valid">Texte de validation</p>
        </div>
    </fieldset>
                          
                        

## État désactivé

L'état désactivé indique que l'utilisateur ne peux pas interagir avec
l'élément.

Légende pour l’ensemble des éléments

Libellé bouton radio

Libellé bouton radio

Libellé bouton radio

###  Extrait de code

    
    
                          <fieldset class="fr-fieldset" id="radio-disabled" aria-labelledby="radio-disabled-legend radio-disabled-messages">
        <legend class="fr-fieldset__legend--regular fr-fieldset__legend" id="radio-disabled-legend">
            Légende pour l’ensemble des éléments
        </legend>
        <div class="fr-fieldset__element">
            <div class="fr-radio-group">
                <input disabled type="radio" id="radio-disabled-1" name="radio-disabled">
                <label class="fr-label" for="radio-disabled-1">
                    Libellé bouton radio
                </label>
            </div>
        </div>
        <div class="fr-fieldset__element">
            <div class="fr-radio-group">
                <input disabled checked type="radio" id="radio-disabled-2" name="radio-disabled">
                <label class="fr-label" for="radio-disabled-2">
                    Libellé bouton radio
                </label>
            </div>
        </div>
        <div class="fr-fieldset__element">
            <div class="fr-radio-group">
                <input disabled type="radio" id="radio-disabled-3" name="radio-disabled">
                <label class="fr-label" for="radio-disabled-3">
                    Libellé bouton radio
                </label>
            </div>
        </div>
        <div class="fr-messages-group" id="radio-disabled-messages" aria-live="assertive">
        </div>
    </fieldset>
                          
                        

## Tailles

Le “bouton radio” est proposé par défaut en 24px (taille Medium - MD) ce choix
a été fait pour optimiser l’ergonomie et l’accessibilité.

Légende pour l’ensemble des éléments

Libellé bouton radio

Libellé bouton radio

Libellé bouton radio

###  Extrait de code

    
    
                          <fieldset class="fr-fieldset" id="radio" aria-labelledby="radio-legend radio-messages">
        <legend class="fr-fieldset__legend--regular fr-fieldset__legend" id="radio-legend">
            Légende pour l’ensemble des éléments
        </legend>
        <div class="fr-fieldset__element">
            <div class="fr-radio-group">
                <input type="radio" id="radio-1" name="radio">
                <label class="fr-label" for="radio-1">
                    Libellé bouton radio
                </label>
            </div>
        </div>
        <div class="fr-fieldset__element">
            <div class="fr-radio-group">
                <input checked type="radio" id="radio-2" name="radio">
                <label class="fr-label" for="radio-2">
                    Libellé bouton radio
                </label>
            </div>
        </div>
        <div class="fr-fieldset__element">
            <div class="fr-radio-group">
                <input type="radio" id="radio-3" name="radio">
                <label class="fr-label" for="radio-3">
                    Libellé bouton radio
                </label>
            </div>
        </div>
        <div class="fr-messages-group" id="radio-messages" aria-live="assertive">
        </div>
    </fieldset>
                          
                        

Il existe également une version plus petite 16 px / Small (SM) correspondant à
la taille standard proposés par les navigateurs. Attention, la zone cliquable
doit être suffisante pour l'utilisation au doigt sur écran tactile (44 px de
hauteur).

Légende pour l’ensemble des éléments

Libellé bouton radio

Libellé bouton radio

Libellé bouton radio

###  Extrait de code

    
    
                          <fieldset class="fr-fieldset" id="radio-small" aria-labelledby="radio-small-legend radio-small-messages">
        <legend class="fr-fieldset__legend--regular fr-fieldset__legend" id="radio-small-legend">
            Légende pour l’ensemble des éléments
        </legend>
        <div class="fr-fieldset__element">
            <div class="fr-radio-group fr-radio-group--sm">
                <input type="radio" id="radio-small-1" name="radio-small">
                <label class="fr-label" for="radio-small-1">
                    Libellé bouton radio
                </label>
            </div>
        </div>
        <div class="fr-fieldset__element">
            <div class="fr-radio-group fr-radio-group--sm">
                <input checked type="radio" id="radio-small-2" name="radio-small">
                <label class="fr-label" for="radio-small-2">
                    Libellé bouton radio
                </label>
            </div>
        </div>
        <div class="fr-fieldset__element">
            <div class="fr-radio-group fr-radio-group--sm">
                <input type="radio" id="radio-small-3" name="radio-small">
                <label class="fr-label" for="radio-small-3">
                    Libellé bouton radio
                </label>
            </div>
        </div>
        <div class="fr-messages-group" id="radio-small-messages" aria-live="assertive">
        </div>
    </fieldset>
                          
                        

## Règles d’utilisation

### Usage

Les boutons radios sont recommandés lorsque l’utilisateur doit choisir un
élément parmi 2 à 5 choix possibles :

  * Au delà de 5 choix ou lorsque l’espace n’est pas suffisant, il est préférable d'utiliser une [liste déroulante](/elements-d-interface/composants/liste-deroulante).
  * Si plusieurs choix sont possibles ou que la sélection n’est pas obligatoire, privilégier les cases à cocher.

### Élément obligatoire

Ajoutez un astérisque à la fin du libellé de la balise `legend `pour informer
qu’un élément est obligatoire. Une légende explicative (“les champs
obligatoires sont marqués d’un *”) doit être présente en haut du formulaire.
Si l’ensemble des éléments est obligatoire, indiquez-le au début du
formulaire.

À noter, pour les autres éléments de formulaires vous pouvez consulter les
composants [champs de saisie](/elements-d-interface/composants/champ-de-
saisie), [liste déroulante](/elements-d-interface/composants/liste-
deroulante), [barre de recherche](/elements-d-interface/composants/barre-de-
recherche) et [case à cocher](/elements-d-interface/composants/case-a-cocher).

### Accessibilité :

  * Les boutons radios doivent être regroupés dans une balise fieldset. 
  * Une balise legend doit être présente car elle constitue l’en-tête du groupe de bouton.
  * Chaque bouton radio est lié à son libellé grâce aux attributs id et for (ex : <input id=”radio-01”><label for=”radio-01”>).
  * Les messages d'erreur ou de succès, s'ils sont présents, sont liés au groupe de boutons radio au niveau de la balise <fieldset>, par un role="group" et une liaison avec aria-labelledby qui référence la légende et le message.

### Contenus :

Pour les titres (legend) et les libellés (label) :

  * Maintenir la cohérence : utilisez les mêmes termes à chaque fois. 
  * Utiliser un libellé clair et concis.
  * Mettre uniquement la première lettre du libellé en majuscule, n’utilisez pas de ponctuation à la fin d’un libellé.
  * Un texte d’aide clarifie la nature du contenu attendu - si cette information est essentielle, éviter de la masquer dans un tooltip ou infobox.

### Personnalisation

Le style de ce composant n’est pas personnalisable. Toutefois, certains
éléments sont optionnels - voir la structure du composant.

### Besoin d'aide ?

L'équipe du DSFR est là pour vous aider.

Retrouvez-la sur :

  * [la communauté slack](https://gouvfr.slack.com/ "la communauté slack - nouvelle fenêtre") pour poser vos questions, et échanger avec d’autres utilisateurs.   
Vous êtes **agent de l’État** et souhaitez accéder au slack ? [Rejoignez la
communauté](https://gouvfr.atlassian.net/servicedesk/customer/portal/1/group/1/create/9
"Rejoignez la communauté - nouvelle fenêtre") dès maintenant !

  * [ le centre de support](https://gouvfr.atlassian.net/servicedesk/customer/portals "le centre de support - nouvelle fenêtre") pour envoyer vos demandes de correctifs et d'évolution.

[Bouton FranceConnect](/composants-et-modeles/composants/bouton-franceconnect)

[Bouton radio riche - Radio rich](/composants-et-modeles/composants/bouton-
radio-riche)

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
