Fermer

# Menu latéral - Sidemenu

Le menu latéral permet aux utilisateurs de naviguer entre les différentes
pages d’une rubrique ou d’un même thème.

Le menu latéral est un système de navigation vertical présentant une liste de
liens placée à côté du contenu (à gauche ou à droite de la page) et donnant
accès jusqu'à 3 niveaux d’arborescence.

Ce composant doit être utilisé sur les sites avec un niveau de profondeur
assez important (2 niveaux de navigation ou plus).

Le menu latéral se compose d’un titre de rubrique (optionnel) et d’une liste
de liens sur 3 niveaux (les pages associées à une même rubrique sont
regroupées dans des collapse).

### Menu latéral avec un seul niveau d’arborescence (accès direct)

Il est composé d’une liste de liens vers les pages de la rubrique ‘courante’.

Dans cette rubrique

Titre de rubrique

  * Accès direct
  * Accès direct
  * Accès direct
  * Accès direct
  * Accès direct
  * Accès direct
  * Accès direct
  * Accès direct
  * Accès direct

###  Extrait de code

    
    
                          <nav class="fr-sidemenu" aria-labelledby="fr-sidemenu-title">
          <div class="fr-sidemenu__inner">
            <button
              class="fr-sidemenu__btn"
              hidden
              aria-controls="fr-sidemenu-wrapper"
              aria-expanded="false"
            >
              Dans cette rubrique
            </button>
            <div class="fr-collapse" id="fr-sidemenu-wrapper">
              <div class="fr-sidemenu__title" id="fr-sidemenu-title">Titre de rubrique</div>
              <ul class="fr-sidemenu__list">
                <li class="fr-sidemenu__item fr-sidemenu__item--active">
                  <a
                    class="fr-sidemenu__link"
                    href="#"
                    target="_self"
                    aria-current="page"
                    >Accès direct</a
                  >
                </li>
                <li class="fr-sidemenu__item">
                  <a class="fr-sidemenu__link" href="#" target="_self"
                    >Accès direct</a
                  >
                </li>
                <li class="fr-sidemenu__item">
                  <a class="fr-sidemenu__link" href="#" target="_self"
                    >Accès direct</a
                  >
                </li>
                <li class="fr-sidemenu__item">
                  <a class="fr-sidemenu__link" href="#" target="_self"
                    >Accès direct</a
                  >
                </li>
                <li class="fr-sidemenu__item">
                  <a class="fr-sidemenu__link" href="#" target="_self"
                    >Accès direct</a
                  >
                </li>
                <li class="fr-sidemenu__item">
                  <a class="fr-sidemenu__link" href="#" target="_self"
                    >Accès direct</a
                  >
                </li>
                <li class="fr-sidemenu__item">
                  <a class="fr-sidemenu__link" href="#" target="_self"
                    >Accès direct</a
                  >
                </li>
                <li class="fr-sidemenu__item">
                  <a class="fr-sidemenu__link" href="#" target="_self"
                    >Accès direct</a
                  >
                </li>
                <li class="fr-sidemenu__item">
                  <a class="fr-sidemenu__link" href="#" target="_self"
                    >Accès direct</a
                  >
                </li>
              </ul>
            </div>
          </div>
        </nav>
                          
                        

## Menu latéral avec deux niveaux d’arborescence

Il permet d’afficher les niveaux secondaires d’une rubrique. Le click sur le
premier niveau fait apparaitre la liste des liens lui étant rattachée.

Dans cette rubrique

Titre de rubrique

  * Niveau 1 

    * Accès direct niveau 2
    * Accès direct niveau 2
    * Accès direct niveau 2
    * Accès direct niveau 2
    * Accès direct niveau 2
    * Accès direct niveau 2

  * Entrée menu active 

    * Accès direct niveau 2
    * Accès direct niveau 2
    * Accès direct niveau 2
    * Accès direct niveau 2
    * Accès direct niveau 2
    * Accès direct niveau 2

  * Accès direct
  * Niveau 1 

    * Accès direct niveau 2
    * Accès direct niveau 2
    * Accès direct niveau 2
    * Accès direct niveau 2
    * Accès direct niveau 2
    * Accès direct niveau 2

  * Niveau 1 

    * Accès direct niveau 2
    * Accès direct niveau 2
    * Accès direct niveau 2
    * Accès direct niveau 2
    * Accès direct niveau 2
    * Accès direct niveau 2

  * Accès direct
  * Niveau 1 

    * Accès direct niveau 2
    * Accès direct niveau 2
    * Accès direct niveau 2
    * Accès direct niveau 2
    * Accès direct niveau 2
    * Accès direct niveau 2

  * Niveau 1 

    * Accès direct niveau 2
    * Accès direct niveau 2
    * Accès direct niveau 2
    * Accès direct niveau 2
    * Accès direct niveau 2
    * Accès direct niveau 2

  * Accès direct
  * Niveau 1 

    * Accès direct niveau 2
    * Accès direct niveau 2
    * Accès direct niveau 2
    * Accès direct niveau 2
    * Accès direct niveau 2
    * Accès direct niveau 2

###  Extrait de code

    
    
                          <nav class="fr-sidemenu" role="navigation" aria-labelledby="fr-sidemenu-title">
          <div class="fr-sidemenu__inner">
            <button
              class="fr-sidemenu__btn"
              aria-controls="fr-sidemenu-wrapper"
              aria-expanded="false"
            >
              Dans cette rubrique
            </button>
            <div class="fr-collapse" id="fr-sidemenu-wrapper">
              <div class="fr-sidemenu__title" id="fr-sidemenu-title">Titre de rubrique</div>
              <ul class="fr-sidemenu__list">
                <li class="fr-sidemenu__item">
                  <button
                    class="fr-sidemenu__btn"
                    aria-expanded="false"
                    aria-controls="fr-sidemenu-item-0"
                  >
                    Niveau 1
                  </button>
                  <div class="fr-collapse" id="fr-sidemenu-item-0">
                    <ul class="fr-sidemenu__list">
                      <li class="fr-sidemenu__item">
                        <a class="fr-sidemenu__link" href="#" target="_self"
                          >Accès direct niveau 2</a
                        >
                      </li>
                      <li class="fr-sidemenu__item">
                        <a class="fr-sidemenu__link" href="#" target="_self"
                          >Accès direct niveau 2</a
                        >
                      </li>
                      <li class="fr-sidemenu__item">
                        <a class="fr-sidemenu__link" href="#" target="_self"
                          >Accès direct niveau 2</a
                        >
                      </li>
                      <li class="fr-sidemenu__item">
                        <a class="fr-sidemenu__link" href="#" target="_self"
                          >Accès direct niveau 2</a
                        >
                      </li>
                      <li class="fr-sidemenu__item">
                        <a class="fr-sidemenu__link" href="#" target="_self"
                          >Accès direct niveau 2</a
                        >
                      </li>
                      <li class="fr-sidemenu__item">
                        <a class="fr-sidemenu__link" href="#" target="_self"
                          >Accès direct niveau 2</a
                        >
                      </li>
                    </ul>
                  </div>
                </li>
                <li class="fr-sidemenu__item fr-sidemenu__item--active">
                  <button
                    class="fr-sidemenu__btn"
                    aria-expanded="false"
                    aria-controls="fr-sidemenu-item-1"
                    aria-current="true"
                  >
                    Entrée menu active
                  </button>
                  <div class="fr-collapse" id="fr-sidemenu-item-1">
                    <ul class="fr-sidemenu__list">
                      <li class="fr-sidemenu__item">
                        <a class="fr-sidemenu__link" href="#" target="_self"
                          >Accès direct niveau 2</a
                        >
                      </li>
                      <li class="fr-sidemenu__item">
                        <a class="fr-sidemenu__link" href="#" target="_self"
                          >Accès direct niveau 2</a
                        >
                      </li>
                      <li class="fr-sidemenu__item fr-sidemenu__item--active">
                        <a
                          class="fr-sidemenu__link"
                          href="#"
                          target="_self"
                          aria-current="page"
                          >Accès direct niveau 2</a
                        >
                      </li>
                      <li class="fr-sidemenu__item">
                        <a class="fr-sidemenu__link" href="#" target="_self"
                          >Accès direct niveau 2</a
                        >
                      </li>
                      <li class="fr-sidemenu__item">
                        <a class="fr-sidemenu__link" href="#" target="_self"
                          >Accès direct niveau 2</a
                        >
                      </li>
                      <li class="fr-sidemenu__item">
                        <a class="fr-sidemenu__link" href="#" target="_self"
                          >Accès direct niveau 2</a
                        >
                      </li>
                    </ul>
                  </div>
                </li>
                <li class="fr-sidemenu__item">
                  <a class="fr-sidemenu__link" href="#" target="_self"
                    >Accès direct</a
                  >
                </li>
                <li class="fr-sidemenu__item">
                  <button
                    class="fr-sidemenu__btn"
                    aria-expanded="false"
                    aria-controls="fr-sidemenu-item-3"
                  >
                    Niveau 1
                  </button>
                  <div class="fr-collapse" id="fr-sidemenu-item-3">
                    <ul class="fr-sidemenu__list">
                      <li class="fr-sidemenu__item">
                        <a class="fr-sidemenu__link" href="#" target="_self"
                          >Accès direct niveau 2</a
                        >
                      </li>
                      <li class="fr-sidemenu__item">
                        <a class="fr-sidemenu__link" href="#" target="_self"
                          >Accès direct niveau 2</a
                        >
                      </li>
                      <li class="fr-sidemenu__item">
                        <a class="fr-sidemenu__link" href="#" target="_self"
                          >Accès direct niveau 2</a
                        >
                      </li>
                      <li class="fr-sidemenu__item">
                        <a class="fr-sidemenu__link" href="#" target="_self"
                          >Accès direct niveau 2</a
                        >
                      </li>
                      <li class="fr-sidemenu__item">
                        <a class="fr-sidemenu__link" href="#" target="_self"
                          >Accès direct niveau 2</a
                        >
                      </li>
                      <li class="fr-sidemenu__item">
                        <a class="fr-sidemenu__link" href="#" target="_self"
                          >Accès direct niveau 2</a
                        >
                      </li>
                    </ul>
                  </div>
                </li>
                <li class="fr-sidemenu__item">
                  <button
                    class="fr-sidemenu__btn"
                    aria-expanded="false"
                    aria-controls="fr-sidemenu-item-4"
                  >
                    Niveau 1
                  </button>
                  <div class="fr-collapse" id="fr-sidemenu-item-4">
                    <ul class="fr-sidemenu__list">
                      <li class="fr-sidemenu__item">
                        <a class="fr-sidemenu__link" href="#" target="_self"
                          >Accès direct niveau 2</a
                        >
                      </li>
                      <li class="fr-sidemenu__item">
                        <a class="fr-sidemenu__link" href="#" target="_self"
                          >Accès direct niveau 2</a
                        >
                      </li>
                      <li class="fr-sidemenu__item">
                        <a class="fr-sidemenu__link" href="#" target="_self"
                          >Accès direct niveau 2</a
                        >
                      </li>
                      <li class="fr-sidemenu__item">
                        <a class="fr-sidemenu__link" href="#" target="_self"
                          >Accès direct niveau 2</a
                        >
                      </li>
                      <li class="fr-sidemenu__item">
                        <a class="fr-sidemenu__link" href="#" target="_self"
                          >Accès direct niveau 2</a
                        >
                      </li>
                      <li class="fr-sidemenu__item">
                        <a class="fr-sidemenu__link" href="#" target="_self"
                          >Accès direct niveau 2</a
                        >
                      </li>
                    </ul>
                  </div>
                </li>
                <li class="fr-sidemenu__item">
                  <a class="fr-sidemenu__link" href="#" target="_self"
                    >Accès direct</a
                  >
                </li>
                <li class="fr-sidemenu__item">
                  <button
                    class="fr-sidemenu__btn"
                    aria-expanded="false"
                    aria-controls="fr-sidemenu-item-6"
                  >
                    Niveau 1
                  </button>
                  <div class="fr-collapse" id="fr-sidemenu-item-6">
                    <ul class="fr-sidemenu__list">
                      <li class="fr-sidemenu__item">
                        <a class="fr-sidemenu__link" href="#" target="_self"
                          >Accès direct niveau 2</a
                        >
                      </li>
                      <li class="fr-sidemenu__item">
                        <a class="fr-sidemenu__link" href="#" target="_self"
                          >Accès direct niveau 2</a
                        >
                      </li>
                      <li class="fr-sidemenu__item">
                        <a class="fr-sidemenu__link" href="#" target="_self"
                          >Accès direct niveau 2</a
                        >
                      </li>
                      <li class="fr-sidemenu__item">
                        <a class="fr-sidemenu__link" href="#" target="_self"
                          >Accès direct niveau 2</a
                        >
                      </li>
                      <li class="fr-sidemenu__item">
                        <a class="fr-sidemenu__link" href="#" target="_self"
                          >Accès direct niveau 2</a
                        >
                      </li>
                      <li class="fr-sidemenu__item">
                        <a class="fr-sidemenu__link" href="#" target="_self"
                          >Accès direct niveau 2</a
                        >
                      </li>
                    </ul>
                  </div>
                </li>
                <li class="fr-sidemenu__item">
                  <button
                    class="fr-sidemenu__btn"
                    aria-expanded="false"
                    aria-controls="fr-sidemenu-item-7"
                  >
                    Niveau 1
                  </button>
                  <div class="fr-collapse" id="fr-sidemenu-item-7">
                    <ul class="fr-sidemenu__list">
                      <li class="fr-sidemenu__item">
                        <a class="fr-sidemenu__link" href="#" target="_self"
                          >Accès direct niveau 2</a
                        >
                      </li>
                      <li class="fr-sidemenu__item">
                        <a class="fr-sidemenu__link" href="#" target="_self"
                          >Accès direct niveau 2</a
                        >
                      </li>
                      <li class="fr-sidemenu__item">
                        <a class="fr-sidemenu__link" href="#" target="_self"
                          >Accès direct niveau 2</a
                        >
                      </li>
                      <li class="fr-sidemenu__item">
                        <a class="fr-sidemenu__link" href="#" target="_self"
                          >Accès direct niveau 2</a
                        >
                      </li>
                      <li class="fr-sidemenu__item">
                        <a class="fr-sidemenu__link" href="#" target="_self"
                          >Accès direct niveau 2</a
                        >
                      </li>
                      <li class="fr-sidemenu__item">
                        <a class="fr-sidemenu__link" href="#" target="_self"
                          >Accès direct niveau 2</a
                        >
                      </li>
                    </ul>
                  </div>
                </li>
                <li class="fr-sidemenu__item">
                  <a class="fr-sidemenu__link" href="#" target="_self"
                    >Accès direct</a
                  >
                </li>
                <li class="fr-sidemenu__item">
                  <button
                    class="fr-sidemenu__btn"
                    aria-expanded="false"
                    aria-controls="fr-sidemenu-item-9"
                  >
                    Niveau 1
                  </button>
                  <div class="fr-collapse" id="fr-sidemenu-item-9">
                    <ul class="fr-sidemenu__list">
                      <li class="fr-sidemenu__item">
                        <a class="fr-sidemenu__link" href="#" target="_self"
                          >Accès direct niveau 2</a
                        >
                      </li>
                      <li class="fr-sidemenu__item">
                        <a class="fr-sidemenu__link" href="#" target="_self"
                          >Accès direct niveau 2</a
                        >
                      </li>
                      <li class="fr-sidemenu__item">
                        <a class="fr-sidemenu__link" href="#" target="_self"
                          >Accès direct niveau 2</a
                        >
                      </li>
                      <li class="fr-sidemenu__item">
                        <a class="fr-sidemenu__link" href="#" target="_self"
                          >Accès direct niveau 2</a
                        >
                      </li>
                      <li class="fr-sidemenu__item">
                        <a class="fr-sidemenu__link" href="#" target="_self"
                          >Accès direct niveau 2</a
                        >
                      </li>
                      <li class="fr-sidemenu__item">
                        <a class="fr-sidemenu__link" href="#" target="_self"
                          >Accès direct niveau 2</a
                        >
                      </li>
                    </ul>
                  </div>
                </li>
              </ul>
            </div>
          </div>
        </nav>
                          
                        

## Menu latéral avec trois niveaux d’arborescence

Il permet d’afficher les niveaux 1, 2 et 3 imbriqués d’une rubrique.

Dans cette rubrique

Titre de rubrique

  * Niveau 1 

    * Accès direct niveau 2
    * Accès direct niveau 2
    * Niveau 2 

      * Accès direct niveau 3 
      * Accès direct niveau 3 
      * Accès direct niveau 3 
      * Accès direct niveau 3 
      * Accès direct niveau 3 
      * Accès direct niveau 3 

    * Accès direct niveau 2
    * Accès direct niveau 2
    * Accès direct niveau 2
    * Accès direct niveau 2

  * Entrée menu active 

    * Accès direct niveau 2
    * Accès direct niveau 2
    * Niveau 2 

      * Accès direct niveau 3 
      * Accès direct niveau 3 
      * Accès direct niveau 3 
      * Accès direct niveau 3 
      * Accès direct niveau 3 
      * Accès direct niveau 3 

    * Accès direct niveau 2
    * Accès direct niveau 2
    * Accès direct niveau 2
    * Accès direct niveau 2

  * Accès direct
  * Niveau 1 

    * Accès direct niveau 2
    * Accès direct niveau 2
    * Niveau 2 

      * Accès direct niveau 3 
      * Accès direct niveau 3 
      * Accès direct niveau 3 
      * Accès direct niveau 3 
      * Accès direct niveau 3 
      * Accès direct niveau 3 

    * Accès direct niveau 2
    * Accès direct niveau 2
    * Accès direct niveau 2
    * Accès direct niveau 2

  * Niveau 1 

    * Accès direct niveau 2
    * Accès direct niveau 2
    * Niveau 2 

      * Accès direct niveau 3 
      * Accès direct niveau 3 
      * Accès direct niveau 3 
      * Accès direct niveau 3 
      * Accès direct niveau 3 
      * Accès direct niveau 3 

    * Accès direct niveau 2
    * Accès direct niveau 2
    * Accès direct niveau 2
    * Accès direct niveau 2

  * Accès direct
  * Niveau 1 

    * Accès direct niveau 2
    * Accès direct niveau 2
    * Niveau 2 

      * Accès direct niveau 3 
      * Accès direct niveau 3 
      * Accès direct niveau 3 
      * Accès direct niveau 3 
      * Accès direct niveau 3 
      * Accès direct niveau 3 

    * Accès direct niveau 2
    * Accès direct niveau 2
    * Accès direct niveau 2
    * Accès direct niveau 2

  * Niveau 1 

    * Accès direct niveau 2
    * Accès direct niveau 2
    * Niveau 2 

      * Accès direct niveau 3 
      * Accès direct niveau 3 
      * Accès direct niveau 3 
      * Accès direct niveau 3 
      * Accès direct niveau 3 
      * Accès direct niveau 3 

    * Accès direct niveau 2
    * Accès direct niveau 2
    * Accès direct niveau 2
    * Accès direct niveau 2

  * Accès direct
  * Niveau 1 

    * Accès direct niveau 2
    * Accès direct niveau 2
    * Niveau 2 

      * Accès direct niveau 3 
      * Accès direct niveau 3 
      * Accès direct niveau 3 
      * Accès direct niveau 3 
      * Accès direct niveau 3 
      * Accès direct niveau 3 

    * Accès direct niveau 2
    * Accès direct niveau 2
    * Accès direct niveau 2
    * Accès direct niveau 2

###  Extrait de code

    
    
                          <nav class="fr-sidemenu" role="navigation" aria-labelledby="fr-sidemenu-title">
          <div class="fr-sidemenu__inner">
            <button
              class="fr-sidemenu__btn"
              aria-controls="fr-sidemenu-wrapper"
              aria-expanded="false"
            >
              Dans cette rubrique
            </button>
            <div class="fr-collapse" id="fr-sidemenu-wrapper">
              <div class="fr-sidemenu__title" id="fr-sidemenu-title">Titre de rubrique</div>
              <ul class="fr-sidemenu__list">
                <li class="fr-sidemenu__item">
                  <button
                    class="fr-sidemenu__btn"
                    aria-expanded="false"
                    aria-controls="fr-sidemenu-item-0"
                  >
                    Niveau 1
                  </button>
                  <div class="fr-collapse" id="fr-sidemenu-item-0">
                    <ul class="fr-sidemenu__list">
                      <li class="fr-sidemenu__item">
                        <a class="fr-sidemenu__link" href="#" target="_self"
                          >Accès direct niveau 2</a
                        >
                      </li>
                      <li class="fr-sidemenu__item">
                        <a class="fr-sidemenu__link" href="#" target="_self"
                          >Accès direct niveau 2</a
                        >
                      </li>
                      <li class="fr-sidemenu__item">
                        <button
                          class="fr-sidemenu__btn"
                          aria-expanded="false"
                          aria-controls="fr-sidemenu-item-0-sub"
                        >
                          Niveau 2
                        </button>
                        <div class="fr-collapse" id="fr-sidemenu-item-0-sub">
                          <ul class="fr-sidemenu__list">
                            <li class="fr-sidemenu__item">
                              <a class="fr-sidemenu__link" href="#" target="_self">
                                Accès direct niveau 3
                              </a>
                            </li>
                            <li class="fr-sidemenu__item">
                              <a class="fr-sidemenu__link" href="#" target="_self">
                                Accès direct niveau 3
                              </a>
                            </li>
                            <li class="fr-sidemenu__item">
                              <a class="fr-sidemenu__link" href="#" target="_self">
                                Accès direct niveau 3
                              </a>
                            </li>
                            <li class="fr-sidemenu__item">
                              <a class="fr-sidemenu__link" href="#" target="_self">
                                Accès direct niveau 3
                              </a>
                            </li>
                            <li class="fr-sidemenu__item">
                              <a class="fr-sidemenu__link" href="#" target="_self">
                                Accès direct niveau 3
                              </a>
                            </li>
                            <li class="fr-sidemenu__item">
                              <a class="fr-sidemenu__link" href="#" target="_self">
                                Accès direct niveau 3
                              </a>
                            </li>
                          </ul>
                        </div>
                      </li>
                      <li class="fr-sidemenu__item">
                        <a class="fr-sidemenu__link" href="#" target="_self"
                          >Accès direct niveau 2</a
                        >
                      </li>
                      <li class="fr-sidemenu__item">
                        <a class="fr-sidemenu__link" href="#" target="_self"
                          >Accès direct niveau 2</a
                        >
                      </li>
                      <li class="fr-sidemenu__item">
                        <a class="fr-sidemenu__link" href="#" target="_self"
                          >Accès direct niveau 2</a
                        >
                      </li>
                      <li class="fr-sidemenu__item">
                        <a class="fr-sidemenu__link" href="#" target="_self"
                          >Accès direct niveau 2</a
                        >
                      </li>
                    </ul>
                  </div>
                </li>
                <li class="fr-sidemenu__item fr-sidemenu__item--active">
                  <button
                    class="fr-sidemenu__btn"
                    aria-expanded="false"
                    aria-controls="fr-sidemenu-item-1"
                    aria-current="true"
                  >
                    Entrée menu active
                  </button>
                  <div class="fr-collapse" id="fr-sidemenu-item-1">
                    <ul class="fr-sidemenu__list">
                      <li class="fr-sidemenu__item">
                        <a class="fr-sidemenu__link" href="#" target="_self"
                          >Accès direct niveau 2</a
                        >
                      </li>
                      <li class="fr-sidemenu__item">
                        <a class="fr-sidemenu__link" href="#" target="_self"
                          >Accès direct niveau 2</a
                        >
                      </li>
                      <li class="fr-sidemenu__item">
                        <button
                          class="fr-sidemenu__btn"
                          aria-expanded="false"
                          aria-controls="fr-sidemenu-item-1-sub"
                        >
                          Niveau 2
                        </button>
                        <div class="fr-collapse" id="fr-sidemenu-item-1-sub">
                          <ul class="fr-sidemenu__list">
                            <li class="fr-sidemenu__item">
                              <a class="fr-sidemenu__link" href="#" target="_self">
                                Accès direct niveau 3
                              </a>
                            </li>
                            <li class="fr-sidemenu__item">
                              <a class="fr-sidemenu__link" href="#" target="_self">
                                Accès direct niveau 3
                              </a>
                            </li>
                            <li class="fr-sidemenu__item">
                              <a class="fr-sidemenu__link" href="#" target="_self">
                                Accès direct niveau 3
                              </a>
                            </li>
                            <li class="fr-sidemenu__item">
                              <a class="fr-sidemenu__link" href="#" target="_self">
                                Accès direct niveau 3
                              </a>
                            </li>
                            <li class="fr-sidemenu__item">
                              <a class="fr-sidemenu__link" href="#" target="_self">
                                Accès direct niveau 3
                              </a>
                            </li>
                            <li class="fr-sidemenu__item">
                              <a class="fr-sidemenu__link" href="#" target="_self">
                                Accès direct niveau 3
                              </a>
                            </li>
                          </ul>
                        </div>
                      </li>
                      <li class="fr-sidemenu__item fr-sidemenu__item--active">
                        <a
                          class="fr-sidemenu__link"
                          href="#"
                          target="_self"
                          aria-current="page"
                          >Accès direct niveau 2</a
                        >
                      </li>
                      <li class="fr-sidemenu__item">
                        <a class="fr-sidemenu__link" href="#" target="_self"
                          >Accès direct niveau 2</a
                        >
                      </li>
                      <li class="fr-sidemenu__item">
                        <a class="fr-sidemenu__link" href="#" target="_self"
                          >Accès direct niveau 2</a
                        >
                      </li>
                      <li class="fr-sidemenu__item">
                        <a class="fr-sidemenu__link" href="#" target="_self"
                          >Accès direct niveau 2</a
                        >
                      </li>
                    </ul>
                  </div>
                </li>
                <li class="fr-sidemenu__item">
                  <a class="fr-sidemenu__link" href="#" target="_self"
                    >Accès direct</a
                  >
                </li>
                <li class="fr-sidemenu__item">
                  <button
                    class="fr-sidemenu__btn"
                    aria-expanded="false"
                    aria-controls="fr-sidemenu-item-3"
                  >
                    Niveau 1
                  </button>
                  <div class="fr-collapse" id="fr-sidemenu-item-3">
                    <ul class="fr-sidemenu__list">
                      <li class="fr-sidemenu__item">
                        <a class="fr-sidemenu__link" href="#" target="_self"
                          >Accès direct niveau 2</a
                        >
                      </li>
                      <li class="fr-sidemenu__item">
                        <a class="fr-sidemenu__link" href="#" target="_self"
                          >Accès direct niveau 2</a
                        >
                      </li>
                      <li class="fr-sidemenu__item">
                        <button
                          class="fr-sidemenu__btn"
                          aria-expanded="false"
                          aria-controls="fr-sidemenu-item-3-sub"
                        >
                          Niveau 2
                        </button>
                        <div class="fr-collapse" id="fr-sidemenu-item-3-sub">
                          <ul class="fr-sidemenu__list">
                            <li class="fr-sidemenu__item">
                              <a class="fr-sidemenu__link" href="#" target="_self">
                                Accès direct niveau 3
                              </a>
                            </li>
                            <li class="fr-sidemenu__item">
                              <a class="fr-sidemenu__link" href="#" target="_self">
                                Accès direct niveau 3
                              </a>
                            </li>
                            <li class="fr-sidemenu__item">
                              <a class="fr-sidemenu__link" href="#" target="_self">
                                Accès direct niveau 3
                              </a>
                            </li>
                            <li class="fr-sidemenu__item">
                              <a class="fr-sidemenu__link" href="#" target="_self">
                                Accès direct niveau 3
                              </a>
                            </li>
                            <li class="fr-sidemenu__item">
                              <a class="fr-sidemenu__link" href="#" target="_self">
                                Accès direct niveau 3
                              </a>
                            </li>
                            <li class="fr-sidemenu__item">
                              <a class="fr-sidemenu__link" href="#" target="_self">
                                Accès direct niveau 3
                              </a>
                            </li>
                          </ul>
                        </div>
                      </li>
                      <li class="fr-sidemenu__item">
                        <a class="fr-sidemenu__link" href="#" target="_self"
                          >Accès direct niveau 2</a
                        >
                      </li>
                      <li class="fr-sidemenu__item">
                        <a class="fr-sidemenu__link" href="#" target="_self"
                          >Accès direct niveau 2</a
                        >
                      </li>
                      <li class="fr-sidemenu__item">
                        <a class="fr-sidemenu__link" href="#" target="_self"
                          >Accès direct niveau 2</a
                        >
                      </li>
                      <li class="fr-sidemenu__item">
                        <a class="fr-sidemenu__link" href="#" target="_self"
                          >Accès direct niveau 2</a
                        >
                      </li>
                    </ul>
                  </div>
                </li>
                <li class="fr-sidemenu__item">
                  <button
                    class="fr-sidemenu__btn"
                    aria-expanded="false"
                    aria-controls="fr-sidemenu-item-4"
                  >
                    Niveau 1
                  </button>
                  <div class="fr-collapse" id="fr-sidemenu-item-4">
                    <ul class="fr-sidemenu__list">
                      <li class="fr-sidemenu__item">
                        <a class="fr-sidemenu__link" href="#" target="_self"
                          >Accès direct niveau 2</a
                        >
                      </li>
                      <li class="fr-sidemenu__item">
                        <a class="fr-sidemenu__link" href="#" target="_self"
                          >Accès direct niveau 2</a
                        >
                      </li>
                      <li class="fr-sidemenu__item">
                        <button
                          class="fr-sidemenu__btn"
                          aria-expanded="false"
                          aria-controls="fr-sidemenu-item-4-sub"
                        >
                          Niveau 2
                        </button>
                        <div class="fr-collapse" id="fr-sidemenu-item-4-sub">
                          <ul class="fr-sidemenu__list">
                            <li class="fr-sidemenu__item">
                              <a class="fr-sidemenu__link" href="#" target="_self">
                                Accès direct niveau 3
                              </a>
                            </li>
                            <li class="fr-sidemenu__item">
                              <a class="fr-sidemenu__link" href="#" target="_self">
                                Accès direct niveau 3
                              </a>
                            </li>
                            <li class="fr-sidemenu__item">
                              <a class="fr-sidemenu__link" href="#" target="_self">
                                Accès direct niveau 3
                              </a>
                            </li>
                            <li class="fr-sidemenu__item">
                              <a class="fr-sidemenu__link" href="#" target="_self">
                                Accès direct niveau 3
                              </a>
                            </li>
                            <li class="fr-sidemenu__item">
                              <a class="fr-sidemenu__link" href="#" target="_self">
                                Accès direct niveau 3
                              </a>
                            </li>
                            <li class="fr-sidemenu__item">
                              <a class="fr-sidemenu__link" href="#" target="_self">
                                Accès direct niveau 3
                              </a>
                            </li>
                          </ul>
                        </div>
                      </li>
                      <li class="fr-sidemenu__item">
                        <a class="fr-sidemenu__link" href="#" target="_self"
                          >Accès direct niveau 2</a
                        >
                      </li>
                      <li class="fr-sidemenu__item">
                        <a class="fr-sidemenu__link" href="#" target="_self"
                          >Accès direct niveau 2</a
                        >
                      </li>
                      <li class="fr-sidemenu__item">
                        <a class="fr-sidemenu__link" href="#" target="_self"
                          >Accès direct niveau 2</a
                        >
                      </li>
                      <li class="fr-sidemenu__item">
                        <a class="fr-sidemenu__link" href="#" target="_self"
                          >Accès direct niveau 2</a
                        >
                      </li>
                    </ul>
                  </div>
                </li>
                <li class="fr-sidemenu__item">
                  <a class="fr-sidemenu__link" href="#" target="_self"
                    >Accès direct</a
                  >
                </li>
                <li class="fr-sidemenu__item">
                  <button
                    class="fr-sidemenu__btn"
                    aria-expanded="false"
                    aria-controls="fr-sidemenu-item-6"
                  >
                    Niveau 1
                  </button>
                  <div class="fr-collapse" id="fr-sidemenu-item-6">
                    <ul class="fr-sidemenu__list">
                      <li class="fr-sidemenu__item">
                        <a class="fr-sidemenu__link" href="#" target="_self"
                          >Accès direct niveau 2</a
                        >
                      </li>
                      <li class="fr-sidemenu__item">
                        <a class="fr-sidemenu__link" href="#" target="_self"
                          >Accès direct niveau 2</a
                        >
                      </li>
                      <li class="fr-sidemenu__item">
                        <button
                          class="fr-sidemenu__btn"
                          aria-expanded="false"
                          aria-controls="fr-sidemenu-item-6-sub"
                        >
                          Niveau 2
                        </button>
                        <div class="fr-collapse" id="fr-sidemenu-item-6-sub">
                          <ul class="fr-sidemenu__list">
                            <li class="fr-sidemenu__item">
                              <a class="fr-sidemenu__link" href="#" target="_self">
                                Accès direct niveau 3
                              </a>
                            </li>
                            <li class="fr-sidemenu__item">
                              <a class="fr-sidemenu__link" href="#" target="_self">
                                Accès direct niveau 3
                              </a>
                            </li>
                            <li class="fr-sidemenu__item">
                              <a class="fr-sidemenu__link" href="#" target="_self">
                                Accès direct niveau 3
                              </a>
                            </li>
                            <li class="fr-sidemenu__item">
                              <a class="fr-sidemenu__link" href="#" target="_self">
                                Accès direct niveau 3
                              </a>
                            </li>
                            <li class="fr-sidemenu__item">
                              <a class="fr-sidemenu__link" href="#" target="_self">
                                Accès direct niveau 3
                              </a>
                            </li>
                            <li class="fr-sidemenu__item">
                              <a class="fr-sidemenu__link" href="#" target="_self">
                                Accès direct niveau 3
                              </a>
                            </li>
                          </ul>
                        </div>
                      </li>
                      <li class="fr-sidemenu__item">
                        <a class="fr-sidemenu__link" href="#" target="_self"
                          >Accès direct niveau 2</a
                        >
                      </li>
                      <li class="fr-sidemenu__item">
                        <a class="fr-sidemenu__link" href="#" target="_self"
                          >Accès direct niveau 2</a
                        >
                      </li>
                      <li class="fr-sidemenu__item">
                        <a class="fr-sidemenu__link" href="#" target="_self"
                          >Accès direct niveau 2</a
                        >
                      </li>
                      <li class="fr-sidemenu__item">
                        <a class="fr-sidemenu__link" href="#" target="_self"
                          >Accès direct niveau 2</a
                        >
                      </li>
                    </ul>
                  </div>
                </li>
                <li class="fr-sidemenu__item">
                  <button
                    class="fr-sidemenu__btn"
                    aria-expanded="false"
                    aria-controls="fr-sidemenu-item-7"
                  >
                    Niveau 1
                  </button>
                  <div class="fr-collapse" id="fr-sidemenu-item-7">
                    <ul class="fr-sidemenu__list">
                      <li class="fr-sidemenu__item">
                        <a class="fr-sidemenu__link" href="#" target="_self"
                          >Accès direct niveau 2</a
                        >
                      </li>
                      <li class="fr-sidemenu__item">
                        <a class="fr-sidemenu__link" href="#" target="_self"
                          >Accès direct niveau 2</a
                        >
                      </li>
                      <li class="fr-sidemenu__item">
                        <button
                          class="fr-sidemenu__btn"
                          aria-expanded="false"
                          aria-controls="fr-sidemenu-item-7-sub"
                        >
                          Niveau 2
                        </button>
                        <div class="fr-collapse" id="fr-sidemenu-item-7-sub">
                          <ul class="fr-sidemenu__list">
                            <li class="fr-sidemenu__item">
                              <a class="fr-sidemenu__link" href="#" target="_self">
                                Accès direct niveau 3
                              </a>
                            </li>
                            <li class="fr-sidemenu__item">
                              <a class="fr-sidemenu__link" href="#" target="_self">
                                Accès direct niveau 3
                              </a>
                            </li>
                            <li class="fr-sidemenu__item">
                              <a class="fr-sidemenu__link" href="#" target="_self">
                                Accès direct niveau 3
                              </a>
                            </li>
                            <li class="fr-sidemenu__item">
                              <a class="fr-sidemenu__link" href="#" target="_self">
                                Accès direct niveau 3
                              </a>
                            </li>
                            <li class="fr-sidemenu__item">
                              <a class="fr-sidemenu__link" href="#" target="_self">
                                Accès direct niveau 3
                              </a>
                            </li>
                            <li class="fr-sidemenu__item">
                              <a class="fr-sidemenu__link" href="#" target="_self">
                                Accès direct niveau 3
                              </a>
                            </li>
                          </ul>
                        </div>
                      </li>
                      <li class="fr-sidemenu__item">
                        <a class="fr-sidemenu__link" href="#" target="_self"
                          >Accès direct niveau 2</a
                        >
                      </li>
                      <li class="fr-sidemenu__item">
                        <a class="fr-sidemenu__link" href="#" target="_self"
                          >Accès direct niveau 2</a
                        >
                      </li>
                      <li class="fr-sidemenu__item">
                        <a class="fr-sidemenu__link" href="#" target="_self"
                          >Accès direct niveau 2</a
                        >
                      </li>
                      <li class="fr-sidemenu__item">
                        <a class="fr-sidemenu__link" href="#" target="_self"
                          >Accès direct niveau 2</a
                        >
                      </li>
                    </ul>
                  </div>
                </li>
                <li class="fr-sidemenu__item">
                  <a class="fr-sidemenu__link" href="#" target="_self"
                    >Accès direct</a
                  >
                </li>
                <li class="fr-sidemenu__item">
                  <button
                    class="fr-sidemenu__btn"
                    aria-expanded="false"
                    aria-controls="fr-sidemenu-item-9"
                  >
                    Niveau 1
                  </button>
                  <div class="fr-collapse" id="fr-sidemenu-item-9">
                    <ul class="fr-sidemenu__list">
                      <li class="fr-sidemenu__item">
                        <a class="fr-sidemenu__link" href="#" target="_self"
                          >Accès direct niveau 2</a
                        >
                      </li>
                      <li class="fr-sidemenu__item">
                        <a class="fr-sidemenu__link" href="#" target="_self"
                          >Accès direct niveau 2</a
                        >
                      </li>
                      <li class="fr-sidemenu__item">
                        <button
                          class="fr-sidemenu__btn"
                          aria-expanded="false"
                          aria-controls="fr-sidemenu-item-9-sub"
                        >
                          Niveau 2
                        </button>
                        <div class="fr-collapse" id="fr-sidemenu-item-9-sub">
                          <ul class="fr-sidemenu__list">
                            <li class="fr-sidemenu__item">
                              <a class="fr-sidemenu__link" href="#" target="_self">
                                Accès direct niveau 3
                              </a>
                            </li>
                            <li class="fr-sidemenu__item">
                              <a class="fr-sidemenu__link" href="#" target="_self">
                                Accès direct niveau 3
                              </a>
                            </li>
                            <li class="fr-sidemenu__item">
                              <a class="fr-sidemenu__link" href="#" target="_self">
                                Accès direct niveau 3
                              </a>
                            </li>
                            <li class="fr-sidemenu__item">
                              <a class="fr-sidemenu__link" href="#" target="_self">
                                Accès direct niveau 3
                              </a>
                            </li>
                            <li class="fr-sidemenu__item">
                              <a class="fr-sidemenu__link" href="#" target="_self">
                                Accès direct niveau 3
                              </a>
                            </li>
                            <li class="fr-sidemenu__item">
                              <a class="fr-sidemenu__link" href="#" target="_self">
                                Accès direct niveau 3
                              </a>
                            </li>
                          </ul>
                        </div>
                      </li>
                      <li class="fr-sidemenu__item">
                        <a class="fr-sidemenu__link" href="#" target="_self"
                          >Accès direct niveau 2</a
                        >
                      </li>
                      <li class="fr-sidemenu__item">
                        <a class="fr-sidemenu__link" href="#" target="_self"
                          >Accès direct niveau 2</a
                        >
                      </li>
                      <li class="fr-sidemenu__item">
                        <a class="fr-sidemenu__link" href="#" target="_self"
                          >Accès direct niveau 2</a
                        >
                      </li>
                      <li class="fr-sidemenu__item">
                        <a class="fr-sidemenu__link" href="#" target="_self"
                          >Accès direct niveau 2</a
                        >
                      </li>
                    </ul>
                  </div>
                </li>
              </ul>
            </div>
          </div>
        </nav>
                          
                        

## Déclinaisons

Le menu latéral peut également être utilisé :

  * en version fixe pour rester affiché tout au long de la navigation 
  * en version fixe et avec une hauteur qui prend 100% de votre page.
  * à droite de votre page 

### Menu latéral fixe

Le menu latéral peut également s’afficher de manière fixe sur votre page, afin
de rester visible tout au long de la navigation de l’utilisateur sur la page
ouverte.

Pour cela il suffit d’associer à l'élément `<nav>` la classe css `fr-sidemenu`
avec le modificateur `fr-sidemenu--sticky`

![Mise en situation d'un menu latéral dans une
page<br>](/uploads/Capture_d_ecran_2020_10_08_a_08_24_51_d2ba5f253f.png)

### Menu latéral fixe, affiché sur 100% de la hauteur de page

Enfin vous pouvez afficher un menu latéral fixe sur 100% de la hauteur de
votre page.

Pour cela il suffit d’associer à l'élément `<nav>` la classe a classe `fr-
sidemenu` avec le modificateur `fr-sidemenu--sticky-full-height` .

![](/uploads/Capture_d_ecran_2020_10_08_a_08_26_18_9a40425123.png)

### Menu latéral à droite de la page

Lorsque le menu est placé à droite de la page, il est nécessaire d’associer à
l'élément `<nav>` la classe `fr-sidemenu` avec le modificateur `fr-sidemenu--
right` afin que la bordure se positionne à gauche du menu. On peut également
le rendre fixe avec la classe `fr-sidemenu--sticky`.

## Responsive

En version mobile, le menu latéral est masqué par défaut et est remplacé par
le bouton ‘Dans cette rubrique'. Au clic sur ce dernier, le menu se déplie et
affiche l’ensemble de la liste de liens.

![](/uploads/Capture_d_ecran_2020_09_25_a_15_52_57_0c4b652c43.png)

## Règles d’utilisation

### Usages

Les pages accessibles depuis le menu latéral, ne sont pas des pages rattachées
à la navigation principale.

Indiquez où se trouve l'utilisateur dans la hiérarchie de navigation en
affichant la page active. Pour cela, utilisez l'état «actif» sur l'élément de
menu correspondant à la page courante.

Par défaut, intégrer le titre de rubrique pour donner un repère à
l’utilisateur.

Le menu latéral peut être éventuellement caché en version mobile grace au
modificateur “…”. Dans ce cas, il faut réintégrer ces éléments de navigation
dans le menu burger.

### Accessibilité

Le ‘titre de rubrique’ - si présent - est placé dans une balise <hx> dont le
niveau dépend du parent.

### Contenus

Le titre des liens du menu latéral peuvent être raccourcis par rapport aux
titres véritables des pages.

### Personnalisation

Ce composant n’est pas personnalisable.

### Besoin d'aide ?

L'équipe du DSFR est là pour vous aider.

Retrouvez-la sur :

  * [la communauté slack](https://gouvfr.slack.com/ "la communauté slack - nouvelle fenêtre") pour poser vos questions, et échanger avec d’autres utilisateurs.   
Vous êtes **agent de l’État** et souhaitez accéder au slack ? [Rejoignez la
communauté](https://gouvfr.atlassian.net/servicedesk/customer/portal/1/group/1/create/9
"Rejoignez la communauté - nouvelle fenêtre") dès maintenant !

  * [ le centre de support](https://gouvfr.atlassian.net/servicedesk/customer/portals "le centre de support - nouvelle fenêtre") pour envoyer vos demandes de correctifs et d'évolution.

[Liste déroulante - Select](/composants-et-modeles/composants/liste-
deroulante)

[Mise en avant - Callout](/composants-et-modeles/composants/mise-en-avant)

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
