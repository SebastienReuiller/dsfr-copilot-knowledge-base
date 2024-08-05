Fermer

# Badge - Badge

Le composant badge permet de mettre en avant une information de type “statut”
ou “état” sur un élément du site.

Le badge n’est pas un composant ‘cliquable’. Il doit être associé à une
information donnée sur une page pour préciser le statut ou l'état associée à
cette information.

## Structure

### Badge par défaut

La composant badge est composée de :

  * un bloc en ligne avec un léger radius - obligatoire
  * un fond de couleur (couleur claire) - obligatoire
  * un texte de couleur (couleur foncée), en majuscule - obligatoire, à adapter en fonction du contexte pour donner la nature de l'état ou du status. Voir les couleurs de personnalisation.

Le composant badge est disponible en deux tailles, SM et MD , à utiliser en
fonction de l’espace disponible.

Label badge

Label badge SM

Label badge

    
    
    <p class="fr-badge">Label badge</p>

**Taille SM**

    
    
    <p class="fr-badge fr-badge--sm">Label badge SM</p>
    

**Couleur personnalisée (** _Voir la section personnalisation.)_

    
    
    <p class="fr-badge fr-badge--green-menthe">Label badge</p>

### Badge système (avec icône optionnelle)

Cette variante peut être utilisée pour préciser l’information donnée par le
texte du badge. Elle doit être obligatoirement et uniquement utilisée quand
les couleurs ‘fonctionnelles’ sont utilisées.L’icône système est optionnelle.

Label badge

Label badge

Label badge

Label badge

Label badge

    
    
    <p class="fr-badge fr-badge--success">Label badge</p>
    
    <p class="fr-badge fr-badge--error">Label badge</p>
    
    <p class="fr-badge fr-badge--info">Label badge</p>
    
    <p class="fr-badge fr-badge--warning">Label badge</p>
    
    <p class="fr-badge fr-badge--new">Label badge</p>

### Badges systèmes sans icône

Label badge

Label badge

Label badge

Label badge

Label badge

    
    
    <p class="fr-badge fr-badge--success fr-badge--no-icon">Label badge</p>
    
    <p class="fr-badge fr-badge--error fr-badge--no-icon">Label badge</p>
    
    <p class="fr-badge fr-badge--info fr-badge--no-icon">Label badge</p>
    
    <p class="fr-badge fr-badge--warning fr-badge--no-icon">Label badge</p>
    
    <p class="fr-badge fr-badge--new fr-badge--no-icon">Label badge</p>

### Badges systèmes SM

Label badge

Label badge

Label badge

Label badge

Label badge

    
    
    <p class="fr-badge fr-badge--success fr-badge--sm fr-badge--no-icon">Label badge</p>
    
    <p class="fr-badge fr-badge--error fr-badge--sm fr-badge--no-icon">Label badge</p>
    
    <p class="fr-badge fr-badge--info fr-badge--sm">Label badge</p>
    
    <p class="fr-badge fr-badge--warning fr-badge--sm">Label badge</p>
    
    <p class="fr-badge fr-badge--new fr-badge--sm">Label badge</p>

**À faire**

 **  
**Utiliser l’icône et la couleur système correspondantes à l’information

![](/uploads/do_couleur_adaptee_1_89410d67a3.jpg)

**À ne pas faire  
**

 **  
**

Utiliser une icône dans un badge standard

![](/uploads/Dont_icone_8709d8ec62.jpg)

  * Label badge

  * Label badge

  * Label badge

  * Label badge

    
    
    <ul class="fr-badge-group">
        <li>
            <p class="fr-badge fr-badge--success">Label badge</p>
        </li>
        <li>
            <p class="fr-badge fr-badge--blue-ecume">Label badge</p>
        </li>
    </ul>
    
    <!-- SM -->
    <ul class="fr-badge-group">
        <li>
            <p class="fr-badge fr-badge--sm fr-badge--success">Label badge</p>
        </li>
        <li>
            <p class="fr-badge fr-badge--sm fr-badge--blue-ecume">Label badge</p>
        </li>
    </ul>

## Règles d’utilisation

Pour catégoriser, classer, organiser des contenus à l'aide de mots-clés,
utiliser plutôt le composant [tag](/elements-d-interface/composants/tag).

![](/uploads/dont_categoriser_782569e98f.jpg)

Le badge doit être placé directement à côté et à la suite de l’élément qu’il
illustre. Exemples :

  * badge associé à du texte ou un lien,
  * badge associé à des cartes ou des tuiles,
  * badge dans une cellule d’un tableau,
  * badge dans des éléments de navigation.

![](/uploads/Capture_d_ecran_2021_12_22_a_11_43_57_1_35954984d8.png)

### Accessibilité

  * Toujours utiliser la balise <p>, ou un <span> si celui-ci est à l'intérieur d'un <p>  

  * Éviter l’utilisation de lettre capitale (préférer l’ajout d’une classe css)
  * Vérifier le bon ratio de contraste entre la couleur du texte et la couleur de fond

### Personnalisation

Il est possible d’utiliser les couleurs illustratives sur les badges
‘standard’ uniquement

Éléments personnalisables Élément | Valeur(s) autorisée(s)  
---|---  
| Token | Classe css  
Fond | $[couleur]-950 (thème clair)  
$[couleur]-100 (thème sombre)  
  
exemples :  
green-emeraude-main-950 /  
green-emeraude-main-100  
  
brown-caramel-main-950 /  
brown-caramel-main-100  
| .fr-badge--[couleur]  
.fr-badge--green-emeraude  
.fr-badge--brown-caramel  
.fr-badge--purple-glycine  
  
Texte | $[couleur]-sun (thème clair)  
$[couleur]-moon (thème sombre)  
  
exemples:  
green-emeraude-sun-425 /  
green-emeraude-moon-753  
  
brown-caramel-425 /  
brown-caramel-moon-901  
  
[Alerte - Alert](/composants-et-modeles/composants/alerte)

[Bandeau d'information importante - Notice 🆕](/composants-et-
modeles/composants/bandeau-d-information-importante)

##### Besoin d'aide ?

L’équipe du DSFR est là pour vous aider.  

Contactez l'équipe

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
