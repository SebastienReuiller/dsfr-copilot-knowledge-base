Fermer

#  Lettre d'information et réseaux sociaux - Newsletter and follow us

Ces composants permettent à l’utilisateur d’avoir accès à des services
complémentaire du site : l’inscription à (aux) lettre(s) d’information
proposée(s), ainsi que des liens vers les comptes de réseaux sociaux de
l’entité.

Ces deux composants s’affichent l’un à coté de l’autre dans le cas ou les deux
‘services’ sont proposés , ou bien seuls si l’entité ne propose qu’une
possibilité.

Ils précèdent immédiatement le footer.

## Mise en avant des réseaux sociaux (RS)

Ce composant permet à l’utilisateur d’accéder aux réseaux sociaux de
l’organisation.

  * un texte : « Suivez-nous sur les réseaux sociaux : » 
  * des pictos réseau sociaux : chaque picto est cliquable et renvoie vers la page du réseau social en question

## Suivez-nous  
sur les réseaux sociaux

  * facebook 
  * X (anciennement Twitter) 
  * instagram 
  * linkedin 
  * youtube 

###  Extrait de code

    
    
                          <div class="fr-follow">
        <div class="fr-container">
            <div class="fr-grid-row">
                <div class="fr-col-12">
                    <div class="fr-follow__social">
                        <h2 class="fr-h5">Suivez-nous
                            <br> sur les réseaux sociaux
                        </h2>
                        <ul class="fr-btns-group">
                            <li>
                                <a class="fr-btn--facebook fr-btn" href="#[À MODIFIER - Lien vers le facebook de l'organisation]" target="_blank" title="[À MODIFIER - Intitulé] - nouvelle fenêtre" rel="noopener external">
                                    facebook
                                </a>
                            </li>
                            <li>
                                <a class="fr-btn--twitter-x fr-btn" href="#[À MODIFIER - Lien vers le twitter de l'organisation]" target="_blank" title="[À MODIFIER - Intitulé] - nouvelle fenêtre" rel="noopener external">
                                    X (anciennement Twitter)
                                </a>
                            </li>
                            <li>
                                <a class="fr-btn--instagram fr-btn" href="#[À MODIFIER - Lien vers l'instagram de l'organisation]" target="_blank" title="[À MODIFIER - Intitulé] - nouvelle fenêtre" rel="noopener external">
                                    instagram
                                </a>
                            </li>
                            <li>
                                <a class="fr-btn--linkedin fr-btn" href="#[À MODIFIER - Lien vers le linkedin de l'organisation]" target="_blank" title="[À MODIFIER - Intitulé] - nouvelle fenêtre" rel="noopener external">
                                    linkedin
                                </a>
                            </li>
                            <li>
                                <a class="fr-btn--youtube fr-btn" href="#[À MODIFIER - Lien vers le youtube de l'organisation]" target="_blank" title="[À MODIFIER - Intitulé] - nouvelle fenêtre" rel="noopener external">
                                    youtube
                                </a>
                            </li>
                        </ul>
                    </div>
                </div>
            </div>
        </div>
    </div>
                          
                        

## Lettre d’information

Ce composant à l’utilisateur de s’inscrire à la newsletter de l’organisation.

Ce composant est proposé selon deux variantes :

  * une première variante qui propose un pied de page intégrant directement le champ de saisie de l’email
  * une seconde variante qui est une simple zone de mise en avant de la newsletter avec un call to action redirigeant vers un formulaire d’inscription plus riche. 

### Formulaire d’inscription à la newsletter

A utiliser pour les newsletters simples avec nécessité de recueillir
uniquement l’adresse mail et le consentement de l’utilisateur.

Le texte de description qui accompagne le titre du bloc sert à présenter la
Newsletter.

Les mentions pour obtenir le consentement et les indications pour la
désinscription sont à adaptés en fonction des cas de figure.

## Abonnez-vous à notre lettre d’information

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Maecenas varius
tortor nibh, sit amet tempor nibh finibus et.

Votre adresse électronique (ex. : nom@domaine.fr)

S'abonner

En renseignant votre adresse électronique, vous acceptez de recevoir nos
actualités par courriel. Vous pouvez vous désinscrire à tout moment à l’aide
des liens de désinscription ou en nous contactant.

###  Extrait de code

    
    
                          <div class="fr-follow">
        <div class="fr-container">
            <div class="fr-grid-row">
                <div class="fr-col-12">
                    <div class="fr-follow__newsletter">
                        <div>
                            <h2 class="fr-h5">Abonnez-vous à notre lettre d’information</h2>
                            <p class="fr-text--sm">Lorem ipsum dolor sit amet, consectetur adipiscing elit. Maecenas varius tortor nibh, sit amet tempor nibh finibus et.</p>
                        </div>
                        <div>
                            <form action="">
                                <div class="fr-input-group">
                                    <label class="fr-label" for="newsletter-email">
                                        Votre adresse électronique (ex. : nom@domaine.fr)
                                    </label>
                                    <div class="fr-input-wrap fr-input-wrap--addon">
                                        <input class="fr-input" title="Votre adresse électronique (ex. : nom@domaine.fr)" autocomplete="email" attributes="[object Object]" aria-describedby="newsletter-email-hint-text newsletter-email-messages" placeholder="Votre adresse électronique (ex. : nom@domaine.fr)" id="newsletter-email" type="email">
                                        <button class="fr-btn" id="newsletter-button" title="S‘abonner à notre lettre d’information" type="submit">
                                            S'abonner
                                        </button>
                                    </div>
                                    <div class="fr-messages-group" id="newsletter-email-messages" aria-live="assertive">
                                    </div>
                                </div>
                                <p id="newsletter-email-hint-text" class="fr-hint-text">En renseignant votre adresse électronique, vous acceptez de recevoir nos actualités par courriel. Vous pouvez vous désinscrire à tout moment à l’aide des liens de désinscription ou en nous contactant.</p>
                            </form>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
                          
                        

La gestion des messages d'erreurs lors de la soumission se fait avec l'état
“erreur” du champ de saisie.

## Abonnez-vous à notre lettre d’information

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Maecenas varius
tortor nibh, sit amet tempor nibh finibus et.

Votre adresse électronique (ex. : nom@domaine.fr)

S'abonner

Le format de l’adresse electronique saisie n’est pas valide. Le format attendu
est : nom@exemple.org

En renseignant votre adresse électronique, vous acceptez de recevoir nos
actualités par courriel. Vous pouvez vous désinscrire à tout moment à l’aide
des liens de désinscription ou en nous contactant.

## Suivez-nous  
sur les réseaux sociaux

  * facebook 
  * X (anciennement Twitter) 
  * instagram 
  * linkedin 
  * youtube 

###  Extrait de code

    
    
                          <div class="fr-follow">
        <div class="fr-container">
            <div class="fr-grid-row">
                <div class="fr-col-12 fr-col-md-8">
                    <div class="fr-follow__newsletter">
                        <div>
                            <h2 class="fr-h5">Abonnez-vous à notre lettre d’information</h2>
                            <p class="fr-text--sm">Lorem ipsum dolor sit amet, consectetur adipiscing elit. Maecenas varius tortor nibh, sit amet tempor nibh finibus et.</p>
                        </div>
                        <div>
                            <form action="">
                                <div class="fr-input-group fr-input-group--error">
                                    <label class="fr-label" for="newsletter-email">
                                        Votre adresse électronique (ex. : nom@domaine.fr)
                                    </label>
                                    <div class="fr-input-wrap fr-input-wrap--addon">
                                        <input class="fr-input" title="Votre adresse électronique (ex. : nom@domaine.fr)" autocomplete="email" aria-describedby="newsletter-email-hint-text newsletter-email-messages" placeholder="Votre adresse électronique (ex. : nom@domaine.fr)" id="newsletter-email" type="email">
                                        <button class="fr-btn" id="newsletter-button" title="S‘abonner à notre lettre d’information" type="submit">
                                            S'abonner
                                        </button>
                                    </div>
                                    <div class="fr-messages-group" id="newsletter-email-messages" aria-live="assertive">
                                        <p class="fr-message fr-message--error" id="newsletter-email-message-error">Le format de l’adresse electronique saisie n’est pas valide. Le format attendu est : nom@exemple.org</p>
                                    </div>
                                </div>
                                <p id="newsletter-email-hint-text" class="fr-hint-text">En renseignant votre adresse électronique, vous acceptez de recevoir nos actualités par courriel. Vous pouvez vous désinscrire à tout moment à l’aide des liens de désinscription ou en nous contactant.</p>
                            </form>
                        </div>
                    </div>
                </div>
                <div class="fr-col-12 fr-col-md-4">
                    <div class="fr-follow__social">
                        <h2 class="fr-h5">Suivez-nous
                            <br> sur les réseaux sociaux
                        </h2>
                        <ul class="fr-btns-group">
                            <li>
                                <a class="fr-btn--facebook fr-btn" href="#[À MODIFIER - Lien vers le facebook de l'organisation]" target="_blank" title="[À MODIFIER - Intitulé] - nouvelle fenêtre" rel="noopener external">
                                    facebook
                                </a>
                            </li>
                            <li>
                                <a class="fr-btn--twitter-x fr-btn" href="#[À MODIFIER - Lien vers le twitter de l'organisation]" target="_blank" title="[À MODIFIER - Intitulé] - nouvelle fenêtre" rel="noopener external">
                                    X (anciennement Twitter)
                                </a>
                            </li>
                            <li>
                                <a class="fr-btn--instagram fr-btn" href="#[À MODIFIER - Lien vers l'instagram de l'organisation]" target="_blank" title="[À MODIFIER - Intitulé] - nouvelle fenêtre" rel="noopener external">
                                    instagram
                                </a>
                            </li>
                            <li>
                                <a class="fr-btn--linkedin fr-btn" href="#[À MODIFIER - Lien vers le linkedin de l'organisation]" target="_blank" title="[À MODIFIER - Intitulé] - nouvelle fenêtre" rel="noopener external">
                                    linkedin
                                </a>
                            </li>
                            <li>
                                <a class="fr-btn--youtube fr-btn" href="#[À MODIFIER - Lien vers le youtube de l'organisation]" target="_blank" title="[À MODIFIER - Intitulé] - nouvelle fenêtre" rel="noopener external">
                                    youtube
                                </a>
                            </li>
                        </ul>
                    </div>
                </div>
            </div>
        </div>
    </div>
                          
                        

Cette variante peut également servir à pré-saisir l’adresse mail de
l’utilisateur pour ensuite renvoyer vers une page de formulaire plus
détaillée.  

### Mise en avant de la lettre d’information

A utiliser pour les newsletters plus complexes avec nécessité de recueillir
plusieurs informations.

Le texte de description qui accompagne le titre du bloc sert à présenter la
Newsletter, et le bouton redirige vers la page d’inscription

## Abonnez-vous à notre lettre d’information

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Maecenas varius
tortor nibh, sit amet tempor nibh finibus et.

S'abonner

###  Extrait de code

    
    
                          <div class="fr-follow">
        <div class="fr-container">
            <div class="fr-grid-row">
                <div class="fr-col-12">
                    <div class="fr-follow__newsletter">
                        <div>
                            <h2 class="fr-h5">Abonnez-vous à notre lettre d’information</h2>
                            <p class="fr-text--sm">Lorem ipsum dolor sit amet, consectetur adipiscing elit. Maecenas varius tortor nibh, sit amet tempor nibh finibus et.</p>
                        </div>
                        <div class="fr-btns-group fr-btns-group--inline-md">
                            <button class="fr-btn" title="S‘abonner à notre lettre d’information">
                                S'abonner
                            </button>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
                          
                        

## Lettre d’information et réseaux sociaux

Si les deux éléments sont proposés, il doivent s’afficher l’un à coté de
l’autre. Il est possible d’utiliser les différentes déclinaisons de la lettre
d’information (formulaire ou mise en avant).

Formulaire d’inscription à la lettre d’information et Réseaux sociaux

## Abonnez-vous à notre lettre d’information

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Maecenas varius
tortor nibh, sit amet tempor nibh finibus et.

Votre adresse électronique (ex. : nom@domaine.fr)

S'abonner

En renseignant votre adresse électronique, vous acceptez de recevoir nos
actualités par courriel. Vous pouvez vous désinscrire à tout moment à l’aide
des liens de désinscription ou en nous contactant.

## Suivez-nous  
sur les réseaux sociaux

  * facebook 
  * X (anciennement Twitter) 
  * instagram 
  * linkedin 
  * youtube 

###  Extrait de code

    
    
                          <div class="fr-follow">
        <div class="fr-container">
            <div class="fr-grid-row">
                <div class="fr-col-12 fr-col-md-8">
                    <div class="fr-follow__newsletter">
                        <div>
                            <h2 class="fr-h5">Abonnez-vous à notre lettre d’information</h2>
                            <p class="fr-text--sm">Lorem ipsum dolor sit amet, consectetur adipiscing elit. Maecenas varius tortor nibh, sit amet tempor nibh finibus et.</p>
                        </div>
                        <div>
                            <form action="">
                                <div class="fr-input-group">
                                    <label class="fr-label" for="newsletter-email">
                                        Votre adresse électronique (ex. : nom@domaine.fr)
                                    </label>
                                    <div class="fr-input-wrap fr-input-wrap--addon">
                                        <input class="fr-input" title="Votre adresse électronique (ex. : nom@domaine.fr)" autocomplete="email" aria-describedby="newsletter-email-hint-text newsletter-email-messages" placeholder="Votre adresse électronique (ex. : nom@domaine.fr)" id="newsletter-email" type="email">
                                        <button class="fr-btn" id="newsletter-button" title="S‘abonner à notre lettre d’information" type="submit">
                                            S'abonner
                                        </button>
                                    </div>
                                    <div class="fr-messages-group" id="newsletter-email-messages" aria-live="assertive">
                                    </div>
                                </div>
                                <p id="newsletter-email-hint-text" class="fr-hint-text">En renseignant votre adresse électronique, vous acceptez de recevoir nos actualités par courriel. Vous pouvez vous désinscrire à tout moment à l’aide des liens de désinscription ou en nous contactant.</p>
                            </form>
                        </div>
                    </div>
                </div>
                <div class="fr-col-12 fr-col-md-4">
                    <div class="fr-follow__social">
                        <h2 class="fr-h5">Suivez-nous
                            <br> sur les réseaux sociaux
                        </h2>
                        <ul class="fr-btns-group">
                            <li>
                                <a class="fr-btn--facebook fr-btn" href="#[À MODIFIER - Lien vers le facebook de l'organisation]" target="_blank" title="[À MODIFIER - Intitulé] - nouvelle fenêtre" rel="noopener external">
                                    facebook
                                </a>
                            </li>
                            <li>
                                <a class="fr-btn--twitter-x fr-btn" href="#[À MODIFIER - Lien vers le twitter de l'organisation]" target="_blank" title="[À MODIFIER - Intitulé] - nouvelle fenêtre" rel="noopener external">
                                    X (anciennement Twitter)
                                </a>
                            </li>
                            <li>
                                <a class="fr-btn--instagram fr-btn" href="#[À MODIFIER - Lien vers l'instagram de l'organisation]" target="_blank" title="[À MODIFIER - Intitulé] - nouvelle fenêtre" rel="noopener external">
                                    instagram
                                </a>
                            </li>
                            <li>
                                <a class="fr-btn--linkedin fr-btn" href="#[À MODIFIER - Lien vers le linkedin de l'organisation]" target="_blank" title="[À MODIFIER - Intitulé] - nouvelle fenêtre" rel="noopener external">
                                    linkedin
                                </a>
                            </li>
                            <li>
                                <a class="fr-btn--youtube fr-btn" href="#[À MODIFIER - Lien vers le youtube de l'organisation]" target="_blank" title="[À MODIFIER - Intitulé] - nouvelle fenêtre" rel="noopener external">
                                    youtube
                                </a>
                            </li>
                        </ul>
                    </div>
                </div>
            </div>
        </div>
    </div>
                          
                        

Mise en avant de la lettre d’information et réseaux sociaux

Abonnez-vous à notre lettre d’information

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Maecenas varius
tortor nibh, sit amet tempor nibh finibus et.

S'abonner

Suivez-nous  
sur les réseaux sociaux

  * facebook 
  * X (anciennement Twitter) 
  * instagram 
  * linkedin 
  * youtube 

###  Extrait de code

    
    
                          <div class="fr-follow">
        <div class="fr-container">
            <div class="fr-grid-row">
                <div class="fr-col-12 fr-col-md-8">
                    <div class="fr-follow__newsletter">
                        <div>
                            <p class="fr-h5">Abonnez-vous à notre lettre d’information</p>
                            <p class="fr-text--sm">Lorem ipsum dolor sit amet, consectetur adipiscing elit. Maecenas varius tortor nibh, sit amet tempor nibh finibus et.</p>
                        </div>
                        <div class="fr-btns-group fr-btns-group--inline-md">
                            <button class="fr-btn" title="S‘abonner à notre lettre d’information">
                                S'abonner
                            </button>
                        </div>
                    </div>
                </div>
                <div class="fr-col-12 fr-col-md-4">
                    <div class="fr-follow__social">
                        <p class="fr-h5">Suivez-nous
                            <br> sur les réseaux sociaux
                        </p>
                        <ul class="fr-btns-group">
                            <li>
                                <a class="fr-btn--facebook fr-btn" title="[À MODIFIER - Intitulé] - nouvelle fenêtre" rel="noopener external" href="#[À MODIFIER - Lien vers le facebook de l'organisation]" target="_blank">
                                    facebook
                                </a>
                            </li>
                            <li>
                                <a class="fr-btn--twitter-x fr-btn" title="[À MODIFIER - Intitulé] - nouvelle fenêtre" rel="noopener external" href="#[À MODIFIER - Lien vers le twitter de l'organisation]" target="_blank">
                                    X (anciennement Twitter)
                                </a>
                            </li>
                            <li>
                                <a class="fr-btn--instagram fr-btn" title="[À MODIFIER - Intitulé] - nouvelle fenêtre" rel="noopener external" href="#[À MODIFIER - Lien vers l'instagram de l'organisation]" target="_blank">
                                    instagram
                                </a>
                            </li>
                            <li>
                                <a class="fr-btn--linkedin fr-btn" title="[À MODIFIER - Intitulé] - nouvelle fenêtre" rel="noopener external" href="#[À MODIFIER - Lien vers le linkedin de l'organisation]" target="_blank">
                                    linkedin
                                </a>
                            </li>
                            <li>
                                <a class="fr-btn--youtube fr-btn" title="[À MODIFIER - Intitulé] - nouvelle fenêtre" rel="noopener external" href="#[À MODIFIER - Lien vers le youtube de l'organisation]" target="_blank">
                                    youtube
                                </a>
                            </li>
                        </ul>
                    </div>
                </div>
            </div>
        </div>
    </div>
                          
                        

## Règles d’utilisation

### Usage

Le ou les composants sont présents sur l’ensemble des pages du site, juste au
dessus du footer.  

### Accessibilité

#### Formulaire d’inscription

Idéalement, un élément <label> explicite doit précéder le champ <input>.
Cependant, il est possible s’en passer dans ce cas en respectant les règles
suivantes :

  * L’attribut placeholder contient un exemple de format attendu placeholder="exemple : [nom@exemple.fr](mailto:nom@exemple.fr)"
  * Si le <label> est présent et masqué (ce qui est le cas ici), il faut ajouter un attribut title à l'<input> (nul besoin de aria-label).Si , pour quelques raisons, il ne peut y avoir de <label> , alors on ajoute un attribut title ET un attribut aria-label (ces 2 attributs doivent être strictement identiques). Exemple : 

    
    
    <input type="email" placeholder="exemple : nom@exemple.fr"
    title="Saisissez votre adresse électronique (exemple : nom@exemple.fr)"  
    aria-label="Saisissez votre adresse électronique (exemple : nom@exemple.fr)">

#### Liens Réseaux sociaux

  * Pour rendre accessibles les liens réseaux sociaux, il suffit de renseigner l’attribut title du lien de façon à ce qu’il indique explicitement sa fonction. 

Exemple :

    
    
    <a class="fr-btn--twitter-x fr-btn" target="_blank" rel="noopener external"
    title="X - nouvelle fenêtre" 
    href="#" >X (anciennement Twitter)</a>

### Contenu

  * Le titre et le texte d’explication est adapté en fonction du contexte. Il s’agit ici de présenter la lettre d’information et la nature des contenus qu’elle traite.
  * Le texte de description “rgpd” sur l’utilisation des données personnels sont à adapter en fonction de la politique de l’organisation. 

### Besoin d'aide ?

L'équipe du DSFR est là pour vous aider.

Retrouvez-la sur :

  * [la communauté slack](https://gouvfr.slack.com/ "la communauté slack - nouvelle fenêtre") pour poser vos questions, et échanger avec d’autres utilisateurs.   
Vous êtes **agent de l’État** et souhaitez accéder au slack ? [Rejoignez la
communauté](https://gouvfr.atlassian.net/servicedesk/customer/portal/1/group/1/create/9
"Rejoignez la communauté - nouvelle fenêtre") dès maintenant !

  * [ le centre de support](https://gouvfr.atlassian.net/servicedesk/customer/portals "le centre de support - nouvelle fenêtre") pour envoyer vos demandes de correctifs et d'évolution.

[Interrupteur - Toggle](/composants-et-modeles/composants/interrupteur)

[Lien - Link](/composants-et-modeles/composants/lien)

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
