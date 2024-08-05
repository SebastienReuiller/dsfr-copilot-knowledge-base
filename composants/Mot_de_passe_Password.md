Fermer

# Mot de passe - Password

Le composant “mot de passe” permet d’aider un utilisateur à créer ou saisir un
mot de passe. Il doit être utilisé lorsque votre service nécessite de demander
à l’utilisateur de créer ou saisir un mot de passe, notamment dans les cas de
création de compte ou de connexion. Des modèles de page pour ces deux usages
sont à disposition : page de création de compte et page de connexion .

Ce composant se base sur le champs de saisie de type “password” et se décline
en deux variantes couvrant les deux cas d’usages de référence :

  * la demande de mot de passe pour la création d’un compte
  * la demande de mot de passe pour la connexion

## Structure du champ mot de passe

Ce composant utilise un champ de saisie classique et s’adapte en fonction du
contexte de demande d’adresse électronique. Le champ dédié au mot de passe
voit sa description être dynamique fonction du contenu saisi se placer sous le
champ. Il est composé des éléments suivants:

Le champ mot de passe est composé des éléments suivant :

  * un label - obligatoire, “Mot de passe”
  * un texte de description - optionnelle, à remplir pour préciser les règles de sécurisation notamment dans les cas de création de compte
  * un champ input “password” - obligatoire
  * une fonctionnalité d’affichage du mot de passe - obligatoire, au clic permet d’afficher en clair les caractères saisis dans le champ

La demande de mot de passe aide l’utilisateur grâce au champ “mot de passe”
car :

  * il permet à l’utilisateur de saisir le mot de passe via un “coller” dans le champ
  * il cache le mot de passe, et donne la possibilité à l’utilisateur de l'afficher au besoin
  * il montre le dernier caractère saisi sur certains navigateurs
  * il autorise la saisie de long mot de passe sans avoir de de nombre caractères maximum

## Création ou modification de mot de passe associé à un compte.

### Par défaut

Dans ce contexte, il est demandé à l’utilisateur de créer un mot de passe
soumis à des contraintes de règles de sécurisation. Pour aider l’utilisateur,
il faut utiliser le texte de description pour préciser les règles à respecter,
et les éventuels formats attendus (longueurs, utilisation de caractères et de
casse spécifiques, etc.) Le champ dédié au mot de passe voit sa description
dynamique fonction du contenu saisi se placer sous le champ.

Mot de passe Texte de description additionnel

Votre mot de passe doit contenir :

12 caractères minimum

1 caractère spécial minimum

1 chiffre minimum

Afficher

###  Extrait de code

    
    
                          <div class="fr-password" id="password-1138">
        <label class="fr-label" for="password-1138-input">
            Mot de passe
            <span class="fr-hint-text">Texte de description additionnel</span>
        </label>
        <div class="fr-input-wrap">
            <input class="fr-password__input fr-input" aria-describedby="password-1138-input-messages" aria-required="true" name="password" autocomplete="new-password" id="password-1138-input" type="password">
        </div>
        <div class="fr-messages-group" id="password-1138-input-messages" aria-live="assertive">
            <p class="fr-message" id="password-1138-input-message">Votre mot de passe doit contenir :</p>
            <p class="fr-message fr-message--info" id="password-1138-input-message-info">12 caractères minimum</p>
            <p class="fr-message fr-message--info" id="password-1138-input-message-info-1">1 caractère spécial minimum</p>
            <p class="fr-message fr-message--info" id="password-1138-input-message-info-2">1 chiffre minimum</p>
        </div>
        <div class="fr-password__checkbox fr-checkbox-group fr-checkbox-group--sm">
            <input aria-label="Afficher le mot de passe" id="password-1138-show" type="checkbox" aria-describedby="password-1138-show-messages">
            <label class="fr-password__checkbox fr-label" for="password-1138-show">
                Afficher
            </label>
            <div class="fr-messages-group" id="password-1138-show-messages" aria-live="assertive">
            </div>
        </div>
    </div>
                          
                        

### Message d’erreur

Dans le cas d’erreur de saisie, il faut reprendre l’affichage d’erreur du
champ input, et préciser dans le texte le type d’erreur rencontré en fonction
des règles de sécurisation (exemple : “le mot de passe doit comporter au moins
un chiffre”, etc.).

Un modèle de page de création de compte est à disposition.

## Demande de mot de passe pour la connexion

### Par défaut

Dans ce contexte, il est demandé à l’utilisateur de rentrer son mot de passe
pour se connecter. Un lien vers la page de récupération de mot de passe doit
être placé en dessous.

Mot de passe

Afficher

Mot de passe oublié ?

###  Extrait de code

    
    
                          <div class="fr-password" id="password-1144">
        <label class="fr-label" for="password-1144-input">
            Mot de passe
        </label>
        <div class="fr-input-wrap">
            <input class="fr-password__input fr-input" aria-describedby="password-1144-input-messages" aria-required="true" name="password" autocomplete="current-password" id="password-1144-input" type="password">
        </div>
        <div class="fr-messages-group" id="password-1144-input-messages" aria-live="assertive">
        </div>
        <div class="fr-password__checkbox fr-checkbox-group fr-checkbox-group--sm">
            <input aria-label="Afficher le mot de passe" id="password-1144-show" type="checkbox" aria-describedby="password-1144-show-messages">
            <label class="fr-password__checkbox fr-label" for="password-1144-show">
                Afficher
            </label>
            <div class="fr-messages-group" id="password-1144-show-messages" aria-live="assertive">
            </div>
        </div>
        <p>
            <a href="#[À MODIFIER - url de la page de récupération]" class="fr-link">Mot de passe oublié ?</a>
        </p>
    </div>
                          
                        

### Messages d’erreur

Dans le cas d’erreur de saisie, il est préférable de ne pas reprendre
l’affichage d’erreur du champ input ‘inviduel’, afin de ne pas indiquer
l’origine de l’erreur (entre l’identifiant ou le mot de passe).

Il faut utiliser dans ce cas le bloc alerte et mettre un message spécifiant
une erreur globale à l’identification, par exemple: “le couple mot de
passe/identifiant saisi n’est pas correct” ou “Erreur d'identification Merci
de vérifier votre email et votre mot de passe”.

Un modèle de page de connexion avec bloc alerte erreur est à disposition.

## Bonnes pratiques

### Règles de sécurisation du mot de passe :

  * Bien s’assurer que le niveau de contrainte suit le besoin de sécurité de votre service pour ne pas rendre la saisie difficile si cela ne le nécessite pas
  * [ Guide des règles de sécurisation de mot de passe de l’ANSSI ](https://www.ssi.gouv.fr/guide/mot-de-passe/ " Guide des règles de sécurisation de mot de passe de l’ANSSI  - nouvelle fenêtre")  

### Changement de mot de passe :

  * Certains services peuvent parfois demander à leurs utilisateurs de changer de mots de passe tous les trimestres, il faut éviter cette pratique car cela complexifie la mémorisation pour l’utilisateur et donc l’accès à votre service. Cette recommandation est à adapter selon les contraintes de sécurité auxquelles votre service est soumis.
  * Si un système de récupération de mot de passe est mis en place, veillez à ne jamais envoyer de mot de passe en clair par courriel ou autre: diriger l’utilisateur vers un formulaire temporaire lui permettant de mettre à jour son mot de passe. 

### Accessibilité

  * [Reprendre les éléments d'accessibilité liés au composant champ de saisie](/elements-d-interface/composants/champ-de-saisie)
  * Utiliser l’attribut autocomplete="new-password" pour la création et autocomplete="current-password" pour la connexion.

[Modale - Modal](/composants-et-modeles/composants/modale)

[Navigation principale - Navigation](/composants-et-
modeles/composants/navigation-principale)

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
