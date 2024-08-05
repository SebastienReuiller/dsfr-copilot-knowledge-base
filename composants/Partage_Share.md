Fermer

# Partage - Share

Les boutons de partage permettent aux utilisateurs de partager facilement un
contenu qu’il consulte à d’autres utilisateur.

## Structure

Les composant permet à l’utilisateur de partager facilement un contenu via :

  * des liens de partages sur les réseaux sociaux
  * les métadonnées nécessaires au bon fonctionnement du partage sur les réseaux sociaux.
  * un bouton d’envoie par mail.
  * un bouton pour copier le lien du contenu dans le presse papier

Les boutons et les liens sont des boutons et liens icônes seules.

Le composant existe en deux versions, une version par défaut et une seconde
version lorsque les cookies ne sont pas activés.

## Partage par défaut

Le composant partage est composé de :

  * un texte « Partager la page : »
  * de lien(s) et de bouton(s) de partage sur les réseaux sociaux (Facebook et/ou Twitter et/ou Linked et/ou Instagram et/ou autre) , 
  * un bouton envoi par mail, optionnel
  * un bouton pour copier le lien, obligatoire

Il est recommandé de ne pas dépasser 5 éléments (3 liens pour les réseaux
sociaux et les deux boutons de partage), afin que le composant reste sur une
ligne.

Partager la page

  * [ Partager sur Facebook ](https://www.facebook.com/sharer.php?u=\[À MODIFIER - url de la page\] "\[À MODIFIER - Intitulé\] - nouvelle fenêtre")
  * [ Partager sur X (anciennement Twitter) ](https://twitter.com/intent/tweet?url=\[À MODIFIER - url de la page\]&text=\[À MODIFIER - titre ou texte descriptif de la page\]&via=\[À MODIFIER - via\]&hashtags=\[À MODIFIER - hashtags\] "\[À MODIFIER - Intitulé\] - nouvelle fenêtre")
  * [ Partager sur LinkedIn ](https://www.linkedin.com/shareArticle?url=\[À MODIFIER - url de la page\]&title=\[À MODIFIER - titre ou texte descriptif de la page\] "\[À MODIFIER - Intitulé\] - nouvelle fenêtre")
  * [ Partager par email ](mailto:?subject=\[À MODIFIER - objet du mail\]&body=\[À MODIFIER - titre ou texte descriptif de la page\] \[À MODIFIER - url de la page\] "\[À MODIFIER - Intitulé\] - nouvelle fenêtre")
  * Copier dans le presse-papier 

    
    
                    <div class="fr-share" id="share-7093">
        <p class="fr-share__title">Partager la page</p>
        <ul class="fr-btns-group">
            <li>
                <a class="fr-btn--facebook fr-btn" target="_blank" rel="noopener" title="[À MODIFIER - Intitulé] - nouvelle fenêtre" id="share-7094" onclick="window.open(this.href,'Partager sur Facebook','toolbar=no,location=yes,status=no,menubar=no,scrollbars=yes,resizable=yes,width=600,height=450'); event.preventDefault();" href="https://www.facebook.com/sharer.php?u=[À MODIFIER - url de la page]">
                    Partager sur Facebook
                </a>
            </li>
            <li>
                <!-- Les paramètres de la reqûete doivent être URI-encodés (ex: encodeURIComponent() en js) -->
                <a class="fr-btn--twitter-x fr-btn" target="_blank" rel="noopener" title="[À MODIFIER - Intitulé] - nouvelle fenêtre" id="share-7095" onclick="window.open(this.href,'Partager sur X (anciennement Twitter)','toolbar=no,location=yes,status=no,menubar=no,scrollbars=yes,resizable=yes,width=600,height=420'); event.preventDefault();" href="https://twitter.com/intent/tweet?url=[À MODIFIER - url de la page]&text=[À MODIFIER - titre ou texte descriptif de la page]&via=[À MODIFIER - via]&hashtags=[À MODIFIER - hashtags]">
                    Partager sur X (anciennement Twitter)
                </a>
            </li>
            <li>
                <a class="fr-btn--linkedin fr-btn" target="_blank" rel="noopener" title="[À MODIFIER - Intitulé] - nouvelle fenêtre" id="share-7096" onclick="window.open(this.href,'Partager sur LinkedIn','toolbar=no,location=yes,status=no,menubar=no,scrollbars=yes,resizable=yes,width=550,height=550'); event.preventDefault();" href="https://www.linkedin.com/shareArticle?url=[À MODIFIER - url de la page]&title=[À MODIFIER - titre ou texte descriptif de la page]">
                    Partager sur LinkedIn
                </a>
            </li>
            <li>
                <a class="fr-btn--mail fr-btn" target="_blank" rel="noopener external" title="[À MODIFIER - Intitulé] - nouvelle fenêtre" id="share-7097" href="mailto:?subject=[À MODIFIER - objet du mail]&body=[À MODIFIER - titre ou texte descriptif de la page] [À MODIFIER - url de la page]">
                    Partager par email
                </a>
            </li>
            <li>
                <button class="fr-btn--copy fr-btn" id="share-7098" onclick="navigator.clipboard.writeText(window.location).then(function() {alert('Adresse copiée dans le presse papier.')});">
                    Copier dans le presse-papier
                </button>
            </li>
        </ul>
    </div>
                    
                  

N’hésitez pas à nous contacter si vous avez besoin d’ajouter d’autres boutons
de réseaux sociaux.

### Partager par email

Le bouton de partage par mail est un lien ‘mail to’ ouvrant le logiciel de
messagerie installé sur le poste de l’utilisateur (comportement par défaut).
Vous pouvez si vous le souhaitez modifier son comportement afin qu’il colle
avec votre infrastructure (envoi de mail via un formulaire, etc.) . Veillez
alors à utiliser la balise adéquate (<a> si c’est un lien ou <button> pour
l’ouverture d’une modale ou autre interaction ).

## Boutons et liens de partage en version inactive

Le code d’intégration des boutons et liens de partage proposé ici sont de
simples liens externes vers les services de partage.

Si vous souhaitez utiliser les différentes intégrations (javascript) proposées
par les différents réseaux sociaux, vous devrez très probablement les intégrer
à votre gestionnaire de consentement afin de que l’utilisateur puisse accepter
ou non les cookies déposés.Par défaut, les services doivent être désactivés,
les boutons sont donc passés en inactifs et une mention d’information
s’affiche pour rediriger vers la modale de consentement.

Partager la page

Veuillez autoriser le dépôt de cookies pour partager sur Facebook, Twitter et
LinkedIn.

  * Partager sur Facebook 
  * Partager sur X (anciennement Twitter) 
  * Partager sur LinkedIn 
  * [ Partager par email ](mailto:?subject=\[À MODIFIER - objet du mail\]&body=\[À MODIFIER - titre ou texte descriptif de la page\] \[À MODIFIER - url de la page\] "\[À MODIFIER - Intitulé\] - nouvelle fenêtre")
  * Copier dans le presse-papier 

    
    
                    <div class="fr-share" id="share-7106">
        <p class="fr-share__title">Partager la page</p>
        <p class="fr-share__text">Veuillez <a href=#[À MODIFIER - url page autorisation cookies]>autoriser le dépôt de cookies</a> pour partager sur Facebook, Twitter et LinkedIn.</p>
        <ul class="fr-btns-group">
            <li>
                <a class="fr-btn--facebook fr-btn" id="share-7107" aria-disabled="true" role="link">
                    Partager sur Facebook
                </a>
            </li>
            <li>
                <a class="fr-btn--twitter-x fr-btn" id="share-7108" aria-disabled="true" role="link">
                    Partager sur X (anciennement Twitter)
                </a>
            </li>
            <li>
                <a class="fr-btn--linkedin fr-btn" id="share-7109" aria-disabled="true" role="link">
                    Partager sur LinkedIn
                </a>
            </li>
            <li>
                <a class="fr-btn--mail fr-btn" target="_blank" rel="noopener external" title="[À MODIFIER - Intitulé] - nouvelle fenêtre" id="share-7110" href="mailto:?subject=[À MODIFIER - objet du mail]&body=[À MODIFIER - titre ou texte descriptif de la page] [À MODIFIER - url de la page]">
                    Partager par email
                </a>
            </li>
            <li>
                <button class="fr-btn--copy fr-btn" id="share-7111" onclick="navigator.clipboard.writeText(window.location).then(function() {alert('Adresse copiée dans le presse papier.')});">
                    Copier dans le presse-papier
                </button>
            </li>
        </ul>
    </div>
                    
                  

## Méta données

Les meta données à placer dans la balise head pour gérer les informations de
partage sur les réseaux sociaux.

    
    
    <meta name="twitter:card" content="summary_large_image">
    <meta name="twitter:site" content="[À MODIFIER - @usernameTwitter]">
    <meta property="og:title" content="[À MODIFIER - Système de Design de l'État]">
    <meta property="og:description" content="[À MODIFIER - Développer vos sites et applications en utilisant des composants prêts à l'emploi, accessibles et ergonomiques]">
    <meta property="og:image" content="[À MODIFIER - https://systeme-de-design.gouv.fr/src/img/systeme-de-design.gouv.fr.jpg]">
    <meta property="og:type" content="website">
    <meta property="og:url" content="[À MODIFIER - https://systeme-de-design.gouv.fr/]">
    <meta property="og:site_name" content="[À MODIFIER - Site officiel du Système de Design de l'État]">
    <meta property="og:image:alt" content="[À MODIFIER - République Française - Système de Design de l'État]">
    <meta name="twitter:image:alt" content="[À MODIFIER - République Française - Système de Design de l'État]">

Élément  
| Valeur par défaut  
| Valeur(s) autorisée(s)  
  
---|---|---  
|  | Token | Classe css  
Bordure | $border-plain-blue-france  
Correspondance :  
Thème clair et sombre =  
$blue-france-main-525  
| $[couleur]-main (thèmes clair / sombre)  
exemples :  
$green-emeraude-main-632  
$brown-caramel-main-648  
  
  
| .fr-highlight--[couleur]  
.fr-highlight--green-emeraude  
.fr-highlight--brown-caramel  
  
## Règles d’utilisation

### Usages

Le composant peut être placé en haut ou en bas de page.

### Accessibilité

  * Les liens désactivés n’ont pas d’attribut href, et possèdent les attributs aria-disabled="true" role="link"
  * Il est nécessaire d'ajouter les attributs data-fr-valid et data-fr-error avec les textes correspondants à l'état (respectivement, en français, "validé" et "en erreur") et de les traduire suivant la langue.

### Ressources utiles

Vous trouverez ci-dessous des liens afin de tester et prévisualiser
l’apparence des partages dans différents réseaux sociaux:

  * Open Graph Check 
  * Facebook Sharing Debugger
  * Twitter Sharing debugger
  * LinkedIn Post Inspector

### Besoin d'aide ?

L'équipe du DSFR est là pour vous aider.

Retrouvez-la sur :

  * [la communauté slack](https://gouvfr.slack.com/ "la communauté slack - nouvelle fenêtre") pour poser vos questions, et échanger avec d’autres utilisateurs.   
Vous êtes **agent de l’État** et souhaitez accéder au slack ? [Rejoignez la
communauté](https://gouvfr.atlassian.net/servicedesk/customer/portal/1/group/1/create/9
"Rejoignez la communauté - nouvelle fenêtre") dès maintenant !

  * [ le centre de support](https://gouvfr.atlassian.net/servicedesk/customer/portals "le centre de support - nouvelle fenêtre") pour envoyer vos demandes de correctifs et d'évolution.

[Paramètre d'affichage - Display](/composants-et-modeles/composants/parametre-
d-affichage)

[Pied de page - Footer](/composants-et-modeles/composants/pied-de-page)

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
