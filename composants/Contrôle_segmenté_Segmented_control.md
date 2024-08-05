Fermer

# Contrôle segmenté - Segmented control 🆕

Le composant "Contrôle segmenté" permet à l'utilisateur de choisir un type de
vue parmi plusieurs options d'affichage disponibles, mutuellement exclusives
avec une valeur sélectionnée par défaut.

## Structure

**Le composant "Contrôle segmenté" se compose des éléments suivants :  
**

  * Plusieurs segments, deux au minimum dont un sélectionné par défaut (obligatoire).
  * Un label explicite (obligatoire). 
  * Une icône à gauche du label uniquement (optionnel).
  * Un comportement au survol, au clic, désactivé et focus (obligatoire).
  * Un contour gris et fond transparent sur l’ensemble du conteneur (obligatoire). 
  * Un contour bleu sur le segment sélectionné (obligatoire).  
  

## Variation(s)

  * Le contrôle segmenté existe en tailles SM et MD. Afin de garder une harmonie visuelle en présence d’autres composants (type bouton, champs de saisie, …), il est important de choisir la même hauteur que ces derniers. Par exemple, un bouton SM et contrôle segmenté SM, côte à côte. 
  * En desktop et en mobile, le composant s’affiche horizontalement. Lorsque le contenu des segments est trop long, le composant s’affiche alors verticalement. Il est donc conseillé d’utiliser des labels courts. Par exemple : "Liste", "Carte", etc.
  * Il est possible d’accompagner le contrôle segmenté d’une légende au-dessus ou à côté du composant (optionnel). Un texte de description additionnel peut également accompagner ce texte de légende.   
  

### Taille SM

#### Label seul

Légende

Libellé

Libellé

Libellé

###  Extrait de code

    
    
                          <fieldset class="fr-segmented fr-segmented--sm">
        <legend class="fr-segmented__legend">
            Légende
        </legend>
        <div class="fr-segmented__elements">
            <div class="fr-segmented__element">
                <input value="1" type="radio" id="segmented-2218-1" name="segmented-2218">
                <label class="fr-label" for="segmented-2218-1">
                    Libellé
                </label>
            </div>
            <div class="fr-segmented__element">
                <input value="2" checked type="radio" id="segmented-2218-2" name="segmented-2218">
                <label class="fr-label" for="segmented-2218-2">
                    Libellé
                </label>
            </div>
            <div class="fr-segmented__element">
                <input value="3" type="radio" id="segmented-2218-3" name="segmented-2218">
                <label class="fr-label" for="segmented-2218-3">
                    Libellé
                </label>
            </div>
        </div>
    </fieldset>
                          
                        

#### Avec une icône

Légende

Libellé

Libellé

Libellé

###  Extrait de code

    
    
                          <fieldset class="fr-segmented fr-segmented--sm">
        <legend class="fr-segmented__legend">
            Légende
        </legend>
        <div class="fr-segmented__elements">
            <div class="fr-segmented__element">
                <input value="1" type="radio" id="segmented-2227-1" name="segmented-2227">
                <label class="fr-icon-road-map-line fr-label" for="segmented-2227-1">
                    Libellé
                </label>
            </div>
            <div class="fr-segmented__element">
                <input value="2" checked type="radio" id="segmented-2227-2" name="segmented-2227">
                <label class="fr-icon-road-map-line fr-label" for="segmented-2227-2">
                    Libellé
                </label>
            </div>
            <div class="fr-segmented__element">
                <input value="3" type="radio" id="segmented-2227-3" name="segmented-2227">
                <label class="fr-icon-road-map-line fr-label" for="segmented-2227-3">
                    Libellé
                </label>
            </div>
        </div>
    </fieldset>
                          
                        

### Taille MD

#### Label seul

Légende

Libellé

Libellé

Libellé

###  Extrait de code

    
    
                          <fieldset class="fr-segmented">
        <legend class="fr-segmented__legend">
            Légende
        </legend>
        <div class="fr-segmented__elements">
            <div class="fr-segmented__element">
                <input value="1" type="radio" id="segmented-2215-1" name="segmented-2215">
                <label class="fr-label" for="segmented-2215-1">
                    Libellé
                </label>
            </div>
            <div class="fr-segmented__element">
                <input value="2" checked type="radio" id="segmented-2215-2" name="segmented-2215">
                <label class="fr-label" for="segmented-2215-2">
                    Libellé
                </label>
            </div>
            <div class="fr-segmented__element">
                <input value="3" type="radio" id="segmented-2215-3" name="segmented-2215">
                <label class="fr-label" for="segmented-2215-3">
                    Libellé
                </label>
            </div>
        </div>
    </fieldset>
                          
                        

#### Avec une icône

Légende

Libellé

Libellé

Libellé

###  Extrait de code

    
    
                          <fieldset class="fr-segmented">
        <legend class="fr-segmented__legend">
            Légende
        </legend>
        <div class="fr-segmented__elements">
            <div class="fr-segmented__element">
                <input value="1" type="radio" id="segmented-3227-1" name="segmented-3227">
                <label class="fr-icon-road-map-line fr-label" for="segmented-3227-1">
                    Libellé
                </label>
            </div>
            <div class="fr-segmented__element">
                <input value="2" checked type="radio" id="segmented-3227-2" name="segmented-3227">
                <label class="fr-icon-road-map-line fr-label" for="segmented-3227-2">
                    Libellé
                </label>
            </div>
            <div class="fr-segmented__element">
                <input value="3" type="radio" id="segmented-3227-3" name="segmented-3227">
                <label class="fr-icon-road-map-line fr-label" for="segmented-3227-3">
                    Libellé
                </label>
            </div>
        </div>
    </fieldset>
                          
                        

### Avec légende sur la même ligne

Légende

Libellé

Libellé

Libellé

###  Extrait de code

    
    
                          <fieldset class="fr-segmented">
        <legend class="fr-segmented__legend fr-segmented__legend--inline">
            Légende
        </legend>
        <div class="fr-segmented__elements">
            <div class="fr-segmented__element">
                <input value="1" type="radio" id="segmented-2221-1" name="segmented-2221">
                <label class="fr-label" for="segmented-2221-1">
                    Libellé
                </label>
            </div>
            <div class="fr-segmented__element">
                <input value="2" checked type="radio" id="segmented-2221-2" name="segmented-2221">
                <label class="fr-label" for="segmented-2221-2">
                    Libellé
                </label>
            </div>
            <div class="fr-segmented__element">
                <input value="3" type="radio" id="segmented-2221-3" name="segmented-2221">
                <label class="fr-label" for="segmented-2221-3">
                    Libellé
                </label>
            </div>
        </div>
    </fieldset>
                          
                        

### Sans légende visible

Légende

Libellé

Libellé

Libellé

###  Extrait de code

    
    
                          <fieldset class="fr-segmented fr-segmented--no-legend">
        <legend class="fr-segmented__legend">
            Légende
        </legend>
        <div class="fr-segmented__elements">
            <div class="fr-segmented__element">
                <input value="1" type="radio" id="segmented-2230-1" name="segmented-2230">
                <label class="fr-label" for="segmented-2230-1">
                    Libellé
                </label>
            </div>
            <div class="fr-segmented__element">
                <input value="2" checked type="radio" id="segmented-2230-2" name="segmented-2230">
                <label class="fr-label" for="segmented-2230-2">
                    Libellé
                </label>
            </div>
            <div class="fr-segmented__element">
                <input value="3" type="radio" id="segmented-2230-3" name="segmented-2230">
                <label class="fr-label" for="segmented-2230-3">
                    Libellé
                </label>
            </div>
        </div>
    </fieldset>
                          
                        

## Règles d’utilisation

### Usage

### Attention

Le contrôle segmenté ne doit pas être utilisé en tant que système de filtre,
mais uniquement pour proposer un type d’affichage d’une vue.

  * Cinq segments maximum (déconseillé). 
  * Un seul segment doit être sélectionné. 
  * Il n'est pas autorisé de mélanger des segments avec et sans icône dans le même composant. 
  * L’utilisation avec une icône seule n’est pas autorisée.  
  

### Personnalisation

Aucune personnalisation de ce composant n’est possible.

[Contenu médias - Content](/composants-et-modeles/composants/contenu-medias)

[Curseur - Range](/composants-et-modeles/composants/curseur-range)

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
