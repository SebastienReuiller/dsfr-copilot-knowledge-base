Fermer

# Tag - Tag

Le tag catégorise/classe/organise les contenus à l'aide de mots-clés. Il aide
les utilisateurs à rechercher et à trouver facilement une information.

Le tag peut être utilisé dans deux contextes :

**Dans le contenu** (carte, en-tête, liste) : il catégorise le contenu auquel
il est apposé. Il peut être cliquable ou non cliquable.

En tant que filtre (dans une page de résultats de recherche par exemple). Dans
ce cas il peut-être :

  * **activable** comme filtre en place à sélectionner/désélectionner,
  *  **supprimable** , il sert de rappel à un filtre qui a été coché dans une sidebar ou une liste déroulante.

# Tag non cliquable

Le tag par défaut permet d’afficher une information sur un contenu.

## Structure

Il se compose des éléments suivants :

  * un libellé - obligatoire.
  * une icône - optionnelle.

Le libellé contient un mot-clé ou une expression qui permet de catégoriser
votre contenu

Label tag

Label tag

    
    
                    <p class="fr-tag">Label tag</p>
    <p class="fr-tag fr-fi-arrow-right-line fr-tag--icon-left">Label tag</p>
                    
                  

## Tailles

Tous les tags sont disponibles en deux tailles SM et MD pour pouvoir s’adapter
au contexte d’affichage. La taille MD est la taille par défaut.

Label tag

Label tag

Label tag

Label tag

    
    
                    <p class="fr-tag">Label tag</p>
    <p class="fr-tag fr-fi-arrow-right-line fr-tag--icon-left">Label tag</p>
    
    <p class="fr-tag fr-tag--sm">Label tag</p>
    <p class="fr-tag fr-tag--sm fr-fi-arrow-right-line fr-tag--icon-left">Label tag</p> 
                    
                  

## Groupe de tags non cliquables

Les tags peuvent être utilisés à plusieurs dans des groupes de tags. Dans ce
cas-là ils appliquent des espacement préalablement définis par le DSFR.

  * Label tag

  * Label tag

  * Label tag

    
    
                    <ul class="fr-tags-group">
        <li>
            <p class="fr-tag fr-tag--sm">Label tag</p>
        </li>
        <li>
            <p class="fr-tag fr-tag--sm">Label tag</p>
        </li>
        <li>
            <p class="fr-tag fr-tag--sm">Label tag</p>
        </li>
    </ul>
                    
                  

# Tag cliquable

## Structure

Le tag cliquable se compose des éléments suivants :

  * un libellé - obligatoire.
  * un lien - obligatoire. 
  * une icône - optionnelle.

Le tag cliquable donne accès à une page avec des contenus associés à ce tag
(liste de contenus, liste de résultats de recherche).

Label tag Label tag Label tag Label tag

    
    
                    <a href="#" class="fr-tag" target="_self">Label tag</a>
    <a href="#" class="fr-tag fr-fi-arrow-right-line fr-tag--icon-left" target="_self">Label tag</a>
    
    <a href="#" class="fr-tag fr-tag--sm" target="_self">Label tag</a>
    <a href="#" class="fr-tag fr-fi-arrow-right-line fr-tag--sm fr-tag--icon-left" target="_self">Label tag</a>
    
                    
                  

## Tailles

Tous les tags sont disponibles en deux tailles SM et MD pour pouvoir s’adapter
au contexte d’affichage. La taille MD est la taille par défaut.

Label tag Label tag Label tag Label tag

    
    
                    <a href="#" class="fr-tag" target="_self">Label tag</a>
    <a href="#" class="fr-tag fr-fi-arrow-right-line fr-tag--icon-left" target="_self">Label tag</a>
    
    <a href="#" class="fr-tag fr-tag--sm" target="_self">Label tag</a>
    <a href="#" class="fr-tag fr-fi-arrow-right-line fr-tag--sm fr-tag--icon-left" target="_self">Label tag</a>
    
                    
                  

## Groupe de tags cliquables

Les tags peuvent être utilisés à plusieurs dans des groupes de tags. Dans ce
cas-là ils appliquent des espacement préalablement définis par le DSFR.

#### Groupe de tags cliquables MD

  * Label tag
  * Label tag
  * Label tag

###  Extrait de code

    
    
                          <ul class="fr-tags-group">
        <li>
            <a href="#" class="fr-tag" target="_self">Label tag</a>
        </li>
        <li>
            <a href="#" class="fr-tag" target="_self">Label tag</a>
        </li>
        <li>
            <a href="#" class="fr-tag" target="_self">Label tag</a>
        </li>
    </ul>
                          
                        

#### Groupe de tags cliquables SM

  * Label tag
  * Label tag
  * Label tag

###  Extrait de code

    
    
                          
    <ul class="fr-tag-list">
        <li>
            <a href="#" class="fr-tag fr-tag--sm" target="_self">Label tag</a>
        </li>
        <li>
            <a href="#" class="fr-tag fr-tag--sm" target="_self">Label tag</a>
        </li>
        <li>
            <a href="#" class="fr-tag fr-tag--sm" target="_self">Label tag</a>
        </li>
    </ul>
    
    
                          
                        

À noter que pour le groupe de tags SM le padding autour du tag est plus
important que lorsqu’il est utilisé seul pour permettre le tap en mobile. Afin
de passer le groupe de tag en taille SM.

# Tag selectionnable (utilisation en filtre)

## Structure

Il se compose des éléments suivants :

  * un libellé - obligatoire. 
  * une coche quand il est sélectionné - obligatoire.

Le tag sélectionnable permet d’activer/désactiver un filtre (liste de
contenus, liste de résultats de recherche). Il reste en place qu’il soit
sélectionné ou désélectionné.

Il est préférable de ne pas utiliser plus de 6 tags sélectionnables dans un
groupe, pour permettre à l’utilisateur de scanner rapidement la liste de
filtres. Dans le cas où il y a plus de 6 filtres, utiliser un tag supprimable
associé à une liste déroulante.

Label tag Label tag sélectionné Label tag Label tag sélectionné

    
    
                    <button class="fr-tag" aria-pressed="false">Label tag</button>
    <button class="fr-tag" aria-pressed="true">Label tag sélectionné</button>
    
    <!-- SM -->
    <button class="fr-tag fr-tag--sm" aria-pressed="false">Label tag</button>
    <button class="fr-tag fr-tag--sm" aria-pressed="true">Label tag sélectionné</button>
                    
                  

**À ne pas faire** \- Utiliser plus de 6 tags sélectionnables pour un même
filtre (ici la thématique)

![](/uploads/Dont_Plus_de_6_tag_select_081d9b8ec0.jpg)

**À faire** \- Utiliser plutôt des tags supprimables associés à une liste
déroulante

![](/uploads/do_utiliser_tag_supp_bbc653c2d3.jpg)

## Tailles

Tous les tags sont disponibles en deux tailles SM et MD pour pouvoir s’adapter
au contexte d’affichage. La taille MD est la taille par défaut. La taille SM
est obtenue par l’ajout du modificateur `fr-tag--sm` .

## Groupes de tags selectionnables

Les tags peuvent être utilisés à plusieurs dans des groupes de tags. Dans ce
cas-là ils appliquent des espacement préalablement définis par le DSFR.

Il est préférable de ne pas utiliser plus de 6 tags activables dans un groupe.

Le groupe est obtenu par une liste `<ul class="fr-tag-list">` (cf exemples
précédents)

# Tag supprimable (utilisation en filtre)

## Structure

Il se compose des éléments suivants :

  * un libellé - obligatoire. 
  * une croix - obligatoire.

Le tag supprimable permet de désactiver un filtre (liste de contenus, liste de
résultats de recherche). Il n’est visible que si l’option de filtre est
sélectionnée.

Le tag ‘supprimable’ n’autorise pas l’utilisation d’icône (autre que la croix
de suppression déjà présente)

Label tag

    
    
                    <button class="fr-tag fr-tag--sm fr-tag--dismiss" aria-label="Retirer [A Modifier - le filtre Label tag]" onclick="event.preventDefault(); this.parentNode.removeChild(this);">Label tag</button>
                    
                  

**Pour les développeurs  
** L’attribut aria-label doit contenir ‘Retirer’ suivi de l’intitulé du filter
visible à l'écran afin de préciser à l’utilisateur l’action réalisable sur le
bouton.

Le javascript donné en exemple est indicatif, à vous de l’implémenter dans
votre environnement.

**À ne pas faire** \- Utiliser une icône sur le tag supprimable

![](/uploads/Capture_d_ecran_2022_01_17_a_18_24_22_e126dce0dc.png)

## Tailles

Tous les tags sont disponibles en deux tailles SM et MD pour pouvoir s’adapter
au contexte d’affichage. La taille MD est la taille par défaut. La taille SM
est obtenue par l’ajout du modificateur `fr-tag--sm` .

## Groupes de tags supprimables

Les tags peuvent être utilisés à plusieurs dans des groupes de tags. Dans ce
cas-là ils appliquent des espacement préalablement définis par le DSFR.Le
groupe est obtenu par une liste `<ul class="fr-tag-list">` (cf exemples
précédents)

# Règles d’utilisation

## Usages

Les tags servent à regrouper par catégorie des contenus (par thème, sujet,
type de document etc…). Ils ne servent pas à donner des informations de
complément à la catégorisation (auteur, date...). Pour ce faire, vous pouvez
utiliser l’élément « détail » prévu sur [les cartes](/elements-d-
interface/composants/carte), et la typo XS « mention » pour les page de
contenu.

Les tags ne doivent pas être utilisés comme [des badges](/elements-d-
interface/composants/badge), ils ne servent pas à donner le statut du contenu
auquel il est associé.

## Accessibilité

Les tags doivent être dans des éléments <p>, <li> ou <a>.

Dans le cas d’un tag cliquable, un attribut title peut être ajouté pour
préciser la cible du lien :

    
    
    <a href=”tag/bike/” title=“Voir tous les articles concernant le vélo”>Vélo</a>

## Contenus

Les libellés des tags doivent être courts et clairs.

## Personnalisation

Les tags cliquables peuvent être accentués.  

[ Tableau - Table 🆕](/composants-et-modeles/composants/tableau)

[Téléchargement de fichier - Download](/composants-et-
modeles/composants/telechargement-de-fichier)

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
