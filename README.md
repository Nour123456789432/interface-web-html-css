
# HTML & CSS — Guide de référence

## Objectif

Comprendre la structure d'une page web, les principales balises HTML, les composants d'interface et les bases du CSS afin de pouvoir créer des pages web de manière autonome.

## 1. HTML, CSS et JavaScript

- **HTML** : structure le contenu de la page.
- **CSS** : définit l'apparence et la disposition des éléments.
- **JavaScript** : ajoute des interactions et des comportements.

À retenir :
- HTML = structure
- CSS = apparence
- JavaScript = comportement

## 2. Structure générale d'une page web

Une page web classique peut être organisée en trois grandes parties :

- **Header** : en-tête de la page.
- **Main** : contenu principal.
- **Footer** : pied de page.

```html
<body>
  <header>
    <!-- En-tête -->
  </header>

  <main>
    <!-- Contenu principal -->
    <section>
      <!-- Une section de contenu -->
    </section>
  </main>

  <footer>
    <!-- Pied de page -->
  </footer>
</body>
```

## 3. Les principales parties d'une page web

### Header — En-tête

Généralement placé en haut de la page.

Il peut contenir :
- Un logo ou le nom du site.
- Un menu de navigation.
- Des liens vers différentes pages.
- Une barre de recherche.
- Des boutons d'action.

Balises courantes : `<header>`, `<nav>`, `<a>`, `<button>`.

### Hero Section — Section de présentation

Souvent située au début du contenu principal.

Elle peut contenir :
- Un titre principal (`h1`).
- Un texte de présentation.
- Un bouton ou un lien d'action.
- Une image ou une illustration.

Le terme `hero` désigne une section de conception web, et non une balise HTML spécifique.

### Main — Contenu principal

La balise `<main>` contient le contenu central de la page.

Elle peut contenir :
- Une section de présentation.
- Des informations ou fonctionnalités.
- Des images et des galeries.
- Des cartes (`cards`).
- Des listes.
- Des formulaires.
- Des articles.
- Une FAQ.

### Section — Section thématique

La balise `<section>` regroupe du contenu lié à un même sujet.

Exemple :

```html
<section>
  <h2>Présentation</h2>
  <p>Une description de cette section.</p>
</section>
```

### Article — Contenu autonome

La balise `<article>` représente un contenu pouvant être compris indépendamment, comme un article, une publication ou une actualité.

### Aside — Contenu complémentaire

La balise `<aside>` représente un contenu complémentaire au contenu principal.

Elle peut servir à afficher :
- Des notes.
- Des informations complémentaires.
- Certains menus latéraux.

### Sidebar — Barre latérale

La sidebar est une zone latérale pouvant contenir :
- Un menu secondaire.
- Des filtres.
- Des liens.
- Des informations complémentaires.

`sidebar` n'est pas une balise HTML spécifique. On peut utiliser `<aside>` ou un conteneur avec une classe CSS.

### Footer — Pied de page

Généralement placé en bas de la page.

Il peut contenir :
- Des liens utiles.
- Des informations de contact.
- Des liens vers les réseaux sociaux.
- Des mentions légales.
- Le copyright.

La balise `<footer>` peut également représenter le pied de page d'un article ou d'une section.

## 4. Les composants d'interface courants

| Composant | Rôle |
|---|---|
| Logo | Identifier le site ou le projet |
| Navigation | Permettre de naviguer entre les pages |
| Search bar | Rechercher du contenu |
| Card | Présenter une information dans un bloc |
| Form | Collecter des informations |
| Modal | Afficher une fenêtre superposée |
| Dropdown | Afficher un menu déroulant |
| Tabs | Passer entre plusieurs panneaux |
| Breadcrumbs | Montrer le chemin de navigation |
| Pagination | Naviguer entre plusieurs pages de résultats |
| Alert / Toast | Afficher un message d'information |
| Accordion | Déplier ou replier du contenu |

Ces composants sont des concepts d'interface, pas des balises HTML spécifiques. Leur utilisation dépend des besoins du projet.

## 5. Les balises HTML essentielles

| Balise | Utilité |
|---|---|
| `<html>` | Élément racine du document |
| `<head>` | Contient les métadonnées |
| `<title>` | Définit le titre de l'onglet |
| `<body>` | Contient le contenu de la page |
| `<header>` | Définit un en-tête |
| `<nav>` | Définit une zone de navigation |
| `<main>` | Définit le contenu principal |
| `<section>` | Regroupe un contenu thématique |
| `<article>` | Définit un contenu autonome |
| `<aside>` | Définit un contenu complémentaire |
| `<footer>` | Définit un pied de page |
| `<div>` | Conteneur générique |
| `<h1>` à `<h6>` | Définit des titres hiérarchisés |
| `<p>` | Définit un paragraphe |
| `<a>` | Crée un lien |
| `<button>` | Crée un bouton d'action |
| `<img>` | Affiche une image |
| `<ul>` | Crée une liste non ordonnée |
| `<ol>` | Crée une liste ordonnée |
| `<li>` | Définit un élément de liste |
| `<form>` | Crée un formulaire |
| `<label>` | Définit l'étiquette d'un champ |
| `<input>` | Crée un champ de saisie |
| `<textarea>` | Crée une zone de texte multiligne |
| `<select>` | Crée une liste de choix |
| `<option>` | Définit une option |
| `<strong>` | Indique une importance particulière |
| `<em>` | Met un texte en emphase |

### Bonnes pratiques HTML

- Utiliser les balises selon leur signification.
- Respecter une hiérarchie logique des titres.
- Ajouter un attribut `alt` pertinent aux images informatives.
- Associer les champs de formulaire à des balises `<label>`.
- Utiliser `<a>` pour naviguer et `<button>` pour déclencher une action.
- Indenter le code pour améliorer sa lisibilité.

## 6. Exemple de structure HTML réutilisable

```html
<!DOCTYPE html>
<html lang="fr">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Ma page web</title>
  <link rel="stylesheet" href="style.css">
</head>

<body>

  <header class="site-header">
    <a href="#" class="logo">Mon projet</a>

    <nav aria-label="Navigation principale">
      <a href="#accueil">Accueil</a>
      <a href="#informations">Informations</a>
      <a href="#contact">Contact</a>
    </nav>
  </header>

  <main>

    <section class="hero" id="accueil">
      <h1>Titre principal</h1>
      <p>Une courte description de la page.</p>
      <a href="#informations">En savoir plus</a>
    </section>

    <section class="content" id="informations">
      <h2>Une section de contenu</h2>

      <article class="card">
        <h3>Titre de la carte</h3>
        <p>Description de cet élément.</p>
      </article>
    </section>

  </main>

  <footer id="contact" class="site-footer">
    <p>&copy; 2026 — Mon projet</p>
  </footer>

</body>
</html>
```

## 7. Les bases du CSS

Le CSS permet de contrôler les couleurs, les dimensions, les espacements, la typographie et la disposition des éléments.

### Comprendre une règle CSS

```css
.card {
  padding: 20px;
  border: 1px solid #dddddd;
  border-radius: 12px;
}
```

- `.card` : sélecteur de classe.
- `padding` : propriété CSS.
- `20px` : valeur de la propriété.

### Les propriétés CSS importantes

| Propriété | Utilité |
|---|---|
| `color` | Couleur du texte |
| `background-color` | Couleur de fond |
| `font-family` | Police de caractères |
| `font-size` | Taille du texte |
| `font-weight` | Épaisseur du texte |
| `margin` | Espace extérieur |
| `padding` | Espace intérieur |
| `border` | Bordure |
| `border-radius` | Arrondi des coins |
| `width` | Largeur |
| `max-width` | Largeur maximale |
| `height` | Hauteur |
| `display` | Type d'affichage |
| `gap` | Espace entre les éléments |
| `justify-content` | Répartition des éléments avec Flexbox |
| `align-items` | Alignement des éléments avec Flexbox |
| `grid-template-columns` | Organisation des colonnes avec Grid |
| `position` | Mode de positionnement |
| `@media` | Adaptation à certaines conditions d'écran |

## 8. Exemple CSS réutilisable

```css
* {
  box-sizing: border-box;
}

body {
  margin: 0;
  font-family: Arial, sans-serif;
  line-height: 1.5;
  color: #222222;
}

.site-header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  gap: 20px;
  padding: 16px 24px;
}

nav {
  display: flex;
  flex-wrap: wrap;
  gap: 16px;
}

nav a {
  color: inherit;
  text-decoration: none;
}

main {
  width: min(100% - 32px, 1100px);
  margin-inline: auto;
}

.hero {
  padding-block: 64px;
  text-align: center;
}

.card {
  padding: 20px;
  border: 1px solid #dddddd;
  border-radius: 12px;
}

.site-footer {
  margin-top: 48px;
  padding: 24px;
  text-align: center;
  background-color: #f3f4f6;
}

@media (max-width: 600px) {
  .site-header {
    align-items: flex-start;
    flex-direction: column;
  }

  .hero {
    padding-block: 40px;
  }
}
```

## 9. Flexbox, Grid et Responsive Design

### Flexbox

Flexbox facilite l'alignement des éléments dans une direction.

Exemples :
- Aligner un logo et un menu.
- Répartir des boutons.
- Centrer du contenu.

### CSS Grid

Grid facilite l'organisation des éléments en lignes et en colonnes.

Exemples :
- Afficher plusieurs cartes.
- Construire une galerie.
- Organiser une mise en page en plusieurs zones.

### Responsive Design

Le responsive design adapte la page aux différentes tailles d'écran : téléphone, tablette et ordinateur.

Bonnes pratiques :
- Utiliser des largeurs flexibles.
- Éviter les largeurs fixes inadaptées.
- Tester la navigation sur mobile.
- Utiliser les media queries lorsque nécessaire.
- Vérifier que le texte reste lisible.

## 10. Méthode pour construire une page web

1. Comprendre l'objectif de la page.
2. Identifier les informations nécessaires.
3. Dessiner un wireframe simple.
4. Organiser les grandes parties : header, main et footer.
5. Construire la structure HTML.
6. Ajouter les styles CSS.
7. Organiser les éléments avec Flexbox ou Grid.
8. Adapter la page aux différentes tailles d'écran.
9. Tester les liens, boutons et formulaires.
10. Vérifier l'accessibilité et la lisibilité.

## 11. Checklist de vérification

- [ ] La page possède un titre clair.
- [ ] La structure HTML est logique.
- [ ] Les titres suivent une hiérarchie compréhensible.
- [ ] Les liens et les boutons ont le bon rôle.
- [ ] Les images informatives ont un texte alternatif pertinent.
- [ ] Les champs de formulaire possèdent des labels.
- [ ] Le CSS est lisible et organisé.
- [ ] La page fonctionne sur téléphone et ordinateur.
- [ ] Les liens et les interactions ont été testés.
- [ ] Les composants utilisés répondent à un besoin réel.

## 12. Mini-quiz

1. Quelle est la différence entre HTML et CSS ?
2. Quelle balise contient le contenu principal ?
3. Quelle est la différence entre `<a>` et `<button>` ?
4. Est-ce que `hero` est une balise HTML ?
5. Quand utiliser Flexbox ?
6. Quand utiliser CSS Grid ?
7. Pourquoi le responsive design est-il important ?
8. Quelle est la différence entre `margin` et `padding` ?

### Réponses

1. HTML structure le contenu ; CSS contrôle son apparence et sa disposition.
2. `<main>`.
3. `<a>` sert à naviguer vers une destination ; `<button>` sert généralement à déclencher une action.
4. Non. `hero` est un nom courant de section, souvent représenté par `<section class="hero">`.
5. Pour aligner et répartir des éléments principalement dans une direction.
6. Pour organiser les éléments en lignes et colonnes.
7. Pour rendre la page utilisable sur différentes tailles d'écran.
8. `margin` est l'espace extérieur à la bordure ; `padding` est l'espace intérieur entre le contenu et la bordure.

---

## Conseil d'apprentissage

Pour chaque élément, pose-toi quatre questions :

1. À quoi sert-il ?
2. Quel contenu doit-il contenir ?
3. Quelle balise HTML exprime correctement son rôle ?
4. Quel CSS permet d'obtenir la disposition souhaitée ?

**L'objectif n'est pas de mémoriser toutes les balises, mais de comprendre quand et pourquoi les utiliser.**

