Fermer

# Contenu médias - Content

Les contenus médias désignent vos contenus photos et vidéos. Lorsqu’ils sont
intégrés à une page de contenu, il est recommandé de suivre les règles
décrites ci-dessous.

## Structure

Les contenus médias se composent des éléments suivants:

  * un media, image, vidéo ou audio - obligatoire.
  * une légende - optionnelle.
  * un lien de transcription textuel - optionnel. 

## Image

![\[À MODIFIER - vide ou texte alternatif de
l’image\]](/img/placeholder.16x9.png)

© Légende de l‘image

    
    
                    <figure class="fr-content-media" role="group" aria-label="© Légende de l‘image">
        <div class="fr-content-media__img">
            <img class="fr-responsive-img fr-ratio-16x9" src="/img/placeholder.16x9.png" alt="[À MODIFIER - vide ou texte alternatif de l’image]" />
            <!-- L’alternative de l’image (attribut alt) doit toujours être présente, sa valeur peut-être vide (image n’apportant pas de sens supplémentaire au contexte) ou non (porteuse de texte ou apportant du sens) selon votre contexte -->
        </div>
        <figcaption class="fr-content-media__caption">© Légende de l‘image</figcaption>
    </figure>
                    
                  

### Les trois tailles proposées pour les images

Si vous souhaitez accentuer la visibilité d'une image vous pouvez utiliser les
différentes tailles à votre disposition :

  * LG : dans cette taille, la largeur de l’image est supérieure à celle du contenu.
  * MD : dans cette taille, la largeur de l’image correspond à celle du contenu.
  * SM : dans cette taille, la largeur de l’image est inférieure à celle du contenu.

#### Image taille LG (125%)

L’image est plus grande que la zone de texte

![\[À MODIFIER | texte alternatif de l’image\]](/img/placeholder.16x9.png)

© Légende de l‘image

    
    
    <figure class="fr-content-media fr-content-media--lg" role="group" aria-label="© Légende de l‘image">
        <div class="fr-content-media__img">
            <img src="/img/placeholder.16x9.png" class="fr-responsive-img" alt="[À MODIFIER | texte alternatif de l’image]" />
            <!-- L’alternative de l’image (attribut alt) doit toujours être présent, sa valeur peut-être vide (image n’apportant pas de sens supplémentaire au contexte) ou non (porteuse de texte ou apportant du sens) selon votre contexte -->
        </div>
        <figcaption class="fr-content-media__caption">© Légende de l‘image</figcaption>
    </figure>

#### Image taille SM (75%)

L’image est plus petite que la zone de texte.

![\[À MODIFIER | texte alternatif de l’image\]](/img/placeholder.16x9.png)

© Légende de l‘image

    
    
    <figure class="fr-content-media fr-content-media--sm" role="group" aria-label="© Légende de l‘image">
        <div class="fr-content-media__img">
            <img src="/img/placeholder.16x9.png" class="fr-responsive-img" alt="[À MODIFIER | texte alternatif de l’image]" />
            <!-- L’alternative de l’image (attribut alt) doit toujours être présent, sa valeur peut-être vide (image n’apportant pas de sens supplémentaire au contexte) ou non (porteuse de texte ou apportant du sens) selon votre contexte -->
        </div>
        <figcaption class="fr-content-media__caption">© Légende de l‘image</figcaption>
    </figure>

### Texte alternatif des images

Il est important de bien choisir l’alternative d’image adéquate. Si l’image
est illustrative, n’apportant pas d'éléments de compréhension supplémentaires
par rapport au texte dans lequel elle se trouve, l’attribut alt doit être vide
`alt=””`. Pour vous aider à faire le bon choix, n’hésitez pas à consulter
l'[arbre de décision alt du w3c (en
anglais)](https://www.w3.org/WAI/tutorials/images/decision-tree/ "arbre de
décision alt du w3c \(en anglais\) - nouvelle fenêtre"), ainsi que [l'adaption
en français (Atalan)](https://blog.atalan.fr/guide-pour-le-remplissage-
dattributs-alt-dimages/ "l'adaption en français \(Atalan\) - nouvelle
fenêtre").

### Images SVG

Les svg répondent aux même impératifs que les autres images concernant leur
alternative textuelle. Si il est inséré via une balise img, l’attribut `alt`
doit être présent, et doit être rempli ou non.

Pour les svg ‘inline’ , le principe est le même: il peut être porteur de sens
(en contenant du texte, ou bien apportant des informations supplémentaire au
contexte dans lequel il se trouve, voir l’arbre de décision) ou non porteur de
sens.

Si le svg est **porteur de sens** il doit contenir les attribut role=”img” et
aria-label contenant la description. <svg role=”img” aria-label=”[A modifier -
titre ou texte contenu dans l’image]”>.

    
    
    <figure class="fr-content-media" role="group" aria-label="Légende de l‘image">
        <div class="fr-content-media__img">
            <!-- Les SVG porteurs de sens doivent avoir l'attribut role="img" et être labeliser par l'attribut aria-label="[A modifier - titre ou texte contenu dans l’image]" -->
            <svg version="1.1" role="img" aria-label=”[A modifier - titre ou texte contenu dans l’image]”>
              (...)
            </svg>
        </div>
        <figcaption class="fr-content-media__caption">Légende de l‘image</figcaption>
    </figure>

Si le svg n’est pas porteur de sens (icône ou illustration), ajouter un
attribut aria-hidden.

    
    
            <svg version="1.1" aria-hidden="true">
              (...)
            </svg>
    

### Ratios d’image

Le format par défaut conseillé des images est le 16:9.  
Toutefois d’autres ratios (4:3, 32:9, etc.) sont disponibles : voir la section
[Ratios dans les fondamentaux](/elements-d-interface/fondamentaux-
techniques/medias).

## Vidéo

Lorsqu’une vidéo est intégrée dans un contenu éditorial, elle est présentée
par défaut en format 16:9 et peut intégrer une légende et un lien pour
afficher la transcription. L’Iframe générée par l’hébergeur de la vidéo peut
être différent du ratio par défaut de 16:9.

Il est possible d’opter pour un format 4:3 de la vidéo, à l’aide du modifier
`.fr-responsive-vid--4x3`.

**Note :** le DSFR fournit uniquement le HTML et CSS du lien “Afficher la
transcription”. La fonctionnalité d’affichage de la transcription (ouverture
d’une nouvelle page ou apparition du texte) n’est pas gérée et devra être
ajoutée.

### Ratio 16:9

Description / Source  Label lien

Transcription

Fermer

#  Titre de la vidéo

Agrandir

    
    
                    <figure role="group" class="fr-content-media">
        <iframe title="Titre de l'iframe" class="fr-responsive-vid" src="https://www.youtube.com/embed/HyirpmPL43I" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
        <figcaption class="fr-content-media__caption">
            Description / Source
            <a class="fr-link" href="#[url - à modifier]">
                Label lien
            </a>
        </figcaption>
    </figure>
        <div class="fr-transcription">
            <button class="fr-transcription__btn" aria-expanded="false" aria-controls="fr-transcription__collapse-transcription-462">Transcription</button>
            <div class="fr-collapse" id="fr-transcription__collapse-transcription-462">
                <dialog id="fr-transcription__modal-transcription-462" class="fr-modal" role="dialog" aria-labelledby="fr-transcription__modal-transcription-462-title">
                    <div class="fr-container fr-container--fluid fr-container-md">
                        <div class="fr-grid-row fr-grid-row--center">
                            <div class="fr-col-12 fr-col-md-10 fr-col-lg-8">
                                <div class="fr-modal__body">
                                    <div class="fr-modal__header">
                                        <button class="fr-btn--close fr-btn" aria-controls="fr-transcription__modal-transcription-462" title="Fermer">
                                            Fermer
                                        </button>
                                    </div>
                                    <div class="fr-modal__content">
                                        <h1 id="fr-transcription__modal-transcription-462-title" class="fr-modal__title">
                                            Titre de la vidéo
                                        </h1>
                                        <!-- données de test -->
                                    </div>
                                    <div class="fr-transcription__footer">
                                        <div class="fr-transcription__actions-group">
                                            <button class="fr-btn fr-btn--fullscreen" aria-controls="fr-transcription__modal-transcription-462" data-fr-opened="false" title="">
                                                Agrandir
                                            </button>
                                        </div>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                </dialog>
            </div>
        </div>
    
                    
                  

### Ratio 4:3

Description / Source  Label lien

Transcription

Agrandir

Fermer

#  Titre de la vidéo

Lorem ipsum dolor sit amet, consectetur adipiscing, [link
test](https://www.systeme-de-design.gouv.fr/) incididunt, ut labore et dolore
magna aliqua. Vitae sapien pellentesque habitant morbi tristique senectus et.
Diam maecenas sed enim ut. Accumsan lacus vel facilisis volutpat est. Ut
aliquam purus sit amet luctus. Lorem ipsum dolor sit amet consectetur
adipiscing elit ut.

Lorem ipsum dolor sit amet, consectetur adipiscing, [link
test](https://www.systeme-de-design.gouv.fr/) incididunt, ut labore et dolore
magna aliqua. Vitae sapien pellentesque habitant morbi tristique senectus et.
Diam maecenas sed enim ut. Accumsan lacus vel facilisis volutpat est. Ut
aliquam purus sit amet luctus. Lorem ipsum dolor sit amet consectetur
adipiscing elit ut.

  * list item
  * list item 
    * list item niveau 2
    * list item niveau 2

    
    
                    <figure role="group" class="fr-content-media">
      <iframe
        title="Titre de l'iframe"
        class="fr-responsive-vid fr-ratio-4x3"
        src="https://www.youtube.com/embed/HyirpmPL43I"
        allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture"
        allowfullscreen
      ></iframe>
      <figcaption class="fr-content-media__caption">
        Description / Source
        <a class="fr-link" href="#[url - à modifier]"> Label lien </a>
      </figcaption>
      <div class="fr-transcription" id="transcription-2160">
        <button
          class="fr-transcription__btn"
          aria-expanded="false"
          aria-controls="fr-transcription-collapse-transcription-2160"
          data-fr-js-collapse-button="true"
        >
          Transcription
        </button>
        <div
          class="fr-collapse"
          id="fr-transcription-collapse-transcription-2160"
          data-fr-js-collapse="true"
        >
          <div class="fr-transcription__footer">
            <div class="fr-transcription__actions-group">
              <button
                class="fr-btn--fullscreen fr-btn"
                aria-controls="fr-transcription-modal-transcription-2160"
                aria-label="Agrandir la transcription"
                data-fr-opened="false"
                id="button-2163"
                data-fr-js-modal-button="true"
              >
                Agrandir
              </button>
            </div>
          </div>
          <div
            id="fr-transcription-modal-transcription-2160"
            class="fr-modal"
            aria-labelledby="fr-transcription-modal-transcription-2160-title"
            data-fr-js-modal="true"
          >
            <div class="fr-container fr-container--fluid fr-container-md">
              <div class="fr-grid-row fr-grid-row--center">
                <div class="fr-col-12 fr-col-md-10 fr-col-lg-8">
                  <div class="fr-modal__body" data-fr-js-modal-body="true">
                    <div class="fr-modal__header">
                      <button
                        class="fr-btn--close fr-btn"
                        aria-controls="fr-transcription-modal-transcription-2160"
                        id="button-2164"
                        title="Fermer"
                        data-fr-js-modal-button="true"
                      >
                        Fermer
                      </button>
                    </div>
                    <div class="fr-modal__content">
                      <h1
                        id="fr-transcription-modal-transcription-2160-title"
                        class="fr-modal__title"
                      >
                        Titre de la vidéo
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
                          maecenas sed enim ut. Accumsan lacus vel facilisis
                          volutpat est. Ut aliquam purus sit amet luctus. Lorem
                          ipsum dolor sit amet consectetur adipiscing elit ut.
                        </p>
                        <p>
                          Lorem ipsum dolor sit amet, consectetur adipiscing,
                          <a
                            href="https://www.systeme-de-design.gouv.fr/"
                            target="_blank"
                            >link test</a
                          >
                          incididunt, ut labore et dolore magna aliqua. Vitae sapien
                          pellentesque habitant morbi tristique senectus et. Diam
                          maecenas sed enim ut. Accumsan lacus vel facilisis
                          volutpat est. Ut aliquam purus sit amet luctus. Lorem
                          ipsum dolor sit amet consectetur adipiscing elit ut.
                        </p>
                        <ul>
                          <li>list item</li>
                          <li>
                            list item
                            <ul>
                              <li>list item niveau 2</li>
                              <li>list item niveau 2</li>
                            </ul>
                          </li>
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
    </figure>
                    
                  

### Les trois tailles proposées pour les vidéos

Si vous souhaitez accentuer la visibilité d'une vidéo vous pouvez utiliser les
différentes tailles à votre disposition.

  * LG : dans cette taille, la largeur de la vidéo est supérieure à celle du contenu.
  * MD : dans cette taille, la largeur de la vidéo correspond à celle du contenu.
  * SM : dans cette taille, la largeur de la vidéo est inférieure à celle du contenu.

#### Vidéo taille LG (125%)

La vidéo est plus grande que la zone de texte.

Exemple de vidéo LG format 16/9 :

    
    
    <figure role="group" class="fr-content-media fr-content-media--lg">
        <iframe title="Titre de l'iframe" class="fr-responsive-vid" src="https://www.youtube.com/embed/HyirpmPL43I" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
        <figcaption class="fr-content-media__caption">
            Description / Source
            <a class="fr-link" href="#[url - à modifier]">
                Label lien
            </a>
        </figcaption>
    </figure>
        <div class="fr-transcription">
            <button class="fr-transcription__btn" aria-expanded="false" aria-controls="fr-transcription__collapse-transcription-468">Transcription</button>
            <div class="fr-collapse" id="fr-transcription__collapse-transcription-468">
                <dialog id="fr-transcription__modal-transcription-468" class="fr-modal" role="dialog" aria-labelledby="fr-transcription__modal-transcription-468-title">
                    <div class="fr-container fr-container--fluid fr-container-md">
                        <div class="fr-grid-row fr-grid-row--center">
                            <div class="fr-col-12 fr-col-md-10 fr-col-lg-8">
                                <div class="fr-modal__body">
                                    <div class="fr-modal__header">
                                        <button class="fr-btn--close fr-btn" aria-controls="fr-transcription__modal-transcription-468" title="Fermer">
                                            Fermer
                                        </button>
                                    </div>
                                    <div class="fr-modal__content">
                                        <h1 id="fr-transcription__modal-transcription-468-title" class="fr-modal__title">
                                            Titre de la vidéo
                                        </h1>
                                        <!-- données de test -->
                                    </div>
                                    <div class="fr-transcription__footer">
                                        <div class="fr-transcription__actions-group">
                                            <button class="fr-btn fr-btn--fullscreen" aria-controls="fr-transcription__modal-transcription-468" data-fr-opened="false" title="">
                                                Agrandir
                                            </button>
                                        </div>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                </dialog>
            </div>
        </div>
    

Exemple de vidéo LG format 4/3 :

    
    
    <figure role="group" class="fr-content-media">
        <iframe title="Titre de l'iframe" class="fr-responsive-vid fr-ratio-4x3" src="https://www.youtube.com/embed/HyirpmPL43I" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
        <figcaption class="fr-content-media__caption">
            Description / Source
            <a class="fr-link" href="#[url - à modifier]">
                Label lien
            </a>
        </figcaption>
    </figure>
        <div class="fr-transcription">
            <button class="fr-transcription__btn" aria-expanded="false" aria-controls="fr-transcription__collapse-transcription-471">Transcription</button>
            <div class="fr-collapse" id="fr-transcription__collapse-transcription-471">
                <dialog id="fr-transcription__modal-transcription-471" class="fr-modal" role="dialog" aria-labelledby="fr-transcription__modal-transcription-471-title">
                    <div class="fr-container fr-container--fluid fr-container-md">
                        <div class="fr-grid-row fr-grid-row--center">
                            <div class="fr-col-12 fr-col-md-10 fr-col-lg-8">
                                <div class="fr-modal__body">
                                    <div class="fr-modal__header">
                                        <button class="fr-btn--close fr-btn" aria-controls="fr-transcription__modal-transcription-471" title="Fermer">
                                            Fermer
                                        </button>
                                    </div>
                                    <div class="fr-modal__content">
                                        <h1 id="fr-transcription__modal-transcription-471-title" class="fr-modal__title">
                                            Titre de la vidéo
                                        </h1>
                                        <!-- données de test -->
                                    </div>
                                    <div class="fr-transcription__footer">
                                        <div class="fr-transcription__actions-group">
                                            <button class="fr-btn fr-btn--fullscreen" aria-controls="fr-transcription__modal-transcription-471" data-fr-opened="false" title="">
                                                Agrandir
                                            </button>
                                        </div>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                </dialog>
            </div>
        </div>
    

#### Vidéo taille SM (75%)

La largeur de la vidéo est plus petite que la zone de texte.

Exemple de vidéo SM format 16/9 :

    
    
    <figure role="group" class="fr-content-media fr-content-media--sm">
        <iframe title="Titre de l'iframe" class="fr-responsive-vid" src="https://www.youtube.com/embed/HyirpmPL43I" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
        <figcaption class="fr-content-media__caption">
            Description / Source
            <a class="fr-link" href="#[url - à modifier]">
                Label lien
            </a>
        </figcaption>
    </figure>
        <div class="fr-transcription">
            <button class="fr-transcription__btn" aria-expanded="false" aria-controls="fr-transcription__collapse-transcription-465">Transcription</button>
            <div class="fr-collapse" id="fr-transcription__collapse-transcription-465">
                <dialog id="fr-transcription__modal-transcription-465" class="fr-modal" role="dialog" aria-labelledby="fr-transcription__modal-transcription-465-title">
                    <div class="fr-container fr-container--fluid fr-container-md">
                        <div class="fr-grid-row fr-grid-row--center">
                            <div class="fr-col-12 fr-col-md-10 fr-col-lg-8">
                                <div class="fr-modal__body">
                                    <div class="fr-modal__header">
                                        <button class="fr-btn--close fr-btn" aria-controls="fr-transcription__modal-transcription-465" title="Fermer">
                                            Fermer
                                        </button>
                                    </div>
                                    <div class="fr-modal__content">
                                        <h1 id="fr-transcription__modal-transcription-465-title" class="fr-modal__title">
                                            Titre de la vidéo
                                        </h1>
                                        <!-- données de test -->
                                    </div>
                                    <div class="fr-transcription__footer">
                                        <div class="fr-transcription__actions-group">
                                            <button class="fr-btn fr-btn--fullscreen" aria-controls="fr-transcription__modal-transcription-465" data-fr-opened="false" title="">
                                                Agrandir
                                            </button>
                                        </div>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                </dialog>
            </div>
        </div>
    

Exemple de vidéo SM format 4/3 :

    
    
    <figure role="group" class="fr-content-media fr-content-media--sm">
        <iframe title="Titre de l'iframe" class="fr-responsive-vid fr-ratio-4x3" src="https://www.youtube.com/embed/HyirpmPL43I" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
        <figcaption class="fr-content-media__caption">
            Description / Source
            <a class="fr-link" href="#[url - à modifier]">
                Label lien
            </a>
        </figcaption>
    </figure>
        <div class="fr-transcription">
            <button class="fr-transcription__btn" aria-expanded="false" aria-controls="fr-transcription__collapse-transcription-474">Transcription</button>
            <div class="fr-collapse" id="fr-transcription__collapse-transcription-474">
                <dialog id="fr-transcription__modal-transcription-474" class="fr-modal" role="dialog" aria-labelledby="fr-transcription__modal-transcription-474-title">
                    <div class="fr-container fr-container--fluid fr-container-md">
                        <div class="fr-grid-row fr-grid-row--center">
                            <div class="fr-col-12 fr-col-md-10 fr-col-lg-8">
                                <div class="fr-modal__body">
                                    <div class="fr-modal__header">
                                        <button class="fr-btn--close fr-btn" aria-controls="fr-transcription__modal-transcription-474" title="Fermer">
                                            Fermer
                                        </button>
                                    </div>
                                    <div class="fr-modal__content">
                                        <h1 id="fr-transcription__modal-transcription-474-title" class="fr-modal__title">
                                            Titre de la vidéo
                                        </h1>
                                        <!-- données de test -->
                                    </div>
                                    <div class="fr-transcription__footer">
                                        <div class="fr-transcription__actions-group">
                                            <button class="fr-btn fr-btn--fullscreen" aria-controls="fr-transcription__modal-transcription-474" data-fr-opened="false" title="">
                                                Agrandir
                                            </button>
                                        </div>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                </dialog>
            </div>
        </div>
    

## Règles d’utilisation

### Usages

  * Utilisez des images et vidéos qui véhiculent un message clair. 
  * Veillez à homogénéiser le style graphique de vos images et vidéos. 
  * Utilisez exclusivement des images, photos et vidéos libres de droit ou veillez à vous acquitter des droits.

#### Accessibilité et traitement des alternatives

  * Si l'image n'apporte pas d'information essentielle à la compréhension du contenu, utiliser une alternative vide : alt="". (Ressources d’aide à la décision en [anglais](https://www.w3.org/WAI/tutorials/images/decision-tree/ "anglais - nouvelle fenêtre") et en [français](https://blog.atalan.fr/guide-pour-le-remplissage-dattributs-alt-dimages/ "français - nouvelle fenêtre")).
  * Si l'image apporte une information essentielle à la compréhension du contenu, renseigner l'alternative avec l'information nécessaire : alt="@alternative". (Ressources d’aide à la décision en [anglais](https://www.w3.org/WAI/tutorials/images/decision-tree/ "anglais - nouvelle fenêtre") et en [français](https://blog.atalan.fr/guide-pour-le-remplissage-dattributs-alt-dimages/ "français - nouvelle fenêtre")).
  * Chaque image complexe a si nécessaire une description détaillée adjacente. Exemple : [Simone Veil : la loi sur l'avortement. Épisode 2](https://www.vie-publique.fr/bd/272944-simone-veil-la-loi-sur-lavortement-episode-2 "Simone Veil : la loi sur l'avortement. Épisode 2  - nouvelle fenêtre").
  * Si une balise figure possède une légende dans une balise **figcaption** , elle doit également avoir un attribut **aria-label** reprenant le texte du **figcaption**.

#### Vidéo ou audio

  * La lecture ne commence pas sans le contrôle de l’utilisateur.
  * Le lecteur est utilisable au clavier selon un ordre logique.
  * La transcription textuelle est pertinente, accessible et adjacente à l'élément vidéo ou audio.
  * Les vidéos (hors direct) sont sous-titrées.

### Personnalisation

Le style de ce composant n’est pas personnalisable.

Toutefois, certains éléments sont optionnels - voir la structure du composant.

### Besoin d'aide ?

L'équipe du DSFR est là pour vous aider.

Retrouvez-la sur :

  * [la communauté slack](https://gouvfr.slack.com/ "la communauté slack - nouvelle fenêtre") pour poser vos questions, et échanger avec d’autres utilisateurs.   
Vous êtes **agent de l’État** et souhaitez accéder au slack ? [Rejoignez la
communauté](https://gouvfr.atlassian.net/servicedesk/customer/portal/1/group/1/create/9
"Rejoignez la communauté - nouvelle fenêtre") dès maintenant !

  * [ le centre de support](https://gouvfr.atlassian.net/servicedesk/customer/portals "le centre de support - nouvelle fenêtre") pour envoyer vos demandes de correctifs et d'évolution.

[Citation - Quote](/composants-et-modeles/composants/citation)

[Contrôle segmenté - Segmented control](/composants-et-
modeles/composants/controle-segmente)

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
