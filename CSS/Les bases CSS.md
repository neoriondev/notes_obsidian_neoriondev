# Notes de cours : CSS
## 1. Principes de base

- Éviter les animations en boucle : Limiter au maximum leur utilisation pour améliorer la performance du site.

- Pas de CSS dans le HTML : Ne pas inclure de styles directement dans les balises HTML.

    Exemple à éviter :

```html

<style> h1 { color: red; } </style>
```

**Bonne pratique :** fichier CSS séparé : Créer un fichier externe pour le CSS (ex : style.css) et le lier au HTML.

Lien dans le fichier HTML :

```html

<link href="style.css" rel="stylesheet">
```

Il est recommandé de placer cette ligne dans la balise <head>, en mettant le nom du fichier au début du chemin si possible.

- Vider le cache : Pour visualiser les modifications en CSS, utiliser le raccourci Ctrl (Fn) + F5 pour vider le cache du navigateur.

- Ressources fiables :

    W3C pour des informations fiables.
    Stack Overflow pour des questions/réponses.

## 2. Les Sélecteurs en CSS

    Le sélecteur est la partie avant dans une règle CSS, exemple :

```css

h1 {
  color: red;
}
```

Pour appliquer la même règle à plusieurs éléments, on peut les séparer par une virgule :

```css

h1, h2 {
  color: red;
}
```
Sélecteurs descendant : Un simple espace dans les sélecteurs CSS indique une arborescence, exemple :

```css

ul li {
  color: blue;
}
```

##3. Les Classes

- Pour appliquer des styles à des éléments spécifiques, on utilise la classe dans le HTML :

```html

<p class="test">Texte avec style</p>
```

En CSS, cela donne :

```css

.test {
  color: purple;
}
```

- Bonnes pratiques de nommage des classes :

    Utiliser des noms clairs et descriptifs pour distinguer les classes.
    Si le nom contient plusieurs mots, utiliser le format lowerCamelCase ou snake_case :
        Exemple : promotionNoel ou promotion_noel
**Ne pas utiliser d'accents ou de caractères spéciaux.**

## 4. Les ID

- Un ID est unique : il ne peut être utilisé qu'une seule fois dans la page.

Exemple en HTML :

```html

<div id="uniqueElement"></div>
```

En CSS, cela donne :

```css

#uniqueElement {
  color: black;
}
```

Les identifiants (ID) sont prioritaires sur les autres sélecteurs (classe, balise, etc.).

**Poids des sélecteurs :**

    Balise = 1 point (ex : h1, h2).
    Classe = 10 points.
    ID = 100 points.

## 5. Les DIV

- La balise <div> permet de regrouper des éléments. Elle peut être associée à une classe ou un ID pour la styliser.

## 6. Autres balises courantes

- Mettre en gras : Utiliser la balise <strong> :

```html

<strong>Texte en gras</strong>
```

- Mettre en italique : Utiliser la balise <em> :

```html

<em>Texte en italique</em>
```

## 7. Liens

    Intégrer un lien en HTML :

```html

<a href="http://google.com">Google</a>
```

Les liens s'affichent par défaut en bleu (cliquables) et deviennent violets lorsqu'ils ont été visités.

### Personnalisation des liens en CSS :

- Pour changer la couleur du lien :

```css

a {
  color: brown;
}
```

- Pour changer la couleur lors du survol (hover) :

```css

a:hover {
  color: aqua;
}
```

- Pour changer la couleur après visite :

```css

a:visited {
  color: purple;
}
```

- Pour personnaliser l'apparence des liens au focus (pour la navigation clavier) :

```css

    a:focus {
      border: 1px dotted black;
    }
```

**Accessibilité : Tous les sites doivent être navigables au clavier, d'où l'importance de gérer les styles de focus.**