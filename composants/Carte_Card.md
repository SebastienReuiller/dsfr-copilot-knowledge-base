Fermer

# Carte - Card

La carte est un lien vers une page éditoriale dont elle donne un aperçu. Elle
fait généralement partie d'une collection ou liste d’aperçus de contenus
similaires. La carte n’est jamais présentée de manière isolée.

La carte existe en trois tailles (LG, MD, SM) et deux formats (horizontal et
vertical) déclinés sur deux supports (desktop et mobile). Les cartes
horizontales sont réservées au desktop (en mobile, une carte horizontale
devient verticale).

## Structure

Elle se compose des éléments suivants :

  * un titre, reprenant celui de l’objet visé (page de destination, action, site) - obligatoire
  * un lien, sur le titre de la carte et dont la zone de click peut s'étendre à toute la carte en ajoutant la classe .fr-enlarge-link - optionnel (mais incompatible avec une zone d’action ou des tags cliquables)
  * un média (image ou vidéo, dans un des ratios prévu par le DSFR), issue ou en lien avec la page de destination - optionnelle
  * une première zone de détail, composée de :
    * une précision, sous forme de tags (cliquables ou non) ou de badges (jusqu'à 4 éléments) - optionnels
    * une icône et un texte - optionnels
  * une description, de 5 lignes maximum (tronquée au-delà) - optionnelle
  * une deuxième zone de détail, composée de :
    * une icône et du texte - optionnels
    * une icône illustrative (par défaut, une flèche) - optionnels
  * une zone d’action, composée de bouton ou de liens (jusqu'à 4 éléments) - optionnelle (mais incompatible avec la deuxième zone de détail)  
  

## Cartes verticales

###  Qu'est-ce que le Pass Culture et comment l’obtenir ?

La carte donne des aperçus cliquables d’une page de contenu à l’utilisateur.
Elle fait généralement partie d'une collection ou liste d’aperçus de contenu
similaires. La carte n’est jamais présentée de manière isolée.

![\[À MODIFIER - vide ou texte alternatif de
l’image\]](/img/placeholder.16x9.png)

###  Extrait de code

    
    
                          <div class="fr-grid-row fr-mb-3w">
        <div class="fr-col fr-col-md-6">
            <div class="fr-card fr-enlarge-link">
                <div class="fr-card__body">
                    <div class="fr-card__content">
                        <h3 class="fr-card__title">
                            <a href="#">Qu'est-ce que le Pass Culture et comment l’obtenir ?</a>
                        </h3>
                        <p class="fr-card__desc">La carte donne des aperçus cliquables d’une page de contenu à l’utilisateur. Elle fait généralement partie d'une collection ou liste d’aperçus de contenu similaires. La carte n’est jamais présentée de manière isolée.</p>
                    </div>
                </div>
                <div class="fr-card__header">
                    <div class="fr-card__img">
                        <img class="fr-responsive-img" src="/img/placeholder.16x9.png" alt="[À MODIFIER - vide ou texte alternatif de l’image]">
                        <!-- L’alternative de l’image (attribut alt) doit toujours être présente, sa valeur peut-être vide (image n’apportant pas de sens supplémentaire au contexte) ou non (porteuse de texte ou apportant du sens) selon votre contexte -->
                    </div>
                </div>
            </div>
        </div>
    </div>
    
                          
                        

## Cartes horizontales

Aucun ratio n’est imposé dans une carte horizontale. La taille de l’image est
déduite en hauteur d’une part par la hauteur du contenu, et en largeur de
l’autre par les proportions choisies de la carte, parmi celles proposées (33%,
40%, 50%). Le ratio par défaut est de 40% pour l’image.  
Pour utiliser les autres ratios :  

  * Pour le ratio 33/66%, utiliser la classe fr-card--horizontal-tier.
  * Pour le ratio 50/50, utiliser la classe fr-card--horizontal-half.  

###  Intitulé de la carte (sur lequel se trouve le lien)

Lorem [...] elit ut.

  * label tag

  * label tag

détail (optionnel)

détail (optionnel)

![\[À MODIFIER - vide ou texte alternatif de
l’image\]](/img/placeholder.16x9.png)

###  Extrait de code

    
    
                          <div class="fr-card fr-enlarge-link fr-card--horizontal">
        <div class="fr-card__body">
            <div class="fr-card__content">
                <h3 class="fr-card__title">
                    <a href="#">Intitulé de la carte (sur lequel se trouve le lien)</a>
                </h3>
                <p class="fr-card__desc">Lorem [...] elit ut.</p>
                <div class="fr-card__start">
                    <ul class="fr-tags-group">
                        <li>
                            <p class="fr-tag">label tag</p>
                        </li>
                        <li>
                            <p class="fr-tag">label tag</p>
                        </li>
                    </ul>
                    <p class="fr-card__detail fr-icon-warning-fill">détail (optionnel)</p>
                </div>
                <div class="fr-card__end">
                    <p class="fr-card__detail fr-icon-warning-fill">détail (optionnel)</p>
                </div>
            </div>
        </div>
        <div class="fr-card__header">
            <div class="fr-card__img">
                <img class="fr-responsive-img" src="/img/placeholder.16x9.png" alt="[À MODIFIER - vide ou texte alternatif de l’image]" />
                <!-- L’alternative de l’image (attribut alt) doit toujours être présente, sa valeur peut-être vide (image n’apportant pas de sens supplémentaire au contexte) ou non (porteuse de texte ou apportant du sens) selon votre contexte -->
            </div>
        </div>
    </div>
                          
                        

###  Intitulé de la carte (sur lequel se trouve le lien)

Lorem [...] elit ut.

  * label tag

  * label tag

détail (optionnel)

détail (optionnel)

![\[À MODIFIER - vide ou texte alternatif de
l’image\]](/img/placeholder.16x9.png)

###  Extrait de code

    
    
                          <div class="fr-card fr-enlarge-link fr-card--horizontal fr-card--horizontal-tier">
        <div class="fr-card__body">
            <div class="fr-card__content">
                <h3 class="fr-card__title">
                    <a href="#">Intitulé de la carte (sur lequel se trouve le lien)</a>
                </h3>
                <p class="fr-card__desc">Lorem [...] elit ut.</p>
                <div class="fr-card__start">
                    <ul class="fr-tags-group">
                        <li>
                            <p class="fr-tag">label tag</p>
                        </li>
                        <li>
                            <p class="fr-tag">label tag</p>
                        </li>
                    </ul>
                    <p class="fr-card__detail fr-icon-warning-fill">détail (optionnel)</p>
                </div>
                <div class="fr-card__end">
                    <p class="fr-card__detail fr-icon-warning-fill">détail (optionnel)</p>
                </div>
            </div>
        </div>
        <div class="fr-card__header">
            <div class="fr-card__img">
                <img class="fr-responsive-img" src="/img/placeholder.16x9.png" alt="[À MODIFIER - vide ou texte alternatif de l’image]" />
                <!-- L’alternative de l’image (attribut alt) doit toujours être présente, sa valeur peut-être vide (image n’apportant pas de sens supplémentaire au contexte) ou non (porteuse de texte ou apportant du sens) selon votre contexte -->
            </div>
        </div>
    </div>
                          
                        

###  Intitulé de la carte (sur lequel se trouve le lien)

Lorem [...] elit ut.

  * label tag

  * label tag

détail (optionnel)

détail (optionnel)

![\[À MODIFIER - vide ou texte alternatif de
l’image\]](/img/placeholder.16x9.png)

###  Extrait de code

    
    
                          <div class="fr-card fr-enlarge-link fr-card--horizontal fr-card--horizontal-half">
        <div class="fr-card__body">
            <div class="fr-card__content">
                <h3 class="fr-card__title">
                    <a href="#">Intitulé de la carte (sur lequel se trouve le lien)</a>
                </h3>
                <p class="fr-card__desc">Lorem [...] elit ut.</p>
                <div class="fr-card__start">
                    <ul class="fr-tags-group">
                        <li>
                            <p class="fr-tag">label tag</p>
                        </li>
                        <li>
                            <p class="fr-tag">label tag</p>
                        </li>
                    </ul>
                    <p class="fr-card__detail fr-icon-warning-fill">détail (optionnel)</p>
                </div>
                <div class="fr-card__end">
                    <p class="fr-card__detail fr-icon-warning-fill">détail (optionnel)</p>
                </div>
            </div>
        </div>
        <div class="fr-card__header">
            <div class="fr-card__img">
                <img class="fr-responsive-img" src="/img/placeholder.16x9.png" alt="[À MODIFIER - vide ou texte alternatif de l’image]" />
                <!-- L’alternative de l’image (attribut alt) doit toujours être présente, sa valeur peut-être vide (image n’apportant pas de sens supplémentaire au contexte) ou non (porteuse de texte ou apportant du sens) selon votre contexte -->
            </div>
        </div>
    </div>
                          
                        

## Carte avec badge dans la zone média

###  Qu'est-ce que le Pass Culture et comment l’obtenir ?

La carte donne des aperçus cliquables d’une page de contenu à l’utilisateur.
Elle fait généralement partie d'une collection ou liste d’aperçus de contenu
similaires. La carte n’est jamais présentée de manière isolée.

![](/img/placeholder.16x9.png)

  * label badge

###  Extrait de code

    
    
                          <div class="fr-grid-row fr-mb-1w">
        <div class="fr-col-md-6 fr-col-md">
            
            <div class="fr-card fr-enlarge-link">
                <div class="fr-card__body">
                    <div class="fr-card__content">
                        <h3 class="fr-card__title">
                            <a href="#">Qu'est-ce que le Pass Culture et comment l’obtenir ?</a>
                        </h3>
                        <p class="fr-card__desc">La carte donne des aperçus cliquables d’une page de contenu à l’utilisateur. Elle fait généralement partie d'une collection ou liste d’aperçus de contenu similaires. La carte n’est jamais présentée de manière isolée.</p>
                    </div>
                </div>
                <div class="fr-card__header">
                    <div class="fr-card__img">
                        <img class="fr-responsive-img" src="/img/placeholder.16x9.png" alt="" />
                        <!-- L’alternative de l’image (attribut alt) doit toujours être présente, sa valeur peut-être vide (image n’apportant pas de sens supplémentaire au contexte) ou non (porteuse de texte ou apportant du sens) selon votre contexte -->
                    </div>
                    <ul class="fr-badges-group">
                        <li>
                            <p class="fr-badge fr-badge--green-emeraude">label badge</p>
                        </li>
                    </ul>
                </div>
            </div>
    
            
        </div>
    </div>
                          
                        

###  Qu'est-ce que le Pass Culture et comment l’obtenir ?

La carte donne des aperçus cliquables d’une page de contenu à l’utilisateur.
Elle fait généralement partie d'une collection ou liste d’aperçus de contenu
similaires. La carte n’est jamais présentée de manière isolée.

![](/img/placeholder.16x9.png)

  * label badge

###  Extrait de code

    
    
                                  <div class="fr-card fr-enlarge-link">
                <div class="fr-card__body">
                    <div class="fr-card__content">
                        <h3 class="fr-card__title">
                            <a href="#">Qu'est-ce que le Pass Culture et comment l’obtenir ?</a>
                        </h3>
                        <p class="fr-card__desc">La carte donne des aperçus cliquables d’une page de contenu à l’utilisateur. Elle fait généralement partie d'une collection ou liste d’aperçus de contenu similaires. La carte n’est jamais présentée de manière isolée.</p>
                    </div>
                </div>
                <div class="fr-card__header">
                    <div class="fr-card__img">
                        <img class="fr-responsive-img" src="/img/placeholder.16x9.png" alt="" />
                        <!-- L’alternative de l’image (attribut alt) doit toujours être présente, sa valeur peut-être vide (image n’apportant pas de sens supplémentaire au contexte) ou non (porteuse de texte ou apportant du sens) selon votre contexte -->
                    </div>
                    <ul class="fr-badges-group">
                        <li>
                            <p class="fr-badge fr-badge--green-emeraude">label badge</p>
                        </li>
                    </ul>
                </div>
            </div>
    
                          
                        

## Carte avec première zone de détail

La carte peut contenir au dessus du titre, une zone avec un ou plusieurs tags
ou badges (le mélange des tags et des badges n’est pas autorisé), se trouvant
dans un élément **fr-tags-group (c** ontenant des élément fr-tag) ou **fr-
badges-group** (contenant des éléments fr-badge.

###  Intitulé de la carte (sur lequel se trouve le lien)

Lorem [...] elit ut.

  * label tag

  * label tag

détail (optionnel)

![](/img/placeholder.16x9.png)

###  Intitulé de la carte (sur lequel se trouve le lien)

Lorem [...] elit ut.

  * label badge

  * label badge

![\[À MODIFIER - vide ou texte alternatif de
l’image\]](/img/placeholder.16x9.png)

###  Extrait de code

    
    
                          <div class="fr-grid-row fr-grid-row--gutters fr-mb-1w">
        <div class="fr-col-md-6 fr-col">
            
            <div class="fr-card fr-enlarge-link">
                <div class="fr-card__body">
                    <div class="fr-card__content">
                        <h3 class="fr-card__title">
                            <a href="#">Intitulé de la carte (sur lequel se trouve le lien)</a>
                        </h3>
                        <p class="fr-card__desc">Lorem [...] elit ut.</p>
                        <div class="fr-card__start">
                            <ul class="fr-tags-group">
                                <li>
                                    <p class="fr-tag">label tag</p>
                                </li>
                                <li>
                                    <p class="fr-tag">label tag</p>
                                </li>
                            </ul>
                            <p class="fr-card__detail fr-icon-warning-fill">détail (optionnel)</p>
                        </div>
                    </div>
                </div>
                <div class="fr-card__header">
                    <div class="fr-card__img">
                        <img class="fr-responsive-img" src="/img/placeholder.16x9.png" alt="" />
                        <!-- L’alternative de l’image (attribut alt) doit toujours être présente, sa valeur peut-être vide (image n’apportant pas de sens supplémentaire au contexte) ou non (porteuse de texte ou apportant du sens) selon votre contexte -->
                    </div>
                </div>
            </div>
        </div>
    
        <div class="fr-col-md-6 fr-col">
            <div class="fr-card fr-enlarge-link">
        <div class="fr-card__body">
            <div class="fr-card__content">
                <h3 class="fr-card__title">
                    <a href="#">Intitulé de la carte (sur lequel se trouve le lien)</a>
                </h3>
                <p class="fr-card__desc">Lorem [...] elit ut.</p>
                <div class="fr-card__start">
                    <ul class="fr-badges-group">
                        <li>
                            <p class="fr-badge">label badge</p>
                        </li>
                        <li>
                            <p class="fr-badge fr-badge--new">label badge</p>
                        </li>
                    </ul>
                </div>
            </div>
        </div>
        <div class="fr-card__header">
            <div class="fr-card__img">
                <img class="fr-responsive-img" src="/img/placeholder.16x9.png" alt="[À MODIFIER - vide ou texte alternatif de l’image]" />
                <!-- L’alternative de l’image (attribut alt) doit toujours être présente, sa valeur peut-être vide (image n’apportant pas de sens supplémentaire au contexte) ou non (porteuse de texte ou apportant du sens) selon votre contexte -->
            </div>
        </div>
    </div>
    
        </div>
    </div>
    
                          
                        

###  Intitulé de la carte (sur lequel se trouve le lien)

Lorem [...] elit ut.

  * label tag

  * label tag

détail (optionnel)

![](/img/placeholder.16x9.png)

###  Extrait de code

    
    
                          <div class="fr-card fr-enlarge-link">
        <div class="fr-card__body">
            <div class="fr-card__content">
                <h3 class="fr-card__title">
                    <a href="#">Intitulé de la carte (sur lequel se trouve le lien)</a>
                </h3>
                <p class="fr-card__desc">Lorem [...] elit ut.</p>
                <div class="fr-card__start">
                    <ul class="fr-tags-group">
                        <li>
                            <p class="fr-tag">label tag</p>
                        </li>
                        <li>
                            <p class="fr-tag">label tag</p>
                        </li>
                    </ul>
                    <p class="fr-card__detail fr-icon-warning-fill">détail (optionnel)</p>
                </div>
            </div>
        </div>
        <div class="fr-card__header">
            <div class="fr-card__img">
                <img class="fr-responsive-img" src="/img/placeholder.16x9.png" alt="" />
                <!-- L’alternative de l’image (attribut alt) doit toujours être présente, sa valeur peut-être vide (image n’apportant pas de sens supplémentaire au contexte) ou non (porteuse de texte ou apportant du sens) selon votre contexte -->
            </div>
        </div>
    </div>
                          
                        

## Carte avec deuxième zone de détail ou zone d’action

Une zone de détail supplémentaire, se trouvant visuellement sous la
description et à côté de l’icône, peut être ajoutée.  

La zone de détail et l’icône ne peuvent être affichées en même temps que la
zone d’action.

###  Intitulé de la carte (sur lequel se trouve le lien)

Lorem [...] elit ut.

détail (optionnel)

![](/img/placeholder.16x9.png)

###  Extrait de code

    
    
                          <div class="fr-grid-row fr-mb-1w">
        <div class="fr-col-md-6 fr-col-md">
    <div class="fr-card fr-enlarge-link">
        <div class="fr-card__body">
            <div class="fr-card__content">
                <h3 class="fr-card__title">
                    <a href="#">Intitulé de la carte (sur lequel se trouve le lien)</a>
                </h3>
                <p class="fr-card__desc">Lorem [...] elit ut.</p>
                <div class="fr-card__end">
                    <p class="fr-card__detail fr-icon-warning-fill">détail (optionnel)</p>
                </div>
            </div>
        </div>
        <div class="fr-card__header">
            <div class="fr-card__img">
                <img class="fr-responsive-img" src="/img/placeholder.16x9.png" alt="" />
                <!-- L’alternative de l’image (attribut alt) doit toujours être présente, sa valeur peut-être vide (image n’apportant pas de sens supplémentaire au contexte) ou non (porteuse de texte ou apportant du sens) selon votre contexte -->
            </div>
        </div>
    </div></div></div>
                          
                        

###  Intitulé de la carte (sur lequel se trouve le lien)

Lorem [...] elit ut.

détail (optionnel)

![](/img/placeholder.16x9.png)

###  Extrait de code

    
    
                          <div class="fr-card fr-enlarge-link">
        <div class="fr-card__body">
            <div class="fr-card__content">
                <h3 class="fr-card__title">
                    <a href="#">Intitulé de la carte (sur lequel se trouve le lien)</a>
                </h3>
                <p class="fr-card__desc">Lorem [...] elit ut.</p>
                <div class="fr-card__end">
                    <p class="fr-card__detail fr-icon-warning-fill">détail (optionnel)</p>
                </div>
            </div>
        </div>
        <div class="fr-card__header">
            <div class="fr-card__img">
                <img class="fr-responsive-img" src="/img/placeholder.16x9.png" alt="" />
                <!-- L’alternative de l’image (attribut alt) doit toujours être présente, sa valeur peut-être vide (image n’apportant pas de sens supplémentaire au contexte) ou non (porteuse de texte ou apportant du sens) selon votre contexte -->
            </div>
        </div>
    </div>
                          
                        

La zone d’action permet d’ajouter des boutons - dans l'élément ul fr-btns-
group- ou des liens - dans l'élément ul fr-links-group. À noter que l’ensemble
de la carte n’est alors plus cliquable, il faut donc retirer la classe fr-
enlarge-link afin que le lien ne soit pas étendu à l’ensemble de la carte.

###  Intitulé de la carte (sur lequel se trouve le lien)

Lorem [...] elit ut.

  * Label 
  * Label 

![\[À MODIFIER - vide ou texte alternatif de
l’image\]](/img/placeholder.16x9.png)

###  Intitulé de la carte (sur lequel se trouve le lien)

Lorem [...] elit ut.

détail (optionnel)

  * label 
  * label 

![\[À MODIFIER - vide ou texte alternatif de
l’image\]](/img/placeholder.16x9.png)

###  Extrait de code

    
    
                          <div class="fr-grid-row fr-grid-row--gutters fr-mb-1w">
        <div class="fr-col-md-6 fr-col-12">
            
    
            <div class="fr-card">
                <div class="fr-card__body">
                    <div class="fr-card__content">
                        <h3 class="fr-card__title">
                            <a href="#">Intitulé de la carte (sur lequel se trouve le lien)</a>
                        </h3>
                        <p class="fr-card__desc">Lorem [...] elit ut.</p>
                    </div>
                    <div class="fr-card__footer">
                        <ul class="fr-btns-group fr-btns-group--inline-reverse fr-btns-group--inline-lg">
                            <li>
                                <button class="fr-btn fr-btn--secondary">
                                    Label
                                </button>
                            </li>
                            <li>
                                <button class="fr-btn">
                                    Label
                                </button>
                            </li>
                        </ul>
                    </div>
                </div>
                <div class="fr-card__header">
                    <div class="fr-card__img">
                        <img class="fr-responsive-img" src="/img/placeholder.16x9.png" alt="[À MODIFIER - vide ou texte alternatif de l’image]" />
                        <!-- L’alternative de l’image (attribut alt) doit toujours être présente, sa valeur peut-être vide (image n’apportant pas de sens supplémentaire au contexte) ou non (porteuse de texte ou apportant du sens) selon votre contexte -->
                    </div>
                </div>
    </div>
    
        </div>
    
        <div class="fr-col-md-6 fr-col-12">
        
            <div class="fr-card">
                <div class="fr-card__body">
                    <div class="fr-card__content">
                        <h3 class="fr-card__title">
                            <a href="#">Intitulé de la carte (sur lequel se trouve le lien)</a>
                        </h3>
                        <p class="fr-card__desc">Lorem [...] elit ut.</p>
                        <div class="fr-card__start">
                            <p class="fr-card__detail fr-icon-warning-fill">détail (optionnel)</p>
                        </div>
                    </div>
                    <div class="fr-card__footer">
                        <ul class="fr-links-group">
                            <li>
                                <a class="fr-link fr-icon-arrow-right-line fr-link--icon-right" href="#">
                                    label
                                </a>
                            </li>
                            <li>
                                <a class="fr-link fr-icon-arrow-right-line fr-link--icon-right" href="#">
                                    label
                                </a>
                            </li>
                        </ul>
                    </div>
                </div>
                <div class="fr-card__header">
                    <div class="fr-card__img">
                        <img class="fr-responsive-img" src="/img/placeholder.16x9.png" alt="[À MODIFIER - vide ou texte alternatif de l’image]" />
                        <!-- L’alternative de l’image (attribut alt) doit toujours être présente, sa valeur peut-être vide (image n’apportant pas de sens supplémentaire au contexte) ou non (porteuse de texte ou apportant du sens) selon votre contexte -->
                    </div>
                </div>
            </div>
    
        </div>
    
    </div>
    
                          
                        

<\--Zone d'action avec boutons-->

###  Intitulé de la carte (sur lequel se trouve le lien)

Lorem [...] elit ut.

détail (optionnel)

  * Label 
  * Label 

![](/img/placeholder.16x9.png)

<\--Zone d'action avec Liens -->

###  Intitulé de la carte (sur lequel se trouve le lien)

Lorem [...] elit ut.

détail (optionnel)

  * label 
  * label 

![](/img/placeholder.16x9.png)

###  Extrait de code

    
    
                          <--Zone d'action avec boutons-->
    
    <div class="fr-card">
        <div class="fr-card__body">
            <div class="fr-card__content">
                <h3 class="fr-card__title">
                    <a href="#">Intitulé de la carte (sur lequel se trouve le lien)</a>
                </h3>
                <p class="fr-card__desc">Lorem [...] elit ut.</p>
                <div class="fr-card__start">
                    <p class="fr-card__detail fr-icon-warning-fill">détail (optionnel)</p>
                </div>
            </div>
            <div class="fr-card__footer">
                <ul class="fr-btns-group fr-btns-group--inline-reverse fr-btns-group--inline-lg">
                    <li>
                        <button class="fr-btn fr-btn--secondary">
                            Label
                        </button>
                    </li>
                    <li>
                        <button class="fr-btn">
                            Label
                        </button>
                    </li>
                </ul>
            </div>
        </div>
        <div class="fr-card__header">
            <div class="fr-card__img">
                <img class="fr-responsive-img" src="/img/placeholder.16x9.png" alt="" />
                <!-- L’alternative de l’image (attribut alt) doit toujours être présente, sa valeur peut-être vide (image n’apportant pas de sens supplémentaire au contexte) ou non (porteuse de texte ou apportant du sens) selon votre contexte -->
            </div>
        </div>
    </div>
    
    
    <--Zone d'action avec Liens -->
    
    <div class="fr-card">
        <div class="fr-card__body">
            <div class="fr-card__content">
                <h3 class="fr-card__title">
                    <a href="#">Intitulé de la carte (sur lequel se trouve le lien)</a>
                </h3>
                <p class="fr-card__desc">Lorem [...] elit ut.</p>
                <div class="fr-card__start">
                    <p class="fr-card__detail fr-icon-warning-fill">détail (optionnel)</p>
                </div>
            </div>
            <div class="fr-card__footer">
                <ul class="fr-links-group">
                    <li>
                        <a class="fr-link fr-icon-arrow-right-line fr-link--icon-right" href="#">
                            label
                        </a>
                    </li>
                    <li>
                        <a class="fr-link fr-icon-arrow-right-line fr-link--icon-right" href="#">
                            label
                        </a>
                    </li>
                </ul>
            </div>
        </div>
        <div class="fr-card__header">
            <div class="fr-card__img">
                <img class="fr-responsive-img" src="/img/placeholder.16x9.png" alt="" />
                <!-- L’alternative de l’image (attribut alt) doit toujours être présente, sa valeur peut-être vide (image n’apportant pas de sens supplémentaire au contexte) ou non (porteuse de texte ou apportant du sens) selon votre contexte -->
            </div>
        </div>
    </div>
                          
                        

## Carte de téléchargement, cas maxi

###  Télécharger le/la [Typologie de document] « [Nom du document] »

Lorem [...] elit ut.

  * label badge

  * label badge

détail (optionnel)

PNG - 1,1 ko

![\[À MODIFIER - vide ou texte alternatif de
l’image\]](/img/placeholder.16x9.png)

###  Extrait de code

    
    
                          <div id="card-1382" class="fr-card fr-enlarge-link fr-card--download">
        <div class="fr-card__body">
            <div class="fr-card__content">
                <h3 class="fr-card__title">
                    <a href="#" download>
                        Télécharger le/la [Typologie de document] « [Nom du document] »
                    </a>
                </h3>
                <p class="fr-card__desc">Lorem [...] elit ut.</p>
                <div class="fr-card__start">
                    <ul class="fr-badges-group">
                        <li>
                            <p class="fr-badge fr-badge--purple-glycine">label badge</p>
                        </li>
                        <li>
                            <p class="fr-badge fr-badge--purple-glycine">label badge</p>
                        </li>
                    </ul>
                    <p class="fr-card__detail fr-icon-warning-fill">détail (optionnel)</p>
                </div>
                <div class="fr-card__end">
                    <p class="fr-card__detail">PNG - 1,1 ko</p>
                </div>
            </div>
        </div>
        <div class="fr-card__header">
            <div class="fr-card__img">
                <img class="fr-responsive-img" src="/img/placeholder.16x9.png" alt="[À MODIFIER - vide ou texte alternatif de l’image]" />
                <!-- L’alternative de l’image (attribut alt) doit toujours être présente, sa valeur peut-être vide (image n’apportant pas de sens supplémentaire au contexte) ou non (porteuse de texte ou apportant du sens) selon votre contexte -->
            </div>
        </div>
    </div>
                          
                        

## Carte avec un bouton dans le titre

Il peut être utile d'utiliser un bouton à la place du lien dans le titre, par
exemple en cas de téléchargement exécuté en js. La zone de clic peut alors
être étendue avec la classe fr-enlarge-button.

###  Télécharger le/la [Typologie de document] « [Nom du document] »

PDF - 48 ko

![\[À MODIFIER - vide ou texte alternatif de
l’image\]](/img/placeholder.16x9.png)

###  Extrait de code

    
    
                          <div id="card-2204" class="fr-card fr-enlarge-button fr-card--sm fr-card--download">
        <div class="fr-card__body">
            <div class="fr-card__content">
                <h3 class="fr-card__title">
                    <button>Télécharger le/la [Typologie de document] « [Nom du document] »</button>
                </h3>
                <div class="fr-card__end">
                    <p class="fr-card__detail">PDF - 48 ko</p>
                </div>
            </div>
        </div>
        <div class="fr-card__header">
            <div class="fr-card__img">
                <img class="fr-responsive-img" src="/img/placeholder.16x9.png" alt="[À MODIFIER - vide ou texte alternatif de l’image]" />
                <!-- L'alternative de l'image (attribut alt) doit toujours être présente, sa valeur peut-être vide (image n'apportant pas de sens supplémentaire au contexte) ou non (porteuse de texte ou apportant du sens) selon votre contexte -->
            </div>
        </div>
    </div>
                          
                        

## Tailles

Les cartes sont disponibles en 3 tailles : SM (fr-card--sm), MD (taille par
défaut) et LG (fr-card--lg)

    
    
    <div class="fr-card fr-card--sm fr-enlarge-link">(...)</div>
    
    <div class="fr-card fr-card--lg fr-enlarge-link">(...)</div>

## Fonds et encadrés

La carte offre différentes variations au niveau du fond et de l’encadré :

  * Carte avec fond gris : fr-card--grey
  * Carte sans sans bordure : fr-card--no-border
  * Carte avec un fond transparent : fr-card--no-background
  * Carte avec ombre portée : fr-card--shadow

    
    
    <div class="fr-card fr-card--grey">(...)</div>
    
    <div class="fr-card fr-card--no-border">(...)</div>
    
    <div class="fr-card  fr-card--no-background">(...)</div>
    
    <div class="fr-card fr-card--shadow">(...)</div>

###  Intitulé de la carte (sur lequel se trouve le lien)

Lorem [...] elit ut.

  * label tag

  * label tag

![\[À MODIFIER - vide ou texte alternatif de
l’image\]](/img/placeholder.16x9.png)

###  Intitulé de la carte (sur lequel se trouve le lien)

Lorem [...] elit ut.

  * label badge

  * label badge

![\[À MODIFIER - vide ou texte alternatif de
l’image\]](/img/placeholder.16x9.png)

###  Intitulé de la carte (sur lequel se trouve le lien)

Lorem [...] elit ut.

détail (optionnel)

![\[À MODIFIER - vide ou texte alternatif de
l’image\]](/img/placeholder.16x9.png)

###  Intitulé de la carte (sur lequel se trouve le lien)

Lorem [...] elit ut.

  * Label 
  * Label 

![\[À MODIFIER - vide ou texte alternatif de
l’image\]](/img/placeholder.16x9.png)

## Responsive

En mobile :

  * les cartes verticales ont le même comportement.
  * les cartes horizontales deviennent automatiquement des cartes verticales.

## Règles d’utilisation

### Usages

Les cartes n’ont pas d’usage imposé, seulement des caractéristiques techniques
et visuelles. Elles peuvent servir à construire des listes de liens, des
grilles de contenus, des blocs de mise en avant, des boutons d’actions
habillés, et bien d’autres usages.

La hauteur de la carte s’adapte à son contenu. La largeur, elle, est définie
selon [la grille](/elements-d-interface/fondamentaux-techniques/grille-et-
points-de-rupture), et les recommandations suivantes :

  * Carte verticale :
    * Desktop :
      * LG : 6 à 8 colonnes
      * MD : 4 à 6 colonnes
      * SM : 3 à 4 colonnes
    * Mobile : 12 colonnes
  * Carte horizontale (desktop uniquement) :
    * LG : 8 à 12 colonnes
    * MD : 6 à 8 colonnes
    * SM : 4 à 6 colonnes.

Au sein d’une liste (affichage sous forme d’une ligne), il faut veiller à
harmoniser la hauteur des cartes par ligne (prendre la hauteur la plus
importante comme référence). Au sein d’une grille (plusieurs lignes), les
hauteurs peuvent varier mais l’ensemble doit garder une cohérence visuelle.

Au sein d’une même liste ou collection, une carte doit avoir le même type
d’affichage (horizontale ou verticale).  

**À faire** \- Aligner la hauteur des cartes d’une ligne (sur la plus haute de
la liste).

![](/uploads/docard_e65c4e77fd.png)

**À ne pas faire** \- Utiliser une zone d’action et une deuxième zone de
détail (avec texte de détail et icône illustrative).

![](/uploads/dontcard1_fda554eab5.png)

**À ne pas faire** \- Utiliser des tags non cliquables avec un fond
personnalisé en $background-constrast.

![](/uploads/dontcard2_b7e715293c.png)

### Accessibilité

  * La carte possède un seul lien : l’intitulé est explicite : la balise <a> est placée sur le titre de la carte (balise Hx). La zone de clic pourra être étendue à toute la carte en css avec la class .fr-enlarge-link.
  * La carte possède plusieurs liens : la zone de clic n’est pas étendue à toute la carte, et les intitulés des liens doivent être explicites.

#### Carte ou tuile ?

Depuis la version 1.5.0, il n’y a plus de différence d’usage entre la carte et
la tuile, puisque la carte n’est pas réservée à un usage. La différence entre
les deux composants est donc uniquement visuelle : la tuile possède une image
en format miniature et une bordure bleue, ce qui n’est pas le cas de la carte,
dont l’image est par défaut en pleine largeur. Dans une tuile, il est
recommandé d’utiliser des pictogrammes à l’emplacement du média.

### Contenus

Dans la mesure où les cartes sont présentées dans des listes ou collections,
il est nécessaire d'éviter les redondances et d’avoir un contenu distinct pour
chaque carte. Il faut par exemple éviter d’utiliser plusieurs fois la même
image en illustration.

## Personnalisation

Certains éléments du composant sont optionnels : voir la structure du
composant

La taille ou l’aspect de certains éléments peuvent être personnalisés :

  * Média : tous les ratios d’image autorisés par le DSFR sont permis. Dans le cas d’une carte horizontale, aucun ratio n’est imposé. Un badge peut être ajouté sur le média.
  * Dans les détails, le texte est par défaut en XS, il peut être passé en SM.
  * L’icône d’illustration (en bleu) ainsi que les icônes des détails peuvent être personnalisées.
  * Zone d’action : cette zone ne peut être affichée avec une deuxième zone de détail. Autrement, son contenu est personnalisable :
    * Boutons : jusqu'à 4 éléments, de tous types (primaires, secondaire, tertiaires) et de toutes tailles
    * Liens : jusqu'à 4 éléments, taille SM uniquement.

### Accentuation

Le fond et la bordure de la carte peuvent être modifiés en utilisant une
couleur neutre. Les détails peuvent également passer dans une couleur plus
prononcée :

Couleurs d'accent Élément | Valeur par défaut | Valeur(s) autorisée(s)  
---|---|---  
|  | Token | Classe css  
Fond | $background-default-grey  
Correspondance :  
Thème clair = $grey-1000  
Thème sombre = $grey-50 | $background-contrast-grey  
Correspondance :  
Thème clair = $grey-950  
Thème sombre = $grey-100 | .fr-card--grey  
aucun fond | .fr-card--no-background  
$background-elevated-grey  
Correspondance :  
Thème clair = $grey-1000 + ombre MD  
Thème sombre = $grey-75 + ombre MD | .fr-card--shadow  
Bordure | $border-default-grey  
Correspondance :  
Thème clair = $grey-925  
Thème sombre = $grey-125 | aucune bordure | .fr-card--no-border  
  
Texte détail | $text-mention-grey  
Correspondance :  
Thème clair = $grey-425  
Thème sombre = $grey-625 | $text-default-grey  
Correspondance :  
Thème clair = $grey-200  
Thème sombre = $grey-850 |  
  
### Besoin d'aide ?

L'équipe du DSFR est là pour vous aider.

Retrouvez-la sur :

  * [la communauté slack](https://gouvfr.slack.com/ "la communauté slack - nouvelle fenêtre") pour poser vos questions, et échanger avec d’autres utilisateurs.   
Vous êtes **agent de l’État** et souhaitez accéder au slack ? [Rejoignez la
communauté](https://gouvfr.atlassian.net/servicedesk/customer/portal/1/group/1/create/9
"Rejoignez la communauté - nouvelle fenêtre") dès maintenant !

  * [ le centre de support](https://gouvfr.atlassian.net/servicedesk/customer/portals "le centre de support - nouvelle fenêtre") pour envoyer vos demandes de correctifs et d'évolution.

[Case à cocher - Checkbox](/composants-et-modeles/composants/case-a-cocher)

[Champ de saisie - Input](/composants-et-modeles/composants/champ-de-saisie)

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
