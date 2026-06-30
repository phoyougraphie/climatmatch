---
name: ClimatMatch
description: Données météo locales, croyances climatiques et projections lisibles en un coup d’œil.
colors:
  charcoal-bg: "#0E0D0B"
  charcoal-surface: "#161512"
  charcoal-surface-raised: "#1E1C18"
  warm-paper: "#F0EDE6"
  muted-stone: "#A19B94"
  faint-stone: "#514D47"
  cold-blue: "#4A9EE8"
  hot-coral: "#E86A45"
  dry-amber: "#C8901A"
  living-green: "#3A9E6A"
  frost-blue: "#A0C8F0"
  heat-soft: "#F09273"
typography:
  display:
    fontFamily: "DM Serif Display, Georgia, serif"
    fontSize: "clamp(2.4rem, 5.5vw, 4rem)"
    fontWeight: 400
    lineHeight: 1.02
    letterSpacing: "-0.02em"
  headline:
    fontFamily: "DM Serif Display, Georgia, serif"
    fontSize: "clamp(2rem, 5vw, 3rem)"
    fontWeight: 400
    lineHeight: 1.05
  body:
    fontFamily: "Outfit, system-ui, sans-serif"
    fontSize: "16px"
    fontWeight: 400
    lineHeight: 1.5
  label:
    fontFamily: "JetBrains Mono, ui-monospace, monospace"
    fontSize: "11px"
    fontWeight: 500
    letterSpacing: "0.08em"
rounded:
  sm: "10px"
  md: "12px"
  lg: "16px"
spacing:
  xs: "4px"
  sm: "8px"
  md: "12px"
  lg: "16px"
  xl: "24px"
  xxl: "40px"
components:
  button-primary:
    backgroundColor: "{colors.warm-paper}"
    textColor: "{colors.charcoal-bg}"
    rounded: "{rounded.sm}"
    padding: "0.72rem 1.25rem"
    height: "44px"
  button-secondary:
    backgroundColor: "{colors.charcoal-surface}"
    textColor: "{colors.warm-paper}"
    rounded: "{rounded.sm}"
    padding: "0.65rem 0.9rem"
    height: "44px"
  input:
    backgroundColor: "{colors.charcoal-surface}"
    textColor: "{colors.warm-paper}"
    rounded: "{rounded.sm}"
    padding: "0.72rem 0.9rem"
    height: "44px"
  card:
    backgroundColor: "{colors.charcoal-surface}"
    textColor: "{colors.warm-paper}"
    rounded: "{rounded.lg}"
    padding: "1.25rem"
---

# Design System: ClimatMatch

## 1. Overview

**Creative North Star: "Le baromètre sensible"**

ClimatMatch doit ressembler à un instrument de mesure que l’on aurait envie de toucher : sombre, précis, atmosphérique, mais jamais froidement administratif. Le système combine un fond charbon, une typographie éditoriale, un mono technique pour les chiffres, et deux pôles climatiques très lisibles : bleu froid et corail chaud.

Le goût général est sérieux ludique avec une exigence de design. Les chiffres doivent rester souverains, mais leur mise en scène doit aider le corps à comprendre : givre, chaleur, bandes de réchauffement, colonnes simples, périodes saisonnières.

**Key Characteristics:**

- Fond sombre chaud, jamais noir pur.
- Grand contraste entre titres éditoriaux et données mono.
- Palette limitée mais expressive : froid, chaud, pluie, soleil, vivant.
- Surfaces sobres, coins doux, bordures fines, effets atmosphériques contrôlés.
- Une phrase utile sous chaque visualisation, pas de bavardage décoratif.

## 2. Colors

La palette oppose un socle charbon chaud à deux forces physiques, le froid bleu et la chaleur corail.

### Primary

- **Charbon profond** (`#0E0D0B`): fond de scène principal. Il doit rester chaud et tactile, pas noir technique.
- **Papier chaud** (`#F0EDE6`): texte fort, boutons primaires et états sélectionnés.

### Secondary

- **Bleu froid** (`#4A9EE8`): ville A, gel, froid, côté givre, valeurs plus fraîches.
- **Corail chaud** (`#E86A45`): ville B, chaleur, canicule, tendance au réchauffement.

### Tertiary

- **Ambre sec** (`#C8901A`): soleil, méthode, attention douce.
- **Vert vivant** (`#3A9E6A`): amélioration ou baisse d’un indicateur négatif.

### Neutral

- **Surface charbon** (`#161512`): cartes et zones de regroupement.
- **Surface relevée** (`#1E1C18`): champs, listes, contrôles et cartes secondaires.
- **Pierre muette** (`#A19B94`): textes secondaires, légendes et aides.
- **Pierre faible** (`#514D47`): séparateurs discrets et textes très secondaires.

### Named Rules

**The Climate Polarity Rule.** Bleu et corail doivent toujours avoir une signification physique claire. Ne pas les utiliser comme simple décoration.

**The Sunlight Test.** Tout texte secondaire doit rester lisible sur mobile en lumière forte. Si le gris paraît élégant mais faible, il est trop faible.

## 3. Typography

**Display Font:** DM Serif Display, avec Georgia en secours  
**Body Font:** Outfit, avec system-ui en secours  
**Label/Mono Font:** JetBrains Mono, avec ui-monospace en secours

**Character:** La paire typographique donne une voix double : DM Serif apporte l’élan éditorial, Outfit garde l’interface simple, JetBrains Mono donne aux chiffres une présence de mesure.

### Hierarchy

- **Display** (400, `clamp(2.4rem, 5.5vw, 4rem)`, 1.02): héros, nom de commune, grands moments narratifs uniquement.
- **Headline** (400, `clamp(2rem, 5vw, 3rem)`, 1.05): titres de sections et chapitres.
- **Title** (700, 17 à 18 px, 1.2): cartes, graphiques, modules.
- **Body** (400, 15 à 16 px, 1.5): explications courtes, avec une longueur cible de 65 à 75 caractères.
- **Label** (500, 10 à 12 px, espacement 0.08 à 0.12 em): sources, périodes, métadonnées, statuts.
- **Data** (700, JetBrains Mono, `clamp(1.8rem, 4vw, 2.55rem)`): valeurs clés, deltas et records.

### Named Rules

**The Child Can Read It Rule.** Une visualisation doit pouvoir être comprise par son titre, sa valeur principale et une phrase courte.

**The Product Control Rule.** Les labels, boutons, champs et onglets restent en Outfit ou JetBrains Mono. La serif ne sert jamais à inventer des contrôles bizarres.

## 4. Elevation

Le système utilise peu d’ombres. La profondeur vient surtout de couches tonales, de bordures fines, de fonds légèrement transparents et d’un seul grand effet d’ambiance dans le héros. Les ombres doivent signaler une scène ou une interaction, pas décorer toutes les cartes.

### Shadow Vocabulary

- **Hero atmosphere** (`0 24px 80px rgba(0,0,0,.32)`): réservé au bandeau image et aux grandes scènes.
- **Autocomplete popover** (`0 8px 24px rgba(0,0,0,.4)`): listes flottantes et menus contextualisés.

### Named Rules

**The Flat Instrument Rule.** Les cartes restent plates au repos. Une bordure fine et un fond bien choisi suffisent.

## 5. Components

### Buttons

- **Shape:** coins doux (`10px`), hauteur minimale `44px`.
- **Primary:** fond papier chaud, texte charbon, graisse 700.
- **Hover / Focus:** léger déplacement vertical, opacité contrôlée, focus visible à 2 px.
- **States:** prévoir default, hover, focus, active, disabled et loading avec le même vocabulaire visuel.
- **Secondary:** fond charbon relevé, bordure claire, texte papier chaud.

### Chips

- **Style:** groupe segmenté avec fond charbon, bouton sélectionné en papier chaud.
- **State:** `aria-pressed` doit refléter l’état visuel, notamment pour Année, Été, Hiver.

### Cards / Containers

- **Corner Style:** `14px` à `16px`.
- **Background:** surfaces charbon, parfois dégradés froid vers chaud pour les modules de synthèse.
- **Shadow Strategy:** ombres rares, bordures fines et couches tonales par défaut.
- **Border:** `1px` ou `0.5px` en blanc très transparent.
- **Internal Padding:** `1rem` à `1.35rem` selon densité.

### Inputs / Fields

- **Style:** fond surface, bordure claire à contraste suffisant, rayon `10px`.
- **Focus:** bordure papier chaud et anneau discret.
- **Disabled / Error:** opacité réduite ou bordure d’état, jamais uniquement un changement de couleur ambigu.

### Navigation

- **Style:** barre sticky sombre, blur léger, logo serif, méta en mono.
- **Mobile:** les champs de recherche restent atteignables, les contrôles gardent 44 px minimum.

### Climate Visualizations

Les graphiques doivent être plus explicatifs que décoratifs : bandes de réchauffement, courbes annuelles, barres pluie, colonnes comparatives. Chaque graphique a besoin d’un titre clair, d’une légende simple et d’une phrase d’aide.

## 6. Do's and Don'ts

### Do:

- **Do** garder le fond charbon chaud `#0E0D0B` comme scène principale.
- **Do** utiliser le bleu pour le froid et le corail pour la chaleur avec cohérence.
- **Do** privilégier des graphiques compréhensibles sans légende complexe.
- **Do** respecter `prefers-reduced-motion` pour les effets de givre, chaleur et transitions.
- **Do** maintenir les textes secondaires au moins aussi lisibles que `#A19B94` sur fond sombre.

### Don't:

- **Don't** produire un tableau météo institutionnel froid, dense et illisible.
- **Don't** créer un dashboard SaaS générique avec cartes répétitives, icônes décoratives et métriques sans narration.
- **Don't** réintroduire des effets météo datés comme pluie ou neige en surcouche gratuite.
- **Don't** basculer dans une esthétique catastrophiste qui culpabilise avant d’expliquer.
- **Don't** utiliser des visualisations scientifiques trop abstraites pour un public non spécialiste.
- **Don't** utiliser de gradient text ou de bordure latérale épaisse comme accent de carte.
- **Don't** employer la serif dans les labels, boutons, formulaires ou données.
