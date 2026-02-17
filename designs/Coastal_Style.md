# Coastal Style Design Reference

Coastal Style is an aesthetic that evokes **the feeling of being by the sea**, integrating elements reminiscent of ocean and beach environments into design. It draws inspiration from locations such as the Hamptons, Western France, and the Mediterranean coast. The style emphasizes **natural light, open spaces, relaxed elegance**, and a palette drawn directly from the shoreline -- sky, sea, sand, driftwood, and weathered stone.

---

## Visual Characteristics

### Core Motifs and Patterns

- **Nautical elements** -- anchors, lifebuoys, ship wheels, compass roses, rope knots
- **Marine life** -- seashells, starfish, coral, seahorses, fish silhouettes
- **Stripes** -- horizontal or vertical nautical-inspired stripe patterns, particularly navy/white
- **Wave patterns** -- undulating, organic wave forms as borders, dividers, or background textures
- **Natural textures** -- woven fibers, rope, driftwood grain, linen weave, sand ripples
- **Weathered / distressed finishes** -- surfaces that appear sun-bleached, salt-worn, or naturally aged
- **Fishing nets and rope accents** -- decorative netting overlays, knotted rope details

### Design Principles

- **Light and airy composition** -- abundant whitespace evoking open skies and wide beaches
- **Open-concept layouts** maximizing the feeling of spaciousness and natural light
- **Casual, relaxed elegance** -- polished but never stiff or overly formal
- **Indoor-outdoor flow** -- blurred boundaries between content sections, seamless transitions
- **Natural material emphasis** -- textures and patterns drawn from organic, coastal materials
- **Layered neutrals with blue accents** -- a restrained base palette punctuated by ocean tones
- **Soft, diffused visual weight** -- avoid hard edges and heavy shadows in favor of gentle gradients

---

## Color Palette

### Primary Scheme

| Role | Colors |
|------|--------|
| **Base** | White, off-white, warm cream |
| **Primary accents** | Ocean blue, sky blue, seafoam |
| **Warm neutrals** | Sand beige, driftwood taupe, pebble gray |

### Full Palette

| Color | Hex | Usage |
|-------|-----|-------|
| Crisp White | `#FFFFFF` | Primary backgrounds, clean open space |
| Linen White | `#F5F0E8` | Warm background alternative, card surfaces |
| Sand | `#E2D7B0` | Secondary backgrounds, footer areas, subtle fills |
| Driftwood | `#847968` | Body text on light backgrounds, muted UI elements |
| Pebble Gray | `#AFBCC5` | Borders, dividers, secondary text |
| Ocean Blue | `#297685` | Primary accent, links, buttons, key headings |
| Sky Blue | `#BBD0DB` | Light accent backgrounds, hover states, highlights |
| Deep Navy | `#1B3A4B` | Dark text, dark sections, header backgrounds |
| Seafoam | `#64B5C1` | Secondary accent, badges, tags, decorative elements |
| Light Aqua | `#C9F1F2` | Subtle tinted backgrounds, light highlights |
| Coral Sunset | `#F29F5A` | Warm accent, call-to-action, notification highlights |
| Sea Glass | `#A8D5BA` | Success states, tertiary accent |
| Coastal Clay | `#8C6B4D` | Earthy accent, warm interactive elements |
| Saltwater Mist | `#D0E2F2` | Hero section backgrounds, gentle washes |

### Suggested CSS Custom Properties

```css
:root {
  /* Backgrounds */
  --coastal-white: #ffffff;
  --coastal-linen: #f5f0e8;
  --coastal-sand: #e2d7b0;
  --coastal-mist: #d0e2f2;

  /* Blues */
  --coastal-ocean: #297685;
  --coastal-sky: #bbd0db;
  --coastal-navy: #1b3a4b;
  --coastal-seafoam: #64b5c1;
  --coastal-aqua: #c9f1f2;

  /* Neutrals */
  --coastal-driftwood: #847968;
  --coastal-pebble: #afbcc5;
  --coastal-clay: #8c6b4d;

  /* Warm accents */
  --coastal-coral: #f29f5a;
  --coastal-seaglass: #a8d5ba;

  /* Functional */
  --coastal-bg-primary: var(--coastal-white);
  --coastal-bg-secondary: var(--coastal-linen);
  --coastal-bg-accent: var(--coastal-mist);
  --coastal-text-primary: var(--coastal-navy);
  --coastal-text-secondary: var(--coastal-driftwood);
  --coastal-accent: var(--coastal-ocean);
  --coastal-accent-light: var(--coastal-sky);
  --coastal-border: var(--coastal-pebble);
  --coastal-cta: var(--coastal-coral);
}
```

### Approaches

- **Predominantly white and cream base** -- let light tones dominate for the bright, airy feel
- **Blue as the signature accent** -- use sparingly but consistently for visual anchoring
- **Warm neutrals for grounding** -- sand, driftwood, and clay tones prevent the palette from feeling cold
- **Coral or sunset orange for energy** -- use minimally for calls-to-action or important highlights
- **Layer opacity** -- use translucent blues and seafoams for overlays and tinted sections

---

## Typography

### Typeface Characteristics

Coastal Style typography features:

- **Clean, open letterforms** with generous spacing -- evoking clarity and calm
- **Light to regular font weights** -- avoid heavy, dense type; favor breezy readability
- **Rounded or softened terminals** -- organic feeling rather than sharp or mechanical
- **Relaxed letter-spacing** -- slightly expanded tracking for a laid-back, spacious feel
- **Serif or slab-serif for headings** -- a touch of classic nautical tradition
- **Clean sans-serif for body text** -- modern coastal readability
- **Script fonts used sparingly** -- for decorative accents only, evoking hand-painted beach signs

### Recommended Web Fonts (Google Fonts)

| Font | Style | Usage |
|------|-------|-------|
| **Playfair Display** | Elegant transitional serif | Headlines, hero text |
| **Libre Baskerville** | Classic, readable serif | Subheadings, pull quotes |
| **Lora** | Brushed, calligraphic serif | Headlines, feature titles |
| **Source Sans 3** | Clean, humanist sans-serif | Body text, UI elements |
| **Nunito** | Rounded, friendly sans-serif | Body text, navigation |
| **Raleway** | Thin geometric elegance | Subheadings, light display text |
| **Josefin Sans** | Vintage geometric sans | Display text, captions |
| **Seaweed Script** | Flowing coastal script | Decorative accents, taglines |
| **Caveat** | Casual handwritten | Annotations, informal labels |
| **Original Surfer** | Retro surf display | Fun accent text, badges |

### Typography CSS Example

```css
/* Headlines */
h1, h2, h3 {
  font-family: 'Playfair Display', 'Lora', Georgia, serif;
  color: var(--coastal-navy);
  font-weight: 400;
  letter-spacing: 0.02em;
  line-height: 1.3;
}

/* Display / Hero text */
.coastal-display {
  font-family: 'Playfair Display', serif;
  font-size: clamp(2.5rem, 6vw, 5rem);
  font-weight: 300;
  letter-spacing: 0.04em;
  line-height: 1.15;
  color: var(--coastal-navy);
}

/* Body text */
body {
  font-family: 'Source Sans 3', 'Nunito', sans-serif;
  font-weight: 400;
  font-size: 1.05rem;
  letter-spacing: 0.01em;
  line-height: 1.8;
  color: var(--coastal-driftwood);
}

/* Decorative script accent */
.coastal-script {
  font-family: 'Seaweed Script', 'Caveat', cursive;
  font-size: 1.4em;
  color: var(--coastal-ocean);
  font-weight: 400;
}

/* Navigation */
nav a {
  font-family: 'Josefin Sans', 'Raleway', sans-serif;
  text-transform: uppercase;
  font-size: 0.85rem;
  letter-spacing: 0.12em;
  font-weight: 400;
  color: var(--coastal-driftwood);
}
```

---

## Layout Principles

### Grid and Structure

- **Open, spacious layouts** -- generous padding and margin throughout; let content breathe
- **Wide containers** -- max-width of 1100-1400px with ample side margins
- **Asymmetric balance** -- natural, organic placement rather than rigid symmetry
- **Full-width hero sections** -- large imagery or gradient washes spanning the viewport
- **Card-based content** -- rounded-corner cards with soft shadows for content grouping
- **Horizontal flow** -- content that moves left-to-right like a shoreline, with gentle staggering

### Section Organization

- Use **subtle gradient dividers** between sections (white fading to light blue or sand)
- Apply **generous vertical spacing** -- 6-8rem between major sections
- Create **hierarchy through weight and color** -- not through cramped spacing
- Employ **rounded containers** -- soft borders and border-radius on cards and panels
- Use **full-bleed imagery** -- large photos of coastal scenes as section backgrounds with overlays
- Incorporate **wave-shaped section dividers** -- SVG curves separating content blocks

---

## CSS/Design Techniques

### Wave Section Divider (SVG)

```css
.coastal-wave-divider {
  position: relative;
  overflow: hidden;
}

.coastal-wave-divider::after {
  content: '';
  position: absolute;
  bottom: 0;
  left: 0;
  width: 100%;
  height: 80px;
  background: var(--coastal-white);
  clip-path: ellipse(55% 100% at 50% 100%);
}
```

```html
<!-- SVG wave divider for more organic shapes -->
<svg class="wave-divider" viewBox="0 0 1440 120" preserveAspectRatio="none">
  <path d="M0,60 C360,120 720,0 1080,60 C1260,90 1380,80 1440,60 L1440,120 L0,120 Z"
        fill="var(--coastal-white)" />
</svg>
```

### Soft Card / Panel

```css
.coastal-card {
  background: var(--coastal-white);
  border-radius: 12px;
  padding: 2rem 2.5rem;
  box-shadow:
    0 2px 8px rgba(27, 58, 75, 0.06),
    0 8px 24px rgba(27, 58, 75, 0.04);
  border: 1px solid rgba(175, 188, 197, 0.3);
  transition: box-shadow 0.3s ease, transform 0.3s ease;
}

.coastal-card:hover {
  box-shadow:
    0 4px 12px rgba(27, 58, 75, 0.08),
    0 12px 32px rgba(27, 58, 75, 0.06);
  transform: translateY(-2px);
}
```

### Ocean Gradient Background

```css
/* Soft sky-to-sea gradient */
.coastal-gradient-hero {
  background: linear-gradient(
    180deg,
    var(--coastal-mist) 0%,
    var(--coastal-sky) 40%,
    var(--coastal-seafoam) 100%
  );
  min-height: 60vh;
  display: flex;
  align-items: center;
  justify-content: center;
}

/* Subtle sand-to-white gradient for content sections */
.coastal-gradient-sand {
  background: linear-gradient(
    180deg,
    var(--coastal-white) 0%,
    var(--coastal-linen) 50%,
    var(--coastal-sand) 100%
  );
}
```

### Stripe Pattern (Nautical)

```css
.coastal-stripes {
  background: repeating-linear-gradient(
    0deg,
    var(--coastal-white) 0px,
    var(--coastal-white) 12px,
    var(--coastal-navy) 12px,
    var(--coastal-navy) 14px
  );
}

/* Horizontal rope-line divider */
.coastal-rope-divider {
  height: 0;
  border: none;
  border-top: 3px solid var(--coastal-sand);
  border-bottom: 1px solid var(--coastal-sand);
  margin: 3rem auto;
  width: 50%;
  position: relative;
}

.coastal-rope-divider::before {
  content: '';
  position: absolute;
  top: -8px;
  left: 50%;
  transform: translateX(-50%);
  width: 16px;
  height: 16px;
  border: 2px solid var(--coastal-sand);
  border-radius: 50%;
  background: var(--coastal-white);
}
```

### Weathered / Driftwood Texture

```css
/* Subtle linen/canvas texture overlay */
.coastal-texture {
  position: relative;
}

.coastal-texture::before {
  content: '';
  position: absolute;
  inset: 0;
  background-image: url("data:image/svg+xml,%3Csvg width='40' height='40' xmlns='http://www.w3.org/2000/svg'%3E%3Cfilter id='n'%3E%3CfeTurbulence baseFrequency='0.65' numOctaves='3' stitchTiles='stitch'/%3E%3C/filter%3E%3Crect width='100%25' height='100%25' filter='url(%23n)' opacity='0.03'/%3E%3C/svg%3E");
  pointer-events: none;
  opacity: 0.4;
}

/* Bleached / sun-washed text effect */
.coastal-washed {
  color: var(--coastal-driftwood);
  text-shadow: 0 1px 0 rgba(255, 255, 255, 0.6);
  opacity: 0.85;
}
```

### Transparent Glass / Sea Glass Effect

```css
.coastal-glass {
  background: rgba(255, 255, 255, 0.55);
  backdrop-filter: blur(12px);
  -webkit-backdrop-filter: blur(12px);
  border: 1px solid rgba(255, 255, 255, 0.3);
  border-radius: 12px;
  padding: 2rem;
}
```

### Button Styles

```css
/* Primary -- Ocean blue */
.coastal-btn-primary {
  background: var(--coastal-ocean);
  color: var(--coastal-white);
  border: none;
  padding: 0.75rem 2rem;
  border-radius: 8px;
  font-family: 'Josefin Sans', sans-serif;
  font-size: 0.9rem;
  letter-spacing: 0.08em;
  text-transform: uppercase;
  cursor: pointer;
  transition: background 0.3s ease, transform 0.15s ease;
}

.coastal-btn-primary:hover {
  background: var(--coastal-navy);
  transform: translateY(-1px);
}

/* Secondary -- Outlined */
.coastal-btn-secondary {
  background: transparent;
  color: var(--coastal-ocean);
  border: 2px solid var(--coastal-ocean);
  padding: 0.7rem 1.8rem;
  border-radius: 8px;
  font-family: 'Josefin Sans', sans-serif;
  font-size: 0.9rem;
  letter-spacing: 0.08em;
  text-transform: uppercase;
  cursor: pointer;
  transition: all 0.3s ease;
}

.coastal-btn-secondary:hover {
  background: var(--coastal-ocean);
  color: var(--coastal-white);
}

/* Warm CTA -- Coral sunset */
.coastal-btn-cta {
  background: var(--coastal-coral);
  color: var(--coastal-white);
  border: none;
  padding: 0.85rem 2.2rem;
  border-radius: 24px;
  font-family: 'Josefin Sans', sans-serif;
  font-size: 0.95rem;
  letter-spacing: 0.06em;
  cursor: pointer;
  transition: background 0.3s ease, box-shadow 0.3s ease;
}

.coastal-btn-cta:hover {
  background: #e08a45;
  box-shadow: 0 4px 16px rgba(242, 159, 90, 0.35);
}
```

### Coastal Image Treatment

```css
/* Rounded image with soft shadow */
.coastal-img {
  border-radius: 12px;
  box-shadow: 0 8px 24px rgba(27, 58, 75, 0.1);
  object-fit: cover;
}

/* Polaroid-style image frame */
.coastal-polaroid {
  background: var(--coastal-white);
  padding: 12px 12px 40px 12px;
  border-radius: 4px;
  box-shadow: 0 4px 16px rgba(27, 58, 75, 0.1);
  transform: rotate(-2deg);
  display: inline-block;
}

/* Image overlay with blue tint */
.coastal-overlay {
  position: relative;
}

.coastal-overlay::after {
  content: '';
  position: absolute;
  inset: 0;
  background: linear-gradient(
    180deg,
    rgba(27, 58, 75, 0.0) 40%,
    rgba(27, 58, 75, 0.6) 100%
  );
  border-radius: 12px;
}
```

---

## Materials and Textures (Visual Metaphors for Web)

Physical Coastal Style materials and their web equivalents:

| Physical Material | Web Equivalent |
|-------------------|----------------|
| Weathered driftwood | Muted taupe/gray backgrounds, subtle grain texture overlays |
| White-washed wood | Off-white backgrounds with faint horizontal striping patterns |
| Linen / Cotton fabric | Light textured backgrounds, `background-image` canvas noise |
| Woven rattan / Wicker | Crosshatch or woven SVG pattern overlays at low opacity |
| Sea glass | Frosted glass `backdrop-filter: blur()` effects with translucent tints |
| Smooth pebbles | Rounded corners, gentle shadows, muted gray palette |
| Sand | Warm beige gradients, grainy texture backgrounds |
| Rope / Jute | Thick decorative borders, knotted divider elements |
| Ceramic / Pottery | Rounded card shapes with earthy shadow tones |
| Sheer white curtain | Semi-transparent white overlays, soft veil effects |

---

## Sub-styles and Variations

### Hamptons Style

- **Expansive, luminous, and comfortable** spaces
- Classic, timeless design pieces prioritizing comfort
- Minimal-yet-elegant decor with natural materials
- Crisp white and navy blue as the dominant pairing
- Tailored, preppy refinement -- think ticking stripes and monogrammed linens
- Web approach: clean layouts, serif typography, high-contrast navy/white, premium feel

### Mediterranean Coastal

- Incorporates lagoon colors: **teal, deep blue, mint**
- Warm accents: **ochre, orange, terracotta**
- Architectural features: arched shapes, wrought-iron styling, carved ornamental details
- Indoor greenery and botanical motifs
- Web approach: warmer palette, arch-shaped containers (`border-radius: 50% 50% 0 0`), terracotta accents, lush imagery

### Modern Coastal

- Blends relaxed and California-casual approaches
- Avoids **overt beach themes** (no anchors or shell decorations)
- Contemporary furniture-inspired layouts with clean lines
- Open layouts, neutral palettes, woven textures, brass accents
- Web approach: minimal, neutral-dominant, subtle blue accents, modern sans-serif typography, generous whitespace

---

## Related Aesthetics

| Aesthetic | Relationship to Coastal Style |
|-----------|-------------------------------|
| **Nautical** | Closest sibling; more focused on maritime tradition, navy/red/white palette |
| **Coastal Grandmother** | Subset; relaxed, warm, Nancy Meyers-inspired, linen-and-book-heavy |
| **Coastal Cowgirl** | Fusion aesthetic blending coastal elements with western motifs |
| **Dark Nautical** | Moody inversion; deep navy and black with maritime elements |
| **Minimalism** | Shared emphasis on clean space, decluttered composition |
| **Scandinavian Design** | Overlapping light palettes, natural materials, functional simplicity |
| **Shabby Chic** | Shared weathered/distressed finishes, soft pastel palette |
| **Rustic** | Common use of natural wood, organic textures, handcrafted feel |
| **Tropical** | Adjacent warm-climate aesthetic with bolder colors, botanical patterns |

---

## Quick-Start: Minimal Coastal Style Page Template

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Coastal Style Page</title>
  <link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@300;400;600&family=Source+Sans+3:wght@300;400;600&family=Josefin+Sans:wght@300;400&display=swap" rel="stylesheet">
  <style>
    :root {
      --coastal-white: #ffffff;
      --coastal-linen: #f5f0e8;
      --coastal-sand: #e2d7b0;
      --coastal-mist: #d0e2f2;
      --coastal-ocean: #297685;
      --coastal-sky: #bbd0db;
      --coastal-navy: #1b3a4b;
      --coastal-seafoam: #64b5c1;
      --coastal-driftwood: #847968;
      --coastal-pebble: #afbcc5;
      --coastal-coral: #f29f5a;
    }

    * { margin: 0; padding: 0; box-sizing: border-box; }

    body {
      background: var(--coastal-white);
      color: var(--coastal-driftwood);
      font-family: 'Source Sans 3', sans-serif;
      font-weight: 400;
      font-size: 1.05rem;
      line-height: 1.8;
      letter-spacing: 0.01em;
    }

    h1, h2, h3 {
      font-family: 'Playfair Display', Georgia, serif;
      color: var(--coastal-navy);
      font-weight: 400;
      letter-spacing: 0.02em;
    }

    .hero {
      background: linear-gradient(180deg, var(--coastal-mist) 0%, var(--coastal-white) 100%);
      text-align: center;
      padding: 8rem 2rem 6rem;
    }

    .hero h1 {
      font-size: clamp(2.5rem, 6vw, 4.5rem);
      font-weight: 300;
      margin-bottom: 1rem;
    }

    .hero p {
      font-family: 'Josefin Sans', sans-serif;
      text-transform: uppercase;
      letter-spacing: 0.12em;
      font-size: 0.9rem;
      color: var(--coastal-ocean);
    }

    /* Wave divider */
    .wave-divider {
      display: block;
      width: 100%;
      height: 80px;
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
      background: var(--coastal-white);
      border-radius: 12px;
      padding: 2rem;
      box-shadow: 0 2px 8px rgba(27,58,75,0.06), 0 8px 24px rgba(27,58,75,0.04);
      border: 1px solid rgba(175,188,197,0.3);
    }

    .accent-section {
      background: var(--coastal-linen);
    }
  </style>
</head>
<body>
  <div class="hero">
    <h1>Coastal Style</h1>
    <p>Light, Airy, Inspired by the Sea</p>
  </div>

  <svg class="wave-divider" viewBox="0 0 1440 80" preserveAspectRatio="none">
    <path d="M0,40 C240,80 480,0 720,40 C960,80 1200,0 1440,40 L1440,80 L0,80 Z"
          fill="#f5f0e8" />
  </svg>

  <section class="accent-section">
    <h2>Section Heading</h2>
    <p>Content with Coastal Style applied. Light backgrounds, ocean-inspired accents, breezy typography.</p>
    <div class="card-grid">
      <div class="card">
        <h3>Card Title</h3>
        <p>Soft rounded cards with gentle shadows evoke smooth sea glass.</p>
      </div>
      <div class="card">
        <h3>Card Title</h3>
        <p>Natural materials and open space define the coastal approach.</p>
      </div>
    </div>
  </section>
</body>
</html>
```
