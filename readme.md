# 🌀 Arcane Quote Generator

Ce projet est un générateur de citations aléatoires inspiré de la série **Arcane**. Il sélectionne dynamiquement une citation et l'affiche dans le navigateur avec un style visuel personnalisé pour chaque personnage.

## 🚀 Fonctionnalités

- Affichage aléatoire de citations tirées de l'univers **Arcane**
- Utilisation d'un tableau d'objets contenant des métadonnées comme la source, l'année, la voix ou le nombre d'épisodes
- Rafraîchissement automatique de la citation toutes les 15 secondes
- Changement de fond en fonction du personnage cité
- Bouton pour générer manuellement une nouvelle citation

## 🧠 Structure du projet

### 1. `quotes[]`

Un tableau d’objets contenant :

- `quote`: le texte de la citation
- `source`: le personnage
- `citation`: l’œuvre ou la saison (optionnel)
- `year`: l'année (optionnel)
- `voice`: l’acteur/actrice de voix (optionnel)
- `episodes`: nombre d’épisodes dans lesquels le personnage apparaît (optionnel)

### 2. `getRandomQuote()`

Retourne un objet aléatoire depuis le tableau `quotes`.

### 3. `printQuote()`

- Appelle `getRandomQuote()`
- Génère dynamiquement une chaîne HTML avec les infos pertinentes (citation, source, etc.)
- Met à jour le contenu du `<div id="quote-box">`
- Change aussi le **background** via `colorQuote()` selon le personnage cité

### 4. `colorQuote()`

Au lieu d’un code couleur généré aléatoirement, j’ai pris la liberté d’associer un **dégradé représentatif à chaque personnage**. Cela renforce visuellement l’identité de chaque figure de l’univers **Arcane**.

### 5. Rafraîchissement automatique

Un `setInterval()` appelle `printQuote()` toutes les **15 secondes**, pour garder l’interface vivante.

---
