Fermer

# Bandeau d'information importante - Notice 🆕

Le bandeau d’information importante permet aux utilisateurs de voir ou
d’accéder à une information importante et temporaire. Il en existe trois
types, qui possèdent chacun leurs variations :

  * Les bandeaux génériques
  * Les bandeaux de vigilance météo
  * Les bandeaux d’alerte

Avant la version 1.12, seul le bandeau générique d’information importante bleu
était disponible. La version 1.12 apporte deux nouvelles variations ainsi que
les bandeaux de vigilance météorologique et d’alerte vitale dont les usages
sont strictement encadrés.

## Usage

Les bandeaux d’information importante doivent être utilisés uniquement pour
une information primordiale ou urgente et de façon temporaire. Leur usage est
encadré par des règles strictes, dont il n’est pas possible de s’affranchir :

  * Placés directement sous la navigation principale et visibles sur toutes les pages du site, quel que soit l’appareil utilisé, la vocation des bandeaux d’information importante est d’attirer l’attention des utilisateurs.
  * L’essentiel de l’information doit être contenue dans le bandeau. Il est toutefois possible d’ajouter un lien permettant de renvoyer l’utilisateur vers une source information complète.  

  * Ils ne sont pas conçus pour relayer une actualité et ne doivent pas se substituer aux pages d’actualité ou tout autre contenu informatif d’un site. Une utilisation excessive ou continue de ce type de bandeaux risquerait de rendre le composant invisible aux yeux des utilisateurs, en les habituant à sa présence.
  * L’état par défaut du bandeau (voir ci-dessous) répond à la plupart des cas d’usages. Tous les autres états sont à utiliser dans un cadre strictement exceptionnel, mettant en danger la sécurité des biens ou des personnes.

## Structure

![](/uploads/Bandeau_structure_png_02f36e0172.png)

  * 1 — Un fond - obligatoire et non-personnalisable
  * 2 — Une icône - optionnelle pour les bandeaux génériques, obligatoire et normée pour les bandeaux de vigilance météo et les bandeaux d’alertes
  * 3 — Un titre en gras - obligatoire, normé pour les bandeaux de vigilance météo et les bandeaux d’alertes.
  * 4 — Une description - optionnelle, texte personnalisable, recommandée pour apporter du contexte
  * 5 — Un lien - optionnel et personnalisable pour les bandeaux génériques, obligatoire et normé pour les bandeaux de vigilance météo et les bandeaux d’alertes
  * 6 — Une icône croix de fermeture - optionnelle

## Mise en situation

![](/uploads/bandeau_situation_png_69236bdffc.PNG)

## Variations

### Bandeaux génériques

#### Bandeau d'information importante - par défaut

Titre du bandeau assez long Texte de description plutot long lorem ipsum sit
consectetur adipiscing elit. Sed Lien de consultation

Masquer le message

###  Extrait de code

    
    
                          <div class="fr-notice fr-notice--info">
        <div class="fr-container">
            <div class="fr-notice__body">
                <p>
                    <span class="fr-notice__title">Titre du bandeau assez long</span>
                    <span class="fr-notice__desc">Texte de description plutot long lorem ipsum sit consectetur adipiscing elit. Sed</span>
                    <a target="_blank" rel="noopener external" title="[À MODIFIER - Intitulé] - nouvelle fenêtre" href="#" class="fr-notice__link">Lien de consultation</a>
                </p>
                <button title="Masquer le message" onclick="const notice = this.parentNode.parentNode.parentNode; notice.parentNode.removeChild(notice)" id="button-1299" class="fr-btn--close fr-btn">Masquer le message</button>
            </div>
        </div>
    </div>
                          
                        

**Quand l'utiliser ?**

  * Pour afficher une information exceptionnelle, mais non critique pour la santé ou la sécurité de l’utilisateur.
  * Ce bandeau répond à la plupart des cas d’usages.

**Quand ne pas l'utiliser ?**  

  * Pour mettre en avant une actualité classique ou une information secondaire en concernant pas directement l’utilisateur.

#### Bandeau d'avertissement

Titre du bandeau d'avertissement Texte de description lorem ipsum sit
consectetur adipiscing. Lien de consultation

Masquer le message

###  Extrait de code

    
    
                          <div class="fr-notice fr-notice--warning">
        <div class="fr-container">
            <div class="fr-notice__body">
                <p>
                    <span class="fr-notice__title">Titre du bandeau d'avertissement</span>
                    <span class="fr-notice__desc">Texte de description lorem ipsum sit consectetur adipiscing.</span>
                    <a target="_blank" rel="noopener external" title="[À MODIFIER - Intitulé] - nouvelle fenêtre" href="#" class="fr-notice__link">Lien de consultation</a>
                </p>
                <button title="Masquer le message" onclick="const notice = this.parentNode.parentNode.parentNode; notice.parentNode.removeChild(notice)" id="button-1305" class="fr-btn--close fr-btn">Masquer le message</button>
            </div>
        </div>
    </div>
                          
                        

**Quand l'utiliser ?**  

  * Pour afficher à l’utilisateur une information qui peut affecter son usage du service (indisponibilité majeure du site ou d’une démarche importante)
  * Pour avertir d’un risque de sécurité lié au site ou service (risque de phishing, usurpations etc.)

**Quand ne pas l'utiliser ?**  

  * Pour mettre en avant une actualité classique ou une information secondaire en concernant pas directement l’utilisateur.
  * Pour afficher une information exceptionnelle mais sans gravité pour l’utilisateur

#### Bandeau d'alerte

Titre du bandeau d'alerte Texte de description lorem ipsum sit consectetur
adipiscing. Lien de consultation

Masquer le message

###  Extrait de code

    
    
                          <div class="fr-notice fr-notice--alert">
        <div class="fr-container">
            <div class="fr-notice__body">
                <p>
                    <span class="fr-notice__title">Titre du bandeau d'alerte</span>
                    <span class="fr-notice__desc">Texte de description lorem ipsum sit consectetur adipiscing.</span>
                    <a target="_blank" rel="noopener external" title="[À MODIFIER - Intitulé] - nouvelle fenêtre" href="#" class="fr-notice__link">Lien de consultation</a>
                </p>
                <button title="Masquer le message" onclick="const notice = this.parentNode.parentNode.parentNode; notice.parentNode.removeChild(notice)" id="button-1308" class="fr-btn--close fr-btn">Masquer le message</button>
            </div>
        </div>
    </div>
                          
                        

**Quand l'utiliser ?**  

  * Pour afficher une information critique pour la santé ou la sécurité de l’utilisateur

**Quand ne pas l'utiliser ?**  

  * Pour mettre en avant une actualité classique ou une information secondaire en concernant pas directement l’utilisateur.
  * Pour afficher une information exceptionnelle mais sans gravité pour l’utilisateur
  * Pour afficher une information non urgente

### Bandeaux vigilance météo

Ces bandeaux servent à relayer des informations sur les niveaux de vigilance
et risques météorologiques communiqués par Météo France  

#### Comment les utiliser ?

Le Système de Design de l’État prévoit que ces bandeaux soient affichés à
partir du niveau de vigilance orange. Les niveaux de vigilance vert et jaune
ne justifiant pas d’afficher un bandeau d’information sur les sites de l’État.

Les niveaux de vigilance étant fixés à l’échelle départementale (sauf pour les
phénomènes d’avalanches et vagues-submersion, localisés plus précisément) les
bandeaux correspondants doivent être affichés de manière pertinente par
rapport à la localisation de l’utilisateur. On affichera donc ce type de
bandeau sur un site ciblant un département ou une région particulière, ou
lorsqu’on sera en mesure de localiser l’utilisateur.

Une couleur de bandeau violette est disponible et réservée à l’Outre-Mer : les
phénomènes météorologiques liés aux cyclones y font l’objet de dispositifs
d’alertes spécifiques à chaque territoire ou région, donnant lieu à une
couleur d’alerte violette figurant le niveau d’alerte maximale.

Les niveaux de vigilance étant revus quotidiennement par Météo France, on fera
en sorte de ne plus afficher ces bandeaux dès lors que le niveau de vigilance
revient à la normale.

#### Les trois niveaux de vigilance

#### Vigilance orange

Vigilance météo orange Texte de description lorem ipsum sit consectetur
adipiscing. Lien de consultation

Masquer le message

###  Extrait de code

    
    
                          <div class="fr-notice fr-notice--weather-orange">
        <div class="fr-container">
            <div class="fr-notice__body">
                <p>
                    <span class="fr-notice__title">Vigilance météo orange</span>
                    <span class="fr-notice__desc">Texte de description lorem ipsum sit consectetur adipiscing.</span>
                    <a target="_blank" rel="noopener external" title="[À MODIFIER - Intitulé] - nouvelle fenêtre" href="#" class="fr-notice__link">Lien de consultation</a>
                </p>
                <button title="Masquer le message" onclick="const notice = this.parentNode.parentNode.parentNode; notice.parentNode.removeChild(notice)" id="button-1311" class="fr-btn--close fr-btn">Masquer le message</button>
            </div>
        </div>
    </div>
                          
                        

Ce niveau est utilisé lorsque des phénomènes dangereux sont prévus. Son rôle
est d’inciter l’utilisateur à suivre l'évolution de la situation ainsi que les
conseils de sécurité émis par les pouvoirs publics.

#### Vigilance rouge

Vigilance météo rouge Texte de description lorem ipsum sit consectetur
adipiscing. Lien de consultation

Masquer le message

###  Extrait de code

    
    
                          <div class="fr-notice fr-notice--weather-red">
        <div class="fr-container">
            <div class="fr-notice__body">
                <p>
                    <span class="fr-notice__title">Vigilance météo rouge</span>
                    <span class="fr-notice__desc">Texte de description lorem ipsum sit consectetur adipiscing.</span>
                    <a target="_blank" rel="noopener external" title="[À MODIFIER - Intitulé] - nouvelle fenêtre" href="#" class="fr-notice__link">Lien de consultation</a>
                </p>
                <button title="Masquer le message" onclick="const notice = this.parentNode.parentNode.parentNode; notice.parentNode.removeChild(notice)" id="button-1314" class="fr-btn--close fr-btn">Masquer le message</button>
            </div>
        </div>
    </div>
                          
                        

Ce niveau est utilisé lorsque des phénomènes dangereux d'intensité
exceptionnelle sont prévus. Il doit inciter l’utilisateur à suivre la
situation et à respecter impérativement les consignes de sécurité émises par
les pouvoirs publics.

#### Vigilance violette

Vigilance météo violette Texte de description lorem ipsum sit consectetur
adipiscing. Lien de consultation

Masquer le message

###  Extrait de code

    
    
                          <div class="fr-notice fr-notice--weather-purple">
        <div class="fr-container">
            <div class="fr-notice__body">
                <p>
                    <span class="fr-notice__title">Vigilance météo violette</span>
                    <span class="fr-notice__desc">Texte de description lorem ipsum sit consectetur adipiscing.</span>
                    <a target="_blank" rel="noopener external" title="[À MODIFIER - Intitulé] - nouvelle fenêtre" href="#" class="fr-notice__link">Lien de consultation</a>
                </p>
                <button title="Masquer le message" onclick="const notice = this.parentNode.parentNode.parentNode; notice.parentNode.removeChild(notice)" id="button-1317" class="fr-btn--close fr-btn">Masquer le message</button>
            </div>
        </div>
    </div>
                          
                        

La vigilance violette ne fait pas partie du référentiel de niveaux de
vigilance Météo France, mais à un référentiel différent : celui de l’alerte
cyclonique, ce bandeau est réservé aux territoires ultra-marins.

**Les 8 phénomènes couverts par les bandeaux d’alerte**

Cette liste est encadrée par [une circulaire
interministérielle](https://www.legifrance.gouv.fr/download/pdf/circ?id=45225
"une circulaire interministérielle  - nouvelle fenêtre") dont les termes sont
précisément définis et associés à une icône précise :

Vent —

Orages —

Pluie-Inondation —

Vagues-submersion —

Grand froid —

Canicule —

Avalanches —

Neige-Verglas —

Quel que soit le niveau de vigilance, **le titre doit comporter le nom du
phénomène concerné en plus du niveau de vigilance** (ou le plus prégnant s’il
s’agit d’une combinaison de plusieurs phénomènes) et le texte d’accompagnement
du bandeau doit comporter :

  1. Une notion du département concerné ou du nombre de départements concernés pour les sites à portée nationale
  2. Le moment de la journée auquel elle s’applique (sans nécessairement détailler les heures, mais pour donner une idée de la temporalité).

### Bandeaux d’alerte :

Les bandeaux d’alerte sont conçus pour relayer des alertes relatifs aux
risques majeurs pour la nation, mettant en danger la sécurité des biens et des
personnes. Ils sont utilisables uniquement dans les cas précis pour lesquels
ils sont prévus.

#### Alerte attentat

Attentat en cours Texte de description lorem ipsum sit consectetur adipiscing.
Lien de consultation

Masquer le message

###  Extrait de code

    
    
                          <div class="fr-notice fr-notice--attack">
        <div class="fr-container">
            <div class="fr-notice__body">
                <p>
                    <span class="fr-notice__title">Attentat en cours</span>
                    <span class="fr-notice__desc">Texte de description lorem ipsum sit consectetur adipiscing.</span>
                    <a target="_blank" rel="noopener external" title="[À MODIFIER - Intitulé] - nouvelle fenêtre" href="#" class="fr-notice__link">Lien de consultation</a>
                </p>
                <button title="Masquer le message" onclick="const notice = this.parentNode.parentNode.parentNode; notice.parentNode.removeChild(notice)" id="button-1320" class="fr-btn--close fr-btn">Masquer le message</button>
            </div>
        </div>
    </div>
                          
                        

Ce bandeau ne doit être affiché qu’uniquement lorsqu'un attentat est en cours.
Cette information étant émise par le Ministère de l’Intérieur, les intitulés
officiels doivent être respectés.  
Attention à ne pas l’utiliser pour signifier un relèvement, un abaissement ou
le niveau en cours du plan Vigipirate : cela est une information et non une
alerte.

#### Appel à témoins

Appel à témoins Texte de description lorem ipsum sit consectetur adipiscing.
Lien de consultation

Masquer le message

###  Extrait de code

    
    
                          <div class="fr-notice fr-notice--witness">
        <div class="fr-container">
            <div class="fr-notice__body">
                <p>
                    <span class="fr-notice__title">Appel à témoins</span>
                    <span class="fr-notice__desc">Texte de description lorem ipsum sit consectetur adipiscing.</span>
                    <a target="_blank" rel="noopener external" title="[À MODIFIER - Intitulé] - nouvelle fenêtre" href="#" class="fr-notice__link">Lien de consultation</a>
                </p>
                <button title="Masquer le message" onclick="const notice = this.parentNode.parentNode.parentNode; notice.parentNode.removeChild(notice)" id="button-1323" class="fr-btn--close fr-btn">Masquer le message</button>
            </div>
        </div>
    </div>
                          
                        

Ce bandeau ne doit être affiché qu’uniquement lorsqu'un appel à témoins est
émis par le Ministère de l’Intérieur ou une préfecture. Les intitulés
officiels doivent être respectés.

#### Alerte technologique

Cyber-attaque Texte de description lorem ipsum sit consectetur adipiscing.
Lien de consultation

Masquer le message

###  Extrait de code

    
    
                          <div class="fr-notice fr-notice--cyberattack">
        <div class="fr-container">
            <div class="fr-notice__body">
                <p>
                    <span class="fr-notice__title">Cyber-attaque</span>
                    <span class="fr-notice__desc">Texte de description lorem ipsum sit consectetur adipiscing.</span>
                    <a target="_blank" rel="noopener external" title="[À MODIFIER - Intitulé] - nouvelle fenêtre" href="#" class="fr-notice__link">Lien de consultation</a>
                </p>
                <button title="Masquer le message" onclick="const notice = this.parentNode.parentNode.parentNode; notice.parentNode.removeChild(notice)" id="button-1326" class="fr-btn--close fr-btn">Masquer le message</button>
            </div>
        </div>
    </div>
                          
                        

Ce bandeau ne doit être affiché qu’uniquement en cas de cyber-attaque
d’ampleur nationale ou d’alerte technologique émise par le Ministère de
l’Intérieur. Les intitulés officiels doivent être respectés.

## Accessibilité

Ne pas sauter ce composant via les liens d'évitement (le bandeau doit être lu
quand l’utilisateur choisit “aller au contenu”)

Le titre est défini par la classe "fr-notice__title", la balise <p> peut être
remplacée par un niveau de titre hx suivant le contexte.

## Personnalisation

Le style de ce composant n’est pas personnalisable. Cependant, certains
éléments sont facultatifs (voir la structure du composant).

[Badge - Badge](/composants-et-modeles/composants/badge)

[Barre de recherche - Search](/composants-et-modeles/composants/barre-de-
recherche)

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
