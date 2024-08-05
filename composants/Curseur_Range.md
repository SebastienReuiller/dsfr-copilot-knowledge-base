Fermer

# Curseur - Range

Le composant curseur est un input composé d'entrées numériques permettant de
délimiter manuellement une sélection par rapport à une valeur minimale et
maximale. Ils sert à montrer en temps réel les options choisies et éclairer la
prise de décision.

## Structure

Le curseur se compose des éléments suivants :

  1. Label ( **obligatoire** )
  2. Texte de description additionnel (optionnel)
  3. Piste avec poignée et valeur sélectionnée ( **obligatoire** )
  4. Valeur min et max (optionnel)
  5. Message d’information défaut ou erreur (optionnel)

![](/uploads/Curseur_Structure_07ed41aca6.png)

## Variations

Le curseur existe en deux version SM et MD :

  * En desktop la taille minimum est 180 px et la taille minimum est 588 px ;
  * En mobile la taille minimum est 136 px et la taille minimum est 288 px ;
  * En mobile, préférez la version MD.  
  

#### Taille SM

**Curseur simple**

Label Texte de description additionnel, valeur de 0 à 100.

50 0 100

###  Extrait de code

    
    
                          <div class="fr-range-group" id="range-2246-group">
        <label class="fr-label">
            Label
            <span class="fr-hint-text">Texte de description additionnel, valeur de 0 à 100.</span>
        </label>
        <div class="fr-range fr-range--sm">
            <span class="fr-range__output">50</span>
            <input id="range-2245" name="range-2245" type="range" aria-labelledby="range-2245-label" max="100" value="50" aria-describedby="range-2245-messages">
            <span class="fr-range__min" aria-hidden="true">0</span>
            <span class="fr-range__max" aria-hidden="true">100</span>
        </div>
        <div class="fr-messages-group" id="range-2245-messages" aria-live="polite">
        </div>
    </div>
                          
                        

**Curseur double**

Label Texte de description additionnel, valeur de 0 à 100.

25 0 100

###  Extrait de code

    
    
                          <div class="fr-range-group" id="range-2271-group">
        <label class="fr-label">
            Label
            <span class="fr-hint-text">Texte de description additionnel, valeur de 0 à 100.</span>
        </label>
        <div class="fr-range fr-range--sm fr-range--double">
            <span class="fr-range__output">25</span>
            <input id="range-2270" name="range-2270" type="range" aria-labelledby="range-2270-label" max="100" value="25" aria-describedby="range-2270-messages">
            <input id="range-2270-2" name="range-2270-2" type="range" aria-labelledby="range-2270-label" max="100" aria-describedby="range-2270-messages">
            <span class="fr-range__min" aria-hidden="true">0</span>
            <span class="fr-range__max" aria-hidden="true">100</span>
        </div>
        <div class="fr-messages-group" id="range-2270-messages" aria-live="polite">
        </div>
    </div>
                          
                        

**Curseur c** **ranté**

Label Texte de description additionnel, valeur de 0 à 100.

50 0 100

###  Extrait de code

    
    
                          <div class="fr-range-group" id="range-2261-group">
        <label class="fr-label">
            Label
            <span class="fr-hint-text">Texte de description additionnel, valeur de 0 à 100.</span>
        </label>
        <div class="fr-range fr-range--sm fr-range--step">
            <span class="fr-range__output">50</span>
            <input id="range-2260" name="range-2260" type="range" aria-labelledby="range-2260-label" max="100" value="50" step="10" aria-describedby="range-2260-messages">
            <span class="fr-range__min" aria-hidden="true">0</span>
            <span class="fr-range__max" aria-hidden="true">100</span>
        </div>
        <div class="fr-messages-group" id="range-2260-messages" aria-live="polite">
        </div>
    </div>
                          
                        

#### Taille MD

**Curseur simple**

Label Texte de description additionnel, valeur de 0 à 100.

50 0 100

###  Extrait de code

    
    
                          <div class="fr-range-group" id="range-2241-group">
        <label class="fr-label">
            Label
            <span class="fr-hint-text">Texte de description additionnel, valeur de 0 à 100.</span>
        </label>
        <div class="fr-range">
            <span class="fr-range__output">50</span>
            <input id="range-2240" name="range-2240" type="range" aria-labelledby="range-2240-label" max="100" value="50" aria-describedby="range-2240-messages">
            <span class="fr-range__min" aria-hidden="true">0</span>
            <span class="fr-range__max" aria-hidden="true">100</span>
        </div>
        <div class="fr-messages-group" id="range-2240-messages" aria-live="polite">
        </div>
    </div>
                          
                        

**Curseur double**

Label Texte de description additionnel, valeur de 0 à 100.

25 0 100

###  Extrait de code

    
    
                          <div class="fr-range-group" id="range-2266-group">
        <label class="fr-label">
            Label
            <span class="fr-hint-text">Texte de description additionnel, valeur de 0 à 100.</span>
        </label>
        <div class="fr-range fr-range--double">
            <span class="fr-range__output">25</span>
            <input id="range-2265" name="range-2265" type="range" aria-labelledby="range-2265-label" max="100" value="25" aria-describedby="range-2265-messages">
            <input id="range-2265-2" name="range-2265-2" type="range" aria-labelledby="range-2265-label" max="100" aria-describedby="range-2265-messages">
            <span class="fr-range__min" aria-hidden="true">0</span>
            <span class="fr-range__max" aria-hidden="true">100</span>
        </div>
        <div class="fr-messages-group" id="range-2265-messages" aria-live="polite">
        </div>
    </div>
                          
                        

**Curseur cranté**

Label Texte de description additionnel, valeur de 0 à 100.

50 0 100

###  Extrait de code

    
    
                          <div class="fr-range-group" id="range-2256-group">
        <label class="fr-label">
            Label
            <span class="fr-hint-text">Texte de description additionnel, valeur de 0 à 100.</span>
        </label>
        <div class="fr-range fr-range--step">
            <span class="fr-range__output">50</span>
            <input id="range-2255" name="range-2255" type="range" aria-labelledby="range-2255-label" max="100" value="50" step="10" aria-describedby="range-2255-messages">
            <span class="fr-range__min" aria-hidden="true">0</span>
            <span class="fr-range__max" aria-hidden="true">100</span>
        </div>
        <div class="fr-messages-group" id="range-2255-messages" aria-live="polite">
        </div>
    </div>
                          
                        

#### Autres variations

**Sans indicateurs minimum et maximum**

Label Texte de description additionnel, valeur de 0 à 100.

50

###  Extrait de code

    
    
                          <div class="fr-range-group" id="range-2251-group">
        <label class="fr-label">
            Label
            <span class="fr-hint-text">Texte de description additionnel, valeur de 0 à 100.</span>
        </label>
        <div class="fr-range">
            <span class="fr-range__output">50</span>
            <input id="range-2250" name="range-2250" type="range" aria-labelledby="range-2250-label" max="100" value="50" aria-describedby="range-2250-messages">
        </div>
        <div class="fr-messages-group" id="range-2250-messages" aria-live="polite">
        </div>
    </div>
                          
                        

**Avec préfixe et suffixe**

Label Texte de description additionnel, valeur de 0 à 100.

~50% ~0% ~100%

###  Extrait de code

    
    
                          <div class="fr-range-group" id="range-2276-group">
        <label class="fr-label">
            Label
            <span class="fr-hint-text">Texte de description additionnel, valeur de 0 à 100.</span>
        </label>
        <div class="fr-range" data-fr-prefix="~" data-fr-suffix="%">
            <span class="fr-range__output">~50%</span>
            <input id="range-2275" name="range-2275" type="range" aria-labelledby="range-2275-label" max="100" value="50" aria-describedby="range-2275-messages">
            <span class="fr-range__min" aria-hidden="true">~0%</span>
            <span class="fr-range__max" aria-hidden="true">~100%</span>
        </div>
        <div class="fr-messages-group" id="range-2275-messages" aria-live="polite">
        </div>
    </div>
                          
                        

#### Désactivé

Label Texte de description additionnel, valeur de 0 à 100.

50 0 100

###  Extrait de code

    
    
                          <div class="fr-range-group fr-range-group--disabled" id="range-2281-group">
        <label class="fr-label">
            Label
            <span class="fr-hint-text">Texte de description additionnel, valeur de 0 à 100.</span>
        </label>
        <div class="fr-range">
            <span class="fr-range__output">50</span>
            <input id="range-2280" name="range-2280" type="range" disabled aria-labelledby="range-2280-label" max="100" value="50" aria-describedby="range-2280-messages">
            <span class="fr-range__min" aria-hidden="true">0</span>
            <span class="fr-range__max" aria-hidden="true">100</span>
        </div>
        <div class="fr-messages-group" id="range-2280-messages" aria-live="polite">
        </div>
    </div>
                          
                        

**Avec erreur**

Label Texte de description additionnel, valeur de 0 à 100.

50 0 100

Valeur sélectionnée impossible

###  Extrait de code

    
    
                          <div class="fr-range-group fr-range-group--error" id="range-2286-group">
        <label class="fr-label">
            Label
            <span class="fr-hint-text">Texte de description additionnel, valeur de 0 à 100.</span>
        </label>
        <div class="fr-range">
            <span class="fr-range__output">50</span>
            <input id="range-2285" name="range-2285" type="range" aria-labelledby="range-2285-label" max="100" value="50" aria-describedby="range-2285-messages">
            <span class="fr-range__min" aria-hidden="true">0</span>
            <span class="fr-range__max" aria-hidden="true">100</span>
        </div>
        <div class="fr-messages-group" id="range-2285-messages" aria-live="polite">
            <p class="fr-message fr-message--error" id="range-2285-message-error">Valeur sélectionnée impossible</p>
        </div>
    </div>
                          
                        

## Règles d'utilisation

#### Usage

  * Utilisez un curseur **lorsque la valeur saisie est imprécise ou à déterminer** : par exemple la luminosité d’un écran. A contrario l’année de naissance est une valeur précise donc préférez un champ de saisie ou une liste déroulante.
  * Sauf cas exceptionnel, **le curseur ne doit pas être utilisé dans les formulaires**.
  * Son usage doit aller de pair avec une actualisation du résultat en temps réel en fonction de la valeur sélectionnée : par exemple en tant que filtre déterminant l’affichage de donnée ou non dans une liste ou un tableau.
  * La valeur du curseur est toujours en nombre. Des unités peuvent y être ajoutées (k€, €, kg, etc).   
  

#### A ne pas faire

  * Évitez d'utiliser un curseur sans fournir un retour visuel immédiat sur les résultats de l'interaction de l'utilisateur.
  * N'utilisez pas de curseur si le nombre de valeurs spécifiques est important, préférez un [champ de saisie](/elements-d-interface/composants/champ-de-saisie) ou une [liste déroulante](/elements-d-interface/composants/liste-deroulante) au curseur cranté.
  * N'utilisez pas d’échelle de valeur trop petite, par exemple 1-3 : préférez dans ce cas de figure des cases à cocher ou des boutons radios. Exemple :  

![](/uploads/Curseur_Attention_2_b4a5a54a48.png)

  * Si l’échelle de valeur est large mais que l’espace est limité, un champ de saisie est un meilleur choix.   

![](/uploads/Curseur_Attention_3_bdd980a78d.png)

  * N'utilisez pas de glissière pour communiquer l’état d’avancement ; utilisez plutôt le composant [Indicateur d'étapes](/elements-d-interface/composants/indicateur-d-etapes).  
  

#### Accessibilité

Voici les points d'attention à prendre en compte dans l'implémentation du
curseur :

  * Le label du curseur doit expliciter la nature de la valeur sélectionnée 
  * Pouvoir cliquer n'importe où sur la piste horizontale (sauf curseur double)
  * Pouvoir utiliser les flèches du clavier pour modifier la valeur et l’emplacement de la poignée
  * Le focus est placé sur la poignée (l'objet visuel que l'utilisateur de la souris déplacerait)  
  

#### Personnalisation

Aucune personnalisation de ce composant n'est possible.

[Contrôle segmenté - Segmented control](/composants-et-
modeles/composants/controle-segmente)

[En-tête - Header](/composants-et-modeles/composants/en-tete)

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
