# Goblincore

## Overview

Goblincore is an aesthetic that celebrates the overlooked treasures of the forest floor: mushrooms, moss, snails, toads, pebbles, acorns, and muddy earth in all its imperfect charm. It rejects polished beauty in favor of the organic, the grimy, and the wonderfully irregular. In digital design, Goblincore translates into warm earth-tone palettes, hand-drawn textures, deliberately imperfect layouts, and a celebration of natural curiosities that feel like they were foraged from a damp woodland path and arranged on a rough wooden table.

## Visual Characteristics

### Core Design Traits

- **Mushroom and moss motifs**: Toadstools, bracket fungi, lichen textures, and dense moss patterns used as decorative and structural elements
- **Earth-tone warmth**: A palette built from soil browns, forest greens, mushroom tans, and lichen yellows with occasional pops of toad-belly orange
- **Handmade imperfection**: Rough edges, hand-drawn borders, slightly uneven spacing, and textures that feel tactile and organic
- **Found-object collections**: Visual arrangements that resemble a nature table: pinecones, river stones, feathers, snail shells, and acorns displayed as treasures
- **Damp forest atmosphere**: Dark, humid-feeling backgrounds with dappled light filtering through canopy, creating a sense of being close to the ground
- **Rough paper and bark textures**: Backgrounds that mimic torn paper, birch bark, weathered wood, and dried leaves
- **Jar and specimen aesthetics**: Content presented as if collected in glass jars, specimen boxes, or field notebooks

### Design Principles

- Embrace imperfection as a core value: uneven lines, rough textures, and organic asymmetry are features, not bugs
- Keep the palette grounded in nature: avoid synthetic or neon colors
- Layer textures generously to create tactile depth
- Treat content as curated collections of found objects rather than polished corporate layouts
- Favor warmth and coziness over sleekness and minimalism
- Let negative space feel like forest floor rather than clinical white space

## Color Palette

| Swatch | Hex | Role |
|--------|-----|------|
| Forest Floor | `#3B2F2F` | Primary dark background, text |
| Toadstool Tan | `#C4A882` | Card backgrounds, warm neutral |
| Moss Green | `#4A6741` | Primary accent, headings |
| Lichen Yellow | `#B8A44C` | Secondary accent, highlights |
| Mushroom Cap | `#8B6F4E` | Borders, secondary surfaces |
| Damp Earth | `#5C4033` | Dark panel backgrounds |
| Snail Shell | `#D4C5A9` | Light surfaces, paper texture |
| Toad Belly | `#C17817` | Call-to-action, warm pop accent |
| Fern Green | `#6B8E5A` | Tertiary accent, decorative fills |
| River Stone | `#8E8E8E` | Muted text, subtle details |

### CSS Custom Properties

```css
:root {
  --goblin-forest-floor: #3B2F2F;
  --goblin-toadstool: #C4A882;
  --goblin-moss: #4A6741;
  --goblin-lichen: #B8A44C;
  --goblin-mushroom-cap: #8B6F4E;
  --goblin-damp-earth: #5C4033;
  --goblin-snail-shell: #D4C5A9;
  --goblin-toad-belly: #C17817;
  --goblin-fern: #6B8E5A;
  --goblin-river-stone: #8E8E8E;
}
```

## Typography

### Recommended Google Fonts

| Font | Weight(s) | Usage | Link |
|------|-----------|-------|------|
| **Caveat** | 400, 500, 600, 700 | Headings; hand-drawn, journal-like script | [Caveat](https://fonts.google.com/specimen/Caveat) |
| **Libre Baskerville** | 400, 700 | Body text; a warm, readable serif that feels like old book pages | [Libre Baskerville](https://fonts.google.com/specimen/Libre+Baskerville) |
| **Patrick Hand** | 400 | Informal labels, captions, annotations | [Patrick Hand](https://fonts.google.com/specimen/Patrick+Hand) |
| **Merriweather** | 300, 400, 700 | Alternative body serif with sturdy readability | [Merriweather](https://fonts.google.com/specimen/Merriweather) |
| **Amatic SC** | 400, 700 | Decorative headings; tall, narrow, hand-lettered feel | [Amatic SC](https://fonts.google.com/specimen/Amatic+SC) |

### Font Pairing Suggestions

| Heading | Body | Mood |
|---------|------|------|
| Caveat 700 | Libre Baskerville 400 | Field journal, warm storytelling |
| Amatic SC 700 | Merriweather 400 | Whimsical naturalist, storybook |
| Patrick Hand 400 | Libre Baskerville 400 | Handwritten notes on old pages |

### CSS Example

```css
@import url('https://fonts.googleapis.com/css2?family=Caveat:wght@400;500;700&family=Libre+Baskerville:wght@400;700&display=swap');

body {
  font-family: 'Libre Baskerville', 'Georgia', serif;
  font-size: 1.05rem;
  line-height: 1.75;
  color: var(--goblin-forest-floor);
  -webkit-font-smoothing: antialiased;
}

h1, h2, h3 {
  font-family: 'Caveat', cursive;
  font-weight: 700;
  letter-spacing: 0.02em;
  color: var(--goblin-moss);
}
```

## Layout Principles

- **Asymmetric organic grid**: Avoid rigid symmetry; let content blocks feel like objects scattered on a table, with slightly irregular spacing and varied sizes
- **Layered textures as backgrounds**: Use paper textures, wood grain, or moss patterns behind content areas to create tactile depth
- **Collection-style arrangement**: Group related elements as if curating a nature specimen display: small cards clustered with varied heights, overlapping edges optional
- **Field-notebook sections**: Content sections styled like torn notebook pages with ragged edges, tape-strip decorations, or pencil-line borders
- **Rounded and irregular shapes**: Avoid perfectly geometric containers; prefer slightly irregular border-radius or wavy SVG clip-paths
- **Responsive approach**: On mobile, stack collection items vertically while preserving rough textures and handmade typography; let the small screen feel like flipping through a pocket field guide

## CSS / Design Techniques

### Foraged Card

```css
.goblin-card {
  background: var(--goblin-snail-shell);
  border: 2px solid var(--goblin-mushroom-cap);
  border-radius: 8px 12px 8px 14px;
  padding: 32px;
  box-shadow:
    2px 3px 0px var(--goblin-mushroom-cap),
    4px 6px 12px rgba(59, 47, 47, 0.15);
  position: relative;
}

.goblin-card::before {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  background: repeating-linear-gradient(
    0deg,
    transparent,
    transparent 28px,
    rgba(139, 111, 78, 0.06) 28px,
    rgba(139, 111, 78, 0.06) 29px
  );
  border-radius: inherit;
  pointer-events: none;
}
```

### Mossy Button

```css
.goblin-button {
  background: var(--goblin-moss);
  color: var(--goblin-snail-shell);
  border: 2px solid var(--goblin-damp-earth);
  border-radius: 6px 10px 6px 8px;
  padding: 12px 28px;
  font-family: 'Caveat', cursive;
  font-weight: 700;
  font-size: 1.15rem;
  cursor: pointer;
  box-shadow: 2px 3px 0px var(--goblin-damp-earth);
  transition: all 0.2s ease;
}

.goblin-button:hover {
  background: var(--goblin-fern);
  transform: translate(-1px, -1px);
  box-shadow: 3px 4px 0px var(--goblin-damp-earth);
}
```

### Woodland Navigation

```css
.goblin-nav {
  background: var(--goblin-damp-earth);
  border-bottom: 3px solid var(--goblin-mushroom-cap);
  padding: 16px 32px;
  display: flex;
  align-items: center;
  justify-content: space-between;
}

.goblin-nav a {
  color: var(--goblin-snail-shell);
  font-family: 'Caveat', cursive;
  font-size: 1.1rem;
  font-weight: 500;
  text-decoration: none;
  transition: color 0.3s ease;
}

.goblin-nav a:hover {
  color: var(--goblin-lichen);
}
```

### Hero Section

```css
.goblin-hero {
  background: var(--goblin-forest-floor);
  color: var(--goblin-snail-shell);
  padding: 80px 40px;
  text-align: center;
  position: relative;
  overflow: hidden;
}

.goblin-hero::before {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  background:
    radial-gradient(ellipse at 30% 70%, rgba(74, 103, 65, 0.15) 0%, transparent 50%),
    radial-gradient(ellipse at 70% 30%, rgba(184, 164, 76, 0.10) 0%, transparent 50%);
  pointer-events: none;
}

.goblin-hero h1 {
  font-family: 'Caveat', cursive;
  font-size: 3.5rem;
  font-weight: 700;
  color: var(--goblin-lichen);
  position: relative;
}

.goblin-hero p {
  font-size: 1.15rem;
  color: rgba(212, 197, 169, 0.80);
  max-width: 560px;
  margin: 12px auto 0;
  position: relative;
}
```

### Twig Divider

```css
.goblin-divider {
  display: flex;
  align-items: center;
  gap: 16px;
  margin: 40px 0;
  padding: 0 20px;
}

.goblin-divider::before,
.goblin-divider::after {
  content: '';
  flex: 1;
  height: 2px;
  background: linear-gradient(to right, transparent, var(--goblin-mushroom-cap), transparent);
}

.goblin-divider span {
  font-family: 'Caveat', cursive;
  font-size: 1.5rem;
  color: var(--goblin-moss);
}
```

### Specimen Tag

```css
.goblin-tag {
  display: inline-block;
  background: var(--goblin-toadstool);
  color: var(--goblin-forest-floor);
  font-family: 'Patrick Hand', cursive;
  font-size: 0.85rem;
  padding: 4px 14px;
  border: 1px dashed var(--goblin-mushroom-cap);
  border-radius: 2px;
  transform: rotate(-2deg);
}
```

## Design Do's and Don'ts

### Do

- Use warm, muddy earth tones and muted forest greens throughout
- Include hand-drawn or handwritten-style typography for headings and labels
- Layer rough textures (paper, bark, moss) behind content for tactile depth
- Embrace irregular shapes, uneven borders, and deliberate imperfection
- Present content as curated collections of found treasures
- Add small nature details: mushroom icons, leaf silhouettes, snail doodles
- Keep the tone cozy, warm, and slightly whimsical

### Don't

- Use polished, corporate-looking layouts with perfect geometric grids
- Apply bright white backgrounds or sterile minimalist spacing
- Choose clean, geometric sans-serif fonts for headings
- Use neon or synthetic colors that feel artificial and unnatural
- Over-refine illustrations; Goblincore thrives on charming roughness
- Mix with high-tech, futuristic, or cyberpunk aesthetics
- Make everything perfectly symmetrical and aligned

## Related Aesthetics

| Aesthetic | Relationship |
|-----------|-------------|
| **Cottagecore** | Close cousin sharing nature-focus and coziness; Cottagecore is sunlit and tidy while Goblincore is damp and messy |
| **Dark Academia** | Both value old-world, collected aesthetics; Dark Academia is scholarly and architectural while Goblincore is feral and forest-dwelling |
| **Cluttercore** | Shares the love of abundant collected objects; Cluttercore is broader in scope while Goblincore is specifically nature-focused |
| **Arts and Crafts** | Both celebrate handmade quality and natural materials; Arts and Crafts is refined and structured while Goblincore is wild |
| **Forestpunk** | Overlaps in woodland setting and earthy palette; Forestpunk adds punk-rebel energy and fantasy world-building |
| **Maximalism** | Goblincore's dense layering of textures and objects shares maximalist instincts but within a narrow natural material register |

## Quick-Start HTML Template

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Goblincore Layout</title>
  <link href="https://fonts.googleapis.com/css2?family=Caveat:wght@400;500;700&family=Libre+Baskerville:wght@400;700&display=swap" rel="stylesheet">
  <style>
    *, *::before, *::after { margin: 0; padding: 0; box-sizing: border-box; }

    body {
      font-family: 'Libre Baskerville', Georgia, serif;
      font-size: 1.05rem;
      line-height: 1.75;
      color: #3B2F2F;
      background: #D4C5A9;
      min-height: 100vh;
    }

    .nav {
      background: #5C4033;
      border-bottom: 3px solid #8B6F4E;
      padding: 16px 32px;
      display: flex;
      align-items: center;
      justify-content: space-between;
    }

    .nav a {
      color: #D4C5A9;
      font-family: 'Caveat', cursive;
      font-size: 1.1rem;
      font-weight: 500;
      text-decoration: none;
    }

    .hero {
      background: #3B2F2F;
      color: #D4C5A9;
      text-align: center;
      padding: 80px 40px;
      position: relative;
    }

    .hero::before {
      content: '';
      position: absolute;
      top: 0; left: 0; right: 0; bottom: 0;
      background:
        radial-gradient(ellipse at 30% 70%, rgba(74,103,65,0.15) 0%, transparent 50%),
        radial-gradient(ellipse at 70% 30%, rgba(184,164,76,0.10) 0%, transparent 50%);
    }

    .hero h1 {
      font-family: 'Caveat', cursive;
      font-size: 3.5rem;
      font-weight: 700;
      color: #B8A44C;
      position: relative;
    }

    .hero p {
      font-size: 1.1rem;
      color: rgba(212,197,169,0.80);
      max-width: 500px;
      margin: 12px auto 0;
      position: relative;
    }

    .content {
      max-width: 900px;
      margin: 60px auto;
      padding: 0 32px;
      display: grid;
      grid-template-columns: 1fr 1fr 1fr;
      gap: 24px;
    }

    .card {
      background: #D4C5A9;
      border: 2px solid #8B6F4E;
      border-radius: 8px 12px 8px 14px;
      padding: 28px;
      box-shadow: 2px 3px 0px #8B6F4E;
    }

    .card h2 {
      font-family: 'Caveat', cursive;
      font-weight: 700;
      font-size: 1.6rem;
      color: #4A6741;
      margin-bottom: 8px;
    }

    .card p {
      color: #3B2F2F;
      font-size: 0.95rem;
      line-height: 1.7;
    }

    .button {
      display: inline-block;
      margin-top: 16px;
      background: #4A6741;
      color: #D4C5A9;
      border: 2px solid #5C4033;
      border-radius: 6px 10px 6px 8px;
      padding: 10px 24px;
      font-family: 'Caveat', cursive;
      font-weight: 700;
      font-size: 1.1rem;
      text-decoration: none;
      box-shadow: 2px 3px 0px #5C4033;
    }

    .tag {
      display: inline-block;
      background: #C4A882;
      color: #3B2F2F;
      font-family: 'Caveat', cursive;
      font-size: 0.85rem;
      padding: 2px 10px;
      border: 1px dashed #8B6F4E;
      margin-bottom: 12px;
      transform: rotate(-2deg);
    }
  </style>
</head>
<body>
  <nav class="nav">
    <a href="#" style="font-size:1.3rem;font-weight:700;">Goblincore</a>
    <div>
      <a href="#">Forage</a>
      <a href="#" style="margin-left:20px;">Collection</a>
      <a href="#" style="margin-left:20px;">Field Notes</a>
    </div>
  </nav>
  <header class="hero">
    <h1>Forest Floor Treasures</h1>
    <p>Mushrooms, moss, snails, and charmingly imperfect
       found objects from muddy woodland paths.</p>
  </header>
  <main class="content">
    <div class="card">
      <span class="tag">specimen #01</span>
      <h2>Toadstool Ring</h2>
      <p>A circle of red-capped mushrooms discovered at the base
         of a mossy oak, still damp with morning dew.</p>
      <a href="#" class="button">Examine</a>
    </div>
    <div class="card">
      <span class="tag">specimen #02</span>
      <h2>River Pebbles</h2>
      <p>Smooth stones collected from the creek bed, each one
         a different shade of grey and brown.</p>
      <a href="#" class="button">Examine</a>
    </div>
    <div class="card">
      <span class="tag">specimen #03</span>
      <h2>Snail Shell</h2>
      <p>A perfect spiral shell found on a rain-soaked fern leaf,
         abandoned by its tiny former tenant.</p>
      <a href="#" class="button">Examine</a>
    </div>
  </main>
</body>
</html>
```
