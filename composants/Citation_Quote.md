Fermer

# Citation - Quote

La citation permet de citer un texte dans une page éditoriale. La citation
peut provenir d'un extrait d’un discours oral formulé par une tierce personne
ou d’un texte écrit.

## Structure

La citation est composée des éléments suivants :

  * le texte de la citation - obligatoire.
  * une icône - obligatoire - qui permet d’informer l’utilisateur qu’il s’agit d’une mise en avant de citation.
  * un texte pour l’auteur - optionnel - afin de préciser quand nécessaire l’auteur de la citation.
  * un texte pour les détails de la citation - optionnel - afin de préciser l’origine du texte cité.
  * image d’illustration - optionnelle. 
  * un séparateur - obligatoire - verticale en desktop, horizontal en mobile. 

La citation est disponible en deux variantes : avec illustration ou sans
illustration.

## Citation avec illustration

La citation avec illustration permet d'incarner l’auteur de la citation avec
une image.  

### Complète

> « Lorem [...] elit ut. »

Auteur

  * Ouvrage
  * Détail 1
  * Détail 2
  * Détail 3
  * Détail 4

![](/img/placeholder.1x1.png)

    
    
                    <figure class="fr-quote fr-quote--column">
        <blockquote cite="[À MODIFIER | https://lien-vers-la-source.fr || supprimer l'attribut si pas d'url pour la source']">
            <p>« Lorem [...] elit ut. »</p>
        </blockquote>
        <figcaption>
            <p class="fr-quote__author">Auteur</p>
            <ul class="fr-quote__source">
                <li>
                    <cite>Ouvrage</cite>
                </li>
                <li>Détail 1</li>
                <li>Détail 2</li>
                <li>Détail 3</li>
                <li>
                  <a target="_blank" rel="noopener external" title="[À MODIFIER - Intitulé] - nouvelle fenêtre" href="#[À MODIFIER | Lien vers la sources ou des infos complémentaires]">Détail 4</a>
                </li>
            </ul>
            <div class="fr-quote__image">
                <img src="/img/placeholder.1x1.png" class="fr-responsive-img" alt="" />
                <!-- L’alternative de l’image (attribut alt) doit rester vide car l’image est illustrative et ne doit pas être restituée aux technologies d’assistance -->
            </div>
        </figcaption>
    </figure>
                    
                  

### Sans auteur

> « Lorem [...] elit ut. »

  * Ouvrage
  * Détail 1
  * Détail 2
  * Détail 3
  * Détail 4

![](//img/placeholder.1x1.png)

    
    
                    <figure class="fr-quote fr-quote--column">
        <blockquote cite="[À MODIFIER | https://lien-vers-la-source.fr || supprimer l'attribut si pas d'url pour la source]">
            <p>« Lorem [...] elit ut. »</p>
        </blockquote>
        <figcaption>
            <ul class="fr-quote__source">
                <li>
                    <cite>Ouvrage</cite>
                </li>
                <li>Détail 1</li>
                <li>Détail 2</li>
                <li>Détail 3</li>
                <li>
                  <a target="_blank" rel="noopener external" title="[À MODIFIER - Intitulé] - nouvelle fenêtre" href="#[À MODIFIER | Lien vers la sources ou des infos complémentaires]">Détail 4</a>
                </li>
            </ul>
            <div class="fr-quote__image">
              <img src="//img/placeholder.1x1.png" class="fr-responsive-img" alt="" />
              <!-- L’alternative de l’image (attribut alt) doit rester vide car l’image est illustrative et ne doit pas être restituée aux technologies d’assistance -->
            </div>
        </figcaption>
    </figure>
                    
                  

### Sans détails

> « Lorem [...] elit ut. »

Auteur

![](/img/placeholder.1x1.png)

    
    
                    <figure class="fr-quote fr-quote--column">
        <blockquote cite="[À MODIFIER | https://lien-vers-la-source.fr || supprimer l'attribut si pas d'url pour la source]">
            <p>« Lorem [...] elit ut. »</p>
        </blockquote>
        <figcaption>
            <p class="fr-quote__author">Auteur</p>
            <div class="fr-quote__image">
                <img src="/img/placeholder.1x1.png" class="fr-responsive-img" alt="" />
                <!-- L’alternative de l’image (attribut alt) doit rester vide car l’image est illustrative et ne doit pas être restituée aux technologies d’assistance -->
            </div>
        </figcaption>
    </figure>
                    
                  

### Sans source

> « Lorem [...] elit ut. »

![](/img/placeholder.1x1.png)

    
    
                    <figure class="fr-quote fr-quote--column">
        <blockquote cite="[À MODIFIER | https://lien-vers-la-source.fr || supprimer l'attribut si pas d'url pour la source]">
            <p>« Lorem [...] elit ut. »</p>
        </blockquote>
        <figcaption>
            <div class="fr-quote__image">
                <img src="/img/placeholder.1x1.png" class="fr-responsive-img" alt="" />
                <!-- L’alternative de l’image (attribut alt) doit rester vide car l’image est illustrative et ne doit pas être restituée aux technologies d’assistance -->
            </div>
        </figcaption>
    </figure>
                    
                  

## Citation sans illustration

La citation sans illustration est à utiliser quand il n’est pas nécessaire ou
pas possible d’incarner l’auteur de la citation.

> « Lorem [...] elit ut. »

Auteur

  * Ouvrage
  * Détail 1
  * Détail 2
  * Détail 3
  * Détail 4

    
    
                    <figure class="fr-quote fr-quote--column">
        <blockquote cite="[À MODIFIER | https://lien-vers-la-source.fr || supprimer l'attribut si pas d'url pour la source]">
            <p>« Lorem [...] elit ut. »</p>
        </blockquote>
        <figcaption>
            <p class="fr-quote__author">Auteur</p>
            <ul class="fr-quote__source">
                <li>
                    <cite>Ouvrage</cite>
                </li>
                <li>Détail 1</li>
                <li>Détail 2</li>
                <li>Détail 3</li>
                <li>
                  <a target="_blank" rel="noopener external" title="[À MODIFIER - Intitulé] - nouvelle fenêtre" href="#[À MODIFIER | Lien vers la sources ou des infos complémentaires]" rel="noopener" >Détail 4</a>
                </li>
            </ul>
        </figcaption>
    </figure> 
                    
                  

La citation sans illustration se décline elle aussi sans auteur, sans citation
et sans source.

## Variante mobile

En mobile, le séparateur passe en dessous le texte de la source sur les deux
versions avec ou sans illustration.

![](/uploads/Capture_d_ecran_2021_06_23_a_15_34_55_5559411f8b.png)

Pour la citation avec illustration, l’image est affichée en dessous le texte
de la citation.

![](/uploads/Capture_d_ecran_2021_06_23_a_15_34_46_32b5154e09.png)

## Règles d’utilisation

  * Pour le texte de la citation, il faut intégrer au début et à la fin des guillemets avec des espaces insécables.
  * Pour la source, un ouvrage doit obligatoirement être en italique. 
  * Des champs détails non précisés sont prévus pour d’autres information, par exemple : édition, collection, date, ville, la fonction ou titre de l’auteur. Pour indiquer une URL dans ce champ, ajouter un soulignement pour en faire un lien.
  * Deux citations ne peuvent se suivre directement.

### Accessibilité/SEO

  * Lorsque la citation reprend un text d’un autre site, ajouter l’url de celui-ci en attribut cite=”” du <blockquote> afin d’indiquer au moteur de recherche la liaison. Ne mettez pas l’attribut si aucune url de ressource n’est disponible.
  * L’ouvrage cité doit être placé dans une balise <cite> et ainsi apparaitre en italique.
  * Le texte de la citation est contenu dans un <blockquote> inséré dans un bloc <figure> et les infos complémentaires (image, auteur, ouvrage... ) dans le <figcaption>.

### Contenus

  * Une citation n’est pas limité en nombre de caractère, tant qu’elle est correctement “sourcée”, il convient cependant de ne pas excéder une taille trop importante pour éviter que le bloc ne prenne trop de place, notamment en mobile.
  * Pour rappel, les citations courtes d’une oeuvre publiée sont autorisées et encadrées en France par le Code de la Propriété Intellectuelle et plus précisément l'[article L122-5](https://www.legifrance.gouv.fr/affichCodeArticle.do?cidTexte=LEGITEXT000006069414&idArticle=LEGIARTI000037388886&dateTexte=20191211).

## Personnalisation

Certains éléments du composant sont optionnels, voir sa structure.

### Taille de l'icone

La taille de l'icone est modifiable selon ces classes :  

Taille  
| Token  
| Dimension  
| Contexte d’utilisation  
  
---|---|---|---  
MD | $md | 16x16 px - 1 rem  
.fr-icon | Taille par défaut, aucun modifiers.  
À utiliser avec la typographie Extra Small (XS), Small (SM) et Medium (MD).  
LG | $lg | 24x24px - 1.5 rem  
.fr-icon--lg | À utiliser avec la typographie Large (LG).  
XL | $xl | 32x32px - 2 rem  
.fr-icon--xl | À utiliser pour les icônes sans texte, par exemple celles des
boutons icônes.  
  
### Couleurs d’accent

L'élément icône peut utiliser les couleurs illustratives :  

Élément  
| Valeur par défaut  
| Valeur(s) autorisée(s)  
| Classe css  
---|---|---|---  
Icône | **$artwork-minor-blue-france**  
Correspondances :  
Thème clair et sombre =  
$blue-france-main-525  
| $[couleur]-main (thèmes clair / sombre)  
exemples :  
$green-emeraude-main-632  
$brown-caramel-main-648  
  
  
| .fr-quote--[couleur]  
exemples :  
.fr-quote--green-emeraude  
.fr-quote--brown-caramel  
  
Exemple :  

![](/uploads/Capture_d_ecran_2021_11_17_a_13_05_01_40240f2566.png)

### Besoin d'aide ?

L'équipe du DSFR est là pour vous aider.

Retrouvez-la sur :

  * la communauté slack pour poser vos questions, et échanger avec d’autres utilisateurs.   
Vous êtes **agent de l’État** et souhaitez accéder au slack ? [Rejoignez la
communauté](https://gouvfr.atlassian.net/servicedesk/customer/portal/1/group/1/create/9
"Rejoignez la communauté - nouvelle fenêtre") dès maintenant !

  * [ le centre de support](https://gouvfr.atlassian.net/servicedesk/customer/portals "le centre de support - nouvelle fenêtre") pour envoyer vos demandes de correctifs et d'évolution.

[Champ de saisie - Input](/composants-et-modeles/composants/champ-de-saisie)

[Contenu médias - Content](/composants-et-modeles/composants/contenu-medias)

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
