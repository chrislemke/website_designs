# Wes Anderson

## Overview

The Wes Anderson aesthetic is a design language derived from the filmmaker's instantly recognizable visual style: obsessive symmetry, carefully curated pastel color palettes, whimsical serif typography, and meticulous compositional precision. Every element is centered, aligned, and color-coordinated with the deliberateness of a museum diorama. In digital design, the Wes Anderson aesthetic translates into centered layouts, vintage-inspired type, muted pastels with one or two warm accent colors, and a sense of deadpan perfection that is simultaneously precise and playful. The style evokes mid-century hotel lobbies, train compartments, and the pages of a fictional adventure novel.

## Visual Characteristics

### Core Design Traits

- **Perfect bilateral symmetry**: Every element centered on a vertical axis; layouts are balanced to the pixel
- **Curated pastel palettes**: Dusty pinks, faded yellows, powder blues, sage greens, and warm creams arranged in deliberate combinations
- **Whimsical serif typography**: Vintage-inspired serif and slab-serif typefaces, often in italics, used for titles and labels with a bookish quality
- **Flat, matte surfaces**: No gradients, no gloss, no depth effects; every surface is a solid, flat color
- **Visible grid and framing**: Thin borders, label plates, numbered elements, and frame-within-frame compositions
- **Mid-century material references**: Leather, brass, wood paneling, tile, and velvet textures referenced through color rather than actual texture
- **Deadpan precision**: The careful arrangement conveys a dry humor; everything is placed with almost absurd exactness

### Design Principles

- **Symmetry above all**: If an element cannot be centered, it should be precisely offset with an equal counterpart
- **Color as character**: Each section or card can have its own dominant pastel color, creating a story through palette shifts
- **Typography as decoration**: Titles, labels, and chapter numbers are decorative elements that contribute to the visual rhythm
- **Restraint with warmth**: The design is controlled and precise but never cold; warmth comes from the color choices and serif typography
- **Everything is labeled**: Cards have titles, sections have chapter numbers, buttons have descriptive labels; the design is self-documenting

## Color Palette

| Swatch | Hex | Role |
|--------|-----|------|
| Lobby Pink | `#E8A0A0` | Primary pastel accent |
| Faded Mustard | `#D4B06A` | Warm secondary accent |
| Powder Blue | `#A4C4D4` | Cool tertiary accent |
| Sage Mint | `#B4C8A8` | Green accent |
| Cream | `#F4EDE4` | Primary background |
| Warm White | `#FAF6F0` | Card background |
| Vintage Red | `#C45C4C` | Emphasis / CTA accent |
| Deep Brown | `#4A3728` | Primary text |
| Dusty Lilac | `#C4A8C8` | Decorative accent |
| Terracotta | `#C88C6C` | Warm decorative accent |
| Soft Gray | `#B8B0A8` | Muted text / borders |
| Off-Black | `#2C2420` | High-contrast text |

### CSS Custom Properties

```css
:root {
  --wa-pink: #E8A0A0;
  --wa-mustard: #D4B06A;
  --wa-blue: #A4C4D4;
  --wa-sage: #B4C8A8;
  --wa-cream: #F4EDE4;
  --wa-white: #FAF6F0;
  --wa-red: #C45C4C;
  --wa-brown: #4A3728;
  --wa-lilac: #C4A8C8;
  --wa-terracotta: #C88C6C;
  --wa-gray: #B8B0A8;
  --wa-black: #2C2420;
}
```

## Typography

### Recommended Google Fonts

| Font | Weight(s) | Usage | Link |
|------|-----------|-------|------|
| **Playfair Display** | 400, 500, 600, 700 | Display headings; high-contrast transitional serif | [Playfair Display](https://fonts.google.com/specimen/Playfair+Display) |
| **Libre Baskerville** | 400, 400i, 700 | Body text and subheadings; classic book serif | [Libre Baskerville](https://fonts.google.com/specimen/Libre+Baskerville) |
| **Courier Prime** | 400, 700 | Labels, numbers, and monospaced accents; typewriter quality | [Courier Prime](https://fonts.google.com/specimen/Courier+Prime) |
| **EB Garamond** | 400, 500, 600 | Elegant body text alternative; old-style proportions | [EB Garamond](https://fonts.google.com/specimen/EB+Garamond) |
| **Josefin Slab** | 300, 400, 500, 600 | Slab-serif for labels and UI; geometric and vintage | [Josefin Slab](https://fonts.google.com/specimen/Josefin+Slab) |

### Font Pairing Suggestions

| Heading | Body | Vibe |
|---------|------|------|
| Playfair Display 600 | Libre Baskerville 400 | Classic Wes Anderson title card |
| Playfair Display 400i | EB Garamond 400 | Italic whimsy with traditional reading |
| Josefin Slab 400 | Libre Baskerville 400 | Geometric vintage with bookish body |

### CSS Example

```css
@import url('https://fonts.googleapis.com/css2?family=Playfair+Display:ital,wght@0,400;0,600;0,700;1,400;1,600&family=Libre+Baskerville:ital,wght@0,400;0,700;1,400&family=Courier+Prime:wght@400;700&display=swap');

body {
  font-family: 'Libre Baskerville', 'Georgia', serif;
  font-size: 1rem;
  line-height: 1.8;
  color: #4A3728;
  -webkit-font-smoothing: antialiased;
}

h1, h2, h3 {
  font-family: 'Playfair Display', serif;
  font-weight: 600;
  letter-spacing: 0.02em;
  color: #2C2420;
}

.label {
  font-family: 'Courier Prime', monospace;
  font-size: 0.8rem;
  text-transform: uppercase;
  letter-spacing: 0.12em;
  color: #B8B0A8;
}
```

## Layout Principles

- **Strict center alignment**: All headings, cards, and content blocks are centered on the page's vertical axis
- **Framed compositions**: Use thin borders and nested frames to create a diorama-like containment of content
- **Chapter structure**: Organize content into numbered chapters or sections, each with a title card
- **Consistent card sizing**: All cards at the same width, evenly spaced, creating a rhythmic visual pattern
- **Flat elevation**: No shadows, no depth; cards are distinguished by background color and borders alone
- **Max-width discipline**: Content at 700-850px max-width, always centered, with generous page margins
- **Responsive approach**: Maintain center alignment on all screens; stack elements vertically; reduce card padding on mobile but preserve symmetry

## CSS / Design Techniques

### Wes Anderson Card

```css
.wa-card {
  background: #FAF6F0;
  border: 2px solid #4A3728;
  border-radius: 0;
  padding: 36px 40px;
  text-align: center;
  position: relative;
  max-width: 500px;
  margin: 0 auto 28px;
}
```

### Chapter Title

```css
.wa-chapter {
  text-align: center;
  margin: 48px 0 32px;
}

.wa-chapter .number {
  font-family: 'Courier Prime', monospace;
  font-size: 0.75rem;
  text-transform: uppercase;
  letter-spacing: 0.2em;
  color: #B8B0A8;
  margin-bottom: 8px;
}

.wa-chapter .title {
  font-family: 'Playfair Display', serif;
  font-size: 1.6rem;
  font-weight: 600;
  font-style: italic;
  color: #4A3728;
}
```

### Label Plate

```css
.wa-label {
  display: inline-block;
  background: #4A3728;
  color: #F4EDE4;
  font-family: 'Courier Prime', monospace;
  font-size: 0.7rem;
  text-transform: uppercase;
  letter-spacing: 0.15em;
  padding: 6px 16px;
  margin-bottom: 16px;
}
```

### Vintage Button

```css
.wa-button {
  display: inline-block;
  background: #C45C4C;
  color: #FAF6F0;
  border: 2px solid #C45C4C;
  border-radius: 0;
  padding: 12px 36px;
  font-family: 'Playfair Display', serif;
  font-size: 0.9rem;
  font-weight: 600;
  cursor: pointer;
  transition: all 0.25s ease;
  text-decoration: none;
}

.wa-button:hover {
  background: transparent;
  color: #C45C4C;
}
```

### Navigation Bar

```css
.wa-nav {
  background: #F4EDE4;
  border-bottom: 2px solid #4A3728;
  padding: 16px 40px;
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 40px;
}

.wa-nav a {
  font-family: 'Playfair Display', serif;
  font-size: 0.9rem;
  font-style: italic;
  color: #4A3728;
  text-decoration: none;
  padding: 4px 0;
  border-bottom: 1px solid transparent;
  transition: border-color 0.2s ease;
}

.wa-nav a:hover {
  border-bottom-color: #4A3728;
}
```

### Hero Section

```css
.wa-hero {
  text-align: center;
  padding: 80px 40px 60px;
  background: #F4EDE4;
}

.wa-hero .label {
  font-family: 'Courier Prime', monospace;
  font-size: 0.7rem;
  text-transform: uppercase;
  letter-spacing: 0.25em;
  color: #B8B0A8;
  margin-bottom: 16px;
}

.wa-hero h1 {
  font-family: 'Playfair Display', serif;
  font-size: 2.8rem;
  font-weight: 600;
  font-style: italic;
  color: #4A3728;
  margin-bottom: 16px;
}

.wa-hero p {
  font-family: 'Libre Baskerville', serif;
  font-size: 1rem;
  color: #4A3728;
  max-width: 480px;
  margin: 0 auto;
  line-height: 1.85;
}
```

### Decorative Rule

```css
.wa-rule {
  border: none;
  border-top: 1px solid #B8B0A8;
  max-width: 60px;
  margin: 32px auto;
}
```

### Color-Block Section

```css
.wa-section-pink {
  background: #E8A0A0;
  padding: 48px 40px;
  text-align: center;
}

.wa-section-blue {
  background: #A4C4D4;
  padding: 48px 40px;
  text-align: center;
}

.wa-section-mustard {
  background: #D4B06A;
  padding: 48px 40px;
  text-align: center;
}
```

## Design Do's and Don'ts

### Do's

- Center every element on a vertical axis; symmetry is non-negotiable
- Use muted, dusty pastel colors with warm undertones
- Choose serif typefaces, especially in italic, for headings and display text
- Add chapter numbers, labels, and framing borders for a curated, self-aware quality
- Use flat, solid background colors with no gradients or depth effects
- Keep consistent spacing between all elements; rhythm and regularity matter
- Apply the same border weight (2px) throughout for visual consistency

### Don'ts

- Avoid asymmetric layouts; off-center content breaks the entire aesthetic
- Avoid sans-serif fonts for headings; they feel too modern and corporate
- Do not use drop shadows, glass effects, or any depth simulation
- Avoid neon or saturated colors; all colors should feel slightly faded and dusty
- Do not use rounded corners on cards or buttons; sharp rectangles define the style
- Avoid complex animations; if any motion is used, it should be slow and deliberate
- Do not mix too many pastel colors in one view; limit to 2-3 pastels per scene plus the neutral background

## Related Aesthetics

| Aesthetic | Relationship |
|-----------|-------------|
| **Art Deco** | Shares symmetry and geometric precision but Art Deco is more glamorous and metallic |
| **Biedermeier** | Both emphasize domestic comfort, warmth, and restrained elegance |
| **American Kitsch** | Shares mid-century color references but Kitsch is louder and more ironic |
| **Cottagecore** | Both use warm, muted palettes but Cottagecore is organic while Wes Anderson is rigidly geometric |
| **Colorful Pop** | Both use distinctive color palettes but Pop is saturated and exuberant while Wes Anderson is dusty and controlled |
| **Baroque** | Both love ornamentation and framing but Baroque is maximalist and dramatic |

## Quick-Start HTML Template

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Wes Anderson Layout</title>
  <link href="https://fonts.googleapis.com/css2?family=Playfair+Display:ital,wght@0,400;0,600;0,700;1,400;1,600&family=Libre+Baskerville:ital,wght@0,400;0,700;1,400&family=Courier+Prime:wght@400;700&display=swap" rel="stylesheet">
  <style>
    *, *::before, *::after { margin: 0; padding: 0; box-sizing: border-box; }

    body {
      font-family: 'Libre Baskerville', Georgia, serif;
      font-size: 1rem;
      line-height: 1.8;
      color: #4A3728;
      background: #F4EDE4;
      min-height: 100vh;
    }

    .container {
      max-width: 560px;
      margin: 0 auto;
      padding: 60px 24px;
      text-align: center;
    }

    .hero {
      padding: 40px 20px 48px;
    }

    .hero .label {
      font-family: 'Courier Prime', monospace;
      font-size: 0.7rem;
      text-transform: uppercase;
      letter-spacing: 0.25em;
      color: #B8B0A8;
      margin-bottom: 16px;
    }

    .hero h1 {
      font-family: 'Playfair Display', serif;
      font-size: 2.6rem;
      font-weight: 600;
      font-style: italic;
      color: #4A3728;
      margin-bottom: 16px;
    }

    .hero p {
      font-size: 1rem;
      max-width: 440px;
      margin: 0 auto;
    }

    .rule {
      border: none;
      border-top: 1px solid #B8B0A8;
      max-width: 60px;
      margin: 32px auto;
    }

    .chapter-number {
      font-family: 'Courier Prime', monospace;
      font-size: 0.7rem;
      text-transform: uppercase;
      letter-spacing: 0.2em;
      color: #B8B0A8;
      margin-bottom: 8px;
    }

    .card {
      background: #FAF6F0;
      border: 2px solid #4A3728;
      padding: 32px 36px;
      margin-bottom: 24px;
      text-align: center;
    }

    .card h2 {
      font-family: 'Playfair Display', serif;
      font-size: 1.3rem;
      font-weight: 600;
      font-style: italic;
      color: #4A3728;
      margin-bottom: 12px;
    }

    .card p {
      font-size: 0.95rem;
      line-height: 1.85;
    }

    .card-pink { background: #E8A0A0; border-color: #4A3728; }
    .card-pink p { color: #4A3728; }

    .card-blue { background: #A4C4D4; border-color: #4A3728; }
    .card-blue p { color: #4A3728; }

    .button {
      display: inline-block;
      background: #C45C4C;
      color: #FAF6F0;
      border: 2px solid #C45C4C;
      padding: 12px 36px;
      font-family: 'Playfair Display', serif;
      font-size: 0.9rem;
      font-weight: 600;
      text-decoration: none;
      cursor: pointer;
      transition: all 0.25s ease;
    }

    .button:hover {
      background: transparent;
      color: #C45C4C;
    }
  </style>
</head>
<body>
  <div class="container">
    <div class="hero">
      <p class="label">A Film by</p>
      <h1>The Grand Lobby</h1>
      <p>A meticulously arranged account of symmetrical
         hallways, pastel elevators, and the concierge
         who alphabetized the guest ledger twice.</p>
    </div>
    <hr class="rule">
    <p class="chapter-number">Chapter I</p>
    <div class="card card-pink">
      <h2>The Lobby</h2>
      <p>Pink marble floors polished to a mirror finish,
         a brass bell at the front desk, and precisely
         twelve potted ferns arranged in two equal rows.</p>
    </div>
    <p class="chapter-number">Chapter II</p>
    <div class="card card-blue">
      <h2>The Elevator</h2>
      <p>Powder-blue doors that open with mechanical
         precision, an operator in a pillbox hat, and
         buttons labeled in a serif typeface.</p>
    </div>
    <p class="chapter-number">Chapter III</p>
    <div class="card">
      <h2>The Rooftop</h2>
      <p>A telescope pointed at exactly thirty-seven
         degrees, two canvas chairs in facing positions,
         and a table set for afternoon tea.</p>
    </div>
    <hr class="rule">
    <div style="margin-top: 24px;">
      <a href="#" class="button">Check In</a>
    </div>
  </div>
</body>
</html>
```

## Implementation Tips

- **Strict centering**: Use `text-align: center` on containers and `margin: 0 auto` on block elements; verify symmetry by toggling a CSS vertical center line during development
- **Border consistency**: Use the same `border: 2px solid #4A3728` on all framed elements; the uniform weight is a signature trait
- **Color sections**: Assign each major card or section a single pastel background color; alternate between 2-3 pastels for visual rhythm
- **Italic headings**: Apply `font-style: italic` to display headings in Playfair Display; the italic adds the whimsical quality essential to the aesthetic
- **Monospace labels**: Use Courier Prime for all meta-text (chapter numbers, categories, timestamps) to create a typewriter-era reference
- **No rounded corners**: Set `border-radius: 0` on all elements; the sharp rectangles are essential to the precise, controlled feel
- **Flat colors only**: Never use gradients, shadows, or transparency; every color should be a single, solid hex value
- **Photography treatment**: Apply `filter: saturate(70%) contrast(95%)` to photographs and consider adding a 2px solid border to frame them like prints
