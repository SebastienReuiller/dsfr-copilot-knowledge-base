Fermer

# Transcription - Transcription

La transcription est présente directement sous le contenu concerné, dans une
zone à déployer au clic. La zone à déployer et le contenu doivent au maximum
tenir sur un écran sans nécessiter de défilement.

Il est également possible de la consulter en plein écran dans une vue dédiée,
via l’ouverture d’une modale.

Le composant reprend l’apparence et le fonctionnement d’un accordéon.
Toutefois, la hauteur de celui-ci est fixe pour permettre aux utilisateurs
d’avoir accès à la transcription en même temps que le média.

D’autre part, puisque ce composant reprend en parti les caractéristiques des
accordéons, l’utilisateur a la possibilité de concevoir le composant par ses
propres moyens en réutilisant le composant accordéon permettant l’ouverture
intégrale du contenu.

## Structure

Ce composant se présente directement sous le contenu concerné dans une zone à
déployer.  
Il comprend :

  * Un label “Transcription” - obligatoire
  * Un contenu - obligatoire
  * Un sommaire - optionnel
  * Un texte de transcription - obligatoire
  * Un bouton “Agrandir“ d’ouverture en modale - obligatoire

Transcription

Agrandir

Fermer

#  Titre de la transcription

Lorem ipsum dolor sit amet, consectetur adipiscing, [link
test](https://www.systeme-de-design.gouv.fr/) incididunt, ut labore et dolore
magna aliqua. Vitae sapien pellentesque habitant morbi tristique senectus et.
Diam maecenas sed enim ut. Accumsan lacus vel facilisis volutpat est. Ut
aliquam purus sit amet luctus. Lorem ipsum dolor sit amet consectetur
adipiscing elit ut.

  * list item
  * list item

###  Extrait de code

    
    
                          <div class="fr-transcription" id="transcription-2147">
      <button
        class="fr-transcription__btn"
        aria-expanded="true"
        aria-controls="fr-transcription-collapse-transcription-2147"
        data-fr-js-collapse-button="true"
      >
        Transcription
      </button>
      <div
        class="fr-collapse fr-collapse--expanded"
        id="fr-transcription-collapse-transcription-2147"
        data-fr-js-collapse="true"
        style="--collapse-max-height: none; --collapse: -210px"
      >
        <div class="fr-transcription__footer">
          <div class="fr-transcription__actions-group">
            <button
              class="fr-btn--fullscreen fr-btn"
              aria-controls="fr-transcription-modal-transcription-2147"
              aria-label="Agrandir la transcription"
              data-fr-opened="false"
              id="button-2150"
              data-fr-js-modal-button="true"
            >
              Agrandir
            </button>
          </div>
        </div>
        <div
          id="fr-transcription-modal-transcription-2147"
          class="fr-modal"
          aria-labelledby="fr-transcription-modal-transcription-2147-title"
          data-fr-js-modal="true"
        >
          <div class="fr-container fr-container--fluid fr-container-md">
            <div class="fr-grid-row fr-grid-row--center">
              <div class="fr-col-12 fr-col-md-10 fr-col-lg-8">
                <div
                  class="fr-modal__body"
                  data-fr-js-modal-body="true"
                  style="--modal-max-height: 719px"
                >
                  <div class="fr-modal__header">
                    <button
                      class="fr-btn--close fr-btn"
                      aria-controls="fr-transcription-modal-transcription-2147"
                      id="button-2151"
                      title="Fermer"
                      data-fr-js-modal-button="true"
                    >
                      Fermer
                    </button>
                  </div>
                  <div class="fr-modal__content">
                    <h1
                      id="fr-transcription-modal-transcription-2147-title"
                      class="fr-modal__title"
                    >
                      Titre de la transcription
                    </h1>
                    <!-- données de test -->
                    <div>
                      <p>
                        Lorem ipsum dolor sit amet, consectetur adipiscing,
                        <a
                          href="https://www.systeme-de-design.gouv.fr/"
                          target="_blank"
                          >link test</a
                        >
                        incididunt, ut labore et dolore magna aliqua. Vitae sapien
                        pellentesque habitant morbi tristique senectus et. Diam
                        maecenas sed enim ut. Accumsan lacus vel facilisis volutpat
                        est. Ut aliquam purus sit amet luctus. Lorem ipsum dolor sit
                        amet consectetur adipiscing elit ut.
                      </p>
                      <ul>
                        <li>list item</li>
                        <li>list item</li>
                      </ul>
                    </div>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
                          
                        

### Bonne pratiques

  * Afficher la transcription sur la même page que la vidéo (pour autoriser la lecture simultanée)  

  * Masquer la transcription quand celle-ci est longue, dans une zone à développer au clic ou sur une page séparée (modale) atteinte via un lien

### Accessibilité

  * Les contenus vidéos doivent être sous-titrés et accompagnés d’une transcription textuelle (RGAA).
  * Les contenus seulement audios sont accompagnés d’une transcription textuelle (RGAA).
  * Les images complexes (infographies, cartes, etc.) sont accompagnées d’une description détaillée (RGAA).
  * Le bouton d’accès à la transcription doit se situer (visuellement et dans le code) juste avant ou après le média.
  * La transcription doit reprendre l’intégralité des informations transmises par le média.

[Téléchargement de fichier - Download](/composants-et-
modeles/composants/telechargement-de-fichier)

[Tuile - Tile](/composants-et-modeles/composants/tuile)

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
