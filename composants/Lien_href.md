Fermer

# Lien - Link

Le lien permet la navigation entre une page et un autre contenu au sein de la
même page, du même site ou externe.

Pour les actions d’un autre type, comme la soumission d’un formulaire, il faut
utiliser le composant bouton.

### Structure

un lien est composé des élements suivant:

  * un libellé - obligatoire.
  * une icône, placée à droite ou à gauche du texte visible ou seule - optionnelle.

## Lien au fil du texte

Ce lien se trouve au sein d’un texte et reprend les caractéristiques
typographiques de celui-ci (font, couleur, taille) tout en étant souligné. Il
peut être suivi d’une icône (par exemple : lien externe).

Lorem [...] elit, lien interne incididunt [...] morbi.

###  Extrait de code

    
    
                          <p>Lorem [...] elit,
        <a href="#" target="_self">lien interne</a> incididunt [...] morbi.</p>
                          
                        

## Lien externe

Le lien ‘externe’ doit être utilisé pour les liens pointant vers un autre site
et ouvrant un nouvel onglet/une nouvelle page (via l’attribut target=”blank”).
Cela est matérialisé par une icône à droite du lien ainsi que par l’attribut
title du lien mentionnant qu’il s’agit d’un lien externe et que l’on ouvre une
nouvelle fenêtre.

### À noter

L'attribut target="_blank" permettant l’ouverture d’une nouvelle fenêtre doit
être accompagné d'un attribut rel="noopener" (et "noreferrer" sur les vieux
navigateurs), en particulier si le lien pointe sur un site externe, afin
d'éviter toute possibilité d’exécution de code malveillant  
Voir [l'article de référence.](https://mathiasbynens.github.io/rel-noopener/)  
  

Lorem [...] elit, intitulé lien externe incididunt [...] morbi.

###  Extrait de code

    
    
                          <p>Lorem [...] elit,
        <a title="[À MODIFIER - Intitulé] - ouvre une nouvelle fenêtre" href="#" target="_blank" rel="noopener external">intitulé lien externe</a> incididunt [...] morbi.</p>
                          
                        

## Lien simple

Le lien simple en dehors du contenu peut se présenter :

  * avec une icône à droite 
  * avec une icône à gauche 
  * texte seul
  * icône seule

Si une icône est présente, son choix et son emplacement doit rendre l’action à
venir ou la destination plus explicite. L’icône seule n'est à utiliser que
très rarement.

lien simple avec icône à droite

###  Extrait de code

    
    
                          <a class="fr-link fr-icon-arrow-right-line fr-link--icon-right" href="#">lien simple avec icône à droite</a>
                          
                        

## Lien de téléchargement

Télécharger le document lorem ipsum sit dolores amet JPG – 61,88 ko

###  Extrait de code

    
    
                          <a class="fr-link--download fr-link" download="true" id="link-3352" href="#/example/img/image.jpg">
        Télécharger le document lorem ipsum sit dolores amet <span class="fr-link__detail">JPG – 61,88 ko</span>
    </a>
                          
                        

## Tailles

Les liens sont disponibles en 3 tailles :

  * La taille MD est la taille de lien par défaut
  * La taille SM et LG permet d’adapter la taille de votre lien à votre besoin

Label lien SM Label lien LG

###  Extrait de code

    
    
                          <!-- Lien taille SM -->
    <a class="fr-link fr-link--sm" href="#">Label lien SM</a>  
    <!-- Lien taille LG -->
    <a class="fr-link fr-link--lg" href="#">Label lien LG</a>  
                          
                        

## Règles d’utilisation

### Usage

Le lien doit être utilisé comme élément de navigation. Pour les actions d’un
autre type, il faut utiliser le composant boutons du Design System.

Le lien simple, ne doit pas être utilisé au sein d’un paragraphe. Pour faire
un lien dans un paragraphe utilisez les liens contextuels.

### Accessibilité

  * Un lien doit toujours avoir un intitulé texte entre les balises <a> et </a>

L’utilisateur doit pouvoir :

  * naviguer au clavier grâce à la tabulation entre les différents liens et actions.
  * valider l’action en cliquant sur “entrée”.
  * identifier visuellement les liens par rapport au texte qui l’entoure (pas seulement avec la couleur). Dans un texte, un lien est *souligné*.
  * le libellé du lien doit être explicite, c’est à dire exprimer clairement ce qui va se passer pour l’utilisateur.
  * l’intitulé doit permettre de comprendre la destination ou la fonction du lien (ex: ‘faire ma demande de carte grise’, ‘Télécharger le rapport du CNN (format pdf - 345Ko)’). 
  * de préférence utiliser un libellé court et direct, notamment lors de son usage hors du contenu (pour un lien simple hors contenu : 3 mots maximum).
  * éviter les intitulés de liens non explicites. Les termes trop génériques, comme “Cliquez ici”, “En savoir plus”, “Lire la suite”, etc, ne permettent pas à l’utilisateur d’identifier la destination ou la fonction du lien. Si vraiment aucune alternative n’est possible , il est possible d’ajouter un attribut title ajoutant des éléments de compréhension à l’intitulé non explicite : <a href=”…” title=”Lire la suite : comment faire ma demande de carte grise”>
  * Un lien peut être rendu explicite grâce à son contexte : [RGAA 4 : contexte du lien](https://www.numerique.gouv.fr/publications/rgaa-accessibilite/methode/glossaire/#contexte-du-lien)

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

[ Lettre d'information et réseaux sociaux - Newsletter and follow
us](/composants-et-modeles/composants/lettre-d-information-et-reseaux-sociaux)

[Lien d'évitement - Skiplink](/composants-et-modeles/composants/lien-d-
evitement)

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
