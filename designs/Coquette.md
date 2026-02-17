# Coquette

## Overview

Coquette is a hyper-feminine aesthetic rooted in Rococo romanticism, reinterpreted through a modern lens of soft-focus luxury. It celebrates satin bows, lace trims, pearl accents, blush-pink palettes, and the delicate opulence of a powder room or boudoir. In digital design, Coquette translates into dreamy, soft-edged interfaces with pastel gradients, ornamental script typography, and an atmosphere of playful, whispered elegance. The style gained significant momentum as a TikTok-driven fashion and interior aesthetic before crossing into web and graphic design.

## Visual Characteristics

### Core Design Traits

- **Satin bows and ribbon motifs**: Decorative bow shapes used as dividers, icons, and ornamental accents throughout the design
- **Lace and filigree textures**: Delicate lace-pattern overlays and filigree borders framing content panels and images
- **Blush-pink dominance**: A palette anchored in soft pinks, rose, and champagne tones with cream and ivory neutrals
- **Pearl and jewel accents**: Small circular pearl-like elements, cameo shapes, and gemstone-inspired decorative dots
- **Soft-focus and bloom effects**: Gaussian blur, vignetting, and diffused lighting that create a dreamy, romantic atmosphere
- **Rounded, pillow-soft shapes**: Generous border-radius values, rounded cards, and organic bubble-like containers
- **Rococo-inspired ornament**: Scrollwork, shell motifs, and asymmetric flourishes borrowed from 18th-century French decorative arts

### Design Principles

- Prioritize softness in every visual decision: soft shadows, soft edges, soft colors
- Use white space generously to maintain an airy, breathable composition
- Layer translucent pinks and creams to create depth without heaviness
- Treat ornamentation as charm, not clutter: every bow and pearl should feel intentional
- Maintain a whispered tone: nothing should feel loud, bold, or aggressive
- Embrace asymmetric balance where decorative elements lean gracefully off-center

## Color Palette

| Swatch | Hex | Role |
|--------|-----|------|
| Blush Pink | `#F4C2C2` | Primary surface color, card backgrounds |
| Rose | `#E8A0BF` | Accent buttons, highlighted elements |
| Champagne | `#F7E7CE` | Warm neutral, secondary backgrounds |
| Ivory Cream | `#FFFDF7` | Page background, white space |
| Pearl White | `#FDEEF4` | Soft card fills, overlays |
| Dusty Mauve | `#C9A0A0` | Muted text accents, secondary type |
| French Pink | `#FD6C9E` | Call-to-action, vibrant accent |
| Soft Lavender | `#E6D7F1` | Tertiary accent, decorative details |
| Antique Gold | `#D4AF37` | Metallic accents, filigree details |
| Deep Rose | `#8E4162` | Dark text on light backgrounds |

### CSS Custom Properties

```css
:root {
  --coquette-blush: #F4C2C2;
  --coquette-rose: #E8A0BF;
  --coquette-champagne: #F7E7CE;
  --coquette-ivory: #FFFDF7;
  --coquette-pearl: #FDEEF4;
  --coquette-mauve: #C9A0A0;
  --coquette-french-pink: #FD6C9E;
  --coquette-lavender: #E6D7F1;
  --coquette-gold: #D4AF37;
  --coquette-deep-rose: #8E4162;
}
```

## Typography

### Recommended Google Fonts

| Font | Weight(s) | Usage | Link |
|------|-----------|-------|------|
| **Playfair Display** | 400, 500, 700 | Elegant serif headings with high contrast and romantic flourishes | [Playfair Display](https://fonts.google.com/specimen/Playfair+Display) |
| **Cormorant Infant** | 300, 400, 500 | Soft serif body text with a delicate, youthful character | [Cormorant Infant](https://fonts.google.com/specimen/Cormorant+Infant) |
| **Great Vibes** | 400 | Ornamental script for decorative labels and pull quotes | [Great Vibes](https://fonts.google.com/specimen/Great+Vibes) |
| **Lora** | 400, 500, 600 | Refined body serif with subtle brush contrast | [Lora](https://fonts.google.com/specimen/Lora) |
| **Quicksand** | 300, 400, 500 | Soft rounded sans-serif for UI elements and captions | [Quicksand](https://fonts.google.com/specimen/Quicksand) |

### Font Pairing Suggestions

| Heading | Body | Mood |
|---------|------|------|
| Playfair Display 700 | Cormorant Infant 400 | Romantic editorial, high contrast |
| Great Vibes 400 | Quicksand 400 | Whimsical, playful femininity |
| Playfair Display 500 | Lora 400 | Sophisticated, understated elegance |

### CSS Example

```css
@import url('https://fonts.googleapis.com/css2?family=Playfair+Display:ital,wght@0,400;0,700;1,400&family=Cormorant+Infant:wght@300;400;500&family=Great+Vibes&display=swap');

body {
  font-family: 'Cormorant Infant', 'Georgia', serif;
  font-size: 1.125rem;
  line-height: 1.8;
  color: var(--coquette-deep-rose);
  -webkit-font-smoothing: antialiased;
}

h1, h2, h3 {
  font-family: 'Playfair Display', serif;
  font-weight: 700;
  letter-spacing: 0.01em;
  color: var(--coquette-deep-rose);
}

.script-accent {
  font-family: 'Great Vibes', cursive;
  font-size: 2rem;
  color: var(--coquette-rose);
}
```

## Layout Principles

- **Centered and intimate**: Content blocks are narrow (600-800px max-width) and centered, creating an intimate reading experience
- **Generous vertical rhythm**: Ample spacing between sections (60-100px) allows the soft palette to breathe and prevents visual clutter
- **Layered softness**: Cards and panels use multiple layers of soft shadows and translucent pink overlays to build gentle depth
- **Ornamental margins**: Decorative flourishes, small bow icons, or pearl-dot dividers fill the space between content sections
- **Image treatment**: All images should feel soft-focus with rounded corners, subtle pink-tinted overlays, or vignette borders
- **Responsive approach**: On mobile, maintain generous padding and keep the single-column intimate feel; scale down ornamental elements rather than removing them entirely

## CSS / Design Techniques

### Soft Blush Card

```css
.coquette-card {
  background: var(--coquette-pearl);
  border: 1px solid rgba(232, 160, 191, 0.35);
  border-radius: 24px;
  padding: 40px;
  box-shadow:
    0 4px 24px rgba(244, 194, 194, 0.25),
    0 1px 4px rgba(142, 65, 98, 0.06);
  position: relative;
}

.coquette-card::before {
  content: '';
  position: absolute;
  top: -1px;
  left: 20%;
  right: 20%;
  height: 2px;
  background: linear-gradient(to right, transparent, var(--coquette-rose), transparent);
}
```

### Ribbon Button

```css
.coquette-button {
  background: linear-gradient(135deg, var(--coquette-rose) 0%, var(--coquette-french-pink) 100%);
  color: #FFFDF7;
  border: none;
  border-radius: 50px;
  padding: 14px 36px;
  font-family: 'Playfair Display', serif;
  font-weight: 500;
  font-size: 0.95rem;
  letter-spacing: 0.06em;
  cursor: pointer;
  box-shadow: 0 4px 16px rgba(253, 108, 158, 0.30);
  transition: all 0.3s ease;
}

.coquette-button:hover {
  transform: translateY(-2px);
  box-shadow: 0 6px 24px rgba(253, 108, 158, 0.45);
}
```

### Lace-Border Navigation

```css
.coquette-nav {
  background: var(--coquette-ivory);
  border-bottom: 1px solid rgba(232, 160, 191, 0.30);
  padding: 20px 40px;
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 40px;
  position: relative;
}

.coquette-nav::after {
  content: '';
  position: absolute;
  bottom: -4px;
  left: 0;
  right: 0;
  height: 4px;
  background: repeating-linear-gradient(
    90deg,
    transparent 0px,
    transparent 6px,
    var(--coquette-blush) 6px,
    var(--coquette-blush) 8px
  );
}

.coquette-nav a {
  color: var(--coquette-deep-rose);
  font-family: 'Quicksand', sans-serif;
  font-size: 0.85rem;
  font-weight: 500;
  letter-spacing: 0.1em;
  text-transform: uppercase;
  text-decoration: none;
  transition: color 0.3s ease;
}

.coquette-nav a:hover {
  color: var(--coquette-french-pink);
}
```

### Dreamy Hero Section

```css
.coquette-hero {
  background: linear-gradient(180deg, var(--coquette-pearl) 0%, var(--coquette-ivory) 100%);
  text-align: center;
  padding: 100px 40px;
  position: relative;
  overflow: hidden;
}

.coquette-hero::before {
  content: '';
  position: absolute;
  top: -50%;
  left: -25%;
  width: 150%;
  height: 150%;
  background: radial-gradient(ellipse at 50% 30%, rgba(244, 194, 194, 0.25) 0%, transparent 60%);
  pointer-events: none;
}

.coquette-hero h1 {
  font-family: 'Playfair Display', serif;
  font-size: 3.5rem;
  font-weight: 700;
  font-style: italic;
  color: var(--coquette-deep-rose);
  position: relative;
}

.coquette-hero .script {
  font-family: 'Great Vibes', cursive;
  font-size: 1.5rem;
  color: var(--coquette-rose);
  display: block;
  margin-bottom: 8px;
}
```

### Pearl Divider

```css
.coquette-divider {
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 12px;
  margin: 48px 0;
}

.coquette-divider::before,
.coquette-divider::after {
  content: '';
  width: 80px;
  height: 1px;
  background: linear-gradient(to right, transparent, var(--coquette-rose), transparent);
}

.coquette-divider span {
  width: 8px;
  height: 8px;
  background: var(--coquette-rose);
  border-radius: 50%;
  box-shadow: 0 0 6px rgba(232, 160, 191, 0.5);
}
```

## Design Do's and Don'ts

### Do

- Use soft, diffused shadows instead of harsh drop shadows
- Layer translucent pinks to create warmth and depth
- Include ornamental script typography for decorative labels and accents
- Round all corners generously (16-32px border-radius)
- Apply soft-focus or pink-tinted treatments to photography
- Use pearl-dot patterns and bow motifs as recurring decorative elements
- Maintain a light, airy composition with abundant white space

### Don't

- Use sharp geometric angles or hard-edged containers
- Apply bold, saturated primary colors (bright red, electric blue) that overpower the soft palette
- Set all text in script fonts; reserve cursive for accents and small labels only
- Use heavy black shadows or dark backgrounds that contradict the dreamy lightness
- Crowd the layout with too many competing ornaments
- Use industrial or brutalist typefaces; the style requires elegance and softness
- Combine Coquette with grunge, cyberpunk, or other hard-edged aesthetics

## Related Aesthetics

| Aesthetic | Relationship |
|-----------|-------------|
| **Rococo** | Direct historical ancestor; Coquette borrows its pastel palette, gilded ornament, and asymmetric flourishes |
| **Baroque** | Shares opulence and ornamentation but Baroque is heavier, darker, and more dramatically theatrical |
| **Cottagecore** | Both celebrate femininity and softness; Cottagecore is rustic and rural while Coquette is urban and luxurious |
| **Art Nouveau** | Shares flowing organic curves and decorative elegance; Art Nouveau is more botanical and structural |
| **Coastal Style** | Overlaps in soft, light color palettes; Coastal is breezy and nautical rather than romantic and ornate |
| **Maximalism** | Coquette's ornamental density shares maximalist instincts but constrains them within a pastel, feminine register |

## Quick-Start HTML Template

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Coquette Layout</title>
  <link href="https://fonts.googleapis.com/css2?family=Playfair+Display:ital,wght@0,400;0,700;1,400&family=Cormorant+Infant:wght@300;400;500&family=Great+Vibes&display=swap" rel="stylesheet">
  <style>
    *, *::before, *::after { margin: 0; padding: 0; box-sizing: border-box; }

    body {
      font-family: 'Cormorant Infant', Georgia, serif;
      font-size: 1.125rem;
      line-height: 1.8;
      color: #8E4162;
      background: #FFFDF7;
      min-height: 100vh;
    }

    .nav {
      background: #FFFDF7;
      border-bottom: 1px solid rgba(232,160,191,0.30);
      padding: 20px 40px;
      display: flex;
      align-items: center;
      justify-content: center;
      gap: 40px;
    }

    .nav a {
      color: #8E4162;
      font-family: 'Cormorant Infant', serif;
      font-size: 0.9rem;
      font-weight: 500;
      letter-spacing: 0.1em;
      text-transform: uppercase;
      text-decoration: none;
    }

    .hero {
      background: linear-gradient(180deg, #FDEEF4 0%, #FFFDF7 100%);
      text-align: center;
      padding: 100px 40px;
      position: relative;
      overflow: hidden;
    }

    .hero::before {
      content: '';
      position: absolute;
      top: -50%; left: -25%; width: 150%; height: 150%;
      background: radial-gradient(ellipse at 50% 30%, rgba(244,194,194,0.25) 0%, transparent 60%);
    }

    .hero .script {
      font-family: 'Great Vibes', cursive;
      font-size: 1.5rem;
      color: #E8A0BF;
      display: block;
      position: relative;
    }

    .hero h1 {
      font-family: 'Playfair Display', serif;
      font-size: 3rem;
      font-weight: 700;
      font-style: italic;
      color: #8E4162;
      position: relative;
    }

    .hero p {
      max-width: 520px;
      margin: 16px auto 0;
      color: #C9A0A0;
      position: relative;
    }

    .content {
      max-width: 800px;
      margin: 60px auto;
      padding: 0 40px;
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 32px;
    }

    .card {
      background: #FDEEF4;
      border: 1px solid rgba(232,160,191,0.35);
      border-radius: 24px;
      padding: 36px;
      box-shadow: 0 4px 24px rgba(244,194,194,0.25);
    }

    .card h2 {
      font-family: 'Playfair Display', serif;
      font-weight: 700;
      font-size: 1.4rem;
      color: #8E4162;
      margin-bottom: 12px;
    }

    .card p {
      color: #8E4162;
      line-height: 1.8;
    }

    .button {
      display: inline-block;
      margin-top: 20px;
      background: linear-gradient(135deg, #E8A0BF 0%, #FD6C9E 100%);
      color: #FFFDF7;
      border: none;
      border-radius: 50px;
      padding: 12px 32px;
      font-family: 'Playfair Display', serif;
      font-size: 0.9rem;
      letter-spacing: 0.06em;
      text-decoration: none;
      cursor: pointer;
      box-shadow: 0 4px 16px rgba(253,108,158,0.30);
    }

    .divider {
      grid-column: 1 / -1;
      display: flex;
      align-items: center;
      justify-content: center;
      gap: 12px;
    }

    .divider::before, .divider::after {
      content: '';
      width: 80px;
      height: 1px;
      background: linear-gradient(to right, transparent, #E8A0BF, transparent);
    }

    .divider span {
      width: 8px;
      height: 8px;
      background: #E8A0BF;
      border-radius: 50%;
    }
  </style>
</head>
<body>
  <nav class="nav">
    <a href="#">Boudoir</a>
    <a href="#">Collection</a>
    <a href="#">Atelier</a>
    <a href="#">About</a>
  </nav>
  <header class="hero">
    <span class="script">une petite</span>
    <h1>Coquette</h1>
    <p>Satin bows, lace, blush pink, pearls, and the soft-focus
       delicacy of Rococo romance.</p>
  </header>
  <main class="content">
    <div class="card">
      <h2>Satin & Pearl</h2>
      <p>Layers of blush satin and scattered pearls create
         an atmosphere of whispered feminine luxury.</p>
      <a href="#" class="button">Discover</a>
    </div>
    <div class="card">
      <h2>Lace & Ribbon</h2>
      <p>Delicate lace borders and silk ribbon bows frame
         every detail with Rococo tenderness.</p>
      <a href="#" class="button">Explore</a>
    </div>
  </main>
</body>
</html>
```
