Fermer

# Liste déroulante - Select

La liste déroulante permet à un utilisateur de choisir un élément dans une
liste donnée.

## Liste déroulante simple

La liste déroule fournit une liste d’option parmi laquelle l’utilisateur peut
choisir. Seule la partie visible du composant est stylisé : la liste d’option
déroulée conserve le style du navigateur.

### Structure

La liste déroulante se compose des éléments suivants:

  * une liste, composée d’un ensemble d’options sélectionnables - obligatoire.
  * un label - obligatoire.
  * une description additionnelle- optionnelle
  * un message d’erreur ou de succès - obligatoire si un changement d'état doit être notifié à l’utilisateur.

Label pour liste déroulante  Sélectionner une option Option 1 Option 2 Option
3 Option 4

###  Extrait de code

    
    
                          <div class="fr-select-group">
      <label class="fr-label" for="select">
        Label pour liste déroulante
      </label>
      <select class="fr-select" id="select" name="select">
        <option value="" selected disabled hidden>Sélectionner une option</option>
        <option value="1">Option 1</option>
        <option value="2">Option 2</option>
        <option value="3">Option 3</option>
        <option value="4">Option 4</option>
      </select>
    </div>
                          
                        

Note : les attributs disabled et hidden, permettent que l’option sélectionnée
par défaut n’apparaisse pas dans la liste de choix. Vous pouvez selon vos
besoins modifier ce comportement en supprimant des attributs.

### État d'erreur

L'état d’erreur est signalé par un changement de couleur et par l’apparition
d'un message d’erreur en-dessous du composant (cf. couleurs fonctionnelles :
le rouge est la couleur de l’état erreur).

Label pour liste déroulante  Sélectionner une option Option 1 Option 2 Option
3 Option 4

Texte d’erreur obligatoire

###  Extrait de code

    
    
                          <div class="fr-select-group fr-select-group--error">
      <label class="fr-label" for="select-error">
        Label pour liste déroulante
      </label>
      <select class="fr-select fr-select--error" aria-describedby="select-error-desc-error" id="select-error" name="select-error">
        <option value="" selected disabled hidden>Sélectionner une option</option>
        <option value="1">Option 1</option>
        <option value="2">Option 2</option>
        <option value="3">Option 3</option>
        <option value="4">Option 4</option>
      </select>
      <p id="select-error-desc-error" class="fr-error-text">
        Texte d’erreur obligatoire
      </p>
    </div>
                          
                        

### État de succès

L'état succès est signalé par un changement de couleur et par l’apparition
d'un message de succès en-dessous du composant (cf. couleurs fonctionnelles :
le vert est la couleur de l’état erreur).  
Le message et le label sont liés par leurs attribut id et aria-describedby.  

Label pour liste déroulante  Sélectionner une option Option 1 Option 2 Option
3 Option 4

Texte de validation

###  Extrait de code

    
    
                          <div class="fr-select-group fr-select-group--valid">
      <label class="fr-label" for="select-valid">
        Label pour liste déroulante
      </label>
      <select class="fr-select fr-select--valid" aria-describedby="select-valid-desc-valid" id="select-valid" name="select-valid">
        <option value="" selected disabled hidden>Sélectionner une option</option>
        <option value="1">Option 1</option>
        <option value="2">Option 2</option>
        <option value="3">Option 3</option>
        <option value="4">Option 4</option>
      </select>
      <p id="select-valid-desc-valid" class="fr-valid-text">
        Texte de validation
      </p>
    </div>
                          
                        

### État désactivé

L'état désactivé indique que utilisateur ne peut pas interagir avec l'élément.  
Cet état peut être utilisée pour empêcher l'utilisateur d'interagir avec la
liste jusqu'à ce qu'une autre action soit terminée.  

Label pour liste déroulante  Sélectionner une option Option 1 Option 2 Option
3 Option 4

###  Extrait de code

    
    
                          <div class="fr-select-group fr-select-group--disabled">
      <label class="fr-label" for="select-disabled">
        Label pour liste déroulante
      </label>
      <select class="fr-select" disabled id="select-disabled" name="select-disabled">
        <option value="" selected disabled hidden>Sélectionner une option</option>
        <option value="1">Option 1</option>
        <option value="2">Option 2</option>
        <option value="3">Option 3</option>
        <option value="4">Option 4</option>
      </select>
    </div>
                          
                        

## Liste déroulante avec texte d’aide

Il est recommandé d’ajouter un texte d’aide sous le libellé afin de faciliter
le choix de l’utilisateur. Il s’affiche sous le libellé du champ.

Label pour liste déroulante Texte de description additionnel Sélectionner une
option Option 1 Option 2 Option 3 Option 4

###  Extrait de code

    
    
                          <div class="fr-select-group">
        <label class="fr-label" for="select-hint">Label pour liste déroulante
            <span class="fr-hint-text">Texte de description additionnel</span>
        </label>
        <select class="fr-select" id="select-hint" name="select-hint">
            <option value="" selected disabled hidden>Sélectionner une option</option>
            <option value="1">Option 1</option>
            <option value="2">Option 2</option>
            <option value="3">Option 3</option>
            <option value="4">Option 4</option>
        </select>
    </div>
                          
                        

## Règles d’utilisation

### Usage

Les listes déroulantes sont à utiliser lorsqu'un utilisateur doit choisir
entre 6 et 15 options possibles et que vous avez un espace limité pour
afficher les options.Éviter d’utiliser la liste déroulante lorsqu’elle
comporte peu de proposition et privilégier dans ce cas [les boutons
radio](/elements-d-interface/composants/bouton-radio), dont la compréhension
est plus simple pour les utilisateurs.

Pour les choix multiples, il est conseillé d’utiliser [des cases à
cocher](/elements-d-interface/composants/case-a-cocher) plus simples à
utiliser que l’option multiple de la liste déroulante (nécessitant une
combinaison avec la touche ctrl).

Ajoutez un astérisque au titre pour informer qu’un élément est obligatoire,
avec une légende en haut ou en bas du formulaire. Si l’ensemble des éléments
sont obligatoires, indiquez le au début du formulaire.

#### Les autres éléments pour construire un formulaire

pour les autres éléments de formulaires, vous pouvez consulter les composants
barre de recherche, bouton radio , champs de saisie, case à cocher

[Lien d'évitement - Skiplink](/composants-et-modeles/composants/lien-d-
evitement)

[Menu latéral - Sidemenu](/composants-et-modeles/composants/menu-lateral)

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
