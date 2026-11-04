# basecamp-redesign

# Cahier des charges --- Refonte du site vitrine Basecamp

**Projet :** Basecamp Redesign\
**Périmètre :** Site vitrine\
**Pages :** Accueil, Tarifs, Contact\
**Équipe :** 3 membres\
**Technologies :** HTML5, CSS3 et JavaScript natif\
**Date :** 4 Novembre 2026

------------------------------------------------------------------------

## 1. Présentation générale

### 1.1. Contexte

Dans le cadre d'un projet de développement web, le groupe doit réaliser
la refonte d'un site web existant. Le choix s'est porté sur
[Basecamp](https://basecamp.com/), une plateforme de gestion de projets
et de collaboration qui permet aux équipes de centraliser leurs tâches,
leurs communications et leurs ressources.

La mission consiste à concevoir une nouvelle version de son **site
vitrine**, avec une interface moderne, une navigation intuitive et une
expérience adaptée aux ordinateurs, tablettes et smartphones.

### 1.2. Objectifs

Le projet doit permettre de :

1.  Reprendre les principales informations du site vitrine original.
2.  Moderniser l'identité visuelle et l'expérience utilisateur.
3.  Améliorer la navigation et l'organisation des informations.
4.  Développer un site entièrement responsive.
5.  Ajouter des interactions en JavaScript natif.
6.  Respecter les bonnes pratiques HTML5 et CSS3.
7.  Produire un code propre, organisé, réutilisable et maintenable.

### 1.3. Périmètre

Le projet comprend trois pages :

-   **Accueil :** présentation de Basecamp et de ses avantages.
-   **Tarifs :** présentation et comparaison des offres.
-   **Contact :** informations de contact et formulaire interactif.

Le projet ne comprend pas la création d'une véritable application de
gestion de projets, d'un espace membre, d'une authentification ou d'un
système de paiement.

------------------------------------------------------------------------

## 2. Contraintes techniques

  Technologie       Utilisation
  ----------------- --------------------------------------------
  HTML5             Structure et contenu des pages
  CSS3              Mise en page, design et responsive
  JavaScript ES6+   Interactions et validation des formulaires

### Technologies interdites

-   PHP ;
-   Bootstrap ;
-   Frameworks CSS;
-   JS du type Bootstrap.

Le site doit être statique.
Il peut être ouvert directement depuis `index.html`.

------------------------------------------------------------------------

## 3. Description fonctionnelle des pages

### 3.1. Page Accueil --- `index.html`

**Objectif :** présenter Basecamp, expliquer sa valeur et inciter les
visiteurs à découvrir le produit.

Sections prévues :

  -----------------------------------------------------------------------
  Section                             Contenu
  ----------------------------------- -----------------------------------
  Header                              Logo, navigation, boutons d'action

  Hero                                Titre principal, description, appel
                                      à l'action et illustration

  Présentation                        Problèmes que Basecamp aide à
                                      résoudre

  Fonctionnalités                     Tâches, discussions, calendrier,
                                      fichiers et collaboration

  Démonstration                       Illustration d'une interface de
                                      projet

  Avantages                           Simplicité, centralisation et
                                      collaboration

  Témoignages                         Exemples de témoignages clairement
                                      identifiés comme fictifs si non
                                      vérifiés

  CTA                                 Invitation à découvrir ou essayer
                                      Basecamp

  Footer                              Liens de navigation, informations
                                      et réseaux sociaux
  -----------------------------------------------------------------------

Améliorations envisagées :

-   créer un hero avec une hiérarchie visuelle claire ;
-   présenter le produit à l'aide d'une illustration ou d'une maquette
    de tableau de bord ;
-   utiliser des cartes de fonctionnalités avec des icônes cohérentes ;
-   intégrer des animations discrètes au défilement ;
-   conserver une navigation facilement accessible pendant le scroll.

### 3.2. Page Tarifs --- `tarifs.html`

**Objectif :** présenter les formules de manière claire et permettre aux
visiteurs de comparer les offres.

Sections prévues :

1.  Introduction à la tarification.
2.  Cartes présentant les différentes formules.
3.  Comparaison des fonctionnalités.
4.  Questions fréquentes.
5.  Appels à l'action.

Améliorations envisagées :

-   concevoir des cartes tarifaires lisibles ;
-   ajouter un tableau comparatif des fonctionnalités ;
-   proposer un sélecteur mensuel/annuel si les données le justifient ;
-   mettre en évidence une formule recommandée sans tromper
    l'utilisateur ;
-   intégrer une FAQ sous forme d'accordéon.

**Point de vigilance :** les prix et les formules de Basecamp peuvent
évoluer. Les informations affichées devront être vérifiées sur la [page
officielle des tarifs](https://basecamp.com/pricing) au moment de la
réalisation. Ne pas inventer de prix ni présenter des tarifs fictifs
comme des tarifs officiels.

### 3.3. Page Contact --- `contact.html`

**Objectif :** permettre aux visiteurs de préparer une demande de
contact facilement.

Sections prévues :

-   introduction ;
-   informations de contact vérifiées ;
-   formulaire ;
-   motif de la demande ;
-   FAQ courte, si pertinente ;
-   footer.

Champs du formulaire :

  -----------------------------------------------------------------------
  Champ                   Type                    Règle
  ----------------------- ----------------------- -----------------------
  Nom complet             `text`                  Obligatoire

  Adresse e-mail          `email`                 Obligatoire et format
                                                  valide

  Sujet                   `select`                Choix parmi des motifs
                                                  proposés

  Message                 `textarea`              Obligatoire, longueur
                                                  minimale définie

  Confidentialité         `checkbox`              Consentement si
                                                  nécessaire au scénario
                                                  retenu
  -----------------------------------------------------------------------

Interactions JavaScript :

-   vérifier les champs obligatoires ;
-   valider le format de l'adresse e-mail ;
-   contrôler la longueur du message ;
-   afficher les erreurs à proximité des champs ;
-   afficher un message de confirmation après validation.

**Limitation importante :** sans backend ni service d'envoi externe, le
formulaire ne transmet pas réellement les messages. Dans ce cas,
afficher clairement qu'il s'agit d'une démonstration et ne pas laisser
croire qu'une demande a été envoyée à Basecamp.

------------------------------------------------------------------------

## 4. Identité visuelle proposée

La direction artistique doit être moderne, professionnelle, chaleureuse
et minimaliste. Elle peut s'inspirer de l'esprit de Basecamp sans copier
exactement son interface.

### 4.1. Palette de couleurs

  -----------------------------------------------------------------------
  Couleur                 Code hexadécimal        Utilisation
  ----------------------- ----------------------- -----------------------
  Bleu foncé              `#163A5B`               Titres, éléments forts
                                                  et boutons principaux

  Bleu moyen              `#2E75A8`               Liens, accents et
                                                  éléments interactifs

  Bleu très clair         `#E9F2F8`               Fonds de sections et
                                                  surfaces secondaires

  Gris très clair         `#F7F8FA`               Fond général

  Gris foncé              `#252B33`               Texte principal
  -----------------------------------------------------------------------

### 4.2. Typographies

-   **Manrope :** titres et éléments importants.
-   **Inter :** paragraphes, libellés et textes d'interface.

Les polices peuvent être intégrées localement ou chargées depuis une
source externe autorisée par les consignes du projet. Prévoir des
polices de remplacement.

### 4.3. Style des composants

-   boutons légèrement arrondis ;
-   cartes sobres ;
-   espaces généreux ;
-   ombres discrètes ;
-   illustrations cohérentes ;
-   transitions courtes et non intrusives ;
-   états visibles au survol, au focus et lors de l'activation.

------------------------------------------------------------------------

## 5. Responsive design

Le site doit s'adapter à trois grandes catégories d'écrans.

  ------------------------------------------------------------------------
  Format                          Largeur indicative Comportement attendu
  --------------------- ---------------------------- ---------------------
  Mobile                             Moins de 768 px Une colonne, menu
                                                     hamburger, boutons
                                                     adaptés au tactile

  Tablette                             768 à 1023 px Grilles réduites et
                                                     navigation adaptée

  Ordinateur                         1024 px et plus Mise en page complète
                                                     et grilles
                                                     multi-colonnes
  ------------------------------------------------------------------------

Règles respectées :

-   aucun débordement horizontal ;
-   images adaptatives avec `max-width: 100%` ;
-   menu hamburger sur mobile ;
-   cartes passant de plusieurs colonnes à une seule ;
-   tailles de texte adaptées aux écrans ;
-   zones cliquables suffisamment grandes ;
-   tableaux tarifaires consultables sur petits écrans, par exemple dans
    un conteneur avec défilement horizontal contrôlé ;
-   tests sur plusieurs largeurs, et pas uniquement sur un appareil
    précis.

------------------------------------------------------------------------

## 6. Fonctionnalités JavaScript

  Fonctionnalité               Page      Priorité
  ---------------------------- --------- -------------
  Menu hamburger               Toutes    Obligatoire
  Navigation et état actif     Toutes    Obligatoire
  FAQ accordéon                Tarifs    Obligatoire
  Comparaison mensuel/annuel   Tarifs    Facultatif
  Validation du formulaire     Contact   Obligatoire
  Message de confirmation      Contact   Obligatoire
  Animations au défilement     Accueil   Facultatif
  Bouton retour en haut        Toutes    Facultatif
  Thème clair/sombre           Toutes    Facultatif

Les interactions sont utiles, accessibles au clavier et
fonctionnent sans framework JavaScript.

------------------------------------------------------------------------

## 7. Architecture des fichiers

Arborescence recommandée :

``` text
basecamp-redesign/
│
├── index.html
├── tarifs.html
├── contact.html
│
├── assets/
│   ├── images/
│   │   ├── hero-dashboard.webp
│   │   ├── collaboration.webp
│   │   └── testimonials/
│   ├── icons/
│   └── fonts/
│
├── css/
│   ├── variables.css
│   ├── reset.css
│   ├── global.css
│   ├── components.css
│   ├── accueil.css
│   ├── tarifs.css
│   ├── contact.css
│   └── responsive.css
│
├── js/
│   ├── main.js
│   ├── navigation.js
│   ├── tarifs.js
│   ├── contact.js
│   └── animations.js
│
└── README.md
```

### Rôle des fichiers CSS

-   `variables.css` : couleurs, polices, espacements et variables
    globales.
-   `reset.css` : harmonisation des styles par défaut du navigateur.
-   `global.css` : règles communes aux pages.
-   `components.css` : boutons, cartes, formulaires et composants
    réutilisables.
-   `accueil.css`, `tarifs.css`, `contact.css` : styles spécifiques aux
    pages.
-   `responsive.css` : adaptations aux différentes tailles d'écran.

Cette organisation est une proposition : elle peut être simplifiée si le
projet reste de taille modeste. Il faut éviter de multiplier inutilement
les fichiers.

------------------------------------------------------------------------

## 8. Répartition du travail entre les trois membres

La répartition se fait par responsabilités. Chaque membre reste
responsable du responsive et des tests de sa propre page.

### Membre 1 : KEEDY --- Page Accueil

Responsabilités :

-   développer `index.html` ;
-   réaliser le header et les sections de présentation de l'accueil, en
    coordination avec le membre chargé de l'intégration ;
-   créer les sections Hero, fonctionnalités et avantages ;
-   intégrer les illustrations ;
-   développer les interactions propres à l'accueil ;
-   rendre la page responsive.

**Livrable :** page d'accueil intégrée et responsive.

### Membre 2 : REDOUANE --- Page Tarifs

Responsabilités :

-   développer `tarifs.html` ;
-   concevoir les cartes tarifaires ;
-   vérifier les informations tarifaires utilisées ;
-   réaliser le comparateur ;
-   développer la FAQ interactive ;
-   rendre la page responsive.

**Livrable :** page tarifs fonctionnelle et responsive.

### Membre 3 : MELVINE --- Page Contact

Responsabilités :

-   développer `contact.html` ;
-   concevoir le formulaire ;
-   implémenter la validation JavaScript ;
-   gérer les messages d'erreur et de confirmation ;
-   vérifier l'accessibilité des champs ;
-   rendre la page responsive.

**Livrable :** page contact fonctionnelle côté navigateur et responsive.

### Groupe --- Intégration, design system et qualité

Responsabilités :

-   définir les variables CSS et la charte graphique ;
-   préparer les composants communs ;
-   coordonner l'intégration du header et du footer ;
-   centraliser les règles responsive communes ;
-   vérifier les liens et la cohérence entre les pages ;
-   organiser les tests et la qualité du code ;
-   maintenir le README et coordonner les fusions Git.

**Livrable :** site harmonisé, intégré, documenté et testé.

------------------------------------------------------------------------

## 9. Organisation du travail avec Git et GitHub

Branches :

``` text
main
└── develop
    ├── feature/accueil
    ├── feature/tarifs
    └─── feature/contact
```

Type de messages de commit :

``` text
feat: add homepage hero section
feat: create pricing cards
feat: validate contact form
style: improve mobile navigation
fix: correct responsive layout
docs: update project README
```

------------------------------------------------------------------------

## 10. Livrables finaux

  Livrable             Description
  -------------------- ------------------------------------------------
  Maquettes Figma      Maquettes des trois pages
  Code source          HTML, CSS et JavaScript
  Dépôt GitHub         Historique du développement
  Site responsive      Version finale fonctionnelle
  README.md            Instructions de lancement et d'utilisation
  Présentation orale   Explication des choix techniques et graphiques

------------------------------------------------------------------------

## 11. Recommandations utilisées pour réussir le projet (proposées par Claude)

1.  **Cohérence visuelle :** les trois pages doivent donner l'impression
    d'appartenir au même site.
2.  **Responsive réel :** ne pas simplement réduire les éléments ;
    adapter la disposition et la navigation.
3.  **JavaScript utile :** chaque interaction doit répondre à un besoin
    utilisateur.
4.  **Qualité du code :** utiliser un HTML sémantique, un CSS organisé
    et un JavaScript modulaire.
5.  **Expérience utilisateur :** privilégier une navigation intuitive,
    un chargement rapide et un contenu compréhensible.
6.  **Fiabilité des informations :** vérifier les prix, les
    fonctionnalités et les coordonnées sur les sources officielles.
7.  **Transparence :** identifier les contenus fictifs et les
    fonctionnalités de démonstration.

Il est préférable de concevoir et de valider les maquettes des trois
pages avant de commencer l'intégration. Une fois la direction artistique
validée par les trois membres, le développement sera plus cohérent et
nécessitera moins de modifications.

------------------------------------------------------------------------

## 12. Ressources de référence

-   [Site officiel de Basecamp](https://basecamp.com/)
-   [Tarifs officiels de Basecamp](https://basecamp.com/pricing)
-   [Présentation de Basecamp](https://basecamp.com/about)
-   [Documentation MDN ---
    HTML](https://developer.mozilla.org/fr/docs/Web/HTML)
-   [Documentation MDN ---
    CSS](https://developer.mozilla.org/fr/docs/Web/CSS)
-   [Documentation MDN ---
    JavaScript](https://developer.mozilla.org/fr/docs/Web/JavaScript)

------------------------------------------------------------------------

**Fin du cahier des charges --- Basecamp Redesign**
