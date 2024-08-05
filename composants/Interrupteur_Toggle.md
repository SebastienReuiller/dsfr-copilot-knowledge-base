Fermer

# Interrupteur - Toggle

Le composant “Interrupteur” permet à l’utilisateur de faire un choix entre
deux états opposés (activé / désactivé).

## Interrupteur

L’usage des interrupteurs est à privilégier pour paramétrer des
fonctionnalités transverses (exemple : activation / désactivation des cookies)
Le changement d'état de l’interrupteur a un effet immédiat (il ne nécessite
pas de validation).

### Structure

L’interrupteur par défaut se compose des éléments suivants:

  * un bouton permettant de basculer entre les deux états - obligatoire.
  * un label, placé à gauche ou à droite - obligatoire.
  * un texte “état” décrivant l'état de l’interrupteur (activé / désactivé), placé en dessous du bouton”. Il est conseillé de le mettre afin de faciliter la compréhension de l’utilisateur - optionnel.
  * une description, placée en dessous du label - optionnelle.
  * un séparateur horizontal - optionnel.

**Attention** : Veillez à ce que le l’interrupteur et son label soient
visuellement proches ([critère 11.4 du
RGAA)](https://accessibilite.numerique.gouv.fr/methode/criteres-et-tests/#11.4
"critère 11.4 du RGAA\) - nouvelle fenêtre") . Idéalement, essayez de
conserver l'interrupteur à gauche et son libellé à droite sans trop d'espace
entre. Autrement, les utilisateurs qui naviguent avec une loupe d'écran
pourraient ne pas faire le lien.  

#### Exemple d’interrupteur avec label à droite

Libellé de l'interrupteur

    
    
                    <div class="fr-toggle">
        <input type="checkbox" class="fr-toggle__input" aria-describedby="toggle-4633-messages" id="toggle-4633">
        <label class="fr-toggle__label" for="toggle-4633">Libellé de l'interrupteur</label>
        <div class="fr-messages-group" id="toggle-4633-messages" aria-live="polite">
        </div>
    </div>
                    
                  

#### Exemple d’interrupteurs avec label à gauche

Il est possible d’afficher le label à droite de l’interrupteur, en utilisant
le modificateur fr-toggle--label-left .

Libellé de l'interrupteur

    
    
                    <div class="fr-toggle fr-toggle--label-left">
        <input type="checkbox" class="fr-toggle__input" aria-describedby="toggle-4693-messages" id="toggle-4693">
        <label class="fr-toggle__label" for="toggle-4693">Libellé de l'interrupteur</label>
        <div class="fr-messages-group" id="toggle-4693-messages" aria-live="polite">
        </div>
    </div>
                    
                  

## Groupe d’interrupteurs

L’interrupteur peut également être utilisé en groupe, afin de rassembler une
liste d’actions de même nature. Lorsqu’il est utilisé en groupe,
l’interrupteur doit respecter le même format. Si le premier interrupteur
affiche l'état ou le séparateur optionnel, alors l’ensemble des interrupteurs
du groupe devront également afficher ces éléments.

#### Exemple de groupe d’interrupteurs avec label à droite

Légende pour l’ensemble des éléments

  * Libellé de l'interrupteur

Texte de description additionnel

  * Libellé de l'interrupteur

Texte de description additionnel

  * Libellé de l'interrupteur

Texte de description additionnel

  * Libellé de l'interrupteur

Texte de description additionnel

  * Libellé de l'interrupteur

Texte de description additionnel

    
    
                    <fieldset class="fr-fieldset" id="toggle-group-4684" aria-labelledby="toggle-group-4684-legend toggle-group-4684-messages">
        <legend class="fr-fieldset__legend" id="toggle-group-4684-legend">
            Légende pour l’ensemble des éléments
        </legend>
        <div class="fr-fieldset__element">
            <ul class="fr-toggle__list">
                <li>
                    <div class="fr-toggle fr-toggle--border-bottom">
                        <input type="checkbox" class="fr-toggle__input" aria-describedby="group-5-toggle-hint-0-hint-text toggle-hint-0-messages" id="group-5-toggle-hint-0">
                        <label class="fr-toggle__label" for="group-5-toggle-hint-0" data-fr-checked-label="Activé" data-fr-unchecked-label="Désactivé">Libellé de l'interrupteur</label>
                        <p class="fr-hint-text" id="group-5-toggle-hint-0-hint-text">Texte de description additionnel</p>
                        <div class="fr-messages-group" id="toggle-hint-0-messages" aria-live="polite">
                        </div>
                    </div>
                </li>
                <li>
                    <div class="fr-toggle fr-toggle--border-bottom">
                        <input type="checkbox" class="fr-toggle__input" aria-describedby="group-5-toggle-hint-1-hint-text toggle-hint-1-messages" id="group-5-toggle-hint-1">
                        <label class="fr-toggle__label" for="group-5-toggle-hint-1" data-fr-checked-label="Activé" data-fr-unchecked-label="Désactivé">Libellé de l'interrupteur</label>
                        <p class="fr-hint-text" id="group-5-toggle-hint-1-hint-text">Texte de description additionnel</p>
                        <div class="fr-messages-group" id="toggle-hint-1-messages" aria-live="polite">
                        </div>
                    </div>
                </li>
                <li>
                    <div class="fr-toggle fr-toggle--border-bottom">
                        <input type="checkbox" class="fr-toggle__input" aria-describedby="group-5-toggle-hint-2-hint-text toggle-hint-2-messages" id="group-5-toggle-hint-2">
                        <label class="fr-toggle__label" for="group-5-toggle-hint-2" data-fr-checked-label="Activé" data-fr-unchecked-label="Désactivé">Libellé de l'interrupteur</label>
                        <p class="fr-hint-text" id="group-5-toggle-hint-2-hint-text">Texte de description additionnel</p>
                        <div class="fr-messages-group" id="toggle-hint-2-messages" aria-live="polite">
                        </div>
                    </div>
                </li>
                <li>
                    <div class="fr-toggle fr-toggle--border-bottom">
                        <input type="checkbox" class="fr-toggle__input" aria-describedby="group-5-toggle-hint-3-hint-text toggle-hint-3-messages" id="group-5-toggle-hint-3">
                        <label class="fr-toggle__label" for="group-5-toggle-hint-3" data-fr-checked-label="Activé" data-fr-unchecked-label="Désactivé">Libellé de l'interrupteur</label>
                        <p class="fr-hint-text" id="group-5-toggle-hint-3-hint-text">Texte de description additionnel</p>
                        <div class="fr-messages-group" id="toggle-hint-3-messages" aria-live="polite">
                        </div>
                    </div>
                </li>
                <li>
                    <div class="fr-toggle fr-toggle--border-bottom">
                        <input type="checkbox" class="fr-toggle__input" aria-describedby="group-5-toggle-hint-4-hint-text toggle-hint-4-messages" id="group-5-toggle-hint-4">
                        <label class="fr-toggle__label" for="group-5-toggle-hint-4" data-fr-checked-label="Activé" data-fr-unchecked-label="Désactivé">Libellé de l'interrupteur</label>
                        <p class="fr-hint-text" id="group-5-toggle-hint-4-hint-text">Texte de description additionnel</p>
                        <div class="fr-messages-group" id="toggle-hint-4-messages" aria-live="polite">
                        </div>
                    </div>
                </li>
            </ul>
        </div>
        <div class="fr-messages-group" id="toggle-group-4684-messages" aria-live="polite">
        </div>
    </fieldset>
                    
                  

#### Exemple de groupe d’interrupteurs avec label à gauche

Légende pour l’ensemble des éléments

  * Libellé de l'interrupteur

Texte de description additionnel

  * Libellé de l'interrupteur

Texte de description additionnel

  * Libellé de l'interrupteur

Texte de description additionnel

  * Libellé de l'interrupteur

Texte de description additionnel

  * Libellé de l'interrupteur

Texte de description additionnel

    
    
                    <fieldset class="fr-fieldset" id="toggle-group-4726" aria-labelledby="toggle-group-4726-legend toggle-group-4726-messages">
        <legend class="fr-fieldset__legend" id="toggle-group-4726-legend">
            Légende pour l’ensemble des éléments
        </legend>
        <div class="fr-fieldset__element">
            <ul class="fr-toggle__list">
                <li>
                    <div class="fr-toggle fr-toggle--border-bottom fr-toggle--label-left">
                        <input type="checkbox" class="fr-toggle__input" aria-describedby="group-11-toggle-hint-0-hint-text toggle-hint-0-messages" id="group-11-toggle-hint-0">
                        <label class="fr-toggle__label" for="group-11-toggle-hint-0" data-fr-checked-label="Activé" data-fr-unchecked-label="Désactivé">Libellé de l'interrupteur</label>
                        <p class="fr-hint-text" id="group-11-toggle-hint-0-hint-text">Texte de description additionnel</p>
                        <div class="fr-messages-group" id="toggle-hint-0-messages" aria-live="polite">
                        </div>
                    </div>
                </li>
                <li>
                    <div class="fr-toggle fr-toggle--border-bottom fr-toggle--label-left">
                        <input type="checkbox" class="fr-toggle__input" aria-describedby="group-11-toggle-hint-1-hint-text toggle-hint-1-messages" id="group-11-toggle-hint-1">
                        <label class="fr-toggle__label" for="group-11-toggle-hint-1" data-fr-checked-label="Activé" data-fr-unchecked-label="Désactivé">Libellé de l'interrupteur</label>
                        <p class="fr-hint-text" id="group-11-toggle-hint-1-hint-text">Texte de description additionnel</p>
                        <div class="fr-messages-group" id="toggle-hint-1-messages" aria-live="polite">
                        </div>
                    </div>
                </li>
                <li>
                    <div class="fr-toggle fr-toggle--border-bottom fr-toggle--label-left">
                        <input type="checkbox" class="fr-toggle__input" aria-describedby="group-11-toggle-hint-2-hint-text toggle-hint-2-messages" id="group-11-toggle-hint-2">
                        <label class="fr-toggle__label" for="group-11-toggle-hint-2" data-fr-checked-label="Activé" data-fr-unchecked-label="Désactivé">Libellé de l'interrupteur</label>
                        <p class="fr-hint-text" id="group-11-toggle-hint-2-hint-text">Texte de description additionnel</p>
                        <div class="fr-messages-group" id="toggle-hint-2-messages" aria-live="polite">
                        </div>
                    </div>
                </li>
                <li>
                    <div class="fr-toggle fr-toggle--border-bottom fr-toggle--label-left">
                        <input type="checkbox" class="fr-toggle__input" aria-describedby="group-11-toggle-hint-3-hint-text toggle-hint-3-messages" id="group-11-toggle-hint-3">
                        <label class="fr-toggle__label" for="group-11-toggle-hint-3" data-fr-checked-label="Activé" data-fr-unchecked-label="Désactivé">Libellé de l'interrupteur</label>
                        <p class="fr-hint-text" id="group-11-toggle-hint-3-hint-text">Texte de description additionnel</p>
                        <div class="fr-messages-group" id="toggle-hint-3-messages" aria-live="polite">
                        </div>
                    </div>
                </li>
                <li>
                    <div class="fr-toggle fr-toggle--border-bottom fr-toggle--label-left">
                        <input type="checkbox" class="fr-toggle__input" aria-describedby="group-11-toggle-hint-4-hint-text toggle-hint-4-messages" id="group-11-toggle-hint-4">
                        <label class="fr-toggle__label" for="group-11-toggle-hint-4" data-fr-checked-label="Activé" data-fr-unchecked-label="Désactivé">Libellé de l'interrupteur</label>
                        <p class="fr-hint-text" id="group-11-toggle-hint-4-hint-text">Texte de description additionnel</p>
                        <div class="fr-messages-group" id="toggle-hint-4-messages" aria-live="polite">
                        </div>
                    </div>
                </li>
            </ul>
        </div>
        <div class="fr-messages-group" id="toggle-group-4726-messages" aria-live="polite">
        </div>
    </fieldset>
                    
                  

## Règles d’utilisation

### Usages

  * Si le label seul ne permet pas de comprendre l’action proposée, nous recommandons d’y associer une description
  * L'état inactif de l’interrupteur permet d’afficher un choix déjà effectué et/ou qui ne peut pas être modifié
  * La largeur du composant est définie par son emplacement dans la grille. 
  * Dans un groupe d’interrupteurs, toujours conserver la même typologie de composant (avec label à gauche ou à droite, avec ou sans texte d’état). 

### Accessibilité

  * Le libellé du champ doit être précis, sans ambiguïté et ne doit pas changer en fonction de l'état de l’interrupteur.
  * Dans le cas où une description est associée au label, les attributs aria-describedby et id sont utilisés.

### Contenus

  * Il est nécessaire que chaque label d’interrupteur soit clair et concis pour l’utilisateur
  * Un label d’interrupteur doit être concis (ne pas dépasser 3 mots si possible) 
  * Lorsque le label n’est pas suffisant pour comprendre l’action requise, il est nécessaire d’utiliser une description pour compléter le label
  * Il est possible d’accompagner ce composant d’un titre pour clarifier le cadre dans lequel il est utilisé.

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

[Infobulle - Tooltip](/composants-et-modeles/composants/infobulle)

[ Lettre d'information et réseaux sociaux - Newsletter and follow
us](/composants-et-modeles/composants/lettre-d-information-et-reseaux-sociaux)

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
