Fermer

# Case à cocher - Checkbox

Les cases à cocher permettent à l’utilisateur de sélectionner une ou plusieurs
options dans une liste. Elles sont utilisées pour effectuer des sélections
multiples (de 0 à N éléments) ou bien pour permettre un choix binaire, lorsque
l’utilisateur peut sélectionner ou désélectionner une seule option.

La case à cocher peut être utilisée seule ou en liste. Évitez les listes de
plus de 5 items et lorsque vous souhaitez contraindre le choix à un seul
élément - utiliser [les boutons radios. ](/elements-d-
interface/composants/bouton-radio)

## Structure

Les cases à cocher sont composés des éléments suivants :

  * un bouton - obligatoire.
  * un label, associé au bouton - obligatoire.
  * un texte additionnel pour le boutons / labels - optionnel.
  * une légende, décrivant le contexte du groupe de bouton - obligatoire pour les groupes de cases.
  * une description additionnelle pour la légende - optionnelle.
  * un message d’erreur ou de succès - obligatoire si un changement d'état doit être notifié à l’utilisateur.

## Liste verticale

Cette organisation verticale d’une liste de cases à cocher est les plus
courante et la plus facile à lire pour l’utilisateur.

Légende pour l’ensemble des éléments

Libellé case à cocher

Libellé case à cocher

Libellé case à cocher

###  Extrait de code

    
    
                          <fieldset class="fr-fieldset" id="checkboxes" aria-labelledby="checkboxes-legend checkboxes-messages">
        <legend class="fr-fieldset__legend--regular fr-fieldset__legend" id="checkboxes-legend">
            Légende pour l’ensemble des éléments
        </legend>
        <div class="fr-fieldset__element">
            <div class="fr-checkbox-group">
                <input name="checkboxes-1" id="checkboxes-1" type="checkbox" aria-describedby="checkboxes-1-messages">
                <label class="fr-label" for="checkboxes-1">
                    Libellé case à cocher
                </label>
                <div class="fr-messages-group" id="checkboxes-1-messages" aria-live="assertive">
                </div>
            </div>
        </div>
        <div class="fr-fieldset__element">
            <div class="fr-checkbox-group">
                <input checked name="checkboxes-2" id="checkboxes-2" type="checkbox" aria-describedby="checkboxes-2-messages">
                <label class="fr-label" for="checkboxes-2">
                    Libellé case à cocher
                </label>
                <div class="fr-messages-group" id="checkboxes-2-messages" aria-live="assertive">
                </div>
            </div>
        </div>
        <div class="fr-fieldset__element">
            <div class="fr-checkbox-group">
                <input name="checkboxes-3" id="checkboxes-3" type="checkbox" aria-describedby="checkboxes-3-messages">
                <label class="fr-label" for="checkboxes-3">
                    Libellé case à cocher
                </label>
                <div class="fr-messages-group" id="checkboxes-3-messages" aria-live="assertive">
                </div>
            </div>
        </div>
        <div class="fr-messages-group" id="checkboxes-messages" aria-live="assertive">
        </div>
    </fieldset>
                          
                        

## Liste horizontale - Inline checkbox

Cette organisation doit être uniquement utilisée lorsque il y a 2 options ou
que les libellés des entrées sont très courtes. Pour les autres cas, il faut
privilégier les listes verticales, plus faciles à lire pour l’utilisateur.

Légende pour l’ensemble des éléments

Libellé case à cocher

Libellé case à cocher

Libellé case à cocher

###  Extrait de code

    
    
                          <fieldset class="fr-fieldset" id="checkboxes-inline" aria-labelledby="checkboxes-inline-legend checkboxes-inline-messages">
        <legend class="fr-fieldset__legend--regular fr-fieldset__legend" id="checkboxes-inline-legend">
            Légende pour l’ensemble des éléments
        </legend>
        <div class="fr-fieldset__element fr-fieldset__element--inline">
            <div class="fr-checkbox-group">
                <input name="checkboxes-inline-1" id="checkboxes-inline-1" type="checkbox" aria-describedby="checkboxes-inline-1-messages">
                <label class="fr-label" for="checkboxes-inline-1">
                    Libellé case à cocher
                </label>
                <div class="fr-messages-group" id="checkboxes-inline-1-messages" aria-live="assertive">
                </div>
            </div>
        </div>
        <div class="fr-fieldset__element fr-fieldset__element--inline">
            <div class="fr-checkbox-group">
                <input name="checkboxes-inline-2" id="checkboxes-inline-2" type="checkbox" aria-describedby="checkboxes-inline-2-messages">
                <label class="fr-label" for="checkboxes-inline-2">
                    Libellé case à cocher
                </label>
                <div class="fr-messages-group" id="checkboxes-inline-2-messages" aria-live="assertive">
                </div>
            </div>
        </div>
        <div class="fr-fieldset__element fr-fieldset__element--inline">
            <div class="fr-checkbox-group">
                <input name="checkboxes-inline-3" id="checkboxes-inline-3" type="checkbox" aria-describedby="checkboxes-inline-3-messages">
                <label class="fr-label" for="checkboxes-inline-3">
                    Libellé case à cocher
                </label>
                <div class="fr-messages-group" id="checkboxes-inline-3-messages" aria-live="assertive">
                </div>
            </div>
        </div>
        <div class="fr-messages-group" id="checkboxes-inline-messages" aria-live="assertive">
        </div>
    </fieldset>
                          
                        

## Liste avec texte d’aide

Il est recommandé d’ajouter un texte d’aide afin de faciliter le choix de
l’utilisateur. Ces précisions peuvent être apportés de 2 façons :

  * via un texte sous le titre du groupe des cases à cocher, afin d’apporter une précision à l’intitulé du groupe.

  * via un texte sous le libellé de chaque case à cocher, afin d’apporter une précision à chaque élément.

Légende pour l’ensemble des éléments

Libellé case à cocher Texte de description additionnel

Libellé case à cocher Texte de description additionnel

Libellé case à cocher Texte de description additionnel

###  Extrait de code

    
    
                          <fieldset class="fr-fieldset" id="checkboxes-hint-el-sm" aria-labelledby="checkboxes-hint-el-sm-legend checkboxes-hint-el-sm-messages">
        <legend class="fr-fieldset__legend--regular fr-fieldset__legend" id="checkboxes-hint-el-sm-legend">
            Légende pour l’ensemble des éléments
        </legend>
        <div class="fr-fieldset__element">
            <div class="fr-checkbox-group fr-checkbox-group--sm">
                <input name="checkboxes-hint-el-sm-1" id="checkboxes-hint-el-sm-1" type="checkbox" aria-describedby="checkboxes-hint-el-sm-1-messages">
                <label class="fr-label" for="checkboxes-hint-el-sm-1">
                    Libellé case à cocher
                    <span class="fr-hint-text">Texte de description additionnel</span>
                </label>
                <div class="fr-messages-group" id="checkboxes-hint-el-sm-1-messages" aria-live="assertive">
                </div>
            </div>
        </div>
        <div class="fr-fieldset__element">
            <div class="fr-checkbox-group fr-checkbox-group--sm">
                <input name="checkboxes-hint-el-sm-2" id="checkboxes-hint-el-sm-2" type="checkbox" aria-describedby="checkboxes-hint-el-sm-2-messages">
                <label class="fr-label" for="checkboxes-hint-el-sm-2">
                    Libellé case à cocher
                    <span class="fr-hint-text">Texte de description additionnel</span>
                </label>
                <div class="fr-messages-group" id="checkboxes-hint-el-sm-2-messages" aria-live="assertive">
                </div>
            </div>
        </div>
        <div class="fr-fieldset__element">
            <div class="fr-checkbox-group fr-checkbox-group--sm">
                <input name="checkboxes-hint-el-sm-3" id="checkboxes-hint-el-sm-3" type="checkbox" aria-describedby="checkboxes-hint-el-sm-3-messages">
                <label class="fr-label" for="checkboxes-hint-el-sm-3">
                    Libellé case à cocher
                    <span class="fr-hint-text">Texte de description additionnel</span>
                </label>
                <div class="fr-messages-group" id="checkboxes-hint-el-sm-3-messages" aria-live="assertive">
                </div>
            </div>
        </div>
        <div class="fr-messages-group" id="checkboxes-hint-el-sm-messages" aria-live="assertive">
        </div>
    </fieldset>
                          
                        

À noter l'état “Indeterminate” n’est pas géré actuellement par le Système de
Design de l'Etat.

## État d’erreur

L'état d’erreur est signalé par un changement de couleur ou l’affichage d’une
ligne (cf. couleurs fonctionnelles : le rouge est la couleur de l’état erreur)
et par l’affichage un message d’erreur apparait en-dessous du composant.

### Pour les développeurs

Pour l'état d’erreur des groupes de cases à cocher, il est nécessaire
d’ajouter un `role="group"` à la balise fieldset. De plus, le message d’erreur
et la balise legend sont liés au fieldset via l’attribut `aria-labelledby`.

Légende pour l’ensemble des éléments

Libellé case à cocher

Libellé case à cocher

Libellé case à cocher

Texte d’erreur obligatoire

###  Extrait de code

    
    
                          <fieldset class="fr-fieldset fr-fieldset--error" id="checkboxes-error" role="group" aria-labelledby="checkboxes-error-legend checkboxes-error-messages">
        <legend class="fr-fieldset__legend--regular fr-fieldset__legend" id="checkboxes-error-legend">
            Légende pour l’ensemble des éléments
        </legend>
        <div class="fr-fieldset__element">
            <div class="fr-checkbox-group">
                <input name="checkboxes-error-1" id="checkboxes-error-1" type="checkbox" aria-describedby="checkboxes-error-1-messages">
                <label class="fr-label" for="checkboxes-error-1">
                    Libellé case à cocher
                </label>
                <div class="fr-messages-group" id="checkboxes-error-1-messages" aria-live="assertive">
                </div>
            </div>
        </div>
        <div class="fr-fieldset__element">
            <div class="fr-checkbox-group">
                <input name="checkboxes-error-2" id="checkboxes-error-2" type="checkbox" aria-describedby="checkboxes-error-2-messages">
                <label class="fr-label" for="checkboxes-error-2">
                    Libellé case à cocher
                </label>
                <div class="fr-messages-group" id="checkboxes-error-2-messages" aria-live="assertive">
                </div>
            </div>
        </div>
        <div class="fr-fieldset__element">
            <div class="fr-checkbox-group">
                <input name="checkboxes-error-3" id="checkboxes-error-3" type="checkbox" aria-describedby="checkboxes-error-3-messages">
                <label class="fr-label" for="checkboxes-error-3">
                    Libellé case à cocher
                </label>
                <div class="fr-messages-group" id="checkboxes-error-3-messages" aria-live="assertive">
                </div>
            </div>
        </div>
        <div class="fr-messages-group" id="checkboxes-error-messages" aria-live="assertive">
            <p class="fr-message fr-message--error" id="checkboxes-error-message-error">Texte d’erreur obligatoire</p>
        </div>
    </fieldset>
                          
                        

Légende pour l’ensemble des éléments

Libellé case à cocher

Libellé case à cocher

Libellé case à cocher

Texte d’erreur obligatoire

###  Extrait de code

    
    
                          <fieldset class="fr-fieldset fr-fieldset--error" id="checkboxes-error-inline" role="group" aria-labelledby="checkboxes-error-inline-legend checkboxes-error-inline-messages">
        <legend class="fr-fieldset__legend--regular fr-fieldset__legend" id="checkboxes-error-inline-legend">
            Légende pour l’ensemble des éléments
        </legend>
        <div class="fr-fieldset__element fr-fieldset__element--inline">
            <div class="fr-checkbox-group">
                <input name="checkboxes-error-inline-1" id="checkboxes-error-inline-1" type="checkbox" aria-describedby="checkboxes-error-inline-1-messages">
                <label class="fr-label" for="checkboxes-error-inline-1">
                    Libellé case à cocher
                </label>
                <div class="fr-messages-group" id="checkboxes-error-inline-1-messages" aria-live="assertive">
                </div>
            </div>
        </div>
        <div class="fr-fieldset__element fr-fieldset__element--inline">
            <div class="fr-checkbox-group">
                <input name="checkboxes-error-inline-2" id="checkboxes-error-inline-2" type="checkbox" aria-describedby="checkboxes-error-inline-2-messages">
                <label class="fr-label" for="checkboxes-error-inline-2">
                    Libellé case à cocher
                </label>
                <div class="fr-messages-group" id="checkboxes-error-inline-2-messages" aria-live="assertive">
                </div>
            </div>
        </div>
        <div class="fr-fieldset__element fr-fieldset__element--inline">
            <div class="fr-checkbox-group">
                <input name="checkboxes-error-inline-3" id="checkboxes-error-inline-3" type="checkbox" aria-describedby="checkboxes-error-inline-3-messages">
                <label class="fr-label" for="checkboxes-error-inline-3">
                    Libellé case à cocher
                </label>
                <div class="fr-messages-group" id="checkboxes-error-inline-3-messages" aria-live="assertive">
                </div>
            </div>
        </div>
        <div class="fr-messages-group" id="checkboxes-error-inline-messages" aria-live="assertive">
            <p class="fr-message fr-message--error" id="checkboxes-error-inline-message-error">Texte d’erreur obligatoire</p>
        </div>
    </fieldset>
                          
                        

## État de succès

L'état de succès est signalé par l’affichage d’une ligne verte et d'un message
de succès en-dessous du composant (cf. couleurs fonctionnelles : le vert est
la couleur de l’état succès).

### Pour les développeurs

Pour l'état de succès des groupes de cases à cocher, il est nécessaire
d’ajouter un `role=”group”` à la balise fieldset. De plus, le message de
validation et la balise legend sont liés au fieldset via l’attribut `aria-
labelledby`. Pour la case à cocher seule, voir le snippet plus bas.

Légende pour l’ensemble des éléments

Libellé case à cocher

Libellé case à cocher

Libellé case à cocher

Texte de validation

###  Extrait de code

    
    
                          <fieldset class="fr-fieldset fr-fieldset--valid" id="checkboxes-valid" role="group" aria-labelledby="checkboxes-valid-legend checkboxes-valid-messages">
        <legend class="fr-fieldset__legend--regular fr-fieldset__legend" id="checkboxes-valid-legend">
            Légende pour l’ensemble des éléments
        </legend>
        <div class="fr-fieldset__element">
            <div class="fr-checkbox-group">
                <input name="checkboxes-valid-1" id="checkboxes-valid-1" type="checkbox" aria-describedby="checkboxes-valid-1-messages">
                <label class="fr-label" for="checkboxes-valid-1">
                    Libellé case à cocher
                </label>
                <div class="fr-messages-group" id="checkboxes-valid-1-messages" aria-live="assertive">
                </div>
            </div>
        </div>
        <div class="fr-fieldset__element">
            <div class="fr-checkbox-group">
                <input name="checkboxes-valid-2" id="checkboxes-valid-2" type="checkbox" aria-describedby="checkboxes-valid-2-messages">
                <label class="fr-label" for="checkboxes-valid-2">
                    Libellé case à cocher
                </label>
                <div class="fr-messages-group" id="checkboxes-valid-2-messages" aria-live="assertive">
                </div>
            </div>
        </div>
        <div class="fr-fieldset__element">
            <div class="fr-checkbox-group">
                <input name="checkboxes-valid-3" id="checkboxes-valid-3" type="checkbox" aria-describedby="checkboxes-valid-3-messages">
                <label class="fr-label" for="checkboxes-valid-3">
                    Libellé case à cocher
                </label>
                <div class="fr-messages-group" id="checkboxes-valid-3-messages" aria-live="assertive">
                </div>
            </div>
        </div>
        <div class="fr-messages-group" id="checkboxes-valid-messages" aria-live="assertive">
            <p class="fr-message fr-message--valid" id="checkboxes-valid-message-valid">Texte de validation</p>
        </div>
    </fieldset>
                          
                        

Légende pour l’ensemble des éléments

Libellé case à cocher

Libellé case à cocher

Libellé case à cocher

Texte de validation

###  Extrait de code

    
    
                          <fieldset class="fr-fieldset fr-fieldset--valid" id="checkboxes-valid-inline" role="group" aria-labelledby="checkboxes-valid-inline-legend checkboxes-valid-inline-messages">
        <legend class="fr-fieldset__legend--regular fr-fieldset__legend" id="checkboxes-valid-inline-legend">
            Légende pour l’ensemble des éléments
        </legend>
        <div class="fr-fieldset__element fr-fieldset__element--inline">
            <div class="fr-checkbox-group">
                <input name="checkboxes-valid-inline-1" id="checkboxes-valid-inline-1" type="checkbox" aria-describedby="checkboxes-valid-inline-1-messages">
                <label class="fr-label" for="checkboxes-valid-inline-1">
                    Libellé case à cocher
                </label>
                <div class="fr-messages-group" id="checkboxes-valid-inline-1-messages" aria-live="assertive">
                </div>
            </div>
        </div>
        <div class="fr-fieldset__element fr-fieldset__element--inline">
            <div class="fr-checkbox-group">
                <input name="checkboxes-valid-inline-2" id="checkboxes-valid-inline-2" type="checkbox" aria-describedby="checkboxes-valid-inline-2-messages">
                <label class="fr-label" for="checkboxes-valid-inline-2">
                    Libellé case à cocher
                </label>
                <div class="fr-messages-group" id="checkboxes-valid-inline-2-messages" aria-live="assertive">
                </div>
            </div>
        </div>
        <div class="fr-fieldset__element fr-fieldset__element--inline">
            <div class="fr-checkbox-group">
                <input name="checkboxes-valid-inline-3" id="checkboxes-valid-inline-3" type="checkbox" aria-describedby="checkboxes-valid-inline-3-messages">
                <label class="fr-label" for="checkboxes-valid-inline-3">
                    Libellé case à cocher
                </label>
                <div class="fr-messages-group" id="checkboxes-valid-inline-3-messages" aria-live="assertive">
                </div>
            </div>
        </div>
        <div class="fr-messages-group" id="checkboxes-valid-inline-messages" aria-live="assertive">
            <p class="fr-message fr-message--valid" id="checkboxes-valid-inline-message-valid">Texte de validation</p>
        </div>
    </fieldset>
                          
                        

**Pour le composant seul**

Sur une case à cocher simple (choix binaire), l'état d’erreur est signalé par
le changement de couleur de la bordure - qui devient rouge - , et par
l’affichage un message d’erreur apparait en-dessous du composant (cf. couleurs
fonctionnelles : le rouge est la couleur de l’état erreur).

#### Pour les développeurs

Le message d’erreur ou de succès, sur case à cocher seule, est lié à l’input
par la présence sur ce dernier d’un attribut `aria-describedby` .

Label checkbox

Texte de validation

###  Extrait de code

    
    
                          <div class="fr-checkbox-group fr-checkbox-group--valid">
        <input aria-describedby="checkbox-valid-messages" id="checkbox-valid" type="checkbox">
        <label class="fr-label" for="checkbox-valid">
            Label checkbox
        </label>
        <div class="fr-messages-group" id="checkbox-valid-messages" aria-live="assertive">
            <p class="fr-message fr-message--valid" id="checkbox-valid-message-valid">Texte de validation</p>
        </div>
    </div>
                          
                        

Label checkbox

Texte d’erreur obligatoire

###  Extrait de code

    
    
                          <div class="fr-checkbox-group fr-checkbox-group--error">
        <input aria-describedby="checkbox-error-messages" id="checkbox-error" type="checkbox">
        <label class="fr-label" for="checkbox-error">
            Label checkbox
        </label>
        <div class="fr-messages-group" id="checkbox-error-messages" aria-live="assertive">
            <p class="fr-message fr-message--error" id="checkbox-error-message-error">Texte d’erreur obligatoire</p>
        </div>
    </div>
                          
                        

## État désactivé

L'état désactivé indique que utilisateur ne peux pas interagir avec l'élément.

Légende pour l’ensemble des éléments

Libellé case à cocher

Libellé case à cocher

Libellé case à cocher

###  Extrait de code

    
    
                          <fieldset class="fr-fieldset" id="checkboxes-disabled" aria-labelledby="checkboxes-disabled-legend checkboxes-disabled-messages">
        <legend class="fr-fieldset__legend--regular fr-fieldset__legend" id="checkboxes-disabled-legend">
            Légende pour l’ensemble des éléments
        </legend>
        <div class="fr-fieldset__element">
            <div class="fr-checkbox-group">
                <input disabled name="checkboxes-disabled-1" id="checkboxes-disabled-1" type="checkbox" aria-describedby="checkboxes-disabled-1-messages">
                <label class="fr-label" for="checkboxes-disabled-1">
                    Libellé case à cocher
                </label>
                <div class="fr-messages-group" id="checkboxes-disabled-1-messages" aria-live="assertive">
                </div>
            </div>
        </div>
        <div class="fr-fieldset__element">
            <div class="fr-checkbox-group">
                <input checked disabled name="checkboxes-disabled-2" id="checkboxes-disabled-2" type="checkbox" aria-describedby="checkboxes-disabled-2-messages">
                <label class="fr-label" for="checkboxes-disabled-2">
                    Libellé case à cocher
                </label>
                <div class="fr-messages-group" id="checkboxes-disabled-2-messages" aria-live="assertive">
                </div>
            </div>
        </div>
        <div class="fr-fieldset__element">
            <div class="fr-checkbox-group">
                <input disabled name="checkboxes-disabled-3" id="checkboxes-disabled-3" type="checkbox" aria-describedby="checkboxes-disabled-3-messages">
                <label class="fr-label" for="checkboxes-disabled-3">
                    Libellé case à cocher
                </label>
                <div class="fr-messages-group" id="checkboxes-disabled-3-messages" aria-live="assertive">
                </div>
            </div>
        </div>
        <div class="fr-messages-group" id="checkboxes-disabled-messages" aria-live="assertive">
        </div>
    </fieldset>
                          
                        

## Tailles

La taille par défaut est de 24px (taille Medium - MD) , ce qui permet
optimiser l’ergonomie et l’accessibilité en ayant un zone cliquable
confortable.

Légende pour l’ensemble des éléments

Libellé case à cocher

Libellé case à cocher

Libellé case à cocher

###  Extrait de code

    
    
                          <fieldset class="fr-fieldset" id="checkboxes" aria-labelledby="checkboxes-legend checkboxes-messages">
        <legend class="fr-fieldset__legend--regular fr-fieldset__legend" id="checkboxes-legend">
            Légende pour l’ensemble des éléments
        </legend>
        <div class="fr-fieldset__element">
            <div class="fr-checkbox-group">
                <input name="checkboxes-1" id="checkboxes-1" type="checkbox" aria-describedby="checkboxes-1-messages">
                <label class="fr-label" for="checkboxes-1">
                    Libellé case à cocher
                </label>
                <div class="fr-messages-group" id="checkboxes-1-messages" aria-live="assertive">
                </div>
            </div>
        </div>
        <div class="fr-fieldset__element">
            <div class="fr-checkbox-group">
                <input checked name="checkboxes-2" id="checkboxes-2" type="checkbox" aria-describedby="checkboxes-2-messages">
                <label class="fr-label" for="checkboxes-2">
                    Libellé case à cocher
                </label>
                <div class="fr-messages-group" id="checkboxes-2-messages" aria-live="assertive">
                </div>
            </div>
        </div>
        <div class="fr-fieldset__element">
            <div class="fr-checkbox-group">
                <input name="checkboxes-3" id="checkboxes-3" type="checkbox" aria-describedby="checkboxes-3-messages">
                <label class="fr-label" for="checkboxes-3">
                    Libellé case à cocher
                </label>
                <div class="fr-messages-group" id="checkboxes-3-messages" aria-live="assertive">
                </div>
            </div>
        </div>
        <div class="fr-messages-group" id="checkboxes-messages" aria-live="assertive">
        </div>
    </fieldset>
                          
                        

Une taille ‘small’ (SM) de 16 px est également disponible. Il s’agit de la
taille standard proposé par les navigateurs. Attention toutefois à laisser une
zone de clic suffisante (notamment pour le tactile ou une zone de 44 px de
hauteur est fortement conseillée).

Légende pour l’ensemble des éléments

Libellé case à cocher

Libellé case à cocher

Libellé case à cocher

###  Extrait de code

    
    
                          <fieldset class="fr-fieldset" id="checkboxes-small" aria-labelledby="checkboxes-small-legend checkboxes-small-messages">
        <legend class="fr-fieldset__legend--regular fr-fieldset__legend" id="checkboxes-small-legend">
            Légende pour l’ensemble des éléments
        </legend>
        <div class="fr-fieldset__element">
            <div class="fr-checkbox-group fr-checkbox-group--sm">
                <input name="checkboxes-small-1" id="checkboxes-small-1" type="checkbox" aria-describedby="checkboxes-small-1-messages">
                <label class="fr-label" for="checkboxes-small-1">
                    Libellé case à cocher
                </label>
                <div class="fr-messages-group" id="checkboxes-small-1-messages" aria-live="assertive">
                </div>
            </div>
        </div>
        <div class="fr-fieldset__element">
            <div class="fr-checkbox-group fr-checkbox-group--sm">
                <input checked name="checkboxes-small-2" id="checkboxes-small-2" type="checkbox" aria-describedby="checkboxes-small-2-messages">
                <label class="fr-label" for="checkboxes-small-2">
                    Libellé case à cocher
                </label>
                <div class="fr-messages-group" id="checkboxes-small-2-messages" aria-live="assertive">
                </div>
            </div>
        </div>
        <div class="fr-fieldset__element">
            <div class="fr-checkbox-group fr-checkbox-group--sm">
                <input name="checkboxes-small-3" id="checkboxes-small-3" type="checkbox" aria-describedby="checkboxes-small-3-messages">
                <label class="fr-label" for="checkboxes-small-3">
                    Libellé case à cocher
                </label>
                <div class="fr-messages-group" id="checkboxes-small-3-messages" aria-live="assertive">
                </div>
            </div>
        </div>
        <div class="fr-messages-group" id="checkboxes-small-messages" aria-live="assertive">
        </div>
    </fieldset>
                          
                        

## Accessibilité

Les règles d’accessibilité pour les champs sont :

  * Chaque champ possède un label auquel il est lié grâce aux attributs id et for (ex : <input id=”champ-01”><label for=”champ-01”>).
  * Les champs dont la saisie est obligatoire sont signalés comme tels au niveau du label et en utilisant l’attribut required.
  * Les groupes de cases à cocher doivent être regroupés dans une balise fieldset. Une balise legend doit alors être présente car elle constitue l’en-tête du groupe de cases à cocher.
  * Les champs de formulaire répétés et ayant la même fonction dans la page ou dans un ensemble de pages ont des libellés cohérents.
  * Les champs de même nature sont regroupés à l’aide d’une balise <fieldset> dont le rôle est décrit dans une balise <legend>.
  * Pour chaque erreur de saisie, le type ou le format de donnée attendu est suggéré.
  * L’oeil lit spontanément de bas en haut, afficher les champs en liste verticale pour faciliter la lecture et optimiser l’ergonomie  

### Personnalisation

Le style de ce composant n’est pas personnalisable. Toutefois, certains
éléments sont optionnels et les icônes peuvent être changées - voir la
structure du composant.

### Besoin d'aide ?

L'équipe du DSFR est là pour vous aider.

Retrouvez-la sur :

  * [la communauté slack](https://gouvfr.slack.com/ "la communauté slack - nouvelle fenêtre") pour poser vos questions, et échanger avec d’autres utilisateurs.   
Vous êtes **agent de l’État** et souhaitez accéder au slack ? [Rejoignez la
communauté](https://gouvfr.atlassian.net/servicedesk/customer/portal/1/group/1/create/9
"Rejoignez la communauté - nouvelle fenêtre") dès maintenant !

  * [ le centre de support](https://gouvfr.atlassian.net/servicedesk/customer/portals "le centre de support - nouvelle fenêtre") pour envoyer vos demandes de correctifs et d'évolution.

[Bouton radio riche - Radio rich](/composants-et-modeles/composants/bouton-
radio-riche)

[Carte - Card](/composants-et-modeles/composants/carte)

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
