Fermer

# Sommaire - Summary

Le sommaire permet aux utilisateurs d’avoir un aperçu du contenu et de
naviguer entre les différentes sections d’une page.

## Sommaire

Le sommaire reprend les titres de section de la page sous forme d'ancre vers
chaque titre de section. Au clic sur un des liens, l’utilisateur est redirigé
dans la page, au niveau de la section cherchée.

Le sommaire est placé en haut de page juste avant le corps de texte de la
page. Il ne s’agit pas d’un élément fixé.

### Structure

Il se compose des éléments suivants :

  * Un titre - obligatoire.
  * Une liste d’ancre - obligatoire. 

## Sommaire

  1. Titre du lien 1
    1. Titre du lien 1.1
    2. Titre du lien 1.2
    3. Titre du lien 1.3
  2. Titre du lien 2

    
    
                    <nav class="fr-summary" role="navigation" aria-labelledby="fr-summary-title">
      <h2 class="fr-summary__title" id="fr-summary-title">Sommaire</h2>
      <ol>
          <li>
              <a class="fr-summary__link" id="summary-link-1" href="#anchor-1">Titre du lien 1</a>
              <ol>
                  <li>
                      <a class="fr-summary__link" id="summary-link-1-1" href="#anchor-1.1">Titre du lien 1.1</a>
                  </li>
                  <li>
                      <a class="fr-summary__link" id="summary-link-1-2" href="#anchor-1.2">Titre du lien 1.2</a>
                  </li>
                  <li>
                      <a class="fr-summary__link" id="summary-link-1-3" href="#anchor-1.3">Titre du lien 1.3</a>
                  </li>
              </ol>
          </li>
          <li>
              <a class="fr-summary__link" id="summary-link-2" href="#anchor-2">Titre du lien 2</a>
          </li>
      </ol>
    </nav>
                    
                  

Le titre “Sommaire” doit toujours être placé au début de la liste de lien.

### Pour les développeurs

Le titre, matérialisé par la classe fr-summary__title peut être : - une balise
<p> : <p class="fr-summary__title"> ou - une balise de titre : <h2 class="fr-
summary__title"> à <h6>. Vous pouvez ainsi adapter le titre du bloc à la
structure et l’architecture de votre contenu.

## Règles d’utilisation

### Usages

Le sommaire est à utiliser dans une page de contenu longue ou à forte densité.
Il n’est pas recommandé de l’utiliser sur des pages courtes.

Le sommaire précède la zone texte d'une page, le fond de couleur est destinée
à le séparer visuellement du contenu .

Si un chapô est présent en début de page, le sommaire s’affiche entre le chapô
et le contenu éditorial.

### Accessibilité

Les ancres sont placées sur les titres <hx> du contenu.

Note : Pour repositionner le focus sur un élément qui n’est pas un lien ou un
bouton, vous devez implémentez un attribut tabindex=”-1” sur l'élément.

Exemple : `<h2 id="titre-ancre-1" tabindex="-1">Titre de l’ancre</h2>`

### Contenus

Le contenu des liens du sommaire doit reprendre le texte exact de chaque titre
de section.

### Personnalisation

Ce composant n’est pas personnalisable.

### Besoin d'aide ?

L'équipe du DSFR est là pour vous aider.

Retrouvez-la sur :

  * [la communauté slack](https://gouvfr.slack.com/ "la communauté slack - nouvelle fenêtre") pour poser vos questions, et échanger avec d’autres utilisateurs.   
Vous êtes **agent de l’État** et souhaitez accéder au slack ? [Rejoignez la
communauté](https://gouvfr.atlassian.net/servicedesk/customer/portal/1/group/1/create/9
"Rejoignez la communauté - nouvelle fenêtre") dès maintenant !

  * [ le centre de support](https://gouvfr.atlassian.net/servicedesk/customer/portals "le centre de support - nouvelle fenêtre") pour envoyer vos demandes de correctifs et d'évolution.

[Sélecteur de langue - Translate](/composants-et-modeles/composants/selecteur-
de-langue)

[ Tableau - Table 🆕](/composants-et-modeles/composants/tableau)

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
