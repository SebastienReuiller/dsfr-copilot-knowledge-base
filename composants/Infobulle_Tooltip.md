Fermer

# Infobulle - Tooltip

Le composant “Infobulle” (ou “bulle d’aide”, “aide contextuelle”) permet
d’afficher du contenu dans le contexte de navigation (non modal) à propos et
lors de l’interaction avec un élément précis de l’interface. Il est caché par
défaut et s’affiche au survol ou au clic de l’élément associé, par-dessus le
reste de la page.

## Structure

#### Déclenchement au survol

L’infobulle au **survol** se compose des éléments suivants :  

  * Un texte (simple, sans formatage riche), obligatoire 
  * Un cadre, obligatoire
  * Une flèche pointant vers l’élément associé, obligatoire  
  

#### Déclenchement au clic

L’infobulle au **clic** se compose des éléments suivants :

  * Une zone de déclenchement (bouton tertiaire sans contour avec icône “question-line”), obligatoire
  * Un texte (simple, sans formatage riche), obligatoire
  * Un cadre, obligatoire
  * Une flèche pointant vers l’élément associé, obligatoire

## Variation(s)

Il existe **deux types d’infobulles** suivant son déclenchement.

  1. L’infobulle au survol (ou au focus), à réserver aux cas où il n’est pas possible d’afficher l’information autrement, et aux parcours majoritairement en desktop (exemple : label d’un bouton à icône unique dans un groupe de boutons à icônes uniques).
  2. L’infobulle au clic (ou information contextuelle), à partir d’une icône représentant un point d’interrogation "?" est adossée à l’élément auquel elle se rapporte.  

#### Déclenchement au survol

L’information contextuelle est liée à son déclencheur par l’attribut aria-
describedby qui est égal à l'id du tooltip.

Exemple  Lorem [...] elit ut.

###  Extrait de code

    
    
                          <a class="fr-link" aria-describedby="tooltip-2989" id="link-2990" href="#">
        Exemple
    </a>
    <span class="fr-tooltip fr-placement" id="tooltip-2989" role="tooltip" aria-hidden="true">Lorem [...] elit ut.</span>
                          
                        

#### Déclenchement au clic

L'ajout de la classe fr-btn--tooltip déclenche l'ouverture du tooltip au clic.

Information contextuelle  Lorem [...] elit ut.

###  Extrait de code

    
    
                          <button class="fr-btn--tooltip fr-btn" type="button" id="button-2995" aria-describedby="tooltip-2994">
        Information contextuelle
    </button>
    <span class="fr-tooltip fr-placement" id="tooltip-2994" role="tooltip" aria-hidden="true">Lorem [...] elit ut.</span>
                          
                        

## Règles d’utilisation

#### Usages

Il est essentiel de réserver son usage **lorsqu'il n’est pas possible
d’afficher l’information directement dans le flux de la page** , sans la
cacher dans une bulle.

Sur mobile, l’infobulle au survol ne s’affiche pas. Elle est donc à éviter
soigneusement sur des sites enregistrant une forte fréquentation mobile.
Aussi, l’affichage au “tap” prolongé peut être mis en place. Plutôt qu’une
infobulle, il est possible d’utiliser une alerte, un accordéon, une mise en
avant, ou même une zone personnalisée.

**D’autre part, il faut veiller à :**

  * Garder les textes courts et concis
  * N’afficher que des informations non essentielles au parcours (par exemple, expliquer pourquoi un composant est désactivé)
  * Ne pas inclure de formatage riche (gras, italique)
  * Ne pas inclure de médias ou d’interactions (boutons, liens)
  * Ne pas multiplier les infobulles dans une page
  * Faire en sorte qu’il ne soit pas possible d’avoir plusieurs infobulles ouvertes dans un affichage
  * Ne pas utiliser d'infobulles pour répéter un label
  * Utiliser une flèche pour lier la zone de texte à l’élément associé
  * Permettre l’affichage d’une infobulle lors de la navigation clavier
  * Reprendre l’attribut <title> de l’élément associé
  * Permettre la lecture par les dispositifs d’aide (aria-describedby)  
  

#### Les questions à se poser avant d'utiliser ce composant

  * L’information que je veux afficher est-elle essentielle à la navigation ou optionnelle ? Si elle est essentielle, l’afficher directement dans la page (en utilisant, par exemple, une mise en avant ou une alerte).  

  * Si l’information n’est pas essentielle : ai-je la place d’afficher une icône "?" ou une autre zone de déclenchement, à côté de mon élément ? Si oui, utiliser une information contextuelle (déclenchée au clic) sinon, utiliser une infobulle déclenchée au survol.  

#### Personnalisation

Aucune personnalisation n'est possible.

[Indicateur d'étapes - Stepper](/composants-et-modeles/composants/indicateur-
d-etapes)

[Interrupteur - Toggle](/composants-et-modeles/composants/interrupteur)

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
