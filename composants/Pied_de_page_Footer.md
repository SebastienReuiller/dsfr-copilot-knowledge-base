Fermer

# Pied de page - Footer

Le pied de page propose des éléments d’information sur le site et une
navigation secondaire pour l’utilisateur afin qu’il poursuive son parcours. Il
est modulable selon les besoins et les exigences du site.

## Pied de page simple

Le pied de page simple est le cas minimal mis à disposition par le DSFR. Il
est sur fond blanc en thème claire et sur fond G800 en thème sombre.

### Structure

Il se compose des éléments suivants:

  * un bloc marque, voir la [charte de marque](https://www.gouvernement.fr/marque-Etat)  

  * un texte de présentation - optionnel.  

  * 4 liens de références de l'écosystème institutionnel - obligatoires.  

  * la liste de liens liés aux obligations légales. Cette liste doit être définie en fonction du site, toutefois les liens & contenus suivants sont obligatoires : “accessibilité : non/partiellement/totalement conforme”, mentions légales, données personnelles et gestion des cookies. - obligatoire.  

  * une mention de la licence - obligatoire  
“Sauf mention contraire, tous les contenus de ce site sont sous licence
etalab-2.0”  

![](/uploads/pied_de_page_simple_png_0bcc71e23a.png)

###  Extrait de code

    
    
    <footer class="fr-footer" role="contentinfo" id="footer-7361">
        <div class="fr-container">
            <div class="fr-footer__body">
                <div class="fr-footer__brand fr-enlarge-link">
                    <a href="/" title="Retour à l'accueil du site - Nom de l'entité (ministère, secrétariat d'état, gouvernement)">
                        <p class="fr-logo">
                            Intitulé
                            <br>officiel
                        </p>
                    </a>
                </div>
                <div class="fr-footer__content">
                    <p class="fr-footer__content-desc">Lorem ipsum dolor sit amet, consectetur adipiscing, incididunt, ut labore et dolore magna aliqua. Vitae sapien pellentesque habitant morbi tristique senectus et. Diam maecenas sed enim ut. Accumsan lacus vel facilisis volutpat est. Ut aliqu</p>
                    <ul class="fr-footer__content-list">
                        <li class="fr-footer__content-item">
                            <a class="fr-footer__content-link" target="_blank" rel="noopener external" title="info.gouv.fr - nouvelle fenêtre" href="https://info.gouv.fr">info.gouv.fr</a>
                        </li>
                        <li class="fr-footer__content-item">
                            <a class="fr-footer__content-link" target="_blank" rel="noopener external" title="service-public.fr - nouvelle fenêtre" href="https://service-public.fr">service-public.fr</a>
                        </li>
                        <li class="fr-footer__content-item">
                            <a class="fr-footer__content-link" target="_blank" rel="noopener external" title="legifrance.gouv.fr - nouvelle fenêtre" href="https://legifrance.gouv.fr">legifrance.gouv.fr</a>
                        </li>
                        <li class="fr-footer__content-item">
                            <a class="fr-footer__content-link" target="_blank" rel="noopener external" title="data.gouv.fr - nouvelle fenêtre" href="https://data.gouv.fr">data.gouv.fr</a>
                        </li>
                    </ul>
                </div>
            </div>
            <div class="fr-footer__bottom">
                <ul class="fr-footer__bottom-list">
                    <li class="fr-footer__bottom-item">
                        <a class="fr-footer__bottom-link" href="#">Plan du site</a>
                    </li>
                    <li class="fr-footer__bottom-item">
                        <a class="fr-footer__bottom-link" href="#">Accessibilité : non/partiellement/totalement conforme</a>
                    </li>
                    <li class="fr-footer__bottom-item">
                        <a class="fr-footer__bottom-link" href="#">Mentions légales</a>
                    </li>
                    <li class="fr-footer__bottom-item">
                        <a class="fr-footer__bottom-link" href="#">Données personnelles</a>
                    </li>
                    <li class="fr-footer__bottom-item">
                        <a class="fr-footer__bottom-link" href="#">Gestion des cookies</a>
                    </li>
                </ul>
                <div class="fr-footer__bottom-copy">
                  <p>Sauf mention explicite de propriété intellectuelle détenue par des tiers, les contenus de ce site sont proposés sous <a href="https://github.com/etalab/licence-ouverte/blob/master/LO.md" target="_blank" rel="noopener external" title="Licence etalab - nouvelle fenêtre">licence etalab-2.0</a>
                  </p>
                </div>
            </div>
        </div>
    </footer>

## Pied de page avec logo opérateur

![](/uploads/pied_de_page_operateur_8a4a4cbec4.png)

**Pour les développeurs** : L’alternative textuelle du logo (attribut alt)
doit impérativement contenir le texte présent dans l’image!

###  Extrait de code

    
    
    <footer class="fr-footer" role="contentinfo" id="footer-7475">
        <div class="fr-container">
            <div class="fr-footer__body">
                <div class="fr-footer__brand fr-enlarge-link">
                    <p class="fr-logo">
                        République
                        <br>Française
                    </p>
                    <a class="fr-footer__brand-link" href="/" title="Retour à l'accueil du site - [À MODIFIER - texte alternatif de l'image : nom de l'opérateur ou du site serviciel] - République Française">
                        <img class="fr-footer__logo" style="width:3.5rem;" src="/example/img/placeholder.9x16.png" alt="[À MODIFIER - texte alternatif de l'image]" />
                        <!-- L'alternative de l'image (attribut alt) doit impérativement être renseignée et reprendre le texte visible dans l'image -->
                    </a>
                </div>
                <div class="fr-footer__content">
                    <p class="fr-footer__content-desc">Lorem [...] elit ut.</p>
                    <ul class="fr-footer__content-list">
                        <li class="fr-footer__content-item">
                            <a target="_blank" rel="noopener external" title="info.gouv.fr - nouvelle fenêtre" id="footer__content-link-7362" class="fr-footer__content-link" href="https://info.gouv.fr">info.gouv.fr</a>
                        </li>
                        <li class="fr-footer__content-item">
                            <a target="_blank" rel="noopener external" title="service-public.fr - nouvelle fenêtre" id="footer__content-link-7363" class="fr-footer__content-link" href="https://service-public.fr">service-public.fr</a>
                        </li>
                        <li class="fr-footer__content-item">
                            <a target="_blank" rel="noopener external" title="legifrance.gouv.fr - nouvelle fenêtre" id="footer__content-link-7364" class="fr-footer__content-link" href="https://legifrance.gouv.fr">legifrance.gouv.fr</a>
                        </li>
                        <li class="fr-footer__content-item">
                            <a target="_blank" rel="noopener external" title="data.gouv.fr - nouvelle fenêtre" id="footer__content-link-7365" class="fr-footer__content-link" href="https://data.gouv.fr">data.gouv.fr</a>
                        </li>
                    </ul>
                </div>
            </div>
            <div class="fr-footer__bottom">
                <ul class="fr-footer__bottom-list">
                    <li class="fr-footer__bottom-item">
                        <a class="fr-footer__bottom-link" href="#">Plan du site</a>
                    </li>
                    <li class="fr-footer__bottom-item">
                        <a class="fr-footer__bottom-link" href="#">Accessibilité : non/partiellement/totalement conforme</a>
                    </li>
                    <li class="fr-footer__bottom-item">
                        <a class="fr-footer__bottom-link" href="#">Mentions légales</a>
                    </li>
                    <li class="fr-footer__bottom-item">
                        <a class="fr-footer__bottom-link" href="#">Données personnelles</a>
                    </li>
                    <li class="fr-footer__bottom-item">
                        <a class="fr-footer__bottom-link" href="#">Gestion des cookies</a>
                    </li>
                </ul>
                <div class="fr-footer__bottom-copy">
                    <p>Sauf mention explicite de propriété intellectuelle détenue par des tiers, les contenus de ce site sont proposés sous <a href="https://github.com/etalab/licence-ouverte/blob/master/LO.md" target="_blank" rel="noopener external" title="Licence etalab - nouvelle fenêtre">licence etalab-2.0</a>
                    </p>
                </div>
            </div>
        </div>
    </footer>
    
    
    Notez quelque chose
    :cloche:

## Pied de page complet

Le pied de page complet reprend les éléments du pied de page simple et intègre
au-dessus une section présentant des listes de liens.

Il est recommandé de choisir le pied de page complet pour les sites profonds
nécessitant de réintégrer des listes de liens en rebond de la navigation.

Il se compose des éléments suivants:

  * Le pied de page simple (voir la structure ci-dessus) - obligatoire
  * une liste de liens - obligatoire  

![](/uploads/pied_de_page_complet_9409bbc7f6.png)

###  Extrait de code

    
    
    <footer class="fr-footer" role="contentinfo" id="footer-7617">
        <div class="fr-footer__top">
            <div class="fr-container">
                <div class="fr-grid-row fr-grid-row--start fr-grid-row--gutters">
                    <div class="fr-col-12 fr-col-sm-3 fr-col-md-2">
                        <h3 class="fr-footer__top-cat">Nom de la catégorie</h3>
                        <ul class="fr-footer__top-list">
                            <li>
                                <a class="fr-footer__top-link" href="#">Lien de navigation</a>
                            </li>
                            <li>
                                <a class="fr-footer__top-link" href="#">Lien de navigation</a>
                            </li>
                            <li>
                                <a class="fr-footer__top-link" href="#">Lien de navigation</a>
                            </li>
                            <li>
                                <a class="fr-footer__top-link" href="#">Lien de navigation</a>
                            </li>
                            <li>
                                <a class="fr-footer__top-link" href="#">Lien de navigation</a>
                            </li>
                            <li>
                                <a class="fr-footer__top-link" href="#">Lien de navigation</a>
                            </li>
                        </ul>
                    </div>
                    <div class="fr-col-12 fr-col-sm-3 fr-col-md-2">
                        <h3 class="fr-footer__top-cat">Nom de la catégorie</h3>
                        <ul class="fr-footer__top-list">
                            <li>
                                <a class="fr-footer__top-link" href="#">Lien de navigation</a>
                            </li>
                            <li>
                                <a class="fr-footer__top-link" href="#">Lien de navigation</a>
                            </li>
                            <li>
                                <a class="fr-footer__top-link" href="#">Lien de navigation</a>
                            </li>
                            <li>
                                <a class="fr-footer__top-link" href="#">Lien de navigation</a>
                            </li>
                            <li>
                                <a class="fr-footer__top-link" href="#">Lien de navigation</a>
                            </li>
                            <li>
                                <a class="fr-footer__top-link" href="#">Lien de navigation</a>
                            </li>
                        </ul>
                    </div>
                    <div class="fr-col-12 fr-col-sm-3 fr-col-md-2">
                        <h3 class="fr-footer__top-cat">Nom de la catégorie</h3>
                        <ul class="fr-footer__top-list">
                            <li>
                                <a class="fr-footer__top-link" href="#">Lien de navigation</a>
                            </li>
                            <li>
                                <a class="fr-footer__top-link" href="#">Lien de navigation</a>
                            </li>
                            <li>
                                <a class="fr-footer__top-link" href="#">Lien de navigation</a>
                            </li>
                            <li>
                                <a class="fr-footer__top-link" href="#">Lien de navigation</a>
                            </li>
                            <li>
                                <a class="fr-footer__top-link" href="#">Lien de navigation</a>
                            </li>
                            <li>
                                <a class="fr-footer__top-link" href="#">Lien de navigation</a>
                            </li>
                        </ul>
                    </div>
                    <div class="fr-col-12 fr-col-sm-3 fr-col-md-2">
                        <h3 class="fr-footer__top-cat">Nom de la catégorie</h3>
                        <ul class="fr-footer__top-list">
                            <li>
                                <a class="fr-footer__top-link" href="#">Lien de navigation</a>
                            </li>
                            <li>
                                <a class="fr-footer__top-link" href="#">Lien de navigation</a>
                            </li>
                            <li>
                                <a class="fr-footer__top-link" href="#">Lien de navigation</a>
                            </li>
                            <li>
                                <a class="fr-footer__top-link" href="#">Lien de navigation</a>
                            </li>
                            <li>
                                <a class="fr-footer__top-link" href="#">Lien de navigation</a>
                            </li>
                            <li>
                                <a class="fr-footer__top-link" href="#">Lien de navigation</a>
                            </li>
                        </ul>
                    </div>
                    <div class="fr-col-12 fr-col-sm-3 fr-col-md-2">
                        <h3 class="fr-footer__top-cat">Nom de la catégorie</h3>
                        <ul class="fr-footer__top-list">
                            <li>
                                <a class="fr-footer__top-link" href="#">Lien de navigation</a>
                            </li>
                            <li>
                                <a class="fr-footer__top-link" href="#">Lien de navigation</a>
                            </li>
                            <li>
                                <a class="fr-footer__top-link" href="#">Lien de navigation</a>
                            </li>
                            <li>
                                <a class="fr-footer__top-link" href="#">Lien de navigation</a>
                            </li>
                            <li>
                                <a class="fr-footer__top-link" href="#">Lien de navigation</a>
                            </li>
                            <li>
                                <a class="fr-footer__top-link" href="#">Lien de navigation</a>
                            </li>
                        </ul>
                    </div>
                    <div class="fr-col-12 fr-col-sm-3 fr-col-md-2">
                        <h3 class="fr-footer__top-cat">Nom de la catégorie</h3>
                        <ul class="fr-footer__top-list">
                            <li>
                                <a class="fr-footer__top-link" href="#">Lien de navigation</a>
                            </li>
                            <li>
                                <a class="fr-footer__top-link" href="#">Lien de navigation</a>
                            </li>
                            <li>
                                <a class="fr-footer__top-link" href="#">Lien de navigation</a>
                            </li>
                            <li>
                                <a class="fr-footer__top-link" href="#">Lien de navigation</a>
                            </li>
                            <li>
                                <a class="fr-footer__top-link" href="#">Lien de navigation</a>
                            </li>
                            <li>
                                <a class="fr-footer__top-link" href="#">Lien de navigation</a>
                            </li>
                        </ul>
                    </div>
                </div>
            </div>
        </div>
        <div class="fr-container">
            <div class="fr-footer__body">
                <div class="fr-footer__brand fr-enlarge-link">
                    <a href="/" title="Retour à l'accueil du site - Nom de l'entité (ministère, secrétariat d'état, gouvernement)">
                        <p class="fr-logo">
                            Intitulé
                            <br>officiel
                        </p>
                    </a>
                </div>
                <div class="fr-footer__content">
                    <p class="fr-footer__content-desc">Lorem [...] elit ut.</p>
                    <ul class="fr-footer__content-list">
                        <li class="fr-footer__content-item">
                            <a target="_blank" rel="noopener external" title="info.gouv.fr - nouvelle fenêtre" id="footer__content-link-7362" class="fr-footer__content-link" href="https://info.gouv.fr">info.gouv.fr</a>
                        </li>
                        <li class="fr-footer__content-item">
                            <a target="_blank" rel="noopener external" title="service-public.fr - nouvelle fenêtre" id="footer__content-link-7363" class="fr-footer__content-link" href="https://service-public.fr">service-public.fr</a>
                        </li>
                        <li class="fr-footer__content-item">
                            <a target="_blank" rel="noopener external" title="legifrance.gouv.fr - nouvelle fenêtre" id="footer__content-link-7364" class="fr-footer__content-link" href="https://legifrance.gouv.fr">legifrance.gouv.fr</a>
                        </li>
                        <li class="fr-footer__content-item">
                            <a target="_blank" rel="noopener external" title="data.gouv.fr - nouvelle fenêtre" id="footer__content-link-7365" class="fr-footer__content-link" href="https://data.gouv.fr">data.gouv.fr</a>
                        </li>
                    </ul>
                </div>
            </div>
            <div class="fr-footer__bottom">
                <ul class="fr-footer__bottom-list">
                    <li class="fr-footer__bottom-item">
                        <a class="fr-footer__bottom-link" href="#">Plan du site</a>
                    </li>
                    <li class="fr-footer__bottom-item">
                        <a class="fr-footer__bottom-link" href="#">Accessibilité : non/partiellement/totalement conforme</a>
                    </li>
                    <li class="fr-footer__bottom-item">
                        <a class="fr-footer__bottom-link" href="#">Mentions légales</a>
                    </li>
                    <li class="fr-footer__bottom-item">
                        <a class="fr-footer__bottom-link" href="#">Données personnelles</a>
                    </li>
                    <li class="fr-footer__bottom-item">
                        <a class="fr-footer__bottom-link" href="#">Gestion des cookies</a>
                    </li>
                </ul>
                <div class="fr-footer__bottom-copy">
                    <p>Sauf mention explicite de propriété intellectuelle détenue par des tiers, les contenus de ce site sont proposés sous <a href="https://github.com/etalab/licence-ouverte/blob/master/LO.md" target="_blank" rel="noopener external" title="Licence etalab - nouvelle fenêtre">licence etalab-2.0</a>
                    </p>
                </div>
            </div>
        </div>
    </footer>

Les listes de liens peuvent être classées par catégorie. Il est possible
d’aller au maximum jusqu'à 6 colonnes de liens. Nous recommandons de ne pas
dépasser des listes de plus de 8 liens.

Cette liste ne doit pas être le miroir des liens présents dans la navigation
principale. Un travail de conception particulier doit être mené pour organiser
les liens : ceux-ci peuvent pointer vers les contenus
populaires/fonctionnalités phares du site ou les pages susceptibles de
répondre aux questions restantes d'un visiteur.

## Pied de page avec partenaires

Dans ses deux versions le pied de page peut intégrer un bloc partenaires.

Il se compose des éléments suivants:

  * Le pied de page simple (voir la structure ci-dessus) - obligatoire
  * du bloc partenaire - obligatoireLogo du partenaire principal, ferré à gauche - obligatoireLogos des partenaires additionnels, ferrés à droite - optionnels.
  * Logo du partenaire principal, ferré à gauche - obligatoire
  * Logos des partenaires additionnels, ferrés à droite - optionnels.

![](/uploads/pied_de_page_partenaires_79570a9347.png)

###  Extrait de code

    
    
    <footer class="fr-footer" role="contentinfo" id="footer-7552">
        <div class="fr-container">
            <div class="fr-footer__body">
                <div class="fr-footer__brand fr-enlarge-link">
                    <a href="/" title="Retour à l'accueil du site - Nom de l'entité (ministère, secrétariat d'état, gouvernement)">
                        <p class="fr-logo">
                            Intitulé
                            <br>officiel
                        </p>
                    </a>
                </div>
                <div class="fr-footer__content">
                    <p class="fr-footer__content-desc">Lorem [...] elit ut.</p>
                    <ul class="fr-footer__content-list">
                        <li class="fr-footer__content-item">
                            <a target="_blank" rel="noopener external" title="info.gouv.fr - nouvelle fenêtre" id="footer__content-link-7654" class="fr-footer__content-link" href="https://info.gouv.fr">info.gouv.fr</a>
                        </li>
                        <li class="fr-footer__content-item">
                            <a target="_blank" rel="noopener external" title="service-public.fr - nouvelle fenêtre" id="footer__content-link-7655" class="fr-footer__content-link" href="https://service-public.fr">service-public.fr</a>
                        </li>
                        <li class="fr-footer__content-item">
                            <a target="_blank" rel="noopener external" title="legifrance.gouv.fr - nouvelle fenêtre" id="footer__content-link-7656" class="fr-footer__content-link" href="https://legifrance.gouv.fr">legifrance.gouv.fr</a>
                        </li>
                        <li class="fr-footer__content-item">
                            <a target="_blank" rel="noopener external" title="data.gouv.fr - nouvelle fenêtre" id="footer__content-link-7657" class="fr-footer__content-link" href="https://data.gouv.fr">data.gouv.fr</a>
                        </li>
                    </ul>
                </div>
            </div>
            <div class="fr-footer__partners">
                <h2 class="fr-footer__partners-title">Nos partenaires</h2>
                <div class="fr-footer__partners-logos">
                    <div class="fr-footer__partners-main">
                        <a class="fr-footer__partners-link" href="#">
                            <img class="fr-footer__logo" style="height: 5.625rem" src="../../../example/img/placeholder.16x9.png" alt="[À MODIFIER - texte alternatif de l'image]" />
                            <!-- L'alternative de l'image (attribut alt) doit impérativement être renseignée et reprendre le texte visible dans l'image -->
                        </a>
                    </div>
                    <div class="fr-footer__partners-sub">
                        <ul>
                            <li>
                                <a class="fr-footer__partners-link" href="#">
                                    <img class="fr-footer__logo" style="height: 5.625rem" src="/example/img/placeholder.16x9.png" alt="[À MODIFIER - texte alternatif de l'image]" />
                                    <!-- L'alternative de l'image (attribut alt) doit impérativement être renseignée et reprendre le texte visible dans l'image -->
                                </a>
                            </li>
                            <li>
                                <a class="fr-footer__partners-link" href="#">
                                    <img class="fr-footer__logo" style="height: 5.625rem" src="/example/img/placeholder.1x1.png" alt="[À MODIFIER - texte alternatif de l'image]" />
                                    <!-- L'alternative de l'image (attribut alt) doit impérativement être renseignée et reprendre le texte visible dans l'image -->
                                </a>
                            </li>
                            <li>
                                <a class="fr-footer__partners-link" href="#">
                                    <img class="fr-footer__logo" style="height: 5.625rem" src="/example/img/placeholder.9x16.png" alt="[À MODIFIER - texte alternatif de l'image]" />
                                    <!-- L'alternative de l'image (attribut alt) doit impérativement être renseignée et reprendre le texte visible dans l'image -->
                                </a>
                            </li>
                        </ul>
                    </div>
                </div>
            </div>
            <div class="fr-footer__bottom">
                <ul class="fr-footer__bottom-list">
                    <li class="fr-footer__bottom-item">
                        <a class="fr-footer__bottom-link" href="#">Plan du site</a>
                    </li>
                    <li class="fr-footer__bottom-item">
                        <a class="fr-footer__bottom-link" href="#">Accessibilité : non/partiellement/totalement conforme</a>
                    </li>
                    <li class="fr-footer__bottom-item">
                        <a class="fr-footer__bottom-link" href="#">Mentions légales</a>
                    </li>
                    <li class="fr-footer__bottom-item">
                        <a class="fr-footer__bottom-link" href="#">Données personnelles</a>
                    </li>
                    <li class="fr-footer__bottom-item">
                        <a class="fr-footer__bottom-link" href="#">Gestion des cookies</a>
                    </li>
                </ul>
                <div class="fr-footer__bottom-copy">
                    <p>Sauf mention explicite de propriété intellectuelle détenue par des tiers, les contenus de ce site sont proposés sous <a href="https://github.com/etalab/licence-ouverte/blob/master/LO.md" target="_blank" rel="noopener external" title="Licence etalab - nouvelle fenêtre">licence etalab-2.0</a>
                    </p>
                </div>
            </div>
        </div>
    </footer>

Le partenaire principal est toujours placé à gauche. Les partenaires
secondaires sont placés à droite si associés à un partenaires principal, sinon
à gauche.

## Lettre d’information et réseaux sociaux

Les composant d’inscription à la newsletter et de la mise en avant des liens
vers les réseaux sociaux doit se trouver juste au dessus du footer sur les
pages utilisant ces composants :  
[Lettre d'information et réseaux sociaux](/elements-d-
interface/composants/lettre-d-information-et-reseaux-sociaux)

## Règles d’utilisation

### Usage

Le pied de page est présent sur l’ensemble des pages du site. Il est situé en
fin de page. Le trait bleu marque la séparation entre le corps de la page et
le pied de page.

### Accessibilité

L'élément footer doit contenir le role aria contentinfo

    
    
    <footer role=”contentinfo”>

La mention de conformité (ou non) au RGAA doit apparaître sur toutes les
pages. Le lien vers la déclaration d’accessibilité du site doit être libellé
de la façon suivante :

  * “Accessibilité : non conforme” si le taux de conformité est inférieur à 50% (ou qu’aucun audit n’a été effectué)
  * “Accessibilité : partiellement conforme” si le taux de conformité est supérieur à 50%.
  * “Accessibilité : totalement conforme” si le taux de conformité est égal à 100%.

Plus d’informations sur [Les outils pour le design numérique et
l'accessibilité - DesignGouv](https://design.numerique.gouv.fr/accessibilite-
numerique/cadre-legal/ "Les outils pour le design numérique et l'accessibilité
- DesignGouv - nouvelle fenêtre")

### Contenu

Le texte de présentation optionnel peut être utilisé pour donner des
informations sur le service (texte de présentation…) ou l’organisation
(contact, adresse…).

Pour les libellés des liens, utiliser des formulations claires et concises. Il
faut respecter la distinction des zones :

  * Les liens liés aux obligations (mentions légales, etc.)
  * Les liens liés à la sphère gouvernementale
  * Les liens internes et externes (liste présente en haut de footer, de la version complète du pied de page). 

### Personnalisation

Le style de ce composant n’est pas personnalisable. Toutefois, certains
éléments sont optionnels - voir la structure du composant.

### Besoin d'aide ?

L'équipe du DSFR est là pour vous aider.

Retrouvez-la sur :

  * [la communauté slack](https://gouvfr.slack.com/ "la communauté slack - nouvelle fenêtre") pour poser vos questions, et échanger avec d’autres utilisateurs.   
Vous êtes **agent de l’État** et souhaitez accéder au slack ? [Rejoignez la
communauté](https://gouvfr.atlassian.net/servicedesk/customer/portal/1/group/1/create/9
"Rejoignez la communauté - nouvelle fenêtre") dès maintenant !

  * [ le centre de support](https://gouvfr.atlassian.net/servicedesk/customer/portals "le centre de support - nouvelle fenêtre") pour envoyer vos demandes de correctifs et d'évolution.

[Partage - Share](/composants-et-modeles/composants/partage)

[Retour en haut de page - Back to top](/composants-et-
modeles/composants/retour-en-haut-de-page)

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
