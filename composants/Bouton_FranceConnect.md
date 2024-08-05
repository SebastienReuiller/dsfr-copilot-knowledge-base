Fermer

# Bouton FranceConnect

Le bouton FranceConnect permet à une administration (ou un fournisseur de
logiciel agissant pour le compte d’une administration) de proposer une
connexion ou une création de compte simplifiée.

L’utilisateur utilise ses identifiants de connexion d’un des fournisseurs
d’identités ([impots.gouv.fr](https://www.impots.gouv.fr/accueil
"impots.gouv.fr - nouvelle fenêtre"), [ameli.fr](https://www.ameli.fr/
"ameli.fr - nouvelle fenêtre"), [l’Identité Numérique La
Poste](https://lidentitenumerique.laposte.fr/ "l’Identité Numérique La Poste -
nouvelle fenêtre"), [MobileConnect et moi](https://www.mobileconnectetmoi.fr/
"MobileConnect et moi - nouvelle fenêtre") ou [msa.fr](https://www.msa.fr/lfp
"msa.fr - nouvelle fenêtre")), le fournisseur de service récupère auprès de
FranceConnect un identifiant unique et une identité vérifiée par l’INSEE.

Le fonctionnement en détail : [https://franceconnect.gouv.fr/partenaires
](https://franceconnect.gouv.fr/partenaires
"https://franceconnect.gouv.fr/partenaires  - nouvelle fenêtre")

Le bouton FranceConnect est primordial dans l’usage du service FranceConnect.
C’est par lui que passe la reconnaissance et la confiance dans la marque
FranceConnect.

## Structure

  * Bouton FranceConnect, composé de :
    * le fond bleu France - obligatoire
    * le logo FranceConnect - obligatoire
    * un libellé “S’identifier avec FranceConnect” - obligatoire
  * un lien “Qu’est-ce que FranceConnect ?” - obligatoire, qui redirige vers l’URL https://franceconnect.gouv.fr/   
  

S’identifier avec FranceConnect

[Qu’est-ce que FranceConnect ?](https://franceconnect.gouv.fr/ "Qu’est-ce que
FranceConnect ? - nouvelle fenêtre")

###  Extrait de code

    
    
                          <div class="fr-connect-group">
        <button class="fr-connect">
            <span class="fr-connect__login">S’identifier avec</span>
            <span class="fr-connect__brand">FranceConnect</span>
        </button>
        <p>
            <a href="https://franceconnect.gouv.fr/" target="_blank"  rel="noopener" title="Qu’est-ce que FranceConnect ? - nouvelle fenêtre">Qu’est-ce que FranceConnect ?</a>
        </p>
    </div>
                          
                        

**À ne pas faire - Changer la couleur du bouton**

![](/uploads/btn_couleurs_8467d8549c.jpg)

**À ne pas faire - Changer la typographie ou le libellé du bouton**

![](/uploads/btn_mauvais_texte_92106120e8.jpg)

## Variante

### FranceConnect+

Si le service utilise FranceConnect+ (pour les démarches nécessitant une
sécurité renforcée), il faut utiliser la variante FranceConnect+.

La structure est sensiblement la même que celle du bouton FranceConnect, le
lien pointe vers l’url <https://franceconnect.gouv.fr/france-connect-plus>.

S’identifier avec FranceConnect

[Qu’est-ce que FranceConnect+ ?](https://franceconnect.gouv.fr/france-connect-
plus "Qu’est-ce que FranceConnect+ ? - nouvelle fenêtre")

###  Extrait de code

    
    
                          <div class="fr-connect-group">
        <button class="fr-connect fr-connect--plus">
            <span class="fr-connect__login">S’identifier avec</span>
            <span class="fr-connect__brand">FranceConnect</span>
        </button>
        <p>
            <a href="https://franceconnect.gouv.fr/france-connect-plus" target="_blank"  rel="noopener" title="Qu’est-ce que FranceConnect+ ? - nouvelle fenêtre">Qu’est-ce que FranceConnect+ ?</a>
        </p>
    </div>
                          
                        

## Règles d’utilisation

### Usage

  * Il est situé en premier mode de connexion (au-dessus des autres moyens d'identification).
  * Il est accompagné du lien « Qu’est-ce que FranceConnect ? » positionné en dessous et redirige vers l’URL www.franceconnect.gouv.fr
  * Il est important de dissocier visuellement vos moyens de connexion natifs de FranceConnect, une séparation visible doit être mise en place.
  * La notion de "ou" doit également y figurer (FranceConnect ou un autre mode d’identification)

  * Pour plus de clarté, le bouton est accompagné de la phrase : « FranceConnect est la solution proposée par l’État pour sécuriser et simplifier la connexion à vos services en ligne ».
  * Merci de faire attention à l’écriture du terme « FranceConnect » et d’accoler les deux mots France et Connect partout où « FranceConnect » est mentionné.
  * FranceConnect n’est pas un réseau social et ne doit pas être présenté ou susceptible d’être perçu comme tel par l’utilisateur. Pour éviter toute confusion, FranceConnect ne doit pas figurer près de liens, d'icônes ou de services d'identification proposés par des réseaux sociaux et/ou autres services similaires.

### Comportement

Au clic sur le bouton, l'utilisateur est redirigé dans son onglet actif vers
la page de choix de fournisseur d’identité.

La page de choix de fournisseur d’identité ne doit pas s’ouvrir dans un modale
ou une pop-up au dessus du site.

À faire - Ouvrir la page de choix des fournisseurs d’identité dans l’onglet
actif

![](/uploads/lien_ok_7837c13427.jpg)

À ne pas faire - Proposer le choix de fournisseurs d’identité dans une modale

![](/uploads/lien_pas_ok_512e6500e1.jpg)

### Accessibilité

  * Le focus (propriété outline) ne doit être ni dégradé ni supprimé.

## Documentation technique

La documentation technique pour la mise en place de FranceConnect en tant que
fournisseur de service peut être consulter sur [le site de
FranceConnect](https://partenaires.franceconnect.gouv.fr/fcp/fournisseur-
service "le site de FranceConnect - nouvelle fenêtre")

[Groupe de boutons - Button group](/composants-et-modeles/composants/groupe-
de-boutons)

[Bouton radio - Radio](/composants-et-modeles/composants/bouton-radio)

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
