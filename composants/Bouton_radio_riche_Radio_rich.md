Fermer

# Bouton radio riche - Radio rich

Les boutons radio riches permettent de sélectionner un choix parmi une liste
d’options illustrées. À la différence du bouton radio simple, l’image permet
d’illustrer et d’accompagner l’utilisateur dans son choix.

## Structure

Un bouton radio riche est composé :

  * D'un [bouton radio](/elements-d-interface/composants/bouton-radio) \- obligatoire
  * D’un label - obligatoire
  * D’un séparateur - obligatoire 
  * D’un pictogramme - obligatoire 
  * D’une description - optionnelle 
  * Un message d’erreur - obligatoire si un changement d'état doit être notifié à l’utilisateur.

La largeur du bouton peut-être définie selon la grille proposée par le Système
de Design de l’État.

## Boutons radio riches sans description

Légende pour l’ensemble des éléments

Libellé bouton radio

Libellé bouton radio

Libellé bouton radio

###  Extrait de code

    
    
                          <fieldset class="fr-fieldset" id="radio-rich" aria-labelledby="radio-rich-legend radio-rich-messages">
        <legend class="fr-fieldset__legend--regular fr-fieldset__legend" id="radio-rich-legend">
            Légende pour l’ensemble des éléments
        </legend>
        <div class="fr-fieldset__element">
            <div class="fr-radio-group fr-radio-rich">
                <input value="1" type="radio" id="radio-rich-1" name="radio-rich">
                <label class="fr-label" for="radio-rich-1">
                    Libellé bouton radio
                </label>
                <div class="fr-radio-rich__pictogram">
                    <svg aria-hidden="true" class="fr-artwork" viewBox="0 0 80 80" width="80px" height="80px">
                        <use class="fr-artwork-decorative" href="../../../dist/artwork/pictograms/buildings/city-hall.svg#artwork-decorative"></use>
                        <use class="fr-artwork-minor" href="../../../dist/artwork/pictograms/buildings/city-hall.svg#artwork-minor"></use>
                        <use class="fr-artwork-major" href="../../../dist/artwork/pictograms/buildings/city-hall.svg#artwork-major"></use>
                    </svg>
                </div>
            </div>
        </div>
        <div class="fr-fieldset__element">
            <div class="fr-radio-group fr-radio-rich">
                <input value="2" checked type="radio" id="radio-rich-2" name="radio-rich">
                <label class="fr-label" for="radio-rich-2">
                    Libellé bouton radio
                </label>
                <div class="fr-radio-rich__pictogram">
                    <svg aria-hidden="true" class="fr-artwork" viewBox="0 0 80 80" width="80px" height="80px">
                        <use class="fr-artwork-decorative" href="../../../dist/artwork/pictograms/buildings/city-hall.svg#artwork-decorative"></use>
                        <use class="fr-artwork-minor" href="../../../dist/artwork/pictograms/buildings/city-hall.svg#artwork-minor"></use>
                        <use class="fr-artwork-major" href="../../../dist/artwork/pictograms/buildings/city-hall.svg#artwork-major"></use>
                    </svg>
                </div>
            </div>
        </div>
        <div class="fr-fieldset__element">
            <div class="fr-radio-group fr-radio-rich">
                <input value="3" type="radio" id="radio-rich-3" name="radio-rich">
                <label class="fr-label" for="radio-rich-3">
                    Libellé bouton radio
                </label>
                <div class="fr-radio-rich__pictogram">
                    <svg aria-hidden="true" class="fr-artwork" viewBox="0 0 80 80" width="80px" height="80px">
                        <use class="fr-artwork-decorative" href="../../../dist/artwork/pictograms/buildings/city-hall.svg#artwork-decorative"></use>
                        <use class="fr-artwork-minor" href="../../../dist/artwork/pictograms/buildings/city-hall.svg#artwork-minor"></use>
                        <use class="fr-artwork-major" href="../../../dist/artwork/pictograms/buildings/city-hall.svg#artwork-major"></use>
                    </svg>
                </div>
            </div>
        </div>
        <div class="fr-messages-group" id="radio-rich-messages" aria-live="polite">
        </div>
    </fieldset>
                          
                        

## Boutons radio riches sans description, en ligne

Légende pour l’ensemble des éléments

Libellé bouton radio

Libellé bouton radio

Libellé bouton radio

###  Extrait de code

    
    
                          <fieldset class="fr-fieldset" id="radio-rich-inline" aria-labelledby="radio-rich-inline-legend radio-rich-inline-messages">
        <legend class="fr-fieldset__legend--regular fr-fieldset__legend" id="radio-rich-inline-legend">
            Légende pour l’ensemble des éléments
        </legend>
        <div class="fr-fieldset__element fr-fieldset__element--inline">
            <div class="fr-radio-group fr-radio-rich">
                <input value="1" type="radio" id="radio-rich-inline-1" name="radio-rich-inline">
                <label class="fr-label" for="radio-rich-inline-1">
                    Libellé bouton radio
                </label>
                <div class="fr-radio-rich__pictogram">
                    <svg aria-hidden="true" class="fr-artwork" viewBox="0 0 80 80" width="80px" height="80px">
                        <use class="fr-artwork-decorative" href="../../../dist/artwork/pictograms/buildings/city-hall.svg#artwork-decorative"></use>
                        <use class="fr-artwork-minor" href="../../../dist/artwork/pictograms/buildings/city-hall.svg#artwork-minor"></use>
                        <use class="fr-artwork-major" href="../../../dist/artwork/pictograms/buildings/city-hall.svg#artwork-major"></use>
                    </svg>
                </div>
            </div>
        </div>
        <div class="fr-fieldset__element fr-fieldset__element--inline">
            <div class="fr-radio-group fr-radio-rich">
                <input value="2" type="radio" id="radio-rich-inline-2" name="radio-rich-inline">
                <label class="fr-label" for="radio-rich-inline-2">
                    Libellé bouton radio
                </label>
                <div class="fr-radio-rich__pictogram">
                    <svg aria-hidden="true" class="fr-artwork" viewBox="0 0 80 80" width="80px" height="80px">
                        <use class="fr-artwork-decorative" href="../../../dist/artwork/pictograms/buildings/city-hall.svg#artwork-decorative"></use>
                        <use class="fr-artwork-minor" href="../../../dist/artwork/pictograms/buildings/city-hall.svg#artwork-minor"></use>
                        <use class="fr-artwork-major" href="../../../dist/artwork/pictograms/buildings/city-hall.svg#artwork-major"></use>
                    </svg>
                </div>
            </div>
        </div>
        <div class="fr-fieldset__element fr-fieldset__element--inline">
            <div class="fr-radio-group fr-radio-rich">
                <input value="3" type="radio" id="radio-rich-inline-3" name="radio-rich-inline">
                <label class="fr-label" for="radio-rich-inline-3">
                    Libellé bouton radio
                </label>
                <div class="fr-radio-rich__pictogram">
                    <svg aria-hidden="true" class="fr-artwork" viewBox="0 0 80 80" width="80px" height="80px">
                        <use class="fr-artwork-decorative" href="../../../dist/artwork/pictograms/buildings/city-hall.svg#artwork-decorative"></use>
                        <use class="fr-artwork-minor" href="../../../dist/artwork/pictograms/buildings/city-hall.svg#artwork-minor"></use>
                        <use class="fr-artwork-major" href="../../../dist/artwork/pictograms/buildings/city-hall.svg#artwork-major"></use>
                    </svg>
                </div>
            </div>
        </div>
        <div class="fr-messages-group" id="radio-rich-inline-messages" aria-live="polite">
        </div>
    </fieldset>
                          
                        

## Boutons radio riches avec description

Les boutons radio riches peuvent également afficher un texte de description en
ajoutant un `<span class="fr-hint-text" id="radio-rich-1-desc-hint">Texte
descriptif</span>` dans la balise </label> comme indiqué ci-dessous.

Légende pour l’ensemble des éléments Texte de description additionnel

Libellé bouton radio Texte de description additionnel

Libellé bouton radio Texte de description additionnel

Libellé bouton radio Texte de description additionnel

###  Extrait de code

    
    
                          <fieldset class="fr-fieldset" id="radio-rich-hint" aria-labelledby="radio-rich-hint-legend radio-rich-hint-messages">
        <legend class="fr-fieldset__legend--regular fr-fieldset__legend" id="radio-rich-hint-legend">
            Légende pour l’ensemble des éléments
            <span class="fr-hint-text">Texte de description additionnel</span>
        </legend>
        <div class="fr-fieldset__element">
            <div class="fr-radio-group fr-radio-rich">
                <input value="1" type="radio" id="radio-rich-hint-1" name="radio-rich-hint">
                <label class="fr-label" for="radio-rich-hint-1">
                    Libellé bouton radio
                    <span class="fr-hint-text">Texte de description additionnel</span>
                </label>
                <div class="fr-radio-rich__pictogram">
                    <svg aria-hidden="true" class="fr-artwork" viewBox="0 0 80 80" width="80px" height="80px">
                        <use class="fr-artwork-decorative" href="../../../dist/artwork/pictograms/buildings/city-hall.svg#artwork-decorative"></use>
                        <use class="fr-artwork-minor" href="../../../dist/artwork/pictograms/buildings/city-hall.svg#artwork-minor"></use>
                        <use class="fr-artwork-major" href="../../../dist/artwork/pictograms/buildings/city-hall.svg#artwork-major"></use>
                    </svg>
                </div>
            </div>
        </div>
        <div class="fr-fieldset__element">
            <div class="fr-radio-group fr-radio-rich">
                <input value="2" type="radio" id="radio-rich-hint-2" name="radio-rich-hint">
                <label class="fr-label" for="radio-rich-hint-2">
                    Libellé bouton radio
                    <span class="fr-hint-text">Texte de description additionnel</span>
                </label>
                <div class="fr-radio-rich__pictogram">
                    <svg aria-hidden="true" class="fr-artwork" viewBox="0 0 80 80" width="80px" height="80px">
                        <use class="fr-artwork-decorative" href="../../../dist/artwork/pictograms/buildings/city-hall.svg#artwork-decorative"></use>
                        <use class="fr-artwork-minor" href="../../../dist/artwork/pictograms/buildings/city-hall.svg#artwork-minor"></use>
                        <use class="fr-artwork-major" href="../../../dist/artwork/pictograms/buildings/city-hall.svg#artwork-major"></use>
                    </svg>
                </div>
            </div>
        </div>
        <div class="fr-fieldset__element">
            <div class="fr-radio-group fr-radio-rich">
                <input value="3" type="radio" id="radio-rich-hint-3" name="radio-rich-hint">
                <label class="fr-label" for="radio-rich-hint-3">
                    Libellé bouton radio
                    <span class="fr-hint-text">Texte de description additionnel</span>
                </label>
                <div class="fr-radio-rich__pictogram">
                    <svg aria-hidden="true" class="fr-artwork" viewBox="0 0 80 80" width="80px" height="80px">
                        <use class="fr-artwork-decorative" href="../../../dist/artwork/pictograms/buildings/city-hall.svg#artwork-decorative"></use>
                        <use class="fr-artwork-minor" href="../../../dist/artwork/pictograms/buildings/city-hall.svg#artwork-minor"></use>
                        <use class="fr-artwork-major" href="../../../dist/artwork/pictograms/buildings/city-hall.svg#artwork-major"></use>
                    </svg>
                </div>
            </div>
        </div>
        <div class="fr-messages-group" id="radio-rich-hint-messages" aria-live="polite">
        </div>
    </fieldset>
                          
                        

## Boutons radio riches avec description, en ligne

Légende pour l’ensemble des éléments Texte de description additionnel

Libellé bouton radio Texte de description additionnel

Libellé bouton radio Texte de description additionnel

Libellé bouton radio Texte de description additionnel

###  Extrait de code

    
    
                          <fieldset class="fr-fieldset" id="radio-rich-hint-inline" aria-labelledby="radio-rich-hint-inline-legend radio-rich-hint-inline-messages">
        <legend class="fr-fieldset__legend--regular fr-fieldset__legend" id="radio-rich-hint-inline-legend">
            Légende pour l’ensemble des éléments
            <span class="fr-hint-text">Texte de description additionnel</span>
        </legend>
        <div class="fr-fieldset__element fr-fieldset__element--inline">
            <div class="fr-radio-group fr-radio-rich">
                <input value="1" type="radio" id="radio-rich-hint-inline-1" name="radio-rich-hint-inline">
                <label class="fr-label" for="radio-rich-hint-inline-1">
                    Libellé bouton radio
                    <span class="fr-hint-text">Texte de description additionnel</span>
                </label>
                <div class="fr-radio-rich__pictogram">
                    <svg aria-hidden="true" class="fr-artwork" viewBox="0 0 80 80" width="80px" height="80px">
                        <use class="fr-artwork-decorative" href="../../../dist/artwork/pictograms/buildings/city-hall.svg#artwork-decorative"></use>
                        <use class="fr-artwork-minor" href="../../../dist/artwork/pictograms/buildings/city-hall.svg#artwork-minor"></use>
                        <use class="fr-artwork-major" href="../../../dist/artwork/pictograms/buildings/city-hall.svg#artwork-major"></use>
                    </svg>
                </div>
            </div>
        </div>
        <div class="fr-fieldset__element fr-fieldset__element--inline">
            <div class="fr-radio-group fr-radio-rich">
                <input value="2" type="radio" id="radio-rich-hint-inline-2" name="radio-rich-hint-inline">
                <label class="fr-label" for="radio-rich-hint-inline-2">
                    Libellé bouton radio
                    <span class="fr-hint-text">Texte de description additionnel</span>
                </label>
                <div class="fr-radio-rich__pictogram">
                    <svg aria-hidden="true" class="fr-artwork" viewBox="0 0 80 80" width="80px" height="80px">
                        <use class="fr-artwork-decorative" href="../../../dist/artwork/pictograms/buildings/city-hall.svg#artwork-decorative"></use>
                        <use class="fr-artwork-minor" href="../../../dist/artwork/pictograms/buildings/city-hall.svg#artwork-minor"></use>
                        <use class="fr-artwork-major" href="../../../dist/artwork/pictograms/buildings/city-hall.svg#artwork-major"></use>
                    </svg>
                </div>
            </div>
        </div>
        <div class="fr-fieldset__element fr-fieldset__element--inline">
            <div class="fr-radio-group fr-radio-rich">
                <input value="3" type="radio" id="radio-rich-hint-inline-3" name="radio-rich-hint-inline">
                <label class="fr-label" for="radio-rich-hint-inline-3">
                    Libellé bouton radio
                    <span class="fr-hint-text">Texte de description additionnel</span>
                </label>
                <div class="fr-radio-rich__pictogram">
                    <svg aria-hidden="true" class="fr-artwork" viewBox="0 0 80 80" width="80px" height="80px">
                        <use class="fr-artwork-decorative" href="../../../dist/artwork/pictograms/buildings/city-hall.svg#artwork-decorative"></use>
                        <use class="fr-artwork-minor" href="../../../dist/artwork/pictograms/buildings/city-hall.svg#artwork-minor"></use>
                        <use class="fr-artwork-major" href="../../../dist/artwork/pictograms/buildings/city-hall.svg#artwork-major"></use>
                    </svg>
                </div>
            </div>
        </div>
        <div class="fr-messages-group" id="radio-rich-hint-inline-messages" aria-live="polite">
        </div>
    </fieldset>
                          
                        

## État d'erreur

L'état d’erreur est signalé par l’affichage d’une ligne rouge et d'un message
d’erreur en-dessous du composant (cf. couleurs fonctionnelles :link: : le
rouge est la couleur de l’état erreur).

### Pour les développeurs

Pour l'état d’erreur, il est nécessaire d’ajouter un `role=”group”` à la
balise fieldset. De plus, le message d’erreur et la balise legend sont liés au
fieldset via l’attribut `aria-labelledby`.

Légende pour l’ensemble des éléments Texte de description additionnel

Libellé bouton radio Texte de description additionnel

Libellé bouton radio Texte de description additionnel

Libellé bouton radio Texte de description additionnel

Texte d’erreur obligatoire

###  Extrait de code

    
    
                          <fieldset class="fr-fieldset fr-fieldset--error" id="radio-rich-error" role="group" aria-labelledby="radio-rich-error-legend radio-rich-error-messages">
        <legend class="fr-fieldset__legend--regular fr-fieldset__legend" id="radio-rich-error-legend">
            Légende pour l’ensemble des éléments
            <span class="fr-hint-text">Texte de description additionnel</span>
        </legend>
        <div class="fr-fieldset__element">
            <div class="fr-radio-group fr-radio-rich">
                <input value="1" type="radio" id="radio-rich-error-1" name="radio-rich-error">
                <label class="fr-label" for="radio-rich-error-1">
                    Libellé bouton radio
                    <span class="fr-hint-text">Texte de description additionnel</span>
                </label>
                <div class="fr-radio-rich__pictogram">
                    <svg aria-hidden="true" class="fr-artwork" viewBox="0 0 80 80" width="80px" height="80px">
                        <use class="fr-artwork-decorative" href="../../../dist/artwork/pictograms/buildings/city-hall.svg#artwork-decorative"></use>
                        <use class="fr-artwork-minor" href="../../../dist/artwork/pictograms/buildings/city-hall.svg#artwork-minor"></use>
                        <use class="fr-artwork-major" href="../../../dist/artwork/pictograms/buildings/city-hall.svg#artwork-major"></use>
                    </svg>
                </div>
            </div>
        </div>
        <div class="fr-fieldset__element">
            <div class="fr-radio-group fr-radio-rich">
                <input value="2" type="radio" id="radio-rich-error-2" name="radio-rich-error">
                <label class="fr-label" for="radio-rich-error-2">
                    Libellé bouton radio
                    <span class="fr-hint-text">Texte de description additionnel</span>
                </label>
                <div class="fr-radio-rich__pictogram">
                    <svg aria-hidden="true" class="fr-artwork" viewBox="0 0 80 80" width="80px" height="80px">
                        <use class="fr-artwork-decorative" href="../../../dist/artwork/pictograms/buildings/city-hall.svg#artwork-decorative"></use>
                        <use class="fr-artwork-minor" href="../../../dist/artwork/pictograms/buildings/city-hall.svg#artwork-minor"></use>
                        <use class="fr-artwork-major" href="../../../dist/artwork/pictograms/buildings/city-hall.svg#artwork-major"></use>
                    </svg>
                </div>
            </div>
        </div>
        <div class="fr-fieldset__element">
            <div class="fr-radio-group fr-radio-rich">
                <input value="3" type="radio" id="radio-rich-error-3" name="radio-rich-error">
                <label class="fr-label" for="radio-rich-error-3">
                    Libellé bouton radio
                    <span class="fr-hint-text">Texte de description additionnel</span>
                </label>
                <div class="fr-radio-rich__pictogram">
                    <svg aria-hidden="true" class="fr-artwork" viewBox="0 0 80 80" width="80px" height="80px">
                        <use class="fr-artwork-decorative" href="../../../dist/artwork/pictograms/buildings/city-hall.svg#artwork-decorative"></use>
                        <use class="fr-artwork-minor" href="../../../dist/artwork/pictograms/buildings/city-hall.svg#artwork-minor"></use>
                        <use class="fr-artwork-major" href="../../../dist/artwork/pictograms/buildings/city-hall.svg#artwork-major"></use>
                    </svg>
                </div>
            </div>
        </div>
        <div class="fr-messages-group" id="radio-rich-error-messages" aria-live="polite">
            <p class="fr-message fr-message--error" id="radio-rich-error-message-error">Texte d’erreur obligatoire</p>
        </div>
    </fieldset>
                          
                        

Légende pour l’ensemble des éléments Texte de description additionnel

Libellé bouton radio Texte de description additionnel

Libellé bouton radio Texte de description additionnel

Libellé bouton radio Texte de description additionnel

Texte d’erreur obligatoire

###  Extrait de code

    
    
                          <fieldset class="fr-fieldset fr-fieldset--error" id="radio-rich-error-inline" role="group" aria-labelledby="radio-rich-error-inline-legend radio-rich-error-inline-messages">
        <legend class="fr-fieldset__legend--regular fr-fieldset__legend" id="radio-rich-error-inline-legend">
            Légende pour l’ensemble des éléments
            <span class="fr-hint-text">Texte de description additionnel</span>
        </legend>
        <div class="fr-fieldset__element fr-fieldset__element--inline">
            <div class="fr-radio-group fr-radio-rich">
                <input value="1" type="radio" id="radio-rich-error-inline-1" name="radio-rich-error-inline">
                <label class="fr-label" for="radio-rich-error-inline-1">
                    Libellé bouton radio
                    <span class="fr-hint-text">Texte de description additionnel</span>
                </label>
                <div class="fr-radio-rich__pictogram">
                    <svg aria-hidden="true" class="fr-artwork" viewBox="0 0 80 80" width="80px" height="80px">
                        <use class="fr-artwork-decorative" href="../../../dist/artwork/pictograms/buildings/city-hall.svg#artwork-decorative"></use>
                        <use class="fr-artwork-minor" href="../../../dist/artwork/pictograms/buildings/city-hall.svg#artwork-minor"></use>
                        <use class="fr-artwork-major" href="../../../dist/artwork/pictograms/buildings/city-hall.svg#artwork-major"></use>
                    </svg>
                </div>
            </div>
        </div>
        <div class="fr-fieldset__element fr-fieldset__element--inline">
            <div class="fr-radio-group fr-radio-rich">
                <input value="2" type="radio" id="radio-rich-error-inline-2" name="radio-rich-error-inline">
                <label class="fr-label" for="radio-rich-error-inline-2">
                    Libellé bouton radio
                    <span class="fr-hint-text">Texte de description additionnel</span>
                </label>
                <div class="fr-radio-rich__pictogram">
                    <svg aria-hidden="true" class="fr-artwork" viewBox="0 0 80 80" width="80px" height="80px">
                        <use class="fr-artwork-decorative" href="../../../dist/artwork/pictograms/buildings/city-hall.svg#artwork-decorative"></use>
                        <use class="fr-artwork-minor" href="../../../dist/artwork/pictograms/buildings/city-hall.svg#artwork-minor"></use>
                        <use class="fr-artwork-major" href="../../../dist/artwork/pictograms/buildings/city-hall.svg#artwork-major"></use>
                    </svg>
                </div>
            </div>
        </div>
        <div class="fr-fieldset__element fr-fieldset__element--inline">
            <div class="fr-radio-group fr-radio-rich">
                <input value="3" type="radio" id="radio-rich-error-inline-3" name="radio-rich-error-inline">
                <label class="fr-label" for="radio-rich-error-inline-3">
                    Libellé bouton radio
                    <span class="fr-hint-text">Texte de description additionnel</span>
                </label>
                <div class="fr-radio-rich__pictogram">
                    <svg aria-hidden="true" class="fr-artwork" viewBox="0 0 80 80" width="80px" height="80px">
                        <use class="fr-artwork-decorative" href="../../../dist/artwork/pictograms/buildings/city-hall.svg#artwork-decorative"></use>
                        <use class="fr-artwork-minor" href="../../../dist/artwork/pictograms/buildings/city-hall.svg#artwork-minor"></use>
                        <use class="fr-artwork-major" href="../../../dist/artwork/pictograms/buildings/city-hall.svg#artwork-major"></use>
                    </svg>
                </div>
            </div>
        </div>
        <div class="fr-messages-group" id="radio-rich-error-inline-messages" aria-live="polite">
            <p class="fr-message fr-message--error" id="radio-rich-error-inline-message-error">Texte d’erreur obligatoire</p>
        </div>
    </fieldset>
                          
                        

## État désactivé

Légende pour l’ensemble des éléments

Libellé bouton radio Texte de description additionnel

Libellé bouton radio Texte de description additionnel

Libellé bouton radio Texte de description additionnel

###  Extrait de code

    
    
                          <fieldset class="fr-fieldset" id="radio-rich-disabled" aria-labelledby="radio-rich-disabled-legend radio-rich-disabled-messages">
        <legend class="fr-fieldset__legend--regular fr-fieldset__legend" id="radio-rich-disabled-legend">
            Légende pour l’ensemble des éléments
        </legend>
        <div class="fr-fieldset__element">
            <div class="fr-radio-group fr-radio-rich">
                <input value="1" disabled type="radio" id="radio-rich-disabled-1" name="radio-rich-disabled">
                <label class="fr-label" for="radio-rich-disabled-1">
                    Libellé bouton radio
                    <span class="fr-hint-text">Texte de description additionnel</span>
                </label>
                <div class="fr-radio-rich__pictogram">
                    <svg aria-hidden="true" class="fr-artwork" viewBox="0 0 80 80" width="80px" height="80px">
                        <use class="fr-artwork-decorative" href="../../../dist/artwork/pictograms/buildings/city-hall.svg#artwork-decorative"></use>
                        <use class="fr-artwork-minor" href="../../../dist/artwork/pictograms/buildings/city-hall.svg#artwork-minor"></use>
                        <use class="fr-artwork-major" href="../../../dist/artwork/pictograms/buildings/city-hall.svg#artwork-major"></use>
                    </svg>
                </div>
            </div>
        </div>
        <div class="fr-fieldset__element">
            <div class="fr-radio-group fr-radio-rich">
                <input value="2" disabled checked type="radio" id="radio-rich-disabled-2" name="radio-rich-disabled">
                <label class="fr-label" for="radio-rich-disabled-2">
                    Libellé bouton radio
                    <span class="fr-hint-text">Texte de description additionnel</span>
                </label>
                <div class="fr-radio-rich__pictogram">
                    <svg aria-hidden="true" class="fr-artwork" viewBox="0 0 80 80" width="80px" height="80px">
                        <use class="fr-artwork-decorative" href="../../../dist/artwork/pictograms/buildings/city-hall.svg#artwork-decorative"></use>
                        <use class="fr-artwork-minor" href="../../../dist/artwork/pictograms/buildings/city-hall.svg#artwork-minor"></use>
                        <use class="fr-artwork-major" href="../../../dist/artwork/pictograms/buildings/city-hall.svg#artwork-major"></use>
                    </svg>
                </div>
            </div>
        </div>
        <div class="fr-fieldset__element">
            <div class="fr-radio-group fr-radio-rich">
                <input value="3" disabled type="radio" id="radio-rich-disabled-3" name="radio-rich-disabled">
                <label class="fr-label" for="radio-rich-disabled-3">
                    Libellé bouton radio
                    <span class="fr-hint-text">Texte de description additionnel</span>
                </label>
                <div class="fr-radio-rich__pictogram">
                    <svg aria-hidden="true" class="fr-artwork" viewBox="0 0 80 80" width="80px" height="80px">
                        <use class="fr-artwork-decorative" href="../../../dist/artwork/pictograms/buildings/city-hall.svg#artwork-decorative"></use>
                        <use class="fr-artwork-minor" href="../../../dist/artwork/pictograms/buildings/city-hall.svg#artwork-minor"></use>
                        <use class="fr-artwork-major" href="../../../dist/artwork/pictograms/buildings/city-hall.svg#artwork-major"></use>
                    </svg>
                </div>
            </div>
        </div>
        <div class="fr-messages-group" id="radio-rich-disabled-messages" aria-live="polite">
        </div>
    </fieldset>
                          
                        

## Responsive

Comme les boutons radio, les boutons radios riche sont à utiliser en groupe en
respectant les espacements définis ci-dessous.

![Indication sur l'espacement à respecter entre des boutons radio riches en
desktop<br>](/uploads/Capture_d_ecran_2020_12_16_a_15_33_21_e718f18916.png)

En mobile, les composants bouton radio riche s’affichent automatiquement les
uns en dessus des autres. L’espacement à respecter entre chaque boutons est de
2W (voir la documentation [Espacement](https://www.systeme-de-
design.gouv.fr/fondamentaux/espacement/)).

![

Indication sur l'espacement à respecter entre des boutons radio riches en
mobile](/uploads/Capture_d_ecran_2020_12_16_a_15_56_35_09ff1c88e4.png)

## Règles d’utilisation

Les règles d’utilisation du bouton radio riches sont identiques à celles déjà
explicité sur [les boutons radio](https://www.systeme-de-
design.gouv.fr/composants-et-modeles/composants/bouton-radio).

### Personnalisation

Le style de ce composant n’est pas personnalisable. Toutefois, certains
éléments sont optionnels - voir la structure du composant.

### Besoin d'aide ?

L'équipe du DSFR est là pour vous aider.

Retrouvez-la sur :

  * [la communauté slack](https://gouvfr.slack.com/ "la communauté slack - nouvelle fenêtre") pour poser vos questions, et échanger avec d’autres utilisateurs.   
Vous êtes **agent de l’État** et souhaitez accéder au slack ? [Rejoignez la
communauté](https://gouvfr.atlassian.net/servicedesk/customer/portal/1/group/1/create/9
"Rejoignez la communauté - nouvelle fenêtre") dès maintenant !

  * [ le centre de support](https://gouvfr.atlassian.net/servicedesk/customer/portals "le centre de support - nouvelle fenêtre") pour envoyer vos demandes de correctifs et d'évolution.

[Bouton radio - Radio](/composants-et-modeles/composants/bouton-radio)

[Case à cocher - Checkbox](/composants-et-modeles/composants/case-a-cocher)

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
