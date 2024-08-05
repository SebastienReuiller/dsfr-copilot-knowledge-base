Fermer

# Alerte - Alert

Les alertes permettent d’attirer l’attention de l’utilisateur sur une
information sans interrompre sa tâche en cours.

L’alerte est disponible en deux tailles : taille médium (MD, par défaut) et
petite taille ‘SM’.

## Structure

L’alerte est composée des éléments suivants :

  * un titre - obligatoire sur la version MD, optionnel sur la version SM.
  * un pictogramme et une couleur - obligatoires.
  * un texte de description - optionnel sur la version MD, obligatoire sur la version SM.
  * une croix de fermeture - optionnelle.

Les alertes s’affichent de manière contextuelle dans une page/un formulaire,
lors d’interactions utilisateurs avec les messages de validation (exemple :
succès ou erreur suite à soumission d’un formulaire) ou lors d’événements
côté application/système (exemple : messages d'information, d’alerte, de
mise à jour…).

#### Pour les développeurs

Nous avons retiré l’attribut role="alert" des exemples de code pour les
alertes présentes au chargement de la page. En effet, l'élément avec un
role="alert" sont les premières choses lues par les technologies d'assistance.
De ce fait, le role="alert" doit être réservé aux alertes ajoutées
(/injectées) dynamiquement au cours de la navigation. Ex: alertes de
notification suite à une action utilisateur ou mise à jour d’une status.

## Types d’alerte

Il y a 4 types d'alerte permettant de donner des informations de différentes
natures  

### Erreur

L'alerte erreur est à utiliser quand il y a plusieurs erreurs dans un
formulaire, ou des erreurs bloquantes à remonter pour l’utilisateur.

### Erreur : titre du message

Description

    
    
                    <div class="fr-alert fr-alert--error">
        <h3 class="fr-alert__title">Erreur : titre du message</h3>
        <p>Description</p>
    </div>
                    
                  

### Succès

L'alerte information sert à indiquer à l’utilisateur qu’une action ou une
tâche a été terminée avec succès.

### Succès de l'envoi

Description

    
    
                    <div class="fr-alert fr-alert--success">
        <h3 class="fr-alert__title">Succès de l'envoi</h3>
        <p>Description</p>
    </div>
                    
                  

### Information

L'alerte information est à utiliser pour mettre en exergue des informations
importantes

### Information : titre du message

Description détaillée du message

    
    
                    <div class="fr-alert fr-alert--info">
        <h3 class="fr-alert__title">Information : titre du message</h3>
        <p>Description détaillée du message</p>
    </div>
                    
                  

### Attention

L'alerte 'attention' (warning) est à utiliser pour mettre en exergue des
risques ou points d’attention importants.

### Attention : titre du message

Description détaillée du message

    
    
                    <div class="fr-alert fr-alert--warning">
        <h3 class="fr-alert__title">Attention : titre du message</h3>
        <p>Description détaillée du message</p>
    </div>
                    
                  

Le composant doit être placé en première place du contenu auquel il est
associé (en haut d’une page, d’un formulaire, d’un container…).

#### Pour les développeurs

Le titre, matérialisé par la classe fr-alert__title est par défaut une balise
h3, mais vous pouvez choisir le niveau de titre convenant à l'arborescence de
votre page (de h2 à h6).

## Tailles disponibles

L’alerte existe en deux tailles, Small et Medium, à utiliser en fonction de
l’espace d’affichage disponible.

### Alerte ‘small’ (SM)

L’alerte small est à utiliser lorsque l’espace d’affichage est réduit.

Information : titre de l'information

Information : titre de l'information

Information : titre de l'information

    
    
    <div class="fr-alert fr-alert--info fr-alert--sm">
        <p>Information : titre de l'information</p>
    </div>
    
    <div class="fr-alert fr-alert--success fr-alert--sm">
        <p>Information : titre de l'information</p>
    </div>
    
    <div class="fr-alert fr-alert--error fr-alert--sm">
        <p>Information : titre de l'information</p>
    </div>

### Alertes ‘medium’ (MD)

L’alerte small est à utiliser lorsque l’espace d’affichage est important.

#### Alerte medium simple

L’alerte medium simple est à utiliser lors qu’un titre seul permet de donner
l’information à l’utilisateur.

### Erreur : description détaillée du message....

    
    
    <div class="fr-alert fr-alert--error">
        <h3 class="fr-alert__title">Erreur : description détaillée du message....</h3>
    </div>

#### Alertes medium avec description

L’alerte medium avec description permet de donner des informations
complémentaires à l’utilisateur, en plus du titre.

### Erreur : titre du message

Description détaillée du message Lorem ipsum dolor sit amet, consectetur
adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna
aliqua.

    
    
    <div class="fr-alert fr-alert--success">
        <h3 class="fr-alert__title">Erreur : titre du message</h3>
        <p>Description détaillée du message Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.</p>
    </div>

### Alertes avec bouton de fermeture

Il est possible d’ajouter un bouton de fermeture afin que l’utilisateur puisse
masquer l’alerte. La fermeture peut ou non être gérée par le javascript du
DSFR.

### Information Covid

Cliquer sur la croix pour fermer l'alerte

Masquer le message

###  Extrait de code

    
    
                          <div class="fr-alert fr-alert--info">
        <h3 class="fr-alert__title">Information Covid</h3>
        <p>Cliquer sur la croix pour fermer l'alerte</p>
        <button class="fr-btn--close fr-btn" title="Masquer le message" onclick="const alert = this.parentNode; alert.parentNode.removeChild(alert)">
            Masquer le message
        </button>
    </div>
                          
                        

Si vous souhaitez gérer vous-même la fermeture du bloc , l’alerte est
également disponible avec le bouton “fermer” sans le comportement javascript
associé, qui est à implémenter dans votre environnement :

### Information

Description

Masquer le message

Description

Masquer le message

###  Extrait de code

    
    
                          <div class="fr-alert fr-alert--success">
        <h3 class="fr-alert__title">Information</h3>
        <p>Description</p>
        <button class="fr-link--close fr-link">Masquer le message</button>
    </div>
    
    <div class="fr-alert fr-alert--success">
        <p>Description</p>
        <button class="fr-link--close fr-link">Masquer le message</button>
    </div>
                          
                        

## Règles d’utilisation

### Usages

  * Le message doit être écrit dans un langage compréhensible facilement. Il faut éviter le jargon. Idéalement, il doit contenir la nature du message porté par le composant (succès, erreur, information), l’icône et la couleur ne garantissent pas à elle seule la bonne compréhension du message pour la totalité des utilisateurs. 
  * Quand l'utilisateur doit faire une action en lien/suite à l’affichage d'une alerte, il faut rendre cette tâche aussi simple que possible en détaillant ce qui est attendu de la part de l’utilisateur dans la description.

### Accessibilité

  * La nature du message (erreur, succès, information) doit être clairement exprimée dans le titre de l’alerte. La couleur ou l’icône n’étant pas accessibles ou compréhensibles par tous les utilisateurs. 
  * Dans le cas où un bouton de fermeture est prévu, lorsque l'alerte est fermée, le focus doit être repositionné sur un élément pertinent dans la page.
  * Si l’alerte apparait en cours de navigation et qu’elle dispose d'un bouton fermer, ce dernier devra prendre le focus lors de son affichage.
  * Le titre de l’alerte - .fr-alert__title - est dans un élément <h3>. Vous pouvez remplacer cette balise par un titre <hx class=”fr-alert__title”> adapté à votre hiérarchie de contenu. 
  * Le bloc doit avoir l’attribut role=”alert” si il apparait dynamiquement en cours de navigation.  

### Contenus

  * Le titre de l'alerte doit être clair et concis.
  * Le texte de description de d'alerte doit détailler clairement l’information/le problème à l’utilisateur.
  * Le ton doit être courtois, il ne faut pas blâmer l’utilisateur, mais l’accompagner. 

### Besoin d'aide ?

L'équipe du DSFR est là pour vous aider.

Retrouvez-la sur :

  * [la communauté slack](https://gouvfr.slack.com/ "la communauté slack - nouvelle fenêtre") pour poser vos questions, et échanger avec d’autres utilisateurs.   
Vous êtes **agent de l’État** et souhaitez accéder au slack ? [Rejoignez la
communauté](https://gouvfr.atlassian.net/servicedesk/customer/portal/1/group/1/create/9
"Rejoignez la communauté - nouvelle fenêtre") dès maintenant !

  * [ le centre de support](https://gouvfr.atlassian.net/servicedesk/customer/portals "le centre de support - nouvelle fenêtre") pour envoyer vos demandes de correctifs et d'évolution.

[Ajout de fichier - Upload](/composants-et-modeles/composants/ajout-de-
fichier)

[Badge - Badge](/composants-et-modeles/composants/badge)

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
