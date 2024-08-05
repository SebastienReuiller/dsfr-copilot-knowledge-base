Fermer

# Téléchargement de fichier - Download

Le lien de téléchargement permet de mettre à disposition un ou plusieurs
fichiers en téléchargement au fil du texte pour que l’utilisateur puisse les
télécharger.

Attention, il s’agit du composant pour que l’usager télécharge un document
depuis votre site. Pour téléverser un document vers votre site, utiliser le
[composant ajout de fichier](/elements-d-interface/composants/ajout-de-
fichier).

## Structure

Il est composé des éléments suivants :

  * **Le nom du fichier** , obligatoire accompagné de la mention “Télécharger” 
  * **Une description** , optionnelle 
  * **Une icône explicitant l’action** , obligatoire 
  * **Le format et poids du fichier** , obligatoire 
  * **La précision de la langue** (dans le libellé) : obligatoire si le document est dans une autre langue que celle de la page courante  
  

### Variations

Ce composant se décline sous trois formes possibles :

  * Lien
  * Carte
  * Tuile  
  

Dans chacun des cas, il est possible de mettre un ou plusieurs documents à
disposition à la suite sur une largeur de 4 à 8 colonnes.  

#### Lien

Télécharger le document lorem ipsum sit dolores amet JPG – 61,88 ko

###  Extrait de code

    
    
                          <a class="fr-link fr-link--download" download href="#[À MODIFIER - example/img/image.jpg]">
        Télécharger le document lorem ipsum sit dolores amet <span class="fr-link__detail">JPG – 61,88 ko</span>
    </a>
                          
                        

Voir la documentation complète du composant "Lien"

#### Carte

###  Télécharger le document lorem ipsum sit dolores amet

Texte de description

JPG – 61,88 ko

###  Extrait de code

    
    
                          <div class="fr-card fr-enlarge-link fr-card--download">
        <div class="fr-card__body">
            <div class="fr-card__content">
                <h3 class="fr-card__title">
                    <a download href="#[À MODIFIER - example/img/image.jpg]">
                        Télécharger le document lorem ipsum sit dolores amet
                    </a>
                </h3>
                <p class="fr-card__desc">Texte de description</p>
                <div class="fr-card__end">
                    <p class="fr-card__detail">JPG – 61,88 ko</p>
                </div>
            </div>
        </div>
    </div>
                          
                        

Voir la documentation complète du composant "Carte"

#### Tuile

###  Télécharger le document XX

Détail (optionel)

###  Extrait de code

    
    
                          <div class="fr-tile fr-tile--download fr-enlarge-link" id="tile-6735">
        <div class="fr-tile__body">
            <div class="fr-tile__content">
                <h3 class="fr-tile__title">
                    <a href="#" download>Télécharger le document XX</a>
                </h3>
                <p class="fr-tile__detail">Détail (optionel)</p>
            </div>
        </div>
        <div class="fr-tile__header">
            <div class="fr-tile__pictogram">
                <svg aria-hidden="true" class="fr-artwork" viewBox="0 0 80 80" width="80px" height="80px">
                    <use class="fr-artwork-decorative" href="/img/artwork/pictograms/city-hall.svg#artwork-decorative"></use>
                    <use class="fr-artwork-minor" href="/img/artwork/pictograms/city-hall.svg#artwork-minor"></use>
                    <use class="fr-artwork-major" href="/img/artwork/pictograms/city-hall.svg#artwork-major"></use>
                </svg>
            </div>
        </div>
    </div>
                          
                        

Voir la documentation du composant Tuile

### Pour les développeurs

  * L’attribut download permet le téléchargement direct de la ressource, sans l'ouvrir. Il est n'est pas obligatoire. Associé à une valeur cela permet aussi de renommer le fichier par cette valeur avant de le télécharger. Si vous souhaitez ouvrir le document dans une nouvelle fenêtre, utiliser l'attribut _target="_blank"._
  * Afin de faciliter le remplissage des données du fichier, il est possible d’ajouter sur le lien l’attribut _data-fr-assess-file_. L’ajout de cet attribut, permet le récupérer et d’afficher l’extension du fichier, son poids et éventuellement sa langue. Associé à la valeur “bytes” _data-fr-assess-file="bytes"_ l'utilitaire converti le poids en Bytes (KB, MB...) plutôt qu'en Octets (ko, Mo). À utiliser sur les pages non francophones.   

    
    
    <a class="fr-link--download fr-link" data-fr-assess-file="bytes" hreflang="fr" download="true" id="link-3368" href="/example/img/image.jpg">
        Download the french document lorem ipsum <span class="fr-link__detail"> </span>
    </a>

  * Si la langue du document est différente de la langue de la page courante. Pour cela, il est nécessaire d’ajouter l’attribut hreflang. 

    
    
    <a class="fr-link--download fr-link" hreflang="en" download="true" id="link-3362" href="exemple.pdf">
        Télécharger le document lorem ipsum sit dolores amet <span class="fr-link__detail">PDF – 1,81 Mo - Anglais</span>
    </a>

### Règles d'utilisation

#### Contenu

Dans le bloc de téléchargement, le nom du document doit être précédé de la
mention “télécharger le/la” ( ex : télécharger le rapport « Experts, acteurs,
ensemble… pour une société qui change »).

#### Accessibilité

  * La langue du document doit être indiquée si elle est différente de la langue de la page courante. 
  * Le document cible, quel que soit sont format, doit répondre aux même critères d’accessibilité que les pages web. Des informations sont disponibles sur le Guide de conception de documents bureautiques accessibles. Sinon, proposez plutôt le contenu au format html (accessible).  
  

#### Personnalisation

Aucune personnalisation n'est possible pour ce composant.

[Tag - Tag](/composants-et-modeles/composants/tag)

[Transcription - Transcription](/composants-et-
modeles/composants/transcription)

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
