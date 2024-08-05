Fermer

# Ajout de fichier - Upload

Ce composant permet aux utilisateurs de sélectionner et envoyer un ou
plusieurs fichiers.

## Structure

Le composant “ajout de fichier” est composé de :

  * Un label - le texte du label exprime clairement l’action attendu pour l’utilisateur, par défaut : “Ajouter un fichier” - obligatoire 
  * Un texte explicatif qui précise les contraintes au niveau du ou des fichiers attendus : format, poids attendus, nombre de fichiers possible… - obligatoire
  * Le bouton “parcourir” et le texte des fichiers qui sont gérés en natif directement par le navigateur - obligatoire

Au clic sur parcourir, la boite de dialogue de sélection de fichier s’affiche.
Les noms des fichiers sélectionnés viennent s’afficher à la place du texte par
défaut.

Ajouter des fichiers Taille maximale : 500 Mo. Formats supportés : jpg, png,
pdf. Plusieurs fichiers possibles. Lorem ipsum dolor sit amet, consectetur
adipiscing.

    
    
                    <div class="fr-upload-group">
        <label class="fr-label" for="file-upload">Ajouter des fichiers
            <span class="fr-hint-text">Taille maximale : 500 Mo. Formats supportés : jpg, png, pdf. Plusieurs fichiers possibles. Lorem ipsum dolor sit amet, consectetur adipiscing.</span>
        </label>
        <input class="fr-upload" type="file" id="file-upload" name="file-upload">
    </div>
                    
                  

### Erreur

Ajouter des fichiers Taille maximale : 500 Mo. Formats supportés : jpg, png,
pdf. Plusieurs fichiers possibles. Lorem ipsum dolor sit amet, consectetur
adipiscing.

Format de fichier non supporté

    
    
                    <!-- Erreur -->
    
    <div class="fr-upload-group fr-input-group--error">
        <label class="fr-label" for="file-upload-with-error">Ajouter des fichiers
            <span class="fr-hint-text">Taille maximale : 500 Mo. Formats supportés : jpg, png, pdf. Plusieurs fichiers possibles. Lorem ipsum dolor sit amet, consectetur adipiscing.</span>
        </label>
        <input class="fr-upload" type="file" aria-describedby="file-upload-with-error-desc-error" id="file-upload-with-error" name="file-upload-with-error">
        <p id="file-upload-with-error-desc-error" class="fr-error-text">
            Format de fichier non supporté 
        </p>
    </div>
                    
                  

### Ajout multiple

Afin de pouvoir sélectionner plusieurs fichiers, il faut ajouter l'attribut
**multiple** à la balise input

Ajouter des fichiers Taille maximale : 500 Mo. Formats supportés : jpg, png,
pdf. Plusieurs fichiers possibles. Lorem ipsum dolor sit amet, consectetur
adipiscing.

    
    
    <!-- Ajout multiple : ajout de l'attribut multiple sur la balise input -->
    
    <input class="fr-upload" type="file" id="file-upload" name="file-upload" multiple>
    

### Désactivé

Ajouter un fichier Taille maximale : 500 Mo. Formats supportés : jpg, png,
pdf. Plusieurs fichiers possibles. Lorem ipsum dolor sit amet, consectetur
adipiscing.

    
    
                    <!-- Désactivé-->
    
    <div class="fr-upload-group fr-input-group--disabled ">
        <label class="fr-label" for="file-upload-disabled">Ajouter un fichier
            <span class="fr-hint-text">Taille maximale : 500 Mo. Formats supportés : jpg, png, pdf. Plusieurs fichiers possibles. Lorem ipsum dolor sit amet, consectetur adipiscing.</span>
        </label>
        <input disabled class="fr-upload" type="file" id="file-upload-disabled" name="file-upload-disabled" >
    </div>
                    
                  

## Règles d’utilisation

### Usage

  * Demander aux utilisateurs d’envoyer un fichier doit être fait que si cela est vraiment essentiel à votre service.
  * Précisez les erreurs rencontrés lors de l’envoi de fichier : Taille du fichier : préciser la taille du fichier attendu.Format : redonner les types de fichiers autorisés.
  * Taille du fichier : préciser la taille du fichier attendu.
  * Format : redonner les types de fichiers autorisés.
  * Quand vous avec plusieurs fichiers à demander aux utilisateurs dans un même formulaire :utiliser l’upload multiple - en ajoutant de l’attribut multiple sur l’input - quand vous demandez à l’utilisateur des fichiers de même nature et respectant les mêmes contraintesutiliser plusieurs champs upload quand vous demandez à l’utilisateur des fichiers de différentes natures avec des contraintes spécifiques.
  * Utiliser l’upload multiple - en ajoutant de l’attribut multiple sur l’input - quand vous demandez à l’utilisateur des fichiers de même nature et respectant les mêmes contraintes.
  * Utiliser plusieurs champs upload quand vous demandez à l’utilisateur des fichiers de différentes natures avec des contraintes spécifiques.

### Accessibilité

  * S’assurer de la pertinence du label (ex. “Téléchargez/Téléversez votre image de profil”)
  * Le texte descriptif doit contenir l’ensemble des formats/poids/tailles attendus (ex. “Votre image de profil doit être au format png ou jpg et ne pas excéder 100ko”). Il est intégré au label comme le [Champs de saisie](/elements-d-interface/composants/champ-de-saisie). 

### Personnalisation

  * Le composant reprend le comportement natif, il y a donc aucun personnalisation graphique possible.

[Accordéon - Accordion](/composants-et-modeles/composants/accordeon)

[Alerte - Alert](/composants-et-modeles/composants/alerte)

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
