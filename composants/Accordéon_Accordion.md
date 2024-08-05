Fermer

# Accordéon - Accordion

Les accordéons permettent aux utilisateurs d'afficher et de masquer des
sections de contenu présentés dans une page.

## Structure

Un accordéon est constitué des éléments suivants :  

  * un en-tête, correspondant au titre de la section - obligatoire.
  * un chevron orienté vers le bas indique que le panneau peut s'ouvrir. Il est orienté vers le haut quand le panneau peut se refermer - obligatoire.   

  * un séparateur - obligatoire   

  * une zone de contenu, masqué par défaut pouvant contenir tout type d'élément - obligatoire.

###  Intitulé accordéon

#### Contenu

Lorem ipsum dolor sit amet, consectetur adipiscing, link test incididunt, ut
labore et dolore magna aliqua. Vitae sapien pellentesque habitant morbi
tristique senectus et. Diam maecenas sed enim ut. Accumsan lacus vel facilisis
volutpat est. Ut aliquam purus sit amet luctus. Lorem ipsum dolor sit amet
consectetur adipiscing elit ut.

    
    
    <section class="fr-accordion">
        <h3 class="fr-accordion__title">
            <button class="fr-accordion__btn" aria-expanded="false" aria-controls="accordion-106">Intitulé accordéon</button>
        </h3>
        <div class="fr-collapse" id="accordion-106">
            <!-- données de test -->
        </div>
    </section>
    

## Groupes d'accordéons

###  Intitulé accordéon

#### Contenu

Lorem ipsum dolor sit amet, consectetur adipiscing, link test incididunt, ut
labore et dolore magna aliqua. Vitae sapien pellentesque habitant morbi
tristique senectus et. Diam maecenas sed enim ut. Accumsan lacus vel facilisis
volutpat est. Ut aliquam purus sit amet luctus. Lorem ipsum dolor sit amet
consectetur adipiscing elit ut.

Lorem ipsum dolor sit amet, consectetur adipiscing, link test incididunt, ut
labore et dolore magna aliqua. Vitae sapien pellentesque habitant morbi
tristique senectus et. Diam maecenas sed enim ut. Accumsan lacus vel facilisis
volutpat est. Ut aliquam purus sit amet luctus. Lorem ipsum dolor sit amet
consectetur adipiscing elit ut.

  * list item
  * list item
  * list item
    * list item niveau 2
    * list item niveau 2
    * list item niveau 2

###  Intitulé accordéon

#### Contenu

Lorem ipsum dolor sit amet, consectetur adipiscing, link test incididunt, ut
labore et dolore magna aliqua. Vitae sapien pellentesque habitant morbi
tristique senectus et. Diam maecenas sed enim ut. Accumsan lacus vel facilisis
volutpat est. Ut aliquam purus sit amet luctus. Lorem ipsum dolor sit amet
consectetur adipiscing elit ut.

Lorem ipsum dolor sit amet, consectetur adipiscing, link test incididunt, ut
labore et dolore magna aliqua. Vitae sapien pellentesque habitant morbi
tristique senectus et. Diam maecenas sed enim ut. Accumsan lacus vel facilisis
volutpat est. Ut aliquam purus sit amet luctus. Lorem ipsum dolor sit amet
consectetur adipiscing elit ut.

  * list item
  * list item
  * list item
    * list item niveau 2
    * list item niveau 2
    * list item niveau 2

###  Intitulé accordéon

#### Contenu

Lorem ipsum dolor sit amet, consectetur adipiscing, link test incididunt, ut
labore et dolore magna aliqua. Vitae sapien pellentesque habitant morbi
tristique senectus et. Diam maecenas sed enim ut. Accumsan lacus vel facilisis
volutpat est. Ut aliquam purus sit amet luctus. Lorem ipsum dolor sit amet
consectetur adipiscing elit ut.

Lorem ipsum dolor sit amet, consectetur adipiscing, link test incididunt, ut
labore et dolore magna aliqua. Vitae sapien pellentesque habitant morbi
tristique senectus et. Diam maecenas sed enim ut. Accumsan lacus vel facilisis
volutpat est. Ut aliquam purus sit amet luctus. Lorem ipsum dolor sit amet
consectetur adipiscing elit ut.

  * list item
  * list item
  * list item
    * list item niveau 2
    * list item niveau 2
    * list item niveau 2

###  Intitulé accordéon

#### Contenu

Lorem ipsum dolor sit amet, consectetur adipiscing, link test incididunt, ut
labore et dolore magna aliqua. Vitae sapien pellentesque habitant morbi
tristique senectus et. Diam maecenas sed enim ut. Accumsan lacus vel facilisis
volutpat est. Ut aliquam purus sit amet luctus. Lorem ipsum dolor sit amet
consectetur adipiscing elit ut.

Lorem ipsum dolor sit amet, consectetur adipiscing, link test incididunt, ut
labore et dolore magna aliqua. Vitae sapien pellentesque habitant morbi
tristique senectus et. Diam maecenas sed enim ut. Accumsan lacus vel facilisis
volutpat est. Ut aliquam purus sit amet luctus. Lorem ipsum dolor sit amet
consectetur adipiscing elit ut.

  * list item
  * list item
  * list item
    * list item niveau 2
    * list item niveau 2
    * list item niveau 2

    
    
                    <div class="fr-accordions-group">
        <section class="fr-accordion">
            <h3 class="fr-accordion__title">
                <button class="fr-accordion__btn" aria-expanded="false" aria-controls="accordion-114">Intitulé accordéon</button>
            </h3>
            <div class="fr-collapse" id="accordion-114">
                <!-- données de test -->
                <h4 class="fr-h4">Contenu </h4>
                <p>Lorem ipsum dolor sit amet, consectetur adipiscing, <a href="#test" target="_blank">link test</a> incididunt, ut labore et dolore magna aliqua. Vitae sapien pellentesque habitant morbi tristique senectus et. Diam maecenas sed enim ut. Accumsan lacus vel facilisis volutpat est. Ut aliquam purus sit amet luctus. Lorem ipsum dolor sit amet consectetur adipiscing elit ut.</p>
                <p>Lorem ipsum dolor sit amet, consectetur adipiscing, <a href="#test" target="_blank">link test</a> incididunt, ut labore et dolore magna aliqua. Vitae sapien pellentesque habitant morbi tristique senectus et. Diam maecenas sed enim ut. Accumsan lacus vel facilisis volutpat est. Ut aliquam purus sit amet luctus. Lorem ipsum dolor sit amet consectetur adipiscing elit ut.</p>
                <ul>
                    <li>list item</li>
                    <li>list item</li>
                    <li>list item<ul>
                            <li>list item niveau 2</li>
                            <li>list item niveau 2</li>
                            <li>list item niveau 2</li>
                        </ul>
                    </li>
                </ul>
            </div>
        </section>
        <section class="fr-accordion">
            <h3 class="fr-accordion__title">
                <button class="fr-accordion__btn" aria-expanded="false" aria-controls="accordion-115">Intitulé accordéon</button>
            </h3>
            <div class="fr-collapse" id="accordion-115">
                <!-- données de test -->
                <h4 class="fr-h4">Contenu </h4>
                <p>Lorem ipsum dolor sit amet, consectetur adipiscing, <a href="#test" target="_blank">link test</a> incididunt, ut labore et dolore magna aliqua. Vitae sapien pellentesque habitant morbi tristique senectus et. Diam maecenas sed enim ut. Accumsan lacus vel facilisis volutpat est. Ut aliquam purus sit amet luctus. Lorem ipsum dolor sit amet consectetur adipiscing elit ut.</p>
                <p>Lorem ipsum dolor sit amet, consectetur adipiscing, <a href="#test" target="_blank">link test</a> incididunt, ut labore et dolore magna aliqua. Vitae sapien pellentesque habitant morbi tristique senectus et. Diam maecenas sed enim ut. Accumsan lacus vel facilisis volutpat est. Ut aliquam purus sit amet luctus. Lorem ipsum dolor sit amet consectetur adipiscing elit ut.</p>
                <ul>
                    <li>list item</li>
                    <li>list item</li>
                    <li>list item<ul>
                            <li>list item niveau 2</li>
                            <li>list item niveau 2</li>
                            <li>list item niveau 2</li>
                        </ul>
                    </li>
                </ul>
            </div>
        </section>
        <section class="fr-accordion">
            <h3 class="fr-accordion__title">
                <button class="fr-accordion__btn" aria-expanded="false" aria-controls="accordion-116">Intitulé accordéon</button>
            </h3>
            <div class="fr-collapse" id="accordion-116">
                <!-- données de test -->
                <h4 class="fr-h4">Contenu </h4>
                <p>Lorem ipsum dolor sit amet, consectetur adipiscing, <a href="#test" target="_blank">link test</a> incididunt, ut labore et dolore magna aliqua. Vitae sapien pellentesque habitant morbi tristique senectus et. Diam maecenas sed enim ut. Accumsan lacus vel facilisis volutpat est. Ut aliquam purus sit amet luctus. Lorem ipsum dolor sit amet consectetur adipiscing elit ut.</p>
                <p>Lorem ipsum dolor sit amet, consectetur adipiscing, <a href="#test" target="_blank">link test</a> incididunt, ut labore et dolore magna aliqua. Vitae sapien pellentesque habitant morbi tristique senectus et. Diam maecenas sed enim ut. Accumsan lacus vel facilisis volutpat est. Ut aliquam purus sit amet luctus. Lorem ipsum dolor sit amet consectetur adipiscing elit ut.</p>
                <ul>
                    <li>list item</li>
                    <li>list item</li>
                    <li>list item<ul>
                            <li>list item niveau 2</li>
                            <li>list item niveau 2</li>
                            <li>list item niveau 2</li>
                        </ul>
                    </li>
                </ul>
            </div>
        </section>
        <section class="fr-accordion">
            <h3 class="fr-accordion__title">
                <button class="fr-accordion__btn" aria-expanded="false" aria-controls="accordion-117">Intitulé accordéon</button>
            </h3>
            <div class="fr-collapse" id="accordion-117">
                <!-- données de test -->
                <h4 class="fr-h4">Contenu </h4>
                <p>Lorem ipsum dolor sit amet, consectetur adipiscing, <a href="#test" target="_blank">link test</a> incididunt, ut labore et dolore magna aliqua. Vitae sapien pellentesque habitant morbi tristique senectus et. Diam maecenas sed enim ut. Accumsan lacus vel facilisis volutpat est. Ut aliquam purus sit amet luctus. Lorem ipsum dolor sit amet consectetur adipiscing elit ut.</p>
                <p>Lorem ipsum dolor sit amet, consectetur adipiscing, <a href="#test" target="_blank">link test</a> incididunt, ut labore et dolore magna aliqua. Vitae sapien pellentesque habitant morbi tristique senectus et. Diam maecenas sed enim ut. Accumsan lacus vel facilisis volutpat est. Ut aliquam purus sit amet luctus. Lorem ipsum dolor sit amet consectetur adipiscing elit ut.</p>
                <ul>
                    <li>list item</li>
                    <li>list item</li>
                    <li>list item<ul>
                            <li>list item niveau 2</li>
                            <li>list item niveau 2</li>
                            <li>list item niveau 2</li>
                        </ul>
                    </li>
                </ul>
            </div>
        </section>
    </div>
                    
                  

Par défaut, les accordéons sont fermés et comprennent l’en tête et le chevron.  

La totalité de la barre de titre est cliquable. En cliquant sur le titre ou
l’icône , le contenu est révélé ou caché et le chevron change d'orientation.

### Pour les développeurs

L’élément fr-accordion est une implémentation du système de collapse, il peut
vivre de manière indépendante dans le code, et ainsi s’ouvrir et se fermer au
clic.  

Il est composé :  

  * d’un bouton doté des attributs aria-expanded="false" (précisant que le collapse est fermé par défaut) et aria-controls="accordion-1" pour lier le bouton à l’id du collapse (ici accordion-1).   

  * d’un élément de collapse avec un id unique et la classe .fr-collapse

Un regroupement de ces éléments peut être fait avec un wrapper .fr-accordions-
group. Lors de l’ouverture d’un item au sein d’un même groupe, les autres
items se fermeront automatiquement.

Il est possible d’utiliser plusieurs groupes au sein d’une même page, et ceux-
si fonctionneront de manière totalement indépendante, c’est-à-dire qu’ouvrir
un item d’un groupe fermera les items de ce même groupe, sans interagir sur
les groupes annexes de la page. Pour cela il faut s’assurer que chaque id de
collapse est unique.

## Règles d’utilisation

### Usages

Les accordéons servent à économiser de l'espace sur de longues pages. Ils
permettent ainsi :  

  * d'alléger des pages de contenus denses en permettant aux utilisateurs de consulter uniquement ce dont ils ont besoin.   

  * de guider les utilisateurs dans des parcours complexes

Ne pas utiliser les accordéons dans des contextes où les utilisateurs ont
besoin de lire tout les contenus compris dans les accordéons.

Ne pas utiliser non plus avec un contenu très court. Dans ce cas, utiliser des
listes ou des paragraphes.

### Accessibilité

Le système d'accordéon utilise le motif de conception ARIA "Accordion". Ce
composant ne nécessite pas d'adaptation particulière. Il faut néanmoins
prendre soin que les niveaux de titre de chaque section de l'accordéon soient
cohérents avec le titrage de la page.

### Contenus

Les titres des en-têtes doivent être brefs et explicites sur le contenu
proposé par l’accordéon.

À l’intérieur de l’accordéon, il est possible d’ajouter tout type de contenu
selon vos besoins.

## Personnalisation

Ce composant n’est pas personnalisable.

[Composants](/composants-et-modeles/composants)

[Ajout de fichier - Upload](/composants-et-modeles/composants/ajout-de-
fichier)

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
