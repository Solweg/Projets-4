# Optimisation du site web de photographie

## Vue d'ensemble

Ce projet consiste à déboguer et optimiser le site portfolio d'une photographe, Nina Carducci. L'objectif principal était d'améliorer les performances de chargement, l'accessibilité, ainsi que le référencement (SEO) du site, afin d'offrir une meilleure expérience utilisateur et un meilleur classement dans les moteurs de recherche.

## Outils utilisés

- **Lighthouse** : pour auditer les performances et l'accessibilité du site web.
- **Wave** : pour évaluer et corriger les problèmes d'accessibilité.
- **TinyPNG** : pour la compression des images.
- **Schema.org** : pour mettre en place le référencement local.
- **GitHub** : pour le développement collaboratif et la gestion des versions.

## Optimisations effectuées

### 1. Performances

Les performances du site ont été analysées et optimisées à l'aide de Lighthouse. Voici les principales optimisations réalisées :

- **Images** :
  - Redimensionnement de 15 images originales pour réduire leur poids.
  - Compression des images avec TinyPNG.
  - Conversion des images en format WebP.
  - Ajout des attributs `width` et `height` dans les balises HTML `<img>`.
  - Mise en place du chargement différé (lazy loading) des images pour réduire le temps de chargement initial.

  **Résultat** : Réduction du poids total des images de **21,23 MB** à **0,452 MB** (gain de 97,87 %).

- **Code** :
  - Minification des fichiers CSS et JavaScript non utilisés.
  - Réduction des ressources CSS inutilisées.
  - Suppression des chaînes de requêtes critiques.

- **SEO** :
  - Ajout d'une balise `<title>` optimisée avec la localisation.
  - Ajout d'une balise `<meta description>`.
  - Hiérarchisation des titres avec des balises `<h1>`, `<h2>`, etc.
  - Réorganisation des balises dans `<head>`.
  - Mise en place des balises Open Graph et Twitter Cards pour améliorer le partage sur les réseaux sociaux.
  - Ajout d'une balise `canonical` pour éviter les contenus dupliqués.

### 2. Accessibilité

Les problèmes d'accessibilité ont été identifiés avec l'outil **Wave** et corrigés pour améliorer l'expérience utilisateur :

- Correction de la navigation au clavier et des problèmes de focus.
- Association des éléments de formulaire aux libellés appropriés.
- Amélioration de la lisibilité des contenus en suivant les recommandations d'accessibilité (contrastes, tailles de police, etc.).

### 3. Réalisation des demandes additionnelles du client

- **Référencement local** : Implémentation des balises `itemprop` pour intégrer les données locales à l'aide de **Schema.org**.
- **Débogage de la galerie** :
  - Correction de la navigation dans la modale de la galerie (images suivantes/précédentes).
  - Correction des filtres de la galerie pour afficher la catégorie sélectionnée avec une couleur de fond dorée.

### 4. Rapports d'audit

Les performances et l'accessibilité avant et après optimisation ont été évaluées et comparées. Les scores de Lighthouse montrent une nette amélioration après optimisation :

- **Score des performances avant optimisation** : 77
- **Score des performances après optimisation** : 98
- **Accessibilité avant optimisation** : 68
- **Accessibilité après optimisation** : 98
- **SEO avant optimisation** : 70
- **SEO après optimisation** : 100

## Structure du projet

- `index.html` : Fichier principal de la page d'accueil, optimisé.
- `assets/` : Dossier contenant les images et ressources, compressées et optimisées.
- `css/` : Fichiers CSS minifiés.
- `js/` : Scripts JavaScript optimisés.

## Comment démarrer le projet

Clonez ce dépôt :
```bash
git clone https://github.com/votre-utilisateur/nina-carducci-photographe.git```


Ouvrez le fichier index.html dans votre navigateur pour voir la version optimisée du site.Conclusion

Ce projet a permis d'améliorer considérablement les performances, l'accessibilité et le référencement du site de Nina Carducci. Ces modifications assurent une meilleure visibilité sur les moteurs de recherche et une expérience utilisateur plus fluide.
