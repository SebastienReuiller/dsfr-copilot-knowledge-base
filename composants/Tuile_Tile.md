Fermer

# Tuile - Tile

La tuile est un raccourci ou point d’entrée qui redirige les utilisateurs vers
des pages de contenu. Elle fait généralement partie d'une collection ou liste
de tuiles similaires. La tuile n’est jamais présentée de manière isolée.

### Structure

Elle se compose des éléments suivants :

  * **Un pictogramme fr-artwork** uniquement (jpg, png, svg, etc), optionnel   

  * **Une première zone de détail** , composée d’une précision, sous forme de tags (cliquables ou non) ou de badges (jusqu'à 4 éléments), optionnels 
  * **Un titre** reprenant celui de l’objet visé (page de destination, action, site), obligatoire
  *  **Une description** , optionnelle
  *  **Une deuxième zone de détail** , composée d’un texte, optionnelle 
  * **Une icône illustrative** (par défaut, une flèche), optionnelle  
  

### Variations

**L'ensemble de la tuile est cliquable.** Elle existe en affichage vertical ou
horizontal, dans deux tailles **MD** et **SM**. En desktop, la taille MD
occupe entre 4 à 6 colonnes, tandis que la taille SM occupe un maximum de 3 à
4 colonnes. Côté mobile, les deux tailles occupent l’intégralité de la largeur
de la grille.  
  

#### Taille MD - Verticale

###  Intitulé de la tuile

Lorem [...] elit ut.

Détail (optionel)

###  Extrait de code

    
    
                          <div class="fr-tile fr-enlarge-link" id="tile-6609">
        <div class="fr-tile__body">
            <div class="fr-tile__content">
                <h3 class="fr-tile__title">
                    <a href="#">Intitulé de la tuile</a>
                </h3>
                <p class="fr-tile__desc">Lorem [...] elit ut.</p>
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
                          
                        

#### Taille MD - Horizontale

###  Intitulé de la tuile

Détail (optionel)

label tag

###  Extrait de code

    
    
                          <div class="fr-tile fr-tile--horizontal fr-enlarge-link" id="tile-7873">
        <div class="fr-tile__body">
            <div class="fr-tile__content">
                <h3 class="fr-tile__title">
                    <a href="#">Intitulé de la tuile</a>
                </h3>
                <p class="fr-tile__detail">Détail (optionel)</p>
                <div class="fr-tile__start">
                    <p class="fr-tag" id="tag-7874">label tag</p>
                </div>
            </div>
        </div>
        <div class="fr-tile__header">
            <div class="fr-tile__pictogram">
                <svg aria-hidden="true" class="fr-artwork" viewBox="0 0 80 80" width="80px" height="80px">
                    <use class="fr-artwork-decorative" href="/img/artwork/pictograms/buildings/city-hall.svg#artwork-decorative"></use>
                    <use class="fr-artwork-minor" href="/img/artwork/pictograms/buildings/city-hall.svg#artwork-minor"></use>
                    <use class="fr-artwork-major" href="/img/artwork/pictograms/buildings/city-hall.svg#artwork-major"></use>
                </svg>
            </div>
        </div>
    </div>
                          
                        

#### Taille SM - Verticale

###  Intitulé de la tuile

Lorem [...] elit ut.

Détail (optionel)

###  Extrait de code

    
    
                          <div class="fr-tile fr-tile--sm fr-enlarge-link" id="tile-6612">
        <div class="fr-tile__body">
            <div class="fr-tile__content">
                <h3 class="fr-tile__title">
                    <a href="#">Intitulé de la tuile</a>
                </h3>
                <p class="fr-tile__desc">Lorem [...] elit ut.</p>
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
                          
                        

#### Taille SM - horizontale

###  Intitulé de la tuile

Détail (optionel)

label badge

###  Extrait de code

    
    
                          <div class="fr-tile fr-tile--sm fr-tile--horizontal fr-enlarge-link" id="tile-6661">
        <div class="fr-tile__body">
            <div class="fr-tile__content">
                <h3 class="fr-tile__title">
                    <a href="#">Intitulé de la tuile</a>
                </h3>
                <p class="fr-tile__detail">Détail (optionel)</p>
                <div class="fr-tile__start">
                    <p class="fr-badge fr-badge--sm fr-badge--purple-glycine">label badge</p>
                </div>
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
                          
                        

#### Tuile de téléchargement

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
                          
                        

#### Tuile de téléchargement avec bouton dans le titre

Il peut être utile d'utiliser un bouton à la place du lien dans le titre, par
exemple en cas de téléchargement exécuté en js. La zone de clic peut alors
être étendue avec la classe fr-enlarge-button.

###  Télécharger le document XX

Description (optionnelle)

Détail obligatoire (Extension - Poids - Langue)

###  Extrait de code

    
    
                          <div class="fr-tile fr-tile--download fr-enlarge-button" id="tile-8365">
        <div class="fr-tile__body">
            <div class="fr-tile__content">
                <h3 class="fr-tile__title">
                    <button>Télécharger le document XX</button>
                </h3>
                <p class="fr-tile__desc">Description (optionnelle)</p>
                <p class="fr-tile__detail">Détail obligatoire (Extension - Poids - Langue)</p>
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
                          
                        

### Pour les développeurs

La tuile .fr-tile est verticale par défaut en mobile et desktop. Elle peut
devenir horizontale, en mobile et desktop, en rajoutant la classe .fr-tile--
horizontal

Il est possible de forcer pour qu’elle soit :

  * verticale à partir du breakpoint MD en rajoutant la classe _.fr-tile--vertical@md_. Cette classe n'est bien entendu utile que si on est dans le contexte d'une tuile horizontale. 
  * horizontale à partir du breakpoint MD en rajoutant la classe _.fr-tile--horizontal@md_. Cette classe n'est bien entendu utile que si on est dans le contexte d'une tuile verticale.  
  

###  Intitulé de la tuile

Détail (optionel)

###  Extrait de code

    
    
                          <div class="fr-tile fr-tile--horizontal fr-tile--vertical@md fr-enlarge-link" id="tile-6664">
        <div class="fr-tile__body">
            <div class="fr-tile__content">
                <h3 class="fr-tile__title">
                    <a href="#">Intitulé de la tuile</a>
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
                          
                        

## Règles d’utilisation

### Usages

  * Bien que la hauteur de la tuile s’adapte à son contenu, sa largeur est, elle, définie selon la grille.
  * Au sein d’une liste de tuile, il faut veiller à harmoniser la hauteur des tuiles par ligne en prenant la plus importante comme référence.
  * Au sein d’une même liste ou collection, toutes les tuiles doivent avoir la même structure.  
  

### Attention

  * Les tuiles ne doivent pas être utilisées pour créer des aperçus du contenu des pages vers lesquelles elles renvoies.
  * Elles ne doivent pas non plus être utilisées pour mettre en avant l’action principale d’une page.
  * Lorsqu’elles ont un titre long, il est préférable d’utiliser une tuile horizontale plutôt qu’une tuile verticale.  
  

### Accessibilité

La tuile possède un seul lien dont l’intitulé est explicite : la balise <a>
est placée dans la balise titre. La zone de clic pourra être étendue à toute
la tuile en css.

### Contenus

  * Les titres et descriptions doivent être synthétiques. 
  * Dans la mesure où les tuiles sont présentées dans des listes/collections, il est nécessaire d'éviter les redondances et d’avoir un contenu distinct pour chaque tuile. Ainsi, il faut éviter de réutiliser plusieurs fois la même image.
  * Attention à utiliser des images correctement dimensionnées et qui s’adaptent aux différents types d’affichages responsive.  
  

## Personnalisation

Certains éléments sont optionnels et peuvent, ou non, être affichés : voir
structure du composant.

Élément | Valeur par défaut | Valeur(s) autorisée(s)  
---|---|---  
|  | Token | Classe css  
**Fond** | **$background-default-grey**  
Correspondance :  
Thème clair = $grey-1000  
Thème sombre = $grey-50 | **$background-contrast-grey**  
Correspondance :  
Thème clair = $grey-950  
Thème sombre = $grey-100 | .fr-tile--grey  
aucun fond | .fr-tile--no-background  
**$background-elevated-grey**  
Correspondance :  
Thème clair = $grey-1000 + ombre MD  
Thème sombre = $grey-75 + ombre MD | .fr-tile--shadow  
**Contour** | **$border-default-grey**  
  
Correspondance :  
Thème clair = $grey-925  
Thème sombre = $grey-125 | aucune bordure | .fr-tile--no-border  
**Pictogramme** | **$artwork-minor-red-marianne**  
  
Correspondance :  
Thème clair = $red-marianne-main-472  
Thème sombre = $red-marianne-main-472 | **$[couleur]-main (thème clair et
sombre)**  
  
 _Exemples : $green-emeraude-main-632_ |  
  
[Transcription - Transcription](/composants-et-
modeles/composants/transcription)

[Blocs fonctionnels](/composants-et-modeles/blocs-fonctionnels)

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
