Fermer

# Bouton - Button

Le bouton est un élément d’interaction avec l’interface permettant à
l’utilisateur d’effectuer une action.

## Structure

Les boutons sont composés de :

  * Un label - obligatoire.
  * Une icône, pouvant être modifiée (voir l[es icônes disponibles](/elements-d-interface/fondamentaux-techniques/icone)) - optionnelle.

## Boutons primaire

Le bouton primaire est utilisé pour les actions principales comme soumettre un
formulaire ou rediriger vers un contenu que l’on souhaite prioriser dans le
parcours utilisateur.

Label bouton

    
    
                    <button class="fr-btn">
        Label bouton
    </button>
                    
                  

**Usages :**

  * Il est nécessaire de bien différencier les boutons des liens. Un bouton permet de déclencher une action dans la même page. Un lien permet à votre utilisateur de naviguer à l'intérieur (ou à l’extérieur) de votre site (ex : retour en arrière, en savoir plus, fil d’Ariane) ou de se déplacer dans la page (ancre).
  * Pour être efficace et hiérarchiser les actions proposées à l’utilisateur, limiter l'usage du bouton primaire à 1 par écran et n'utilisez jamais deux boutons primaires côte à côte. Vous pouvez aligner un bouton primaire avec un bouton secondaire ou lien.

## Boutons secondaires

Le bouton secondaire est utilisé lorsque l’action est moins prioritaire que
l'action principale, comme réinitialiser les valeurs d’un formulaire.

Label bouton

    
    
                    <button class="fr-btn fr-btn--secondary">
        Label bouton
    </button>
                    
                  

## Bouton tertiaire

Le bouton tertiaire est réservé pour des actions contextuelles ou alternatives
: fermeture de modale, annuler, réinitialiser, partager, suivre sur un réseau
social, copier un lien.  
Rappel : le bouton est utilisé pour déclencher une action alors que le lien
est utiliser pour naviguer (au sein de la page, vers une autre page).

Le bouton tertiaire est caractérisé par un fond transparent et soit une
absence de contour, soit un contour $border-default-grey.  
La présence ou non de contour gris ne doit pas indiquer de hiérarchie entre
deux boutons tertiaire.

Label bouton  Label bouton

    
    
                    <button class="fr-btn fr-btn--tertiary">
        Label bouton
    </button>
    
    <button class="fr-btn fr-btn--tertiary-no-outline">
        Label bouton
    </button>
                    
                  

## État désactivé

L'état désactivé indique que l'utilisateur ne peut pas interagir avec le
bouton. Il ne doit être utilisé que très ponctuellement. Par exemple,
lorsqu’on veut indiquer à l’utilisateur qu’il doit procéder à une action en
amont.

Bouton primaire désactivé  
  
Bouton secondaire désactivé  
  
Label bouton  
  
Label bouton

    
    
    <button class="fr-btn" disabled>
      Bouton primaire désactivé
    </button>
     
    <button class="fr-btn fr-btn--secondary" disabled>
       Bouton secondaire désactivé
    </button>
    
    <button class="fr-btn fr-btn--tertiary" disabled>
        Label bouton
    </button>
    
    <button class="fr-btn fr-btn--tertiary-no-outline" disabled>
        Label bouton
    </button>

## Boutons avec icônes

Il est possible d'ajouter une icône à votre bouton permettant une meilleure
compréhension de l’action. Pour cela il suffit d’utiliser la classe CSS de
l’icône ([voir la documentation des icônes](/elements-d-
interface/fondamentaux-techniques/icone))

Trois déclinaisons sont possibles, pour les boutons primaires et secondaires :

  * avec icône à droite
  * avec icône à gauche
  * icône seule : limitez l’usage de ces boutons. Ils peuvent être utilisés uniquement pour les actions récurrentes, et facilement identifiable (ex : engrenage pour les paramètres ou loupe pour la recherche). Ce button doit contenir un libellé, qui sera ainsi lu par les assi. L'attribut title reprenant l'intitulé du bouton peut être ajouté pour permettre l'affichage d'une infobulle.  

Label bouton  Label bouton  Label bouton  Label bouton  
  
Label bouton  Label bouton  Label bouton  Label bouton  
  
Label bouton  Label bouton  Label bouton  Label bouton

    
    
    <!-- Bouton  icône à gauche-->
    
    <button class="fr-btn fr-btn--icon-left fr-icon-checkbox-circle-line">
        Label bouton
    </button>
    
    
    <!-- Bouton icône à droite--> 
    
    <button class="fr-btn fr-btn--icon-right fr-icon-checkbox-circle-line">
        Label bouton
    </button>
    
    
    <!-- Bouton icône seule -->
    
    <button class="fr-btn  fr-icon-checkbox-circle-line" title="Label bouton">
       Label bouton
    </button>

## Tailles

Les boutons primaires et secondaires sont disponibles en 3 tailles :

  * SM pour Small, MD pour Medium, LG pour large.
  * La taille medium (MD) est la taille de bouton par défaut.
  * Les formats MD et LG sont à utiliser en priorité.
  * Le format SM pourra être utilisé pour créer certains composants, évitez de l’utiliser en mobile car la zone de “touch” sur écran tactile n’est pas suffisante.

Il est possible de modifier la taille des boutons à l'aide de classes
spécifiques (`modifiers`) à ajouter à la classe principale. La classe `.fr-btn
--lg` permet par exemple d'obtenir la taille “Large” (LG), `.fr-btn--sm` la
taillle “Small” (SM).

Label bouton SM  Label bouton MD (défaut)  Label bouton LG

    
    
                    <!-- bouton au format SM -->
    
    <button class="fr-btn fr-btn--sm fr-fi-checkbox-circle-line fr-btn--icon-left fr-btn--secondary">
       Label bouton SM
    </button>
     
    
    <button class="fr-btn fr-fi-checkbox-circle-line fr-btn--icon-left fr-btn--secondary">
       Label bouton MD (défaut)
    </button>
     
    
    <button class="fr-btn fr-btn--lg fr-fi-checkbox-circle-line fr-btn--icon-left fr-btn--secondary">
       Label bouton LG
    </button>
                    
                  

## Règles d’utilisation

### Usages

  * Il est nécessaire de bien différencier les boutons des liens. Un bouton permet de déclencher une action dans la même page. Un lien permet à votre utilisateur de naviguer à l'intérieur (ou à l’extérieur) de votre site (ex : retour en arrière, en savoir plus, fil d'Ariane) ou de se déplacer dans la page (ancre). 
  * Pour être efficace et hiérarchiser les actions proposées à l’utilisateur, limiter l'usage du bouton primaire à 1 par écran et n'utilisez jamais deux boutons primaires côte à côte. Vous pouvez aligner un bouton primaire avec un bouton secondaire ou lien.
  * La couleur bleu du bouton ne peut pas être modifiée : cette couleur est utilisée et sanctuarisée pour signaler une interaction sur les éléments principaux (cf. [couleurs](/elements-d-interface/fondamentaux-de-l-identite-de-l-etat/couleurs-utilisation-dans-le-dsfr)) du DSFR.

### Accessibilité

  * Il est nécessaire de bien différencier les boutons des liens. Lorsque l'action déclenchée agit sur la page elle-même il faut utiliser un bouton.
  * Le contraste entre la couleur de fond du bouton et du texte doit être de 4.5:1.
  * Les libellés doivent être explicites.
  * L’utilisation de l’attribut title (ou aria-label) doit être utilisé uniquement si l’intitulé du bouton n’est pas explicite (ce qui n’est pas recommandé).
  * Pour aria-label, la valeur utilisée doit reprendre l'intitulé visible (indispensable pour les utilisateurs en commande vocale).
  * Le focus (propriété outline) ne doit être ni dégradé ni supprimé.

Dans le cas d'un bouton “icône seule”, les règles spécifiques sont les
suivantes :

  * Ajouter un attribut title contenant la fonction du bouton.
  * Vérifier que la couleur de l'icône est suffisamment contrastée (rapport de 3:1) par rapport à la couleur du fond du bouton.
  * Si le bouton utilise plusieurs icônes de couleur différente pour symboliser plusieurs états, assurez-vous que le rapport de contraste entre les différentes couleurs est de 3:1 au moins.

### Contenus

Le libellé de bouton doit :  

  * commencer par un verbe, de préférence d’action qui exprime clairement ce qui va se passer pour l’utilisateur.
  * être court et compréhensible facilement : utiliser 3 mots maximum.

Il faut utiliser le même format d'écriture sur tout vos libellés de boutons
(Exemple : 1ère lettre en majuscule, le reste en minuscule, impératif).

### Personnalisation

Le style de ce composant n’est pas personnalisable.Toutefois, certains
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

### Voir aussi

#### [Groupe de boutons - Button group](/composants-et-
modeles/composants/groupe-de-boutons)

Les boutons dans le contexte d'un groupe suivent les même règles que le
composant bouton.

![](/uploads/thumbnail_composants_groupe_de_boutons_6db9a05d35.png)

[Barre de recherche - Search](/composants-et-modeles/composants/barre-de-
recherche)

[Groupe de boutons - Button group](/composants-et-modeles/composants/groupe-
de-boutons)

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
