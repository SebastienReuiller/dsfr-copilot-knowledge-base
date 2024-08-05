Fermer

# Mise en exergue - Highlight

La mise en exergue permet à l’utilisateur de distinguer et repérer une
information facilement.

## Mise en exergue

La mise en exergue met en évidence une information déjà présente dans le reste
du contenu : soit une reformulation, soit une reprise du texte. Pour mettre en
évidence une information complémentaire, utilisez [la mise en
avant](/elements-d-interface/composants/mise-en-avant).

### Structure

Elle se compose le l'élément suivant :

  * un texte - obligatoire.

Les parents d’enfants de 11 à 14 ans n’ont aucune démarche à accomplir : les
CAF versent automatiquement l’ARS aux familles déjà allocataires qui
remplissent les conditions.

    
    
                    <div class="fr-highlight">
        <p>Les parents d’enfants de 11 à 14 ans n’ont aucune démarche à accomplir : 
           les CAF versent automatiquement l’ARS aux familles déjà allocataires qui 
            remplissent les conditions.
        </p>
    </div>
                    
                  

Lorsqu’elle est intégrée dans un contenu la mise en exergue n’est pas alignée
sur la gauche avec le corps de texte. Cela permet de la mettre en avant comme
illustré dans la mise en situation ci-dessous.

## Variantes tailles et couleurs

Par défaut le composant est proposé en taille MD.Il peut également être
utilisé en taille SM ou LG en utilisant les classes utilitaires dédiées (fr-
text--BP).

Les parents d’enfants de 11 à 14 ans n’ont aucune démarche à accomplir : les
CAF versent automatiquement l’ARS aux familles déjà allocataires qui
remplissent les conditions.

Les parents d’enfants de 11 à 14 ans n’ont aucune démarche à accomplir : les
CAF versent automatiquement l’ARS aux familles déjà allocataires qui
remplissent les conditions.

    
    
                    <div class="fr-highlight">
        <p class="fr-text--sm">Les parents d’enfants de 11 à 14 ans n’ont aucune démarche à accomplir : les CAF versent automatiquement l’ARS aux familles déjà allocataires qui remplissent les conditions.</p>
    </div>
    
    <div class="fr-highlight">
        <p class="fr-text--lg">Les parents d’enfants de 11 à 14 ans n’ont aucune démarche à accomplir : les CAF versent automatiquement l’ARS aux familles déjà allocataires qui remplissent les conditions.</p>
    </div>
                    
                  

## Règles d’utilisation

### Usages

Les messages d’erreur, d’alerte ou de confirmation, ne sont pas des mises en
avant. Pour utiliser ces blocs, rendez-vous dans la section
["Alerte"](/elements-d-interface/composants/alerte) du DSFR

### Accessibilité

Pas de règle particulière tant que la sémantique html est respectée (hx et p)

### Contenus

Les informations présentées doivent être synthétiques pour être facilement
lues par l’utilisateur.

### Personnalisation

#### Couleurs d’accent

L'élément bordure peut utiliser les couleurs illustratives :

Élément  
| Valeur par défaut  
| Valeur(s) autorisée(s)  
  
---|---|---  
|  | Token | Classe css  
**Bordure** | **$border-default-blue-france**  
Correspondances :  
Thème clair et sombre =  
**$blue-france-main-525**  
| $[couleur]-main (thèmes clair / sombre)  
exemples :  
$green-emeraude-main-632  
$brown-caramel-main-648>  
  
  
| .fr-highlight--[couleur]  
exemples :  
.fr-highlight--green-emeraude  
.fr-highlight--brown-caramel  
**Fond** | **$background-contrast-neutral**  
Correspondances :  
Thème clair = **$grey-950**  
Thème sombre = **$grey-100**  
| $[couleur]-950 (thème clair)  
$[couleur]-100 (thème sombre)  
exemples :  
thème clair = green-emeraude-950  
thème sombre = green-emeraude-100  
  
thème clair = brown-caramel-950  
thème sombre = brown-caramel-100  
  
  
Les parents d’enfants de 11 à 14 ans n’ont aucune démarche à accomplir : les
CAF versent automatiquement l’ARS aux familles déjà allocataires qui
remplissent les conditions.

  

Les parents d’enfants de 11 à 14 ans n’ont aucune démarche à accomplir : les
CAF versent automatiquement l’ARS aux familles déjà allocataires qui
remplissent les conditions.

### Besoin d'aide ?

L'équipe du DSFR est là pour vous aider.

Retrouvez-la sur :

  * [la communauté slack](https://gouvfr.slack.com/ "la communauté slack - nouvelle fenêtre") pour poser vos questions, et échanger avec d’autres utilisateurs.   
Vous êtes **agent de l’État** et souhaitez accéder au slack ? [Rejoignez la
communauté](https://gouvfr.atlassian.net/servicedesk/customer/portal/1/group/1/create/9
"Rejoignez la communauté - nouvelle fenêtre") dès maintenant !

  * [ le centre de support](https://gouvfr.atlassian.net/servicedesk/customer/portals "le centre de support - nouvelle fenêtre") pour envoyer vos demandes de correctifs et d'évolution.

[Mise en avant - Callout](/composants-et-modeles/composants/mise-en-avant)

[Modale - Modal](/composants-et-modeles/composants/modale)

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
