Fermer

# Groupe de boutons - Button group

Les boutons dans le contexte d'un groupe suivent les même règles que le
composant bouton :  

  * Il prend en charge les 2 types de boutons (primaire, secondaire)
  * Il gère les 3 tailles (SM, MD, LG) et les variantes ( Icônes / texte seul, avec icônes à gauche / droite)

## Groupe de boutons vertical

Cette disposition permet d’associer plusieurs boutons d’actions à la verticale
:

  * Alignement des boutons en colonne les uns au dessus des autres avec un espacement de 2W. 
  * La largeur des boutons prend 100% de la largeur du container (« full width ») par défaut. 
  * Des modificateurs permettent de changer l’orientation des boutons à partir de points de rupture donnés (voir groupes de bouton horizontal).

  * Label bouton 
  * Label bouton 

    
    
                    <ul class="fr-btns-group">
        <li>
            <button class="fr-btn">
                Label bouton
            </button>
        </li>
        <li>
            <button class="fr-btn fr-btn--secondary">
                Label bouton
            </button>
        </li>
    </ul>
                    
                  

## Groupe de boutons horizontal

Cette disposition permet d’associer plusieurs boutons d’actions à
l’horizontale :

  * Espacement de 2W à droite de chaque bouton excepté le dernier (en savoir plus sur les espacements du DSFR.
  * Espacement en dessous de chaque bouton de 2W.
  * Boutons placés les uns à côté des autres avec un retour à la ligne si dépassement de la taille du conteneur.  

![](/uploads/Capture_d_ecran_2021_01_11_a_12_58_32_ec2de94645.png)

  * Label bouton 
  * Label bouton 

  * Label bouton 
  * Label bouton 2 
  * Label bouton 3 

Il est aussi possible d’appliquer le mode horizontal à partir d’un point de
rupture défini en ajoutant l'extension `-sm`, `-md`, ou `-lg` au modificateur
`fr-btns-group--inline` , ainsi :

  * fr-btns-group--inline-sm applique le mode horizontal à partir du point de rupture SM (576px).
  * fr-btns-group--inline-md applique le mode horizontal à partir du point de rupture MD (768px).
  * fr-btns-group--inline-lg applique le mode horizontal à partir du point de rupture LG (992px).

    
    
    <ul class="fr-btns-group fr-btns-group--inline-sm"> ...</ul>
    <ul class="fr-btns-group fr-btns-group--inline-md"> ...</ul>
    <ul class="fr-btns-group fr-btns-group--inline-lg"> ...</ul>

## Placement

Par défaut le groupe de boutons horizontal est ferré à gauche du conteneur. Il
est possible de le centrer et de le ferrer à droite avec les modificateurs
suivants :

  * fr-btns-group--center Pour aligner les boutons au centre du conteneur.
  * fr-btns-group--right pour aligner les boutons sur la droite.En cas d’alignement a droite, il existe une option pour inverser l’ordre des boutons : fr-btns-group--inline-reverse. Cela permet de conserver l’ordre des boutons (bouton primaire en première position dans le flux et donc en mobile) tout en plaçant le bouton primaire à droite en desktop.

## Tailles

Dans un groupe de boutons, la gestion de la taille des boutons SM, MD et LG se
fait au niveau du groupe uniquement.La taille MD est la taille par défaut. Les
modificateurs `fr-btns-group--sm` , ou `fr-btns-group--lg` sur le groupe
permettent d'appliquer les tailles SM et LG aux boutons.

  * Label bouton 
  * Label bouton 

  * Label bouton 
  * Label bouton 

    
    
                    <!-- Groupes de boutons en taille small -->
    
    <ul class="fr-btns-group fr-btns-group--sm">
        <li>
            <button class="fr-btn">
                Label bouton
            </button>
        </li>
        <li>
            <button class="fr-btn fr-btn--secondary">
                Label bouton
            </button>
        </li>
    </ul>
    
    <!-- Groupes de boutons en taille large -->
    
    <ul class="fr-btns-group fr-btns-group--lg">
        <li>
            <button class="fr-btn">
                Label bouton
            </button>
        </li>
        <li>
            <button class="fr-btn fr-btn--secondary">
                Label bouton
            </button>
        </li>
    </ul>
                    
                  

### Pour les designers Sketch

Les groupes de boutons verticaux sont constitués de boutons “fluides”
disponibles par défaut à 588 px pour s’intégrer dans un prototype mobile. Ces
symboles sont prévus pour s’adapter à la largeur des conteneurs de vos
designs.

Les groupes de boutons horizontaux sont constitués des boutons “avec padding”,
qui se redimensionnent automatiquement en fonction du contenu texte.

La modularité proposée en code permet d’obtenir des boutons d’une même largeur
dans un groupe horizontal, la largeur étant définie par le bouton le plus
large. Pour les utiliser il faudra créer le groupe avec les symboles de
boutons “fluides” présents dans “02 Composants / - Éléments - ne pas utiliser
/ Boutons / Fluides“, et respecter les spécifications d’espacements du groupe
de boutons horizontaux.

### Pour les développeurs

**Ajouter des icônes au groupe de boutons**

Il est possible, d’utiliser dans le groupe des boutons, des boutons avec
icônes. La gestion des icônes, est gérée au niveau de chaque bouton. De la
même façon qu’un bouton seul.

Attention, pour que le texte s’affiche (si vous souhaitez des boutons avec
texte et bouton), il faut ajouter les modifiers `fr-btns-group--icon-left` ou
`fr-btns-group--icon-right` sur la liste `fr-btns-group.`Voir : [Documentation
sur les boutons](https://www.systeme-de-design.gouv.fr/composants-et-
modeles/composants/bouton) pour l’affichage des icônes. A noter que les icônes
ont la même place au sein d’un groupe (à droite ou à gauche).

**Forcer une même largeur pour l’ensemble des boutons du groupe**

Une option permet de mettre automatiquement tous les boutons d’un groupe à la
même largeur, en se basant sur le bouton le plus large. Cela permet une
uniformité des boutons en mode horizontal comme vertical.

En mode vertical et en mobile, cette option permet aussi d'éviter que les
boutons prennent 100% de la largeur du conteneur. Le modificateur `fr-btns-
group--equisized` permet d’exécuter le JavaScript fixant la taille des
boutons.

Cette option peut être combiné avec les modificateurs d’alignements `fr-btns-
group--right et ` et `fr-btns-group--center` pour aligner les boutons sur la
droite ou au centre du conteneur. (Par défaut : alignés à gauche)

**Exemple d’un groupe de boutons de même taille :**

  * Label bouton 
  * lorem ipsum label très long 

    
    
                    <ul class="fr-btns-group fr-btns-group--equisized">
        <li>
            <button class="fr-btn">
                Label bouton
            </button>
        </li>
        <li>
            <button class="fr-btn fr-btn--secondary">
                lorem ipsum label très long
            </button>
        </li>
    </ul>
                    
                  

## Règles d’utilisation

### Usages

Pour chaque groupe de boutons, veillez à :

  * Avoir un seul bouton primaire pour l'action principale, les autres boutons en secondaire.
  * Toujours positionner le bouton primaire avant les boutons secondaires quand le groupe est ferré à gauche ou centré.
  * Toujours positionner le bouton primaire après les boutons secondaires quand le groupe est ferré à droite.
  * Utiliser la même taille pour tous les boutons du groupe (SM, MD , LG).
  * Utiliser la même typologie pour tous les boutons du groupe (icônes ou texte seul, avec icônes à gauche ou droite).

### Accessibilité

  * Les libellés doivent être explicites.
  * L’utilisation de l’attribut title (ou aria-label) ne doit être utilisé uniquement que si l’intitulé du bouton n’est pas explicite (ce qui n’est pas recommandé).
  * Dans le cas (fortement déconseillé) d’un bouton icône seule, préciser le rôle du bouton à l’aide de l’attribut title en suivant les règles ci-dessous.

### Contenus

  * Le libellé des boutons doit commencer par un verbe, de préférence d’action qui exprime clairement ce qui va se passer pour l’utilisateur.
  * Le libellé doit être court et compréhensible facilement : utiliser 3 mots maximum.
  * Il faut utiliser le même format d'écriture sur tout vos libellés de boutons (exemple : 1ère lettre en majuscule, le reste en minuscule, infinitif, etc).

### Personnalisation

Le style de ce composant n’est pas personnalisable. Toutefois, certains
éléments des boutons sont optionnels et les icônes peuvent être changées -
voir la structure du composant [bouton](/elements-d-
interface/composants/bouton).

### Besoin d'aide ?

L'équipe du DSFR est là pour vous aider.

Retrouvez-la sur :

  * [la communauté slack](https://gouvfr.slack.com/ "la communauté slack - nouvelle fenêtre") pour poser vos questions, et échanger avec d’autres utilisateurs.   
Vous êtes **agent de l’État** et souhaitez accéder au slack ? [Rejoignez la
communauté](https://gouvfr.atlassian.net/servicedesk/customer/portal/1/group/1/create/9
"Rejoignez la communauté - nouvelle fenêtre") dès maintenant !

  * [ le centre de support](https://gouvfr.atlassian.net/servicedesk/customer/portals "le centre de support - nouvelle fenêtre") pour envoyer vos demandes de correctifs et d'évolution.

[Bouton - Button](/composants-et-modeles/composants/bouton)

[Bouton FranceConnect](/composants-et-modeles/composants/bouton-franceconnect)

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
