# Tuscan Rustic Design Reference

Tuscan Rustic is an aesthetic rooted in the **rural Italian countryside**, evoking the warmth and simplicity of a Tuscan farmhouse or villa. It emphasizes **earth tones, natural materials, handcrafted details, and a lived-in sense of enduring history**. The style celebrates wrought iron, exposed stone, terracotta, distressed wood, and sun-baked plaster -- all arranged with a non-fussy, welcoming elegance that prioritizes comfort and warmth over refinement. Every surface tells a story of age, use, and organic beauty.

---

## Visual Characteristics

### Core Motifs and Patterns

- **Wrought iron scrollwork** -- ornamental curling iron details used for railings, gates, fixtures, dividers, and decorative accents
- **Grape vines and olive branches** -- trailing botanical motifs suggesting Tuscan vineyards and orchards
- **Terracotta tile patterns** -- warm, earthy repeating tile grids evoking Italian "cotto" flooring
- **Arched forms** -- rounded archways over doors, windows, and content frames inspired by Italian villa architecture
- **Deruta-style painted plates** -- colorful hand-painted ceramic medallions used as decorative focal points
- **Exposed ceiling beams** -- heavy, dark horizontal timber elements crossing overhead
- **Stone and brick textures** -- rough, porous natural stone surfaces and aged brick patterns
- **Rustic pottery silhouettes** -- round-bellied wine jugs, olive oil vessels, and terracotta planters
- **Wooden shutters (persiane)** -- louvered or paneled window shutters suggesting Mediterranean warmth
- **Hand-carved wood details** -- ornamental woodworking with visible grain, knots, and distressed finish

### Design Principles

- **Warm, earthy, grounded composition** -- every element should feel sun-baked, weathered, and rooted in the land
- **Non-fussy simplicity** -- functional elegance without pretension; rustic but never sloppy
- **Textural richness** -- layered surfaces suggesting stone, plaster, wood, and iron rather than flat digital smoothness
- **Lived-in authenticity** -- imperfections are welcomed; distressed, aged, and hand-finished feels preferred over machine precision
- **Indoor-outdoor continuity** -- blurred boundaries evoking courtyards, terraces, and open countryside
- **Substantial weight** -- heavy, solid elements conveying permanence and rootedness
- **Warm light and golden atmosphere** -- everything bathed in the amber glow of late-afternoon Tuscan sun

---

## Color Palette

### Primary Scheme

| Role | Colors |
|------|--------|
| **Base** | Warm cream, aged plaster white, sandstone beige |
| **Primary accents** | Terracotta, burnt sienna, olive green |
| **Warm neutrals** | Warm brown, walnut, aged timber |
| **Rich accents** | Deep red wine, burnished gold, rustic copper |

### Full Palette

| Color | Hex | Usage |
|-------|-----|-------|
| Aged Plaster | `#F5EDE0` | Primary backgrounds, wall surfaces |
| Warm Cream | `#FAF3E6` | Light backgrounds, card surfaces |
| Sandstone | `#D9C9A5` | Secondary backgrounds, footer areas, subtle fills |
| Terracotta | `#C2703E` | Primary accent, links, buttons, key decorative elements |
| Burnt Sienna | `#A0522D` | Warm midtone accent, borders, hover states |
| Tuscan Red | `#8B3A2F` | Deep accent, headings on light backgrounds, rich panels |
| Olive Green | `#6B7035` | Secondary accent, botanical elements, success states |
| Deep Olive | `#4A4F28` | Dark accent, text on light backgrounds |
| Walnut Brown | `#5C4033` | Body text, structural elements, dark accents |
| Aged Timber | `#7B6348` | Secondary text, muted UI elements, borders |
| Burnished Gold | `#C19A3E` | Metallic accents, ornamental details, highlights |
| Rustic Copper | `#B87333` | Warm metallic accent, interactive elements |
| Wrought Iron | `#3B3131` | Dark structural elements, text on warm backgrounds |
| Wine | `#722F37` | Deep accent panels, dramatic sections |
| Tuscan Sun | `#E8B84B` | Warm highlights, call-to-action, notification accents |
| Sage Leaf | `#9CAD7F` | Tertiary accent, subtle botanical details |

### Suggested CSS Custom Properties

```css
:root {
  /* Backgrounds */
  --tuscan-plaster: #f5ede0;
  --tuscan-cream: #faf3e6;
  --tuscan-sandstone: #d9c9a5;

  /* Earth tones */
  --tuscan-terracotta: #c2703e;
  --tuscan-sienna: #a0522d;
  --tuscan-red: #8b3a2f;
  --tuscan-wine: #722f37;

  /* Greens */
  --tuscan-olive: #6b7035;
  --tuscan-olive-deep: #4a4f28;
  --tuscan-sage: #9cad7f;

  /* Browns */
  --tuscan-walnut: #5c4033;
  --tuscan-timber: #7b6348;
  --tuscan-iron: #3b3131;

  /* Metallics */
  --tuscan-gold: #c19a3e;
  --tuscan-copper: #b87333;
  --tuscan-sun: #e8b84b;

  /* Functional */
  --tuscan-bg-primary: var(--tuscan-plaster);
  --tuscan-bg-secondary: var(--tuscan-cream);
  --tuscan-bg-accent: var(--tuscan-sandstone);
  --tuscan-text-primary: var(--tuscan-walnut);
  --tuscan-text-secondary: var(--tuscan-timber);
  --tuscan-accent: var(--tuscan-terracotta);
  --tuscan-accent-dark: var(--tuscan-sienna);
  --tuscan-border: var(--tuscan-timber);
  --tuscan-cta: var(--tuscan-sun);
}
```

### Approaches

- **Warm plaster and cream base** -- dominant light backgrounds that feel sun-warmed rather than clinical white
- **Terracotta as the signature accent** -- the defining color, used consistently for links, buttons, and decorative elements
- **Earth tones for grounding** -- walnut, sienna, and timber tones create depth without coldness
- **Olive green for natural contrast** -- botanical greens used sparingly for secondary accents and variety
- **Gold and copper for warmth** -- metallic warm accents suggesting aged fixtures and afternoon sunlight
- **Never use pure white or pure black** -- all tones should feel organically warm and slightly aged

---

## Typography

### Typeface Characteristics

Tuscan Rustic typography features:

- **Warm, traditional serif typefaces** with old-style proportions -- evoking hand-set Italian print
- **Medium to regular font weights** -- solid and readable but never heavy or oppressive
- **Generous line-height** -- relaxed, unhurried spacing reflecting the Tuscan pace of life
- **Slightly rough or organic letterforms** -- typefaces that suggest hand-carving or letterpress printing
- **Italic used for warmth** -- gentle italic for accents, quotes, and decorative labels
- **Serif for both headings and body** -- maintaining consistency with the traditional, pre-digital feel
- **Script fonts sparingly** -- for decorative accents only, evoking hand-painted Italian signage

### Recommended Web Fonts (Google Fonts)

| Font | Style | Usage |
|------|-------|-------|
| **Playfair Display** | Elegant transitional serif | Headlines, hero text |
| **Lora** | Brushed, warm serif | Headlines, feature titles |
| **Cormorant Garamond** | Organic old-style serif | Body text, subheadings |
| **EB Garamond** | Classic humanist serif | Body copy, long-form reading |
| **Libre Baskerville** | Refined transitional serif | Body text, pull quotes |
| **Cinzel** | Roman inscriptional capitals | Section titles, formal headings |
| **Sorts Mill Goudy** | Warm, aged old-style serif | Body text, captions |
| **Great Vibes** | Flowing calligraphic script | Decorative accents, taglines |
| **Satisfy** | Casual brush script | Hand-painted sign feel, labels |
| **Josefin Slab** | Geometric slab serif | Navigation, UI elements |

### Typography CSS Example

```css
/* Headlines */
h1, h2, h3 {
  font-family: 'Playfair Display', 'Lora', Georgia, serif;
  color: var(--tuscan-walnut);
  font-weight: 400;
  letter-spacing: 0.02em;
  line-height: 1.3;
}

/* Display / Hero text */
.tuscan-display {
  font-family: 'Playfair Display', serif;
  font-size: clamp(2.5rem, 6vw, 5rem);
  font-weight: 400;
  letter-spacing: 0.04em;
  line-height: 1.15;
  color: var(--tuscan-red);
}

/* Body text */
body {
  font-family: 'Cormorant Garamond', 'EB Garamond', Georgia, serif;
  font-weight: 400;
  font-size: 1.1rem;
  letter-spacing: 0.01em;
  line-height: 1.8;
  color: var(--tuscan-walnut);
}

/* Decorative script accent */
.tuscan-script {
  font-family: 'Great Vibes', 'Satisfy', cursive;
  font-size: 1.5em;
  color: var(--tuscan-terracotta);
  font-weight: 400;
}

/* Navigation */
nav a {
  font-family: 'Josefin Slab', 'Libre Baskerville', serif;
  text-transform: uppercase;
  font-size: 0.85rem;
  letter-spacing: 0.1em;
  font-weight: 400;
  color: var(--tuscan-timber);
}
```

---

## Layout Principles

### Grid and Structure

- **Warm, grounded layouts** -- generous padding with an earthy, settled feel; nothing floats or feels weightless
- **Medium-width containers** -- max-width of 1000-1200px with comfortable side margins
- **Symmetrical, centered composition** -- balanced and traditional, reflecting Italian villa architecture
- **Arched hero sections** -- large sections with rounded top edges or arch-shaped clipping evoking stone doorways
- **Card-based content with texture** -- cards that feel like stone tablets or aged paper rather than flat digital panels
- **Horizontal timber-beam dividers** -- thick, dark separators between sections evoking exposed ceiling beams

### Section Organization

- Use **wrought iron-style dividers** between sections (ornamental scrollwork separators)
- Apply **generous vertical spacing** -- 5-7rem between major sections, unhurried and open
- Create **hierarchy through warmth and weight** -- darker earth tones for emphasis, lighter plaster tones for supporting content
- Employ **arched containers** -- rounded-top frames for hero elements and featured content
- Use **textured backgrounds** -- subtle plaster, stone, or linen textures rather than flat solid colors
- Incorporate **terracotta tile-pattern section borders** -- decorative top/bottom edges on accent sections

---

## CSS/Design Techniques

### Arch-Shaped Container

```css
.tuscan-arch {
  border-radius: 50% 50% 8px 8px / 25% 25% 8px 8px;
  overflow: hidden;
  background: var(--tuscan-cream);
  border: 3px solid var(--tuscan-timber);
  padding: 3rem 2.5rem 2.5rem;
}
```

### Tuscan Card / Stone Panel

```css
.tuscan-card {
  background: var(--tuscan-cream);
  border: 2px solid var(--tuscan-sandstone);
  border-radius: 8px;
  padding: 2rem 2.5rem;
  position: relative;
  box-shadow:
    0 2px 8px rgba(92, 64, 51, 0.08),
    0 8px 24px rgba(92, 64, 51, 0.06);
  transition: box-shadow 0.3s ease, transform 0.3s ease;
}

.tuscan-card:hover {
  box-shadow:
    0 4px 12px rgba(92, 64, 51, 0.12),
    0 12px 32px rgba(92, 64, 51, 0.08);
  transform: translateY(-2px);
}
```

### Plaster Wall Texture

```css
/* Subtle aged plaster texture overlay */
.tuscan-plaster-texture {
  position: relative;
}

.tuscan-plaster-texture::before {
  content: '';
  position: absolute;
  inset: 0;
  background-image: url("data:image/svg+xml,%3Csvg width='60' height='60' xmlns='http://www.w3.org/2000/svg'%3E%3Cfilter id='n'%3E%3CfeTurbulence baseFrequency='0.5' numOctaves='4' stitchTiles='stitch'/%3E%3C/filter%3E%3Crect width='100%25' height='100%25' filter='url(%23n)' opacity='0.04'/%3E%3C/svg%3E");
  pointer-events: none;
  opacity: 0.5;
}
```

### Wrought Iron Divider

```css
.tuscan-divider {
  height: 0;
  border: none;
  border-top: 2px solid var(--tuscan-timber);
  margin: 3rem auto;
  width: 50%;
  position: relative;
}

.tuscan-divider::before {
  content: '\2766'; /* floral heart ornament */
  position: absolute;
  top: -0.65em;
  left: 50%;
  transform: translateX(-50%);
  background: var(--tuscan-plaster);
  padding: 0 0.6em;
  color: var(--tuscan-iron);
  font-size: 1.1rem;
}

/* Double iron scroll variant */
.tuscan-divider-scroll {
  height: 30px;
  width: 40%;
  margin: 2.5rem auto;
  background: no-repeat center / 80% auto;
  background-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 300 30'%3E%3Cpath d='M0,15 C30,5 60,25 90,15 C120,5 150,25 180,15 C210,5 240,25 270,15 L300,15' fill='none' stroke='%233b3131' stroke-width='1.5'/%3E%3Ccircle cx='150' cy='15' r='4' fill='none' stroke='%233b3131' stroke-width='1.5'/%3E%3C/svg%3E");
  opacity: 0.6;
}
```

### Tuscan Warm Gradient Backgrounds

```css
/* Golden-hour gradient for hero sections */
.tuscan-gradient-hero {
  background: linear-gradient(
    180deg,
    var(--tuscan-cream) 0%,
    var(--tuscan-sandstone) 60%,
    var(--tuscan-plaster) 100%
  );
  min-height: 50vh;
  display: flex;
  align-items: center;
  justify-content: center;
}

/* Warm earth gradient for accent sections */
.tuscan-gradient-earth {
  background: linear-gradient(
    180deg,
    var(--tuscan-plaster) 0%,
    #ede0cc 50%,
    var(--tuscan-sandstone) 100%
  );
}

/* Sunset wash for dramatic sections */
.tuscan-gradient-sunset {
  background: linear-gradient(
    135deg,
    rgba(194, 112, 62, 0.08) 0%,
    rgba(139, 58, 47, 0.05) 50%,
    rgba(107, 112, 53, 0.06) 100%
  );
}
```

### Terracotta Tile Pattern

```css
/* Repeating terracotta tile grid */
.tuscan-tile-border {
  height: 12px;
  background: repeating-linear-gradient(
    90deg,
    var(--tuscan-terracotta) 0px,
    var(--tuscan-terracotta) 20px,
    var(--tuscan-sandstone) 20px,
    var(--tuscan-sandstone) 22px
  );
  opacity: 0.5;
}

/* Diamond tile pattern */
.tuscan-tile-bg {
  background-color: var(--tuscan-plaster);
  background-image: url("data:image/svg+xml,%3Csvg width='40' height='40' xmlns='http://www.w3.org/2000/svg'%3E%3Cpath d='M20 0 L40 20 L20 40 L0 20 Z' fill='none' stroke='%23c2703e' stroke-width='0.5' opacity='0.1'/%3E%3C/svg%3E");
}
```

### Stone Wall Texture

```css
/* Rough stone surface simulation */
.tuscan-stone {
  background-color: var(--tuscan-sandstone);
  background-image:
    radial-gradient(ellipse at 30% 40%, rgba(92, 64, 51, 0.06) 0%, transparent 50%),
    radial-gradient(ellipse at 70% 60%, rgba(123, 99, 72, 0.08) 0%, transparent 40%),
    radial-gradient(ellipse at 50% 20%, rgba(160, 82, 45, 0.04) 0%, transparent 45%);
}
```

### Button Styles

```css
/* Primary -- Terracotta */
.tuscan-btn-primary {
  background: var(--tuscan-terracotta);
  color: var(--tuscan-cream);
  border: none;
  padding: 0.75rem 2rem;
  border-radius: 6px;
  font-family: 'Libre Baskerville', serif;
  font-size: 0.9rem;
  letter-spacing: 0.06em;
  cursor: pointer;
  transition: background 0.3s ease, transform 0.15s ease;
}

.tuscan-btn-primary:hover {
  background: var(--tuscan-sienna);
  transform: translateY(-1px);
}

/* Secondary -- Outlined */
.tuscan-btn-secondary {
  background: transparent;
  color: var(--tuscan-terracotta);
  border: 2px solid var(--tuscan-terracotta);
  padding: 0.7rem 1.8rem;
  border-radius: 6px;
  font-family: 'Libre Baskerville', serif;
  font-size: 0.9rem;
  letter-spacing: 0.06em;
  cursor: pointer;
  transition: all 0.3s ease;
}

.tuscan-btn-secondary:hover {
  background: var(--tuscan-terracotta);
  color: var(--tuscan-cream);
}

/* Warm CTA -- Tuscan Sun */
.tuscan-btn-cta {
  background: var(--tuscan-sun);
  color: var(--tuscan-walnut);
  border: none;
  padding: 0.85rem 2.2rem;
  border-radius: 6px;
  font-family: 'Libre Baskerville', serif;
  font-size: 0.95rem;
  letter-spacing: 0.04em;
  font-weight: 600;
  cursor: pointer;
  transition: background 0.3s ease, box-shadow 0.3s ease;
}

.tuscan-btn-cta:hover {
  background: #d4a63a;
  box-shadow: 0 4px 16px rgba(232, 184, 75, 0.3);
}
```

### Image Treatment

```css
/* Aged frame with warm shadow */
.tuscan-img {
  border-radius: 6px;
  border: 3px solid var(--tuscan-sandstone);
  box-shadow: 0 6px 20px rgba(92, 64, 51, 0.15);
  object-fit: cover;
}

/* Rustic framed image */
.tuscan-frame {
  background: var(--tuscan-cream);
  padding: 10px;
  border: 2px solid var(--tuscan-timber);
  border-radius: 4px;
  box-shadow:
    0 4px 12px rgba(92, 64, 51, 0.12),
    inset 0 0 8px rgba(92, 64, 51, 0.05);
  display: inline-block;
}

/* Warm overlay for images */
.tuscan-overlay {
  position: relative;
}

.tuscan-overlay::after {
  content: '';
  position: absolute;
  inset: 0;
  background: linear-gradient(
    180deg,
    rgba(194, 112, 62, 0.0) 40%,
    rgba(92, 64, 51, 0.5) 100%
  );
  border-radius: 6px;
}
```

### Warm Glow / Afternoon Light Effect

```css
/* Golden-hour radial warmth behind focal elements */
.tuscan-glow {
  background: radial-gradient(
    ellipse at 50% 40%,
    rgba(232, 184, 75, 0.1) 0%,
    rgba(194, 112, 62, 0.05) 40%,
    transparent 70%
  );
}

/* Warm inner glow for panels */
.tuscan-inner-glow {
  box-shadow:
    inset 0 0 40px rgba(194, 112, 62, 0.04),
    0 4px 16px rgba(92, 64, 51, 0.08);
}
```

---

## Materials and Textures (Visual Metaphors for Web)

Physical Tuscan Rustic materials and their web equivalents:

| Physical Material | Web Equivalent |
|-------------------|----------------|
| Aged plaster walls | Warm cream/beige backgrounds with subtle noise texture overlays |
| Terracotta tile | Warm orange-brown accent colors, repeating tile-grid patterns |
| Exposed stone | Mottled multi-tone beige backgrounds with radial gradient variation |
| Distressed wood | Dark brown tones with visible grain-like horizontal line patterns |
| Wrought iron | Dark iron-gray decorative borders, ornamental Unicode dividers, SVG scrollwork |
| Travertine / Marble | Light warm stone backgrounds with faint veining via diagonal gradient streaks |
| Brick | Warm red-brown repeating patterns, rough-textured accent borders |
| Linen / Natural fabric | Subtle canvas-weave texture overlays at very low opacity |
| Copper / Brass fixtures | Warm metallic gradient accents (`#b87333` to `#c19a3e`) |
| Hand-painted ceramic | Colorful decorative accent elements, circular medallion shapes |
| Olive wood | Rich warm brown tones with organic, swirling grain suggestion |
| Roof tiles | Warm terracotta repeating scallop patterns for decorative borders |

---

## Sub-styles and Variations

### Tuscan Villa

- Emphasis on **architectural grandeur** -- arched colonnades, symmetrical facades, formal gardens
- Marble and travertine flooring dominating over rough stone
- More refined and polished while retaining earthy warmth
- Web approach: wider layouts, arched containers, symmetrical grids, marble-texture backgrounds, slightly more formal typography

### Tuscan Farmhouse (Rustico)

- The most **rustic and informal** variant -- rough stone, heavy timber, agricultural simplicity
- Emphasis on reclaimed and salvaged materials, visible repairs and patching
- Hearth and kitchen as the spiritual center
- Web approach: heavier textures, more distressed effects, darker earth tones, chunky borders, hand-drawn-feeling elements

### Modern Tuscan

- Blends traditional Tuscan warmth with **contemporary clean lines**
- Retains the color palette and materials but simplifies ornamentation
- Open-plan layouts, minimal decorative clutter
- Web approach: cleaner grid, fewer textures, simplified palette (cream + terracotta + olive only), modern sans-serif body type

---

## Related Aesthetics

| Aesthetic | Relationship to Tuscan Rustic |
|-----------|-------------------------------|
| **Rustic** | Parent aesthetic; Tuscan Rustic is a regional Italian specialization |
| **French Provincial Style** | Sibling style; similar warmth and countryside feel with French inflections |
| **Country** | Broader rural aesthetic; Tuscan Rustic adds Italian architectural specificity |
| **Coastal Style** | Overlapping Mediterranean warmth; Coastal leans maritime, Tuscan leans inland |
| **Eco-Beige** | Shared earth-tone palette and natural-material emphasis; Eco-Beige is more minimal |
| **Autumn** | Shared warm color palette of oranges, browns, and golds |
| **Frasurbane** | Suburban comfort aesthetic with overlapping warm, traditional sensibilities |

---

## Quick-Start: Minimal Tuscan Rustic Page Template

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Tuscan Rustic Page</title>
  <link href="https://fonts.googleapis.com/css2?family=Playfair+Display:ital,wght@0,400;0,600;1,400&family=Cormorant+Garamond:ital,wght@0,400;0,500;1,400&family=Great+Vibes&display=swap" rel="stylesheet">
  <style>
    :root {
      --tuscan-plaster: #f5ede0;
      --tuscan-cream: #faf3e6;
      --tuscan-sandstone: #d9c9a5;
      --tuscan-terracotta: #c2703e;
      --tuscan-sienna: #a0522d;
      --tuscan-red: #8b3a2f;
      --tuscan-olive: #6b7035;
      --tuscan-walnut: #5c4033;
      --tuscan-timber: #7b6348;
      --tuscan-iron: #3b3131;
      --tuscan-gold: #c19a3e;
      --tuscan-sun: #e8b84b;
    }

    * { margin: 0; padding: 0; box-sizing: border-box; }

    body {
      background: var(--tuscan-plaster);
      color: var(--tuscan-walnut);
      font-family: 'Cormorant Garamond', Georgia, serif;
      font-weight: 400;
      font-size: 1.1rem;
      line-height: 1.8;
      letter-spacing: 0.01em;
    }

    h1, h2, h3 {
      font-family: 'Playfair Display', Georgia, serif;
      color: var(--tuscan-walnut);
      font-weight: 400;
      letter-spacing: 0.02em;
    }

    .hero {
      background: linear-gradient(
        180deg,
        var(--tuscan-cream) 0%,
        var(--tuscan-sandstone) 80%,
        var(--tuscan-plaster) 100%
      );
      text-align: center;
      padding: 8rem 2rem 6rem;
      position: relative;
    }

    .hero h1 {
      font-size: clamp(2.5rem, 6vw, 4.5rem);
      font-weight: 400;
      color: var(--tuscan-red);
      margin-bottom: 0.5rem;
    }

    .hero .subtitle {
      font-family: 'Great Vibes', cursive;
      font-size: 1.8rem;
      color: var(--tuscan-terracotta);
    }

    /* Wrought iron ornament divider */
    .tuscan-divider {
      width: 50%;
      margin: 2rem auto;
      border: none;
      border-top: 2px solid var(--tuscan-timber);
      position: relative;
    }

    .tuscan-divider::before {
      content: '\2766';
      position: absolute;
      top: -0.65em;
      left: 50%;
      transform: translateX(-50%);
      background: var(--tuscan-plaster);
      padding: 0 0.6em;
      color: var(--tuscan-iron);
      font-size: 1.1rem;
    }

    section {
      max-width: 960px;
      margin: 0 auto;
      padding: 4rem 2rem;
    }

    section h2 {
      margin-bottom: 1.5rem;
    }

    .card-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
      gap: 2rem;
      margin-top: 2rem;
    }

    .card {
      background: var(--tuscan-cream);
      border: 2px solid var(--tuscan-sandstone);
      border-radius: 8px;
      padding: 2rem;
      box-shadow:
        0 2px 8px rgba(92, 64, 51, 0.08),
        0 8px 24px rgba(92, 64, 51, 0.06);
    }

    .card h3 {
      color: var(--tuscan-terracotta);
      margin-bottom: 0.75rem;
    }

    .accent-section {
      background: linear-gradient(
        180deg,
        var(--tuscan-plaster) 0%,
        #ede0cc 50%,
        var(--tuscan-sandstone) 100%
      );
    }

    /* Terracotta tile border */
    .tile-border {
      height: 8px;
      background: repeating-linear-gradient(
        90deg,
        var(--tuscan-terracotta) 0px,
        var(--tuscan-terracotta) 18px,
        var(--tuscan-sandstone) 18px,
        var(--tuscan-sandstone) 20px
      );
      opacity: 0.4;
    }
  </style>
</head>
<body>
  <div class="hero">
    <h1>Tuscan Rustic</h1>
    <div class="subtitle">Warmth from the Italian Countryside</div>
    <hr class="tuscan-divider">
  </div>

  <div class="tile-border"></div>

  <section class="accent-section">
    <h2>Section Heading</h2>
    <p>Content with Tuscan Rustic styling applied. Warm earth tones, aged textures, and handcrafted details evoke the Italian countryside.</p>
    <div class="card-grid">
      <div class="card">
        <h3>Card Title</h3>
        <p>Stone-like cards with warm shadows and sandstone borders feel grounded and substantial.</p>
      </div>
      <div class="card">
        <h3>Card Title</h3>
        <p>Natural materials and earthy palettes define the Tuscan approach to warmth and simplicity.</p>
      </div>
    </div>
  </section>
</body>
</html>
```
