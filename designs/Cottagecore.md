# Cottagecore

## Overview

Cottagecore is a romanticized pastoral aesthetic that celebrates an idealized vision of rural life, handmade crafts, and simple pleasures. It draws from wildflower meadows, gingham patterns, hand-lettered signage, sun-dappled linen textures, and the warmth of a countryside kitchen. In digital design, Cottagecore translates into soft, warm color palettes, organic shapes, hand-drawn illustration elements, and typography that evokes handwriting or vintage letterpress printing. The aesthetic rejects sleek minimalism in favor of cozy imperfection and natural abundance.

## Visual Characteristics

### Core Design Traits

- **Soft, warm color palette**: Muted earth tones, sage greens, dusty pinks, butter yellows, and cream whites that evoke a sun-warmed garden
- **Hand-drawn elements**: Botanical illustrations, sketched borders, watercolor textures, and imperfect line art that convey a handmade quality
- **Natural textures**: Linen weaves, parchment paper, dried flower pressings, wood grain, and woven basket patterns used as backgrounds and accents
- **Gingham and plaid patterns**: Checked fabric patterns in soft colors used as borders, backgrounds, or decorative strips
- **Rounded, organic shapes**: Soft curves, scalloped edges, and irregular forms inspired by petals, leaves, and natural contours
- **Floral abundance**: Wildflowers, herbs, trailing vines, and botanical motifs as decorative elements throughout the layout
- **Vintage ephemera**: Postage stamps, seed packet labels, mason jar illustrations, and hand-written recipe cards as visual references

### Design Principles

- **Warmth over precision**: Favor slightly imperfect, hand-touched elements over pixel-perfect geometry
- **Layered texture**: Combine multiple subtle textures (linen, paper, watercolor wash) to create tactile depth
- **Generous whitespace**: Let designs breathe like an open meadow; avoid cramped layouts
- **Nature as ornament**: Use botanical elements for decoration rather than abstract geometric shapes
- **Nostalgic simplicity**: Evoke a slower, gentler time through deliberate design restraint and vintage references

## Color Palette

| Swatch | Hex | Role |
|--------|-----|------|
| Meadow Cream | `#FDF6EC` | Primary background |
| Linen White | `#FAF3E8` | Card / surface background |
| Sage Green | `#8B9E7E` | Primary accent |
| Dusty Rose | `#C9A0A0` | Secondary accent |
| Butter Yellow | `#E8D5A3` | Warm highlight |
| Terracotta | `#C07856` | Call-to-action / emphasis |
| Lavender Mist | `#B8A9C9` | Tertiary accent |
| Bramble Brown | `#6B4E3D` | Primary text |
| Faded Denim | `#7E8FA6` | Muted secondary text |
| Parchment | `#F0E6D3` | Alternate background |
| Forest Moss | `#5E7153` | Dark accent |
| Wild Berry | `#8E4162` | Highlight accent |

### CSS Custom Properties

```css
:root {
  --cc-cream: #FDF6EC;
  --cc-linen: #FAF3E8;
  --cc-sage: #8B9E7E;
  --cc-dusty-rose: #C9A0A0;
  --cc-butter: #E8D5A3;
  --cc-terracotta: #C07856;
  --cc-lavender: #B8A9C9;
  --cc-brown: #6B4E3D;
  --cc-denim: #7E8FA6;
  --cc-parchment: #F0E6D3;
  --cc-moss: #5E7153;
  --cc-berry: #8E4162;
}
```

## Typography

### Recommended Google Fonts

| Font | Weight(s) | Usage | Link |
|------|-----------|-------|------|
| **Lora** | 400, 500, 600, 700 | Headings; elegant serif with gentle curves | [Lora](https://fonts.google.com/specimen/Lora) |
| **Crimson Text** | 400, 600, 700 | Body text; warm, readable old-style serif | [Crimson Text](https://fonts.google.com/specimen/Crimson+Text) |
| **Caveat** | 400, 500, 600, 700 | Decorative hand-lettered text, labels, quotes | [Caveat](https://fonts.google.com/specimen/Caveat) |
| **Cormorant Garamond** | 300, 400, 500, 600 | Display headings; refined and romantic | [Cormorant Garamond](https://fonts.google.com/specimen/Cormorant+Garamond) |
| **Nunito** | 300, 400, 600 | UI labels, navigation; soft rounded sans-serif | [Nunito](https://fonts.google.com/specimen/Nunito) |

### Font Pairing Suggestions

| Heading | Body | Vibe |
|---------|------|------|
| Cormorant Garamond 500 | Crimson Text 400 | Classic romantic editorial |
| Lora 600 | Nunito 400 | Warm and approachable |
| Caveat 600 | Crimson Text 400 | Hand-lettered charm with readable body |

### CSS Example

```css
@import url('https://fonts.googleapis.com/css2?family=Cormorant+Garamond:wght@400;500;600&family=Crimson+Text:wght@400;600&family=Caveat:wght@400;600&display=swap');

body {
  font-family: 'Crimson Text', 'Georgia', serif;
  font-size: 1.1rem;
  line-height: 1.8;
  color: #6B4E3D;
  -webkit-font-smoothing: antialiased;
}

h1, h2, h3 {
  font-family: 'Cormorant Garamond', 'Garamond', serif;
  font-weight: 500;
  letter-spacing: 0.01em;
  color: #5E7153;
}

.handwritten {
  font-family: 'Caveat', cursive;
  font-size: 1.4rem;
}
```

## Layout Principles

- **Single-column or gentle two-column layouts**: Avoid complex multi-column grids; favor a natural, vertical reading flow like a journal page
- **Generous padding**: Internal padding of 32-48px on cards, 24-40px gaps between sections; the design should feel spacious and unhurried
- **Organic section breaks**: Use botanical dividers, hand-drawn lines, or floral ornaments instead of hard horizontal rules
- **Scalloped and rounded containers**: Cards and content areas should use rounded corners (12-20px) or scalloped/wavy borders
- **Layered paper effect**: Stack elements with subtle box-shadows to create the feeling of paper layers, cards, or pinned notes
- **Centered content with max-width**: Keep content readable at 700-900px max-width, centered on the page
- **Responsive approach**: Stack columns vertically on mobile; maintain generous padding; scale floral decorations down gracefully

## CSS / Design Techniques

### Cottagecore Card

```css
.cottage-card {
  background: #FAF3E8;
  border: 1px solid #E8D5A3;
  border-radius: 16px;
  padding: 32px;
  box-shadow: 0 2px 8px rgba(107, 78, 61, 0.08);
  position: relative;
}

.cottage-card::before {
  content: '';
  position: absolute;
  top: -1px;
  left: 20px;
  right: 20px;
  height: 3px;
  background: linear-gradient(90deg, #8B9E7E, #C9A0A0, #E8D5A3);
  border-radius: 3px;
}
```

### Cottagecore Button

```css
.cottage-button {
  background: #8B9E7E;
  color: #FDF6EC;
  border: none;
  border-radius: 24px;
  padding: 12px 32px;
  font-family: 'Crimson Text', serif;
  font-size: 1rem;
  font-weight: 600;
  cursor: pointer;
  transition: all 0.3s ease;
  box-shadow: 0 2px 6px rgba(94, 113, 83, 0.25);
}

.cottage-button:hover {
  background: #5E7153;
  box-shadow: 0 4px 12px rgba(94, 113, 83, 0.35);
  transform: translateY(-1px);
}
```

### Gingham Background Pattern

```css
.gingham {
  background-color: #FDF6EC;
  background-image:
    linear-gradient(45deg, #C9A0A022 25%, transparent 25%, transparent 75%, #C9A0A022 75%),
    linear-gradient(45deg, #C9A0A022 25%, transparent 25%, transparent 75%, #C9A0A022 75%);
  background-size: 20px 20px;
  background-position: 0 0, 10px 10px;
}
```

### Botanical Divider

```css
.botanical-divider {
  text-align: center;
  margin: 40px 0;
  color: #8B9E7E;
  font-size: 1.5rem;
  letter-spacing: 0.5em;
  opacity: 0.6;
}

.botanical-divider::before {
  content: '\2740 \2740 \2740';
}
```

### Linen Texture Background

```css
.linen-bg {
  background-color: #FDF6EC;
  background-image:
    repeating-linear-gradient(
      0deg,
      transparent,
      transparent 2px,
      rgba(107, 78, 61, 0.03) 2px,
      rgba(107, 78, 61, 0.03) 3px
    ),
    repeating-linear-gradient(
      90deg,
      transparent,
      transparent 2px,
      rgba(107, 78, 61, 0.02) 2px,
      rgba(107, 78, 61, 0.02) 3px
    );
}
```

### Hero Section

```css
.cottage-hero {
  background: linear-gradient(180deg, #FDF6EC 0%, #F0E6D3 100%);
  padding: 80px 40px;
  text-align: center;
  position: relative;
  overflow: hidden;
}

.cottage-hero h1 {
  font-family: 'Cormorant Garamond', serif;
  font-size: 3rem;
  font-weight: 500;
  color: #5E7153;
  margin-bottom: 16px;
}

.cottage-hero p {
  font-family: 'Crimson Text', serif;
  font-size: 1.25rem;
  color: #6B4E3D;
  max-width: 600px;
  margin: 0 auto;
  line-height: 1.8;
}
```

### Navigation Bar

```css
.cottage-nav {
  background: #FAF3E8;
  border-bottom: 2px solid #E8D5A3;
  padding: 16px 32px;
  display: flex;
  align-items: center;
  justify-content: space-between;
}

.cottage-nav a {
  font-family: 'Crimson Text', serif;
  font-size: 1rem;
  color: #6B4E3D;
  text-decoration: none;
  padding: 8px 16px;
  border-radius: 8px;
  transition: background 0.2s ease;
}

.cottage-nav a:hover {
  background: rgba(139, 158, 126, 0.15);
  color: #5E7153;
}
```

## Design Do's and Don'ts

### Do's

- Use botanical illustrations, pressed flower graphics, and nature-inspired ornaments
- Pair serif fonts with handwriting fonts for a layered, artisanal feel
- Apply soft, warm shadows with brown-tinted rgba values
- Use cream, linen, and parchment tones as backgrounds instead of pure white
- Incorporate subtle textile textures (linen, gingham, burlap) as background patterns
- Keep color saturation low and warmth high; everything should feel sun-faded
- Use scalloped edges, rounded corners, and organic shapes for containers

### Don'ts

- Avoid neon colors, electric blues, or high-contrast corporate palettes
- Avoid sharp geometric shapes, hard angles, or rigid grid systems
- Do not use sans-serif fonts exclusively; serifs and handwriting fonts are essential
- Avoid glossy gradients, glass effects, or chrome-like surfaces
- Do not overcrowd layouts; Cottagecore needs room to breathe
- Avoid dark mode or black backgrounds; the aesthetic is fundamentally light and warm
- Do not use stock photography of modern cityscapes or tech products

## Related Aesthetics

| Aesthetic | Relationship |
|-----------|-------------|
| **Arts and Crafts** | Shares the emphasis on handmade quality, natural materials, and rejection of industrial aesthetics |
| **Coastal Style** | Both use soft, muted palettes and natural textures but Coastal leans cool (ocean) while Cottagecore leans warm (meadow) |
| **Wabi-Sabi** | Shares appreciation for imperfection and natural materials, but Wabi-Sabi is more austere and Japanese-inflected |
| **Art Nouveau** | Both draw from botanical forms, but Art Nouveau is more stylized and ornamental |
| **Cluttercore** | Cottagecore's maximalist cousin; both celebrate collected objects but Cluttercore embraces visual chaos |
| **Biedermeier** | Shares domestic warmth and comfort-focused design, with a similar muted palette |

## Quick-Start HTML Template

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Cottagecore Layout</title>
  <link href="https://fonts.googleapis.com/css2?family=Cormorant+Garamond:wght@400;500;600&family=Crimson+Text:wght@400;600&family=Caveat:wght@400;600&display=swap" rel="stylesheet">
  <style>
    *, *::before, *::after { margin: 0; padding: 0; box-sizing: border-box; }

    body {
      font-family: 'Crimson Text', Georgia, serif;
      font-size: 1.1rem;
      line-height: 1.8;
      color: #6B4E3D;
      background-color: #FDF6EC;
      background-image:
        repeating-linear-gradient(0deg, transparent, transparent 2px, rgba(107,78,61,0.03) 2px, rgba(107,78,61,0.03) 3px),
        repeating-linear-gradient(90deg, transparent, transparent 2px, rgba(107,78,61,0.02) 2px, rgba(107,78,61,0.02) 3px);
    }

    .container {
      max-width: 800px;
      margin: 0 auto;
      padding: 40px 24px;
    }

    .hero {
      text-align: center;
      padding: 60px 20px;
      margin-bottom: 40px;
    }

    .hero h1 {
      font-family: 'Cormorant Garamond', serif;
      font-size: 2.8rem;
      font-weight: 500;
      color: #5E7153;
      margin-bottom: 12px;
    }

    .hero .subtitle {
      font-family: 'Caveat', cursive;
      font-size: 1.5rem;
      color: #C9A0A0;
    }

    .divider {
      text-align: center;
      margin: 32px 0;
      color: #8B9E7E;
      font-size: 1.2rem;
      letter-spacing: 0.5em;
      opacity: 0.5;
    }

    .card {
      background: #FAF3E8;
      border: 1px solid #E8D5A3;
      border-radius: 16px;
      padding: 32px;
      margin-bottom: 24px;
      box-shadow: 0 2px 8px rgba(107, 78, 61, 0.08);
      position: relative;
    }

    .card::before {
      content: '';
      position: absolute;
      top: -1px;
      left: 20px;
      right: 20px;
      height: 3px;
      background: linear-gradient(90deg, #8B9E7E, #C9A0A0, #E8D5A3);
      border-radius: 3px;
    }

    .card h2 {
      font-family: 'Cormorant Garamond', serif;
      font-size: 1.6rem;
      font-weight: 500;
      color: #5E7153;
      margin-bottom: 12px;
    }

    .button {
      display: inline-block;
      background: #8B9E7E;
      color: #FDF6EC;
      border: none;
      border-radius: 24px;
      padding: 12px 32px;
      font-family: 'Crimson Text', serif;
      font-size: 1rem;
      font-weight: 600;
      cursor: pointer;
      text-decoration: none;
      transition: all 0.3s ease;
      box-shadow: 0 2px 6px rgba(94, 113, 83, 0.25);
    }

    .button:hover {
      background: #5E7153;
      transform: translateY(-1px);
    }
  </style>
</head>
<body>
  <div class="container">
    <div class="hero">
      <h1>A Quiet Afternoon</h1>
      <p class="subtitle">where wildflowers meet warm linen</p>
    </div>
    <div class="divider">&bull; &bull; &bull;</div>
    <div class="card">
      <h2>From the Garden</h2>
      <p>Sun-warmed tomatoes, trailing rosemary, and the gentle hum of bees
         among the lavender. Every detail is touched by the unhurried rhythm
         of a countryside morning.</p>
    </div>
    <div class="card">
      <h2>By the Hearth</h2>
      <p>A wool blanket, a cup of chamomile, and the crackle of birch logs.
         The design embraces warmth, softness, and the beauty of simple things.</p>
    </div>
    <div style="text-align: center; margin-top: 32px;">
      <a href="#" class="button">Explore the Meadow</a>
    </div>
  </div>
</body>
</html>
```

## Implementation Tips

- **Linen and paper textures**: Use CSS repeating-linear-gradient patterns to simulate textile weave rather than loading heavy image textures
- **Botanical SVG ornaments**: Inline simple SVG leaf or flower motifs for dividers and corners; keep them single-color and low-opacity
- **Warm shadows**: Always tint box-shadows with brown (`rgba(107, 78, 61, 0.08)`) rather than pure black for a softer, warmer feel
- **Muted images**: Apply a slight sepia or warm filter to photographs (`filter: sepia(10%) saturate(85%)`) to maintain palette cohesion
- **Scalloped borders**: Use CSS `radial-gradient` masks or SVG clip-paths for scalloped container edges when you want extra whimsy
- **Avoid pure white**: Use `#FDF6EC` or `#FAF3E8` instead of `#FFFFFF` for backgrounds; pure white feels cold against this palette
