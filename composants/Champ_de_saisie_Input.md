Fermer

# Champ de saisie - Input

Les champs permettent à un utilisateur d'entrer du contenu et données. Le
champ simple est un champ de saisie libre, qui accepte une courte ligne de
contenu (texte ou/ et nombre). Le libellé se trouve au-dessus du champ de
saisie, pour faciliter la lecture.

### Structure

Le champ de saisie est composé des éléments suivants :

  * un champ - obligatoire.
  * un label, relié au champ - obligatoire.
  * une description additionnelle - optionnelle.
  * une icône, pouvant être modifiée (voir les icônes disponibles) - optionnelle.
  * un message d’erreur ou de succès - obligatoire si un changement d'état doit être notifié à l’utilisateur.

### État par défaut

Il est important de préciser pour ce libellé, un attribut `for` désignant
l’`id` du champ lié à celui-ci.

Label champ de saisie

    
    
                    <label class="fr-label" for="text-input-text">Label champ de saisie</label>
    <input class="fr-input" type="text" id="text-input-text" name="text-input-text">
                    
                  

### États erreur et succès

Ils sont signalés par le changement de couleur de la bordure (cf. couleurs
fonctionnelles) et l’apparition d’un message sous le champ, obligatoire pour
le cas d’erreur. Le message et le label sont liés par leurs attribut id et
aria-describedby.  

Label champs de saisie

Texte d’erreur obligatoire

Label champs de saisie

Texte de validation

    
    
                    <!-- Etat erreur -->
    <div class="fr-input-group fr-input-group--error">
        <label class="fr-label" for="text-input-error">
          Label champs de saisie
        </label>
        <input class="fr-input fr-input--error" aria-describedby="text-input-error-desc-error" type="text" id="text-input-error" name="text-input-error">
        <p id="text-input-error-desc-error" class="fr-error-text">
          Texte d’erreur obligatoire
        </p>
    </div>
    
    <!-- Etat validé -->
    <div class="fr-input-group fr-input-group--valid">
        <label class="fr-label" for="text-input-valid">
          Label champs de saisie
        </label>
        <input class="fr-input fr-input--valid" aria-describedby="text-input-valid-desc-valid" type="text" id="text-input-valid" name="text-input-valid">
        <p id="text-input-valid-desc-valid" class="fr-valid-text">
          Texte de validation
        </p>
    </div>
                    
                  

### État désactivé

L'état désactivé est utilisé lorsque le champ ne peut être utilisé. Il indique
que utilisateur ne peux pas saisir de contenu, par exemple jusqu'à ce qu'une
autre action soit terminée. Il ne doit être utilisé que très ponctuellement,
préférez masquer le champ si celui-ci n’est pas requis.

Label champs de saisie

    
    
                    <div class="fr-input-group fr-input-group--disabled">
        <label class="fr-label" for="text-input-disabled">Label champs de saisie</label>
        <input class="fr-input" disabled type="text" id="text-input-disabled" name="text-input-disabled">
    </div>
                    
                  

## Champ avec texte d’aide

Il est recommandé d’ajouter un texte d’aide sous le libellé afin de faciliter
la saisie.

Label champs de saisie Texte de description additionnel

    
    
                    <div class="fr-input-group">
        <label class="fr-label" for="text-input-groups1">Label champs de saisie
            <span class="fr-hint-text">Texte de description additionnel</span>
        </label>
        <input class="fr-input" type="text" id="text-input-groups1" name="text-input-groups1">
    </div>
                    
                  

## Zone de texte - textarea

Le champ “zone de texte” est un champ de saisie libre, qui accepte plus d’une
ligne de contenu (texte ou/ et nombre). Il reprend le style du champ simple et
augmente uniquement sa hauteur.

Label champs de saisie

    
    
                    <div class="fr-input-group">
        <label class="fr-label" for="textarea">
          Label champs de saisie
        </label>
        <textarea class="fr-input" id="textarea" name="textarea"></textarea>
    </div>
                    
                  

## Autres types de champs

À partir des éléments présentés ci-dessus, vous pouvez décliner les champs
selon vos besoins. Pour certains champs vous aurez besoin d’ajouter une icône
au sein du champ. Voici nos recommandations pour concevoir :

Libellé champs de saisie Texte de description additionnel

Libellé champs de saisie

Label champs de saisie

    
    
                    <!-- Champ avec icône -->
    <div class="fr-input-group">
        <label class="fr-label" for="text-input-icon">
            Libellé champs de saisie
            <span class="fr-hint-text">Texte de description additionnel</span>
        </label>
        <div class="fr-input-wrap fr-icon-alert-line">
            <input class="fr-input" aria-describedby="text-input-icon-messages" id="text-input-icon" type="text">
        </div>
        <div class="fr-messages-group" id="text-input-icon-messages" aria-live="assertive">
        </div>
    </div>
    
    <!-- Champ type date -->
    <div class="fr-input-group">
        <label class="fr-label" for="text-input-date">
            Libellé champs de saisie
        </label>
        <input class="fr-input" aria-describedby="text-input-date-messages" id="text-input-date" type="date">
        <div class="fr-messages-group" id="text-input-date-messages" aria-live="assertive">
        </div>
    </div>
    <!-- Champ type number -->
    <div class="fr-input-group">
      <label class="fr-label" for="text-input-number">
        Label champs de saisie
      </label>
      <input class="fr-input" pattern="[0-9]*" inputmode="numeric" type="number" id="text-input-number" name="text-input-number">
    </div>
                    
                  

Pour les champs de recherche, voir le composant “[barre de
recherche](/elements-d-interface/composants/barre-de-recherche)”.

## Règles d’utilisation

### Usage

#### Lecture et organisation :

  * Veillez à conserver le même libellé (label) pour les champs demandant la même information.
  * Un texte d’aide peut accompagner ce libellé pour clarifier notamment la nature du contenu attendu. Si un format précis est attendu il faut l’indiquer de la manière la plus claire possible et indiquer des exemples). 
  * Il ne faut pas cacher d’information dans un tooltip ou infobulle si ce contenu est essentiel pour saisir le champ.
  * Évitez l’utilisation de placeholder car il peut créer de la confusion chez l’utilisateur. Si toutefois vous souhaitez l’utiliser, il est nécessaire de respecter la couleur proposée afin de rester accessible, et son contenu doit présenter des informations non indispensables à la compréhension du champ. En aucun cas il ne peut remplacer un label et Il est uniquement à réserver pour des aides à la saisie secondaires : 

Url du site : Saisissez une url valide, commençant par https://

    
    
                    <div class="fr-input-group">
        <label class="fr-label" for="text-input-hint">Url du site :
            <span class="fr-hint-text">Saisissez une url valide, commençant par https://</span>
        </label>
        <input class="fr-input" type="text" placeholder="https://" id="text-input-hint" name="text-input-hint">
    </div>
                    
                  

  * L’oeil lit spontanément de bas en haut, afficher les champs en liste verticale pour faciliter la lecture et optimiser l’ergonomie.
  * La largeur des champs indique à l’utilisateur la quantité de contenu attendu. Par exemple, les champs de saisie des codes postaux doivent avoir une largeur plus petite que les champs des e-mails.

#### Champs obligatoires :

Ajoutez un astérisque au titre pour informer qu’un élément est obligatoire,
avec une légende en haut du formulaire. Si l’ensemble des éléments sont
obligatoires, indiquez le au début du formulaire.

#### Validation

  * Utilisez un un bouton primaire pour valider un champs de saisie ou un formulaire, le bouton secondaire sera utilisé pour réinitialiser le formulaire ou abandonner la saisie.
  * La soumission d'un champ doit être suivie d'un message indiquant la réussite ou non de l'action souhaitée.

### Accessibilité

Les règles d’accessibilité pour les champs sont :

  * Les champs dont la saisie est obligatoire sont signalés comme tels en l’indiquant au niveau de l'étiquette du champ de saisie et en utilisant l’attribut required.
  * Chaque champ possède une étiquette auquel il est lié grâce aux attributs id et for (ex : <input id=”champ-01”><label for=”champ-01”>).
  * Les champs de formulaire répétés et ayant la même fonction dans la page ou dans un ensemble de pages ont des libellés cohérents.
  * Les champs de même nature sont regroupés à l’aide d’une balise <fieldset> dont le rôle est décrit dans une balise <legend>.
  * Les instructions et indications du type de données attendues sont indiquées dans l’étiquette ou le passage de texte associé au champ préalablement à la validation du formulaire.
  * Pour chaque erreur de saisie, le type ou le format de donnée attendu est suggéré.
  * Pour les champs de saisie se rapportant à une information concernant l’utilisateur, un attribut autocomplete pourvu d’une valeur ([voir la liste des valeurs possibles](https://www.numerique.gouv.fr/publications/rgaa-accessibilite/methode-rgaa/glossaire/#champ-de-saisie-de-formulaire)) doit être ajouté sur la balise. ([RGAA critère 11.13](https://www.numerique.gouv.fr/publications/rgaa-accessibilite/methode-rgaa/criteres/#crit-11-13)).

### Personnalisation

Le style de ce composant n’est pas personnalisable. Toutefois, certains
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

[Carte - Card](/composants-et-modeles/composants/carte)

[Citation - Quote](/composants-et-modeles/composants/citation)

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
