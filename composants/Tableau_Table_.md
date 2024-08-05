Fermer

#  Tableau - Table 🆕

Le tableau permet de présenter une liste structurée de données textuelles
et/ou numériques dans le but de simplifier l’analyse et la comparaison
d’informations pour l’utilisateur.

### La version 1.12 apporte une nouvelle version du composant Tableau - Table  

Cette évolution amène notamment différentes variations de taille, des
fonctionnalités de tri à l’intérieur des colonnes et la possibilité d’intégrer
d’autres composants à l’intérieur des cellules. Si vous utilisez déjà des
tableaux sur votre site, la version 1.12 fera évoluer leur design tout en
conservant leurs fonctionnalités mais ils ne seront plus mis à jour dans le
futur.  
[Leur code reste visible sur ce lien](https://main--ds-
gouv.netlify.app/example/component/table/deprecated/)  

## Usage

**Quand l’utiliser ?**

  * Pour permettre une visualisation de données organisées en lignes et en colonnes
  * Pour permettre l’analyse et la comparaison d’informations
  * Pour servir d’alternative textuelle à un graphique, si vous souhaitez que l'utilisateur puisse lire les valeurs exactes des données plutôt que de les estimer visuellement par exemple

**Quand ne pas l’utiliser ?**

Si les tableaux sont très pratiques, ils peuvent très vite devenir complexes
et générer des difficultés de compréhension. Soyez donc créatifs pour que
votre interface soit synthétique, intuitive et agréable à utiliser en
proposant, si c’est nécessaire, plusieurs modes de présentation des données.
Vous trouverez des exemples de vues alternatives dans la planche Figma.

  * Envisagez d'autres formats de présentation lorsque les données sont très simples, par exemple si votre tableau possède moins de 4 lignes ou moins de 3 colonnes.
  * Sur des écrans plus petits, envisagez d’autres formats de présentation pour les données des tableaux. Les données d’un tableau peuvent, par exemple, être présentées sous la forme de listes ou de cartes (lien vers le composant).
  * Ce composant tableau n’est pas un tableur, il ne permet pas (sauf développement ad hoc) de réaliser d'opérations avec les données.  

  * N'utilisez pas de tableaux pour créer des mises en page. Les tableaux sont destinés à présenter des données.

## Structure

![](/uploads/tableau_structure_db3388e63d.png)

  * 1 — Un titre (caption) - obligatoire - qui peut être positionné en haut (par défaut), en bas ou hors écran
  * 2 — Une ligne d’en-tête de colonne (thead) - obligatoire
  * 3 — Plusieurs ligne de corps - obligatoires
  * 4 — Des bordures horizontales entre les lignes - obligatoires
  * 5 — Des bordure verticales entre les colonnes - optionnelles (obligatoires dans le cas d’un tableau complexe)
  * 6 — Une colonne d’en-tête de ligne à gauche du tableau - optionnelle
  * 7 — Une colonne de sélection de ligne - optionnelle, toujours ferrée à gauche
  * 8 — Une barre d’actions haute - optionnelle 
    * Cette barre d'actions haute peut contenir uniquement et dans cet ordre : le nombre de lignes sélectionnées, une barre de recherche, des boutons d’actions liés à la sélection de lignes et un contrôle segmenté.
  * 9 — Une barre d’actions basse - optionnelle 
    * Cette barre d'actions basse peut contenir uniquement et dans cet ordre : le nombre total de lignes du tableau, une liste déroulante, une pagination, des boutons d’actions agissants sur tout le tableau.

## Spécifications

  * Par défaut, la largeur des cellules s’adapte automatiquement à votre contenu. Mais les largeurs peuvent être adaptées en développement par les classes fr-col.
  * Le conteneur du tableau peut être scrollable horizontalement. Ceci est courant sur les écrans plus petits où il peut être impossible d'afficher le tableau complet sur l'écran de l'appareil. Prenez garde toutefois à ce que les informations clés soit visibles au premier coup d’oeil même sur un écran de petite taille.
  * Le conteneur est responsive par défaut mais vous pouvez lui donner une taille fixe grâce à la classe fr-table-no-scroll.

## Variation(s)

### Tailles

Il existe 3 tailles pour les cellules du tableau : SM / MD / LG. Si la taille
des composants intégrés dans les cellules ne change pas, cela vous permet de
varier la densité d’affichage de votre tableau en fonction de son contenu.

#### Tableau simple SM

Titre du tableau (caption)  th0  |  th1  |  th2  |  th3  
---|---|---|---  
Lorem [...] elit ut.  |  Lorem [...] elit ut.  |  Lorem [...] elit ut.  |
Lorem [...] elit ut.  
Lorem [...] elit ut.  |  Lorem [...] elit ut.  |  Lorem [...] elit ut.  |
Lorem [...] elit ut.  
Lorem [...] elit ut.  |  Lorem [...] elit ut.  |  Lorem [...] elit ut.  |
Lorem [...] elit ut.  
Lorem [...] elit ut.  |  Lorem [...] elit ut.  |  Lorem [...] elit ut.  |
Lorem [...] elit ut.  
  
###  Extrait de code

    
    
                          <div class="fr-table--sm fr-table fr-table" id="table-sm-component">
        <div class="fr-table__wrapper">
            <div class="fr-table__container">
                <div class="fr-table__content">
                    <table id="table-sm">
                        <caption>
                            Titre du tableau (caption)
                        </caption>
                        <thead>
                            <tr>
                                <th scope="col">
                                    th0
                                </th>
                                <th scope="col">
                                    th1
                                </th>
                                <th scope="col">
                                    th2
                                </th>
                                <th scope="col">
                                    th3
                                </th>
                            </tr>
                        </thead>
                        <tbody>
                            <tr id="table-sm-row-key-1" data-row-key="1">
                                <td>
                                    Lorem [...] elit ut.
                                </td>
                                <td>
                                    Lorem [...] elit ut.
                                </td>
                                <td>
                                    Lorem [...] elit ut.
                                </td>
                                <td>
                                    Lorem [...] elit ut.
                                </td>
                            </tr>
                            <tr id="table-sm-row-key-2" data-row-key="2">
                                <td>
                                    Lorem [...] elit ut.
                                </td>
                                <td>
                                    Lorem [...] elit ut.
                                </td>
                                <td>
                                    Lorem [...] elit ut.
                                </td>
                                <td>
                                    Lorem [...] elit ut.
                                </td>
                            </tr>
                            <tr id="table-sm-row-key-3" data-row-key="3">
                                <td>
                                    Lorem [...] elit ut.
                                </td>
                                <td>
                                    Lorem [...] elit ut.
                                </td>
                                <td>
                                    Lorem [...] elit ut.
                                </td>
                                <td>
                                    Lorem [...] elit ut.
                                </td>
                            </tr>
                            <tr id="table-sm-row-key-4" data-row-key="4">
                                <td>
                                    Lorem [...] elit ut.
                                </td>
                                <td>
                                    Lorem [...] elit ut.
                                </td>
                                <td>
                                    Lorem [...] elit ut.
                                </td>
                                <td>
                                    Lorem [...] elit ut.
                                </td>
                            </tr>
                        </tbody>
                    </table>
                </div>
            </div>
        </div>
    </div>
                          
                        

#### Tableau simple MD - par défaut

Titre du tableau (caption)  th0  |  th1  |  th2  |  th3  
---|---|---|---  
Lorem [...] elit ut.  |  Lorem [...] elit ut.  |  Lorem [...] elit ut.  |
Lorem [...] elit ut.  
Lorem [...] elit ut.  |  Lorem [...] elit ut.  |  Lorem [...] elit ut.  |
Lorem [...] elit ut.  
Lorem [...] elit ut.  |  Lorem [...] elit ut.  |  Lorem [...] elit ut.  |
Lorem [...] elit ut.  
Lorem [...] elit ut.  |  Lorem [...] elit ut.  |  Lorem [...] elit ut.  |
Lorem [...] elit ut.  
  
###  Extrait de code

    
    
                          <div class="fr-table" id="table-md-component">
        <div class="fr-table__wrapper">
            <div class="fr-table__container">
                <div class="fr-table__content">
                    <table id="table-md">
                        <caption>
                            Titre du tableau (caption)
                        </caption>
                        <thead>
                            <tr>
                                <th scope="col">
                                    th0
                                </th>
                                <th scope="col">
                                    th1
                                </th>
                                <th scope="col">
                                    th2
                                </th>
                                <th scope="col">
                                    th3
                                </th>
                            </tr>
                        </thead>
                        <tbody>
                            <tr id="table-md-row-key-1" data-row-key="1">
                                <td>
                                    Lorem [...] elit ut.
                                </td>
                                <td>
                                    Lorem [...] elit ut.
                                </td>
                                <td>
                                    Lorem [...] elit ut.
                                </td>
                                <td>
                                    Lorem [...] elit ut.
                                </td>
                            </tr>
                            <tr id="table-md-row-key-2" data-row-key="2">
                                <td>
                                    Lorem [...] elit ut.
                                </td>
                                <td>
                                    Lorem [...] elit ut.
                                </td>
                                <td>
                                    Lorem [...] elit ut.
                                </td>
                                <td>
                                    Lorem [...] elit ut.
                                </td>
                            </tr>
                            <tr id="table-md-row-key-3" data-row-key="3">
                                <td>
                                    Lorem [...] elit ut.
                                </td>
                                <td>
                                    Lorem [...] elit ut.
                                </td>
                                <td>
                                    Lorem [...] elit ut.
                                </td>
                                <td>
                                    Lorem [...] elit ut.
                                </td>
                            </tr>
                            <tr id="table-md-row-key-4" data-row-key="4">
                                <td>
                                    Lorem [...] elit ut.
                                </td>
                                <td>
                                    Lorem [...] elit ut.
                                </td>
                                <td>
                                    Lorem [...] elit ut.
                                </td>
                                <td>
                                    Lorem [...] elit ut.
                                </td>
                            </tr>
                        </tbody>
                    </table>
                </div>
            </div>
        </div>
    </div>
                          
                        

#### Tableau simple LG

Titre du tableau (caption)  th0  |  th1  |  th2  |  th3  
---|---|---|---  
Lorem [...] elit ut.  |  Lorem [...] elit ut.  |  Lorem [...] elit ut.  |
Lorem [...] elit ut.  
Lorem [...] elit ut.  |  Lorem [...] elit ut.  |  Lorem [...] elit ut.  |
Lorem [...] elit ut.  
Lorem [...] elit ut.  |  Lorem [...] elit ut.  |  Lorem [...] elit ut.  |
Lorem [...] elit ut.  
Lorem [...] elit ut.  |  Lorem [...] elit ut.  |  Lorem [...] elit ut.  |
Lorem [...] elit ut.  
  
###  Extrait de code

    
    
                          <div class="fr-table--lg fr-table fr-table" id="table-lg-component">
        <div class="fr-table__wrapper">
            <div class="fr-table__container">
                <div class="fr-table__content">
                    <table id="table-lg">
                        <caption>
                            Titre du tableau (caption)
                        </caption>
                        <thead>
                            <tr>
                                <th scope="col">
                                    th0
                                </th>
                                <th scope="col">
                                    th1
                                </th>
                                <th scope="col">
                                    th2
                                </th>
                                <th scope="col">
                                    th3
                                </th>
                            </tr>
                        </thead>
                        <tbody>
                            <tr id="table-lg-row-key-1" data-row-key="1">
                                <td>
                                    Lorem [...] elit ut.
                                </td>
                                <td>
                                    Lorem [...] elit ut.
                                </td>
                                <td>
                                    Lorem [...] elit ut.
                                </td>
                                <td>
                                    Lorem [...] elit ut.
                                </td>
                            </tr>
                            <tr id="table-lg-row-key-2" data-row-key="2">
                                <td>
                                    Lorem [...] elit ut.
                                </td>
                                <td>
                                    Lorem [...] elit ut.
                                </td>
                                <td>
                                    Lorem [...] elit ut.
                                </td>
                                <td>
                                    Lorem [...] elit ut.
                                </td>
                            </tr>
                            <tr id="table-lg-row-key-3" data-row-key="3">
                                <td>
                                    Lorem [...] elit ut.
                                </td>
                                <td>
                                    Lorem [...] elit ut.
                                </td>
                                <td>
                                    Lorem [...] elit ut.
                                </td>
                                <td>
                                    Lorem [...] elit ut.
                                </td>
                            </tr>
                            <tr id="table-lg-row-key-4" data-row-key="4">
                                <td>
                                    Lorem [...] elit ut.
                                </td>
                                <td>
                                    Lorem [...] elit ut.
                                </td>
                                <td>
                                    Lorem [...] elit ut.
                                </td>
                                <td>
                                    Lorem [...] elit ut.
                                </td>
                            </tr>
                        </tbody>
                    </table>
                </div>
            </div>
        </div>
    </div>
                          
                        

### Séparateurs verticaux

Vous avez également la possibilité de mettre des séparateurs de colonnes
(obligatoires en cas de tableaux complexes)

#### Tableau simple avec bordures verticales

Titre du tableau (caption)  th0  |  th1  |  th2  |  th3  
---|---|---|---  
Lorem [...] elit ut.  |  Lorem [...] elit ut.  |  Lorem [...] elit ut.  |
Lorem [...] elit ut.  
Lorem [...] elit ut.  |  Lorem [...] elit ut.  |  Lorem [...] elit ut.  |
Lorem [...] elit ut.  
Lorem [...] elit ut.  |  Lorem [...] elit ut.  |  Lorem [...] elit ut.  |
Lorem [...] elit ut.  
Lorem [...] elit ut.  |  Lorem [...] elit ut.  |  Lorem [...] elit ut.  |
Lorem [...] elit ut.  
  
###  Extrait de code

    
    
                          <div class="fr-table fr-table--bordered" id="table-bordered-component">
        <div class="fr-table__wrapper">
            <div class="fr-table__container">
                <div class="fr-table__content">
                    <table id="table-bordered">
                        <caption>
                            Titre du tableau (caption)
                        </caption>
                        <thead>
                            <tr>
                                <th scope="col">
                                    th0
                                </th>
                                <th scope="col">
                                    th1
                                </th>
                                <th scope="col">
                                    th2
                                </th>
                                <th scope="col">
                                    th3
                                </th>
                            </tr>
                        </thead>
                        <tbody>
                            <tr id="table-bordered-row-key-1" data-row-key="1">
                                <td>
                                    Lorem [...] elit ut.
                                </td>
                                <td>
                                    Lorem [...] elit ut.
                                </td>
                                <td>
                                    Lorem [...] elit ut.
                                </td>
                                <td>
                                    Lorem [...] elit ut.
                                </td>
                            </tr>
                            <tr id="table-bordered-row-key-2" data-row-key="2">
                                <td>
                                    Lorem [...] elit ut.
                                </td>
                                <td>
                                    Lorem [...] elit ut.
                                </td>
                                <td>
                                    Lorem [...] elit ut.
                                </td>
                                <td>
                                    Lorem [...] elit ut.
                                </td>
                            </tr>
                            <tr id="table-bordered-row-key-3" data-row-key="3">
                                <td>
                                    Lorem [...] elit ut.
                                </td>
                                <td>
                                    Lorem [...] elit ut.
                                </td>
                                <td>
                                    Lorem [...] elit ut.
                                </td>
                                <td>
                                    Lorem [...] elit ut.
                                </td>
                            </tr>
                            <tr id="table-bordered-row-key-4" data-row-key="4">
                                <td>
                                    Lorem [...] elit ut.
                                </td>
                                <td>
                                    Lorem [...] elit ut.
                                </td>
                                <td>
                                    Lorem [...] elit ut.
                                </td>
                                <td>
                                    Lorem [...] elit ut.
                                </td>
                            </tr>
                        </tbody>
                    </table>
                </div>
            </div>
        </div>
    </div>
                          
                        

### Tableau non scrollable

Titre du tableau (caption)  th0  |  th1  |  th2  |  th3  
---|---|---|---  
Lorem [...] elit ut.  |  Lorem [...] elit ut.  |  Lorem [...] elit ut.  |
Lorem [...] elit ut.  
Lorem [...] elit ut.  |  Lorem [...] elit ut.  |  Lorem [...] elit ut.  |
Lorem [...] elit ut.  
Lorem [...] elit ut.  |  Lorem [...] elit ut.  |  Lorem [...] elit ut.  |
Lorem [...] elit ut.  
Lorem [...] elit ut.  |  Lorem [...] elit ut.  |  Lorem [...] elit ut.  |
Lorem [...] elit ut.  
  
###  Extrait de code

    
    
                          <div class="fr-table fr-table--no-scroll" id="table-no-scroll-component">
        <div class="fr-table__wrapper">
            <div class="fr-table__container">
                <div class="fr-table__content">
                    <table id="table-no-scroll">
                        <caption>
                            Titre du tableau (caption)
                        </caption>
                        <thead>
                            <tr>
                                <th scope="col">
                                    th0
                                </th>
                                <th scope="col">
                                    th1
                                </th>
                                <th scope="col">
                                    th2
                                </th>
                                <th scope="col">
                                    th3
                                </th>
                            </tr>
                        </thead>
                        <tbody>
                            <tr id="table-no-scroll-row-key-1" data-row-key="1">
                                <td>
                                    Lorem [...] elit ut.
                                </td>
                                <td>
                                    Lorem [...] elit ut.
                                </td>
                                <td>
                                    Lorem [...] elit ut.
                                </td>
                                <td>
                                    Lorem [...] elit ut.
                                </td>
                            </tr>
                            <tr id="table-no-scroll-row-key-2" data-row-key="2">
                                <td>
                                    Lorem [...] elit ut.
                                </td>
                                <td>
                                    Lorem [...] elit ut.
                                </td>
                                <td>
                                    Lorem [...] elit ut.
                                </td>
                                <td>
                                    Lorem [...] elit ut.
                                </td>
                            </tr>
                            <tr id="table-no-scroll-row-key-3" data-row-key="3">
                                <td>
                                    Lorem [...] elit ut.
                                </td>
                                <td>
                                    Lorem [...] elit ut.
                                </td>
                                <td>
                                    Lorem [...] elit ut.
                                </td>
                                <td>
                                    Lorem [...] elit ut.
                                </td>
                            </tr>
                            <tr id="table-no-scroll-row-key-4" data-row-key="4">
                                <td>
                                    Lorem [...] elit ut.
                                </td>
                                <td>
                                    Lorem [...] elit ut.
                                </td>
                                <td>
                                    Lorem [...] elit ut.
                                </td>
                                <td>
                                    Lorem [...] elit ut.
                                </td>
                            </tr>
                        </tbody>
                    </table>
                </div>
            </div>
        </div>
    </div>
                          
                        

## États

  * Défaut
  * Ligne sélectionnée

Les états désactivé, focus et cliqué sont propres aux composants au sein des
cellules

Titre du tableau (caption)  Sélectionner |  th0  |  th1  |  th2  |  th3  
---|---|---|---|---  
  
Sélectionner la ligne 1

|  Lorem [...] elit ut.  |  Lorem [...] elit ut.  |  Lorem [...] elit ut.  |
Lorem [...] elit ut.  
  
Sélectionner la ligne 2

|  Lorem [...] elit ut.  |  Lorem [...] elit ut.  |  Lorem [...] elit ut.  |
Lorem [...] elit ut.  
  
Sélectionner la ligne 3

|  Lorem [...] elit ut.  |  Lorem [...] elit ut.  |  Lorem [...] elit ut.  |
Lorem [...] elit ut.  
  
Sélectionner la ligne 4

|  Lorem [...] elit ut.  |  Lorem [...] elit ut.  |  Lorem [...] elit ut.  |
Lorem [...] elit ut.  
  
###  Extrait de code

    
    
                          <div class="fr-table" id="table-selectable-component">
        <div class="fr-table__wrapper">
            <div class="fr-table__container">
                <div class="fr-table__content">
                    <table id="table-selectable">
                        <caption>
                            Titre du tableau (caption)
                        </caption>
                        <thead>
                            <tr>
                                <th class="fr-cell--fixed" role="columnheader">
                                    <span class="fr-sr-only">Sélectionner</span>
                                </th>
                                <th scope="col">
                                    th0
                                </th>
                                <th scope="col">
                                    th1
                                </th>
                                <th scope="col">
                                    th2
                                </th>
                                <th scope="col">
                                    th3
                                </th>
                            </tr>
                        </thead>
                        <tbody>
                            <tr id="table-selectable-row-key-1" data-row-key="1">
                                <th class="fr-cell--fixed" scope="row">
                                    <div class="fr-checkbox-group fr-checkbox-group--sm">
                                        <input name="row-select" id="table-select-checkbox-7748--0" type="checkbox">
                                        <label class="fr-label" for="table-select-checkbox-7748--0">
                                            Sélectionner la ligne 1
                                        </label>
                                    </div>
                                </th>
                                <td>
                                    Lorem [...] elit ut.
                                </td>
                                <td>
                                    Lorem [...] elit ut.
                                </td>
                                <td>
                                    Lorem [...] elit ut.
                                </td>
                                <td>
                                    Lorem [...] elit ut.
                                </td>
                            </tr>
                            <tr id="table-selectable-row-key-2" data-row-key="2">
                                <th class="fr-cell--fixed" scope="row">
                                    <div class="fr-checkbox-group fr-checkbox-group--sm">
                                        <input name="row-select" id="table-select-checkbox-7750--1" type="checkbox">
                                        <label class="fr-label" for="table-select-checkbox-7750--1">
                                            Sélectionner la ligne 2
                                        </label>
                                    </div>
                                </th>
                                <td>
                                    Lorem [...] elit ut.
                                </td>
                                <td>
                                    Lorem [...] elit ut.
                                </td>
                                <td>
                                    Lorem [...] elit ut.
                                </td>
                                <td>
                                    Lorem [...] elit ut.
                                </td>
                            </tr>
                            <tr id="table-selectable-row-key-3" data-row-key="3">
                                <th class="fr-cell--fixed" scope="row">
                                    <div class="fr-checkbox-group fr-checkbox-group--sm">
                                        <input name="row-select" id="table-select-checkbox-7752--2" type="checkbox">
                                        <label class="fr-label" for="table-select-checkbox-7752--2">
                                            Sélectionner la ligne 3
                                        </label>
                                    </div>
                                </th>
                                <td>
                                    Lorem [...] elit ut.
                                </td>
                                <td>
                                    Lorem [...] elit ut.
                                </td>
                                <td>
                                    Lorem [...] elit ut.
                                </td>
                                <td>
                                    Lorem [...] elit ut.
                                </td>
                            </tr>
                            <tr id="table-selectable-row-key-4" data-row-key="4">
                                <th class="fr-cell--fixed" scope="row">
                                    <div class="fr-checkbox-group fr-checkbox-group--sm">
                                        <input name="row-select" id="table-select-checkbox-7754--3" type="checkbox">
                                        <label class="fr-label" for="table-select-checkbox-7754--3">
                                            Sélectionner la ligne 4
                                        </label>
                                    </div>
                                </th>
                                <td>
                                    Lorem [...] elit ut.
                                </td>
                                <td>
                                    Lorem [...] elit ut.
                                </td>
                                <td>
                                    Lorem [...] elit ut.
                                </td>
                                <td>
                                    Lorem [...] elit ut.
                                </td>
                            </tr>
                        </tbody>
                    </table>
                </div>
            </div>
        </div>
    </div>
                          
                        

## Fonctionnalités

Les tableaux peuvent comporter les fonctionnalités suivantes pour permettre à
vos utilisateurs d’interagir avec les données que vous leur mettez à
disposition. À ce stade, le Système de Design ne prévoit pas la possibilité
d’éditer le contenu des cellules.

#### Tri et ordre

  * Trier le contenu de chaque colonne, par ordre croissant ou décroissant

#### Navigation dans le tableau

  * Il est possible de rendre la première colonne flottante et de faire défiler le reste du tableau s’il est plus large que la fenêtre
  * S’il y a beaucoup de lignes, il est possible d’ajouter une pagination dans la barre d’outils
  * Il est possible de choisir le nombre de lignes affichées par page du tableau via une liste déroulante

#### Actions

  * Il est possible de sélectionner des lignes par une case à cocher placée tout à gauche de la ligne
  * Il est possible de mettre un ou des boutons d’actions spécifiques à une ligne dans une cellule. Pensez à utiliser les boutons secondaires et tertiaires pour apporter la bonne hiérarchie entre les différents niveaux d’actions possibles.
  * Il est possible d’intégrer une barre d'actions, toujours positionnée en haut à droite du tableau. Ces actions peuvent concerner les lignes sélectionnées (si vous utilisez cette fonctionnalité) ou l’entièreté du tableau (pour imprimer ou exporter par exemple).

#### Fusion de cellules

Il est possible de fusionner des cellules d’en-tête et de contenu, de façon
verticale et/ou horizontale (on parle dès lors de tableau complexe cf partie
Accessibilité)

Titre du tableau (caption)

(Résumé) Emploi du temps horaire des Groupes 1 et 2, le matin des jours de la
semaine ouvrée (Lundi au Vendredi) :

  * la première colonne représente le planning de la journée de Lundi pour les groupes 1 et 2,
  * la deuxième colonne représente le planning de la journée de Mardi pour les groupes 1 et 2,
  * la troisième colonne représente le planning des journées de Mercredi et Jeudi pour le groupe 1,
  * la quatrième colonne représente le planning des journées de Mercredi et Jeudi pour le groupe 2,
  * la cinquième colonne représente le planning de la journée de Vendredi pour les groupes 1 et 2.

Horaires |  Lundi  |  Mardi  |  Mercredi & Jeudi  
_Exemple de 2 cellules fusionnées dans le Header_ |  Vendredi  
---|---|---|---|---  
Groupes 1 & 2  |  Groupes 1 & 2  |  Groupe 1  |  Groupe 2  |  Groupes 1 & 2  
8h  |  Français  |  Mathématiques  |  LV1  |  Histoire - Géographie  |  EPS  
9h  |  Etude dirigée  
_Exemple de colspan sur toute la ligne_  
10h  |  Mathématiques  |  Histoire - Géographie  |  Arts appliqués  
|  LV2  |  Sciences  
11h  |  Français  |  EPS  |  Histoire - Géographie  |  Physique - Chimie  
12h  |  Sciences  |  LV1  |  EPS  
_Exemple de colspan sur 2 cellules_ |  LV2  
  
###  Extrait de code

    
    
                          <div class="fr-table fr-table--bordered" id="table-complex-component">
        <div class="fr-table__wrapper">
            <div class="fr-table__container">
                <div class="fr-table__content">
                    <table id="table-complex">
                        <caption>
                            Titre du tableau (caption)
                            <div class="fr-table__caption__desc">(Résumé) Emploi du temps horaire des Groupes 1 et 2, le matin des jours de la semaine ouvrée (Lundi au Vendredi) : <ul>
                                    <li>la première colonne représente le planning de la journée de Lundi pour les groupes 1 et 2,</li>
                                    <li>la deuxième colonne représente le planning de la journée de Mardi pour les groupes 1 et 2,</li>
                                    <li>la troisième colonne représente le planning des journées de Mercredi et Jeudi pour le groupe 1,</li>
                                    <li>la quatrième colonne représente le planning des journées de Mercredi et Jeudi pour le groupe 2,</li>
                                    <li>la cinquième colonne représente le planning de la journée de Vendredi pour les groupes 1 et 2.</li>
                                </ul>
                            </div>
                        </caption>
                        <thead>
                            <tr>
                                <th class="fr-cell--fixed" role="columnheader" rowspan="2" id="complex-thead-0-col-0">
                                    <span class="fr-sr-only">Horaires</span>
                                </th>
                                <th id="complex-thead-0-col-1">
                                    Lundi
                                </th>
                                <th id="complex-thead-0-col-2">
                                    Mardi
                                </th>
                                <th colspan="2" id="complex-thead-0-col-3">
                                    Mercredi & Jeudi
                                    <br>
                                    <i>Exemple de 2 cellules fusionnées dans le Header</i>
                                </th>
                                <th id="complex-thead-0-col-4">
                                    Vendredi
                                </th>
                            </tr>
                            <tr>
                                <th headers="complex-thead-0-col-1" id="complex-thead-1-col-0">
                                    Groupes 1 & 2
                                </th>
                                <th headers="complex-thead-0-col-2" id="complex-thead-1-col-1">
                                    Groupes 1 & 2
                                </th>
                                <th headers="complex-thead-0-col-3" id="complex-thead-1-col-2">
                                    Groupe 1
                                </th>
                                <th headers="complex-thead-0-col-3" id="complex-thead-1-col-3">
                                    Groupe 2
                                </th>
                                <th headers="complex-thead-0-col-4" id="complex-thead-1-col-4">
                                    Groupes 1 & 2
                                </th>
                            </tr>
                        </thead>
                        <tbody>
                            <tr id="table-complex-row-key-1" data-row-key="1">
                                <th class="fr-cell--fixed" id="complex-row-0" headers="complex-thead-0-col-0">
                                    8h
                                </th>
                                <td headers="complex-row-0 complex-thead-0-col-1 complex-thead-1-col-1">
                                    Français
                                </td>
                                <td headers="complex-row-0 complex-thead-0-col-2 complex-thead-1-col-2">
                                    Mathématiques
                                </td>
                                <td headers="complex-row-0 complex-thead-0-col-3 complex-thead-1-col-3">
                                    LV1
                                </td>
                                <td headers="complex-row-0 complex-thead-0-col-3 complex-thead-1-col-4">
                                    Histoire - Géographie
                                </td>
                                <td headers="complex-row-0 complex-thead-0-col-4 complex-thead-1-col-5">
                                    EPS
                                </td>
                            </tr>
                            <tr id="table-complex-row-key-2" data-row-key="2">
                                <th class="fr-cell--fixed" id="complex-row-1" headers="complex-thead-0-col-0">
                                    9h
                                </th>
                                <td colspan="5" headers="complex-row-1 complex-thead-0-col-1 complex-thead-0-col-2 complex-thead-0-col-3 complex-thead-0-col-4 complex-thead-1-col-1 complex-thead-1-col-2 complex-thead-1-col-3 complex-thead-1-col-4 complex-thead-1-col-5">
                                    Etude dirigée
                                    <br>
                                    <i>Exemple de colspan sur toute la ligne</i>
                                </td>
                            </tr>
                            <tr id="table-complex-row-key-3" data-row-key="3">
                                <th class="fr-cell--fixed" id="complex-row-2" headers="complex-thead-0-col-0">
                                    10h
                                </th>
                                <td headers="complex-row-2 complex-thead-0-col-1 complex-thead-1-col-1">
                                    Mathématiques
                                </td>
                                <td headers="complex-row-2 complex-thead-0-col-2 complex-thead-1-col-2">
                                    Histoire - Géographie
                                </td>
                                <td rowspan="2" headers="complex-row-2 complex-row-3 complex-thead-0-col-3 complex-thead-1-col-3">
                                    Arts appliqués
                                    <br>
                                    <svg aria-hidden="true" class="fr-artwork" viewBox="0 0 80 80" width="80px" height="80px">
                                        <use class="fr-artwork-decorative" href="../../../dist/artwork/pictograms/environment/environment.svg#artwork-decorative"></use>
                                        <use class="fr-artwork-minor" href="../../../dist/artwork/pictograms/environment/environment.svg#artwork-minor"></use>
                                        <use class="fr-artwork-major" href="../../../dist/artwork/pictograms/environment/environment.svg#artwork-major"></use>
                                    </svg>
                                </td>
                                <td headers="complex-row-2 complex-thead-0-col-3 complex-thead-1-col-4">
                                    LV2
                                </td>
                                <td headers="complex-row-2 complex-thead-0-col-4 complex-thead-1-col-5">
                                    Sciences
                                </td>
                            </tr>
                            <tr id="table-complex-row-key-4" data-row-key="4">
                                <th class="fr-cell--fixed" id="complex-row-3" headers="complex-thead-0-col-0">
                                    11h
                                </th>
                                <td headers="complex-row-3 complex-thead-0-col-1 complex-thead-1-col-1">
                                    Français
                                </td>
                                <td headers="complex-row-3 complex-thead-0-col-2 complex-thead-1-col-2">
                                    EPS
                                </td>
                                <td headers="complex-row-3 complex-thead-0-col-3 complex-thead-1-col-4">
                                    Histoire - Géographie
                                </td>
                                <td headers="complex-row-3 complex-thead-0-col-4 complex-thead-1-col-5">
                                    Physique - Chimie
                                </td>
                            </tr>
                            <tr id="table-complex-row-key-5" data-row-key="5">
                                <th class="fr-cell--fixed" id="complex-row-4" headers="complex-thead-0-col-0">
                                    12h
                                </th>
                                <td headers="complex-row-4 complex-thead-0-col-1 complex-thead-1-col-1">
                                    Sciences
                                </td>
                                <td headers="complex-row-4 complex-thead-0-col-2 complex-thead-1-col-2">
                                    LV1
                                </td>
                                <td colspan="2" headers="complex-row-4 complex-thead-0-col-3 complex-thead-1-col-3 complex-thead-1-col-4">
                                    EPS
                                    <br>
                                    <i>Exemple de colspan sur 2 cellules</i>
                                </td>
                                <td headers="complex-row-4 complex-thead-0-col-4 complex-thead-1-col-5">
                                    LV2
                                </td>
                            </tr>
                        </tbody>
                    </table>
                </div>
            </div>
        </div>
    </div>
                          
                        

## Contenu des cellules

### Contenus autorisés

Vous pouvez intégrer dans les cellules du tableau les types d’éléments
suivants :

  * Texte
  * Chiffres
  * Icône
  * Pictogramme
  * Tag et groupe de tags
  * Badge et groupe de badges
  * Bouton et groupe de boutons
  * Lien
  * Champ de saisie
  * Info-bulle
  * Interrupteur
  * Liste déroulante

### Alignement

Par défaut, le contenu des cellules est aligné à gauche et centré
verticalement. Vous avez à votre disposition des classes CSS pour modifier
l’alignement des cellules de contenu :

fr-cell--top, fr-cell--bottom pour l'alignement vertical et fr-cell--center,
fr-cell--right pour l'alignement horizontal

Titre du tableau (caption)  top  |  bottom  |  center  |  right  
---|---|---|---  
Lorem [...] elit ut.  |  Lorem [...] elit ut.  |  Lorem [...] elit ut.  |
Lorem  
Lorem [...  
Lorem [...] elit ut.  
Lorem [...] elit ut.  |  Lorem [...] elit ut.  |  Lorem [...] elit ut.  |
Lorem  
Lorem [...  
Lorem [...] elit ut.  
Lorem [...] elit ut.  |  Lorem [...] elit ut.  |  Lorem [...] elit ut.  |
Lorem  
Lorem [...  
Lorem [...] elit ut.  
Lorem [...] elit ut.  |  Lorem [...] elit ut.  |  Lorem [...] elit ut.  |
Lorem  
Lorem [...  
Lorem [...] elit ut.  
  
###  Extrait de code

    
    
                          <div class="fr-table fr-table--bordered" id="table-default-component">
        <div class="fr-table__wrapper">
            <div class="fr-table__container">
                <div class="fr-table__content">
                    <table id="table-default">
                        <caption>
                            Titre du tableau (caption)
                        </caption>
                        <thead>
                            <tr>
                                <th>
                                    top
                                </th>
                                <th>
                                    bottom
                                </th>
                                <th>
                                    center
                                </th>
                                <th>
                                    right
                                </th>
                            </tr>
                        </thead>
                        <tbody>
                            <tr id="table-default-row-key-1" data-row-key="1">
                                <td class="fr-cell--top">
                                    Lorem [...] elit ut.
                                </td>
                                <td class="fr-cell--bottom">
                                    Lorem [...] elit ut.
                                </td>
                                <td class="fr-cell--center">
                                    Lorem [...] elit ut.
                                </td>
                                <td class="fr-cell--right">
                                    Lorem
                                    <br>Lorem [...
                                    <br>Lorem [...] elit ut.
                                </td>
                            </tr>
                            <tr id="table-default-row-key-2" data-row-key="2">
                                <td class="fr-cell--top">
                                    Lorem [...] elit ut.
                                </td>
                                <td class="fr-cell--bottom">
                                    Lorem [...] elit ut.
                                </td>
                                <td class="fr-cell--center">
                                    Lorem [...] elit ut.
                                </td>
                                <td class="fr-cell--right">
                                    Lorem
                                    <br>Lorem [...
                                    <br>Lorem [...] elit ut.
                                </td>
                            </tr>
                            <tr id="table-default-row-key-3" data-row-key="3">
                                <td class="fr-cell--top">
                                    Lorem [...] elit ut.
                                </td>
                                <td class="fr-cell--bottom">
                                    Lorem [...] elit ut.
                                </td>
                                <td class="fr-cell--center">
                                    Lorem [...] elit ut.
                                </td>
                                <td class="fr-cell--right">
                                    Lorem
                                    <br>Lorem [...
                                    <br>Lorem [...] elit ut.
                                </td>
                            </tr>
                            <tr id="table-default-row-key-4" data-row-key="4">
                                <td class="fr-cell--top">
                                    Lorem [...] elit ut.
                                </td>
                                <td class="fr-cell--bottom">
                                    Lorem [...] elit ut.
                                </td>
                                <td class="fr-cell--center">
                                    Lorem [...] elit ut.
                                </td>
                                <td class="fr-cell--right">
                                    Lorem
                                    <br>Lorem [...
                                    <br>Lorem [...] elit ut.
                                </td>
                            </tr>
                        </tbody>
                    </table>
                </div>
            </div>
        </div>
    </div>
                          
                        

Le contenu en ligne des cellules est par défaut affiché sur une seule ligne
grâce à la propriété CSS white-space: nowrap; qui empêche des retours à la
ligne. Ce comportement peut être désactivé en ajoutant la classe fr-cell--
multiline sur l'element <table>, une ligne <tr> ou une cellule <th> ou <td> du
tableau.

Titre du tableau (caption)  th0  |  th1  |  th2  |  th3  
---|---|---|---  
Lorem [...] elit ut.  |  Lorem [...] elit ut.  |  Lorem [...] elit ut.  |
Lorem [...] elit ut.  
Lorem [...] elit ut.  |  Lorem [...] elit ut.  |  Lorem [...] elit ut.  |
Lorem [...] elit ut.  
Lorem [...] elit ut.  |  Lorem [...] elit ut.  |  Lorem [...] elit ut.  |
Lorem [...] elit ut.  
Lorem [...] elit ut.  |  Lorem [...] elit ut.  |  Lorem [...] elit ut.  |
Lorem [...] elit ut.  
  
###  Extrait de code

    
    
                          <div class="fr-table" id="table-multiline-component">
        <div class="fr-table__wrapper">
            <div class="fr-table__container">
                <div class="fr-table__content">
                    <table class="fr-cell--multiline" id="table-multiline">
                        <caption>
                            Titre du tableau (caption)
                        </caption>
                        <thead>
                            <tr>
                                <th scope="col">
                                    th0
                                </th>
                                <th scope="col">
                                    th1
                                </th>
                                <th scope="col">
                                    th2
                                </th>
                                <th scope="col">
                                    th3
                                </th>
                            </tr>
                        </thead>
                        <tbody>
                            <tr id="table-multiline-row-key-1" data-row-key="1">
                                <td>
                                    Lorem [...] elit ut.
                                </td>
                                <td>
                                    Lorem [...] elit ut.
                                </td>
                                <td>
                                    Lorem [...] elit ut.
                                </td>
                                <td>
                                    Lorem [...] elit ut.
                                </td>
                            </tr>
                            <tr id="table-multiline-row-key-2" data-row-key="2">
                                <td>
                                    Lorem [...] elit ut.
                                </td>
                                <td>
                                    Lorem [...] elit ut.
                                </td>
                                <td>
                                    Lorem [...] elit ut.
                                </td>
                                <td>
                                    Lorem [...] elit ut.
                                </td>
                            </tr>
                            <tr id="table-multiline-row-key-3" data-row-key="3">
                                <td>
                                    Lorem [...] elit ut.
                                </td>
                                <td>
                                    Lorem [...] elit ut.
                                </td>
                                <td>
                                    Lorem [...] elit ut.
                                </td>
                                <td>
                                    Lorem [...] elit ut.
                                </td>
                            </tr>
                            <tr id="table-multiline-row-key-4" data-row-key="4">
                                <td>
                                    Lorem [...] elit ut.
                                </td>
                                <td>
                                    Lorem [...] elit ut.
                                </td>
                                <td>
                                    Lorem [...] elit ut.
                                </td>
                                <td>
                                    Lorem [...] elit ut.
                                </td>
                            </tr>
                        </tbody>
                    </table>
                </div>
            </div>
        </div>
    </div>
                          
                        

## Accessibilité

Sur ce composant plus qu’ailleurs, le respect des règles de gestion de
l’accessibilité est primordial pour assurer la bonne utilisation par les
technologies d’assistance. Les pré-requis sont :

  * Le tableau propose une balise caption contenant un titre pertinent
  * Les en-têtes de lignes et de colonnes doivent être déclarées comme telles (balise th)
  * Les cellules d'en-têtes (th) doivent être associées aux cellules de données : 
    * Pour les en-têtes de ligne avec un attribut scope="row" ;
    * Pour les en-têtes de colonne avec un attribut scope="col".
  * Dans les tableaux dits complexes, l’utilisation de cellules fusionnées en en-tête ou dans le corps du tableau implique de préciser la composition du tableau dans le caption afin d’aider un utilisateur à appréhender son contenu. Il faudra également lier les cellules de contenu aux cellules d’en-tête via l’attribut headers et les id des cellules d’en-tête séparés par un espace. Dans ce cas, les attributs d’en-tête de ligne et colonne scope n’ont plus lieu d’être ajoutés. Source Acces42

## Bonnes pratiques

  * Synthétisez les contenus à l’intérieur de chaque cellule
  * Alignez les chiffres à droite au sein de la cellule
  * Utilisez des titres de colonne et, le cas échéant, de lignes, clairs et concis
  * Les titres de colonnes commencent toujours par une majuscule et ne se terminent jamais par un élément de ponctuation (virgule, point ou point virgule)
  * Si une colonne intègre une unité de mesure, il est nécessaire que l’information soit donnée dans le titre, afin d'éviter les répétitions dans les cellules de contenu
  * Placez les actions de colonnes toujours à droite au sein de la cellule d’en-tête
  * Si une cellule est vide, indiquez “N/A”
  * Placez la colonne de case à cocher à gauche
  * Placez la cellule d’action par ligne à droite
  * Améliorez la lisibilité du tableau en version mobile en utilisant une vue plus adaptée comme la liste
  * Utilisez des bordures verticales pour améliorer la lisibilité du tableau

## Personnalisation

Aucune personnalisation n’est possible sur ce composant

[Sommaire - Summary](/composants-et-modeles/composants/sommaire)

[Tag - Tag](/composants-et-modeles/composants/tag)

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
