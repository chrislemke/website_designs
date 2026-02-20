# Coastal Grandmother Design Reference

Coastal Grandmother is a fashion and lifestyle aesthetic coined by TikTok creator Lex Nicoleta in early 2022, inspired by the effortlessly elegant heroines of Nancy Meyers films such as *Something's Gotta Give* and *It's Complicated*. It celebrates a vision of refined seaside living defined by linen fabrics, warm neutrals, cashmere wraps, wicker baskets, farmers' markets, and reading on a sun-dappled porch. The lifestyle channels the domestic sophistication of Ina Garten and the breezy, collected calm of a well-appointed Hamptons kitchen. In web and UI design, Coastal Grandmother translates into warm cream and sand backgrounds, restrained typography with classic serifs, generous whitespace that evokes open coastal rooms, and an overall feeling of quiet luxury -- never flashy, always tasteful. The palette avoids bright nautical blues in favor of muted slate, driftwood gray, and soft linen tones, distinguishing it from generic "beach" aesthetics by emphasizing an older, more cultivated sensibility.

---

## Visual Characteristics

### Core Design Traits

- **Warm neutral dominance**: Cream, linen, sand, oatmeal, and warm white form the backbone of every surface -- backgrounds feel like sun-bleached cotton, not sterile paper
- **Muted, desaturated accents**: Where color appears, it is softened and grayed -- dusty blue, sage green, weathered terracotta -- never saturated or electric
- **Natural material textures**: Linen weave, wicker crosshatch, raw cotton, sea-worn wood, and ceramic surfaces inform background patterns and container treatments
- **Classic serif typography**: Elegant, traditional typefaces with generous letter-spacing and light weights evoke the spines of well-read novels on a porch bookshelf
- **Abundant whitespace**: Layouts breathe like airy coastal rooms with high ceilings -- generous padding and margin are essential, not decorative
- **Soft, diffused shadows**: Box shadows use warm, brown-tinted RGBA values at low opacity, imitating the gentle light of a late afternoon by the sea
- **Understated photography**: Images favor natural light, neutral tones, and domestic subjects -- linen tablecloths, ceramic bowls, hydrangeas, open windows with sheer curtains
- **Refined restraint**: Every element is curated rather than accumulated; ornament is minimal and purposeful, reflecting an "edited" life
- **Organic, rounded forms**: Soft border-radius values and curved containers echo the smoothed edges of sea glass and worn pebbles
- **Layered neutrals over contrast**: Hierarchy is achieved through subtle shifts in warmth and weight rather than strong color contrast

### Design Principles

- **Quiet luxury**: Design should feel expensive and considered without ever being loud or ostentatious
- **Comfort as elegance**: Prioritize readability, generous spacing, and a relaxed pace over visual density or stimulation
- **Natural over synthetic**: Favor textures, colors, and shapes found in nature and handmade objects over digital-native effects like gradients or glows
- **Timelessness over trend**: Choose classic typefaces, enduring color relationships, and layouts that will feel appropriate in ten years
- **Edited simplicity**: Every visible element should feel intentional; remove anything that does not contribute to the serene, collected atmosphere
- **Warmth in neutrality**: Even a minimal palette should feel warm and inviting, never cold or clinical -- cream over white, sand over gray

---

## Color Palette

| Swatch | Hex | Role / Usage |
|--------|-----|-------------|
| Linen White | `#FAF6F0` | Primary background, page canvas |
| Warm Cream | `#F3EDE4` | Card surfaces, secondary backgrounds |
| Oatmeal | `#E8DFD2` | Alternate section backgrounds, input fields |
| Sand | `#D5C9B5` | Borders, dividers, subtle accents |
| Driftwood | `#A69882` | Secondary text, muted UI elements |
| Cashmere Taupe | `#8C7E6D` | Body text, icon fills |
| Slate Charcoal | `#4A4440` | Primary text, headings |
| Dusty Sage | `#9EAD94` | Tertiary accent, success states, nature references |
| Hydrangea Blue | `#8FA3B0` | Primary accent, links, interactive elements |
| Soft Chambray | `#B5C4CE` | Light accent backgrounds, hover states |
| Sheer Sky | `#D8E2E8` | Hero washes, tinted sections |
| Weathered Terracotta | `#BF9B7A` | Warm accent, call-to-action highlights |
| Porcelain | `#FFFFFF` | High-contrast surfaces, modal backgrounds |
| Dried Lavender | `#B0A4B8` | Sparse decorative accent, tags |

### CSS Custom Properties

```css
:root {
  /* Backgrounds */
  --cg-linen: #FAF6F0;
  --cg-cream: #F3EDE4;
  --cg-oatmeal: #E8DFD2;
  --cg-porcelain: #FFFFFF;

  /* Neutrals */
  --cg-sand: #D5C9B5;
  --cg-driftwood: #A69882;
  --cg-cashmere: #8C7E6D;
  --cg-charcoal: #4A4440;

  /* Accents */
  --cg-sage: #9EAD94;
  --cg-hydrangea: #8FA3B0;
  --cg-chambray: #B5C4CE;
  --cg-sky: #D8E2E8;
  --cg-terracotta: #BF9B7A;
  --cg-lavender: #B0A4B8;

  /* Functional aliases */
  --cg-bg-primary: var(--cg-linen);
  --cg-bg-secondary: var(--cg-cream);
  --cg-bg-tertiary: var(--cg-oatmeal);
  --cg-text-primary: var(--cg-charcoal);
  --cg-text-secondary: var(--cg-cashmere);
  --cg-text-muted: var(--cg-driftwood);
  --cg-accent: var(--cg-hydrangea);
  --cg-accent-light: var(--cg-chambray);
  --cg-border: var(--cg-sand);
  --cg-cta: var(--cg-terracotta);
}
```

---

## Typography

### Recommended Google Fonts

| Font | Style | Weight(s) | Usage |
|------|-------|-----------|-------|
| **Cormorant Garamond** | Elegant old-style serif | 300, 400, 500, 600 | Display headings, hero text |
| **Libre Baskerville** | Classic transitional serif | 400, 700 | Subheadings, pull quotes |
| **Lora** | Calligraphic brushed serif | 400, 500, 600, 700 | Headings, feature titles |
| **Alegreya** | Warm rhythmic serif | 400, 500, 700 | Body text alternative |
| **Source Serif 4** | Clean editorial serif | 300, 400, 600 | Body text, long-form reading |
| **Nunito Sans** | Soft humanist sans-serif | 300, 400, 600 | Navigation, UI labels, captions |
| **Raleway** | Thin geometric elegance | 300, 400, 500 | Subheadings, light display text |
| **EB Garamond** | Refined classic serif | 400, 500, 600 | Body text, editorial layouts |

### Font Pairing Suggestions

| Heading | Body | Vibe |
|---------|------|------|
| Cormorant Garamond 400 | Source Serif 4 400 | Refined literary elegance -- the Nancy Meyers bookshelf |
| Lora 500 | Nunito Sans 400 | Warm sophistication with modern readability |
| Libre Baskerville 400 | Alegreya 400 | Classic editorial warmth, like a lifestyle magazine |
| Cormorant Garamond 300 | EB Garamond 400 | All-serif pairing for maximum timelessness |
| Raleway 300 | Source Serif 4 400 | Modern-classic hybrid, airy and light |

### CSS Example

```css
@import url('https://fonts.googleapis.com/css2?family=Cormorant+Garamond:ital,wght@0,300;0,400;0,500;0,600;1,400&family=Source+Serif+4:ital,wght@0,300;0,400;0,600;1,400&family=Nunito+Sans:wght@300;400;600&display=swap');

body {
  font-family: 'Source Serif 4', 'Georgia', serif;
  font-size: 1.08rem;
  line-height: 1.85;
  color: var(--cg-cashmere);
  -webkit-font-smoothing: antialiased;
}

h1, h2, h3 {
  font-family: 'Cormorant Garamond', 'Garamond', serif;
  font-weight: 400;
  color: var(--cg-charcoal);
  letter-spacing: 0.015em;
  line-height: 1.3;
}

h1 {
  font-size: clamp(2.2rem, 5vw, 3.6rem);
  font-weight: 300;
  letter-spacing: 0.03em;
}

h2 {
  font-size: clamp(1.5rem, 3vw, 2.2rem);
}

h3 {
  font-size: 1.3rem;
  font-weight: 500;
}

/* UI elements -- navigation, buttons, labels */
nav, button, .label, .caption {
  font-family: 'Nunito Sans', 'Helvetica Neue', sans-serif;
  letter-spacing: 0.06em;
}

/* Italic accent for quotes and asides */
blockquote {
  font-family: 'Cormorant Garamond', serif;
  font-style: italic;
  font-size: 1.3rem;
  color: var(--cg-driftwood);
  line-height: 1.7;
}
```

---

## Layout Principles

- **Generous, room-like spacing**: Use 6-10rem between major sections and 2-3rem internal padding on containers; the layout should feel like walking through a spacious coastal home
- **Centered single-column for reading content**: Keep body text in a 680-780px max-width column, centered on the page, like a well-set book
- **Wide containers for feature sections**: Allow hero and gallery sections to stretch to 1100-1280px or full-width with internal max-width constraints
- **Subtle asymmetry**: Offset images slightly from text, stagger card grids gently -- avoid rigid, mechanical symmetry in favor of a natural, lived-in arrangement
- **Layered neutral backgrounds**: Alternate between linen, cream, and oatmeal section backgrounds to create depth without introducing color
- **Soft dividers over hard rules**: Use thin 1px borders in the sand color, or simple typographic ornaments, rather than heavy horizontal rules
- **Full-bleed imagery with warm overlays**: Large photographs should span the viewport width with semi-transparent warm cream overlays for text readability
- **Responsive with grace**: On mobile, increase vertical spacing rather than reducing it; the breezy, unhurried feeling should intensify, not collapse
- **Vertical rhythm**: Maintain consistent line-height multiples and spacing scales to create a calm, predictable reading cadence

---

## CSS / Design Techniques

### Card Component

```css
.cg-card {
  background: var(--cg-cream);
  border: 1px solid var(--cg-sand);
  border-radius: 8px;
  padding: 2rem 2.25rem;
  box-shadow: 0 1px 4px rgba(74, 68, 64, 0.04),
              0 4px 16px rgba(74, 68, 64, 0.03);
  transition: box-shadow 0.3s ease, transform 0.3s ease;
}

.cg-card:hover {
  box-shadow: 0 2px 8px rgba(74, 68, 64, 0.06),
              0 8px 24px rgba(74, 68, 64, 0.05);
  transform: translateY(-2px);
}

.cg-card h3 {
  font-family: 'Cormorant Garamond', serif;
  font-size: 1.4rem;
  font-weight: 500;
  color: var(--cg-charcoal);
  margin-bottom: 0.75rem;
}

.cg-card p {
  color: var(--cg-cashmere);
  line-height: 1.8;
}
```

### Button Component

```css
/* Primary -- Warm terracotta */
.cg-btn {
  background: var(--cg-terracotta);
  color: var(--cg-linen);
  border: none;
  border-radius: 4px;
  padding: 0.8rem 2rem;
  font-family: 'Nunito Sans', sans-serif;
  font-size: 0.85rem;
  font-weight: 600;
  letter-spacing: 0.1em;
  text-transform: uppercase;
  cursor: pointer;
  transition: background 0.3s ease, transform 0.15s ease;
}

.cg-btn:hover {
  background: #A8855F;
  transform: translateY(-1px);
}

/* Secondary -- Outlined */
.cg-btn-secondary {
  background: transparent;
  color: var(--cg-cashmere);
  border: 1.5px solid var(--cg-sand);
  border-radius: 4px;
  padding: 0.75rem 1.8rem;
  font-family: 'Nunito Sans', sans-serif;
  font-size: 0.85rem;
  font-weight: 600;
  letter-spacing: 0.1em;
  text-transform: uppercase;
  cursor: pointer;
  transition: all 0.3s ease;
}

.cg-btn-secondary:hover {
  border-color: var(--cg-cashmere);
  color: var(--cg-charcoal);
  background: var(--cg-oatmeal);
}

/* Ghost -- Minimal text link style */
.cg-btn-ghost {
  background: none;
  border: none;
  color: var(--cg-hydrangea);
  font-family: 'Nunito Sans', sans-serif;
  font-size: 0.85rem;
  font-weight: 600;
  letter-spacing: 0.08em;
  text-transform: uppercase;
  cursor: pointer;
  padding: 0.5rem 0;
  border-bottom: 1px solid transparent;
  transition: border-color 0.3s ease;
}

.cg-btn-ghost:hover {
  border-bottom-color: var(--cg-hydrangea);
}
```

### Navigation Bar

```css
.cg-nav {
  background: var(--cg-linen);
  border-bottom: 1px solid var(--cg-sand);
  padding: 1.25rem 2.5rem;
  display: flex;
  align-items: center;
  justify-content: space-between;
  position: sticky;
  top: 0;
  z-index: 100;
}

.cg-nav-brand {
  font-family: 'Cormorant Garamond', serif;
  font-size: 1.5rem;
  font-weight: 400;
  color: var(--cg-charcoal);
  text-decoration: none;
  letter-spacing: 0.04em;
}

.cg-nav-links {
  display: flex;
  gap: 2rem;
  list-style: none;
}

.cg-nav-links a {
  font-family: 'Nunito Sans', sans-serif;
  font-size: 0.8rem;
  font-weight: 600;
  letter-spacing: 0.1em;
  text-transform: uppercase;
  color: var(--cg-cashmere);
  text-decoration: none;
  padding: 0.4rem 0;
  border-bottom: 1.5px solid transparent;
  transition: color 0.2s ease, border-color 0.2s ease;
}

.cg-nav-links a:hover,
.cg-nav-links a.active {
  color: var(--cg-charcoal);
  border-bottom-color: var(--cg-terracotta);
}
```

### Hero Section

```css
.cg-hero {
  background: linear-gradient(
    180deg,
    var(--cg-sky) 0%,
    var(--cg-cream) 60%,
    var(--cg-linen) 100%
  );
  text-align: center;
  padding: 8rem 2rem 6rem;
  position: relative;
}

.cg-hero h1 {
  font-family: 'Cormorant Garamond', serif;
  font-size: clamp(2.5rem, 6vw, 4.2rem);
  font-weight: 300;
  color: var(--cg-charcoal);
  margin-bottom: 1.25rem;
  letter-spacing: 0.04em;
}

.cg-hero p {
  font-family: 'Source Serif 4', serif;
  font-size: 1.15rem;
  color: var(--cg-cashmere);
  max-width: 560px;
  margin: 0 auto 2rem;
  line-height: 1.85;
}

.cg-hero .cg-tagline {
  font-family: 'Nunito Sans', sans-serif;
  font-size: 0.8rem;
  font-weight: 600;
  letter-spacing: 0.15em;
  text-transform: uppercase;
  color: var(--cg-driftwood);
  margin-bottom: 1rem;
}
```

### Linen Texture Background

```css
/* Simulated linen weave using CSS only */
.cg-linen-texture {
  background-color: var(--cg-linen);
  background-image:
    repeating-linear-gradient(
      0deg,
      transparent,
      transparent 3px,
      rgba(74, 68, 64, 0.015) 3px,
      rgba(74, 68, 64, 0.015) 4px
    ),
    repeating-linear-gradient(
      90deg,
      transparent,
      transparent 3px,
      rgba(74, 68, 64, 0.01) 3px,
      rgba(74, 68, 64, 0.01) 4px
    );
}
```

### Elegant Divider

```css
/* Thin ornamental divider */
.cg-divider {
  border: none;
  text-align: center;
  margin: 3.5rem auto;
  max-width: 240px;
  position: relative;
}

.cg-divider::before {
  content: '';
  display: block;
  width: 100%;
  height: 1px;
  background: var(--cg-sand);
  position: absolute;
  top: 50%;
}

.cg-divider::after {
  content: '\2022';
  position: relative;
  background: var(--cg-linen);
  padding: 0 1rem;
  color: var(--cg-driftwood);
  font-size: 0.7rem;
  letter-spacing: 0.6em;
}

/* Alternate: simple three-dot divider */
.cg-dots {
  text-align: center;
  margin: 3rem 0;
  color: var(--cg-sand);
  font-size: 1.2rem;
  letter-spacing: 0.8em;
}
```

### Image Treatment

```css
/* Warm-toned image with soft frame */
.cg-image {
  border-radius: 6px;
  box-shadow: 0 4px 16px rgba(74, 68, 64, 0.08);
  object-fit: cover;
  filter: saturate(0.9) contrast(0.95) brightness(1.02);
}

/* Image with linen-colored mat border, like a framed print */
.cg-framed-image {
  background: var(--cg-cream);
  padding: 12px;
  border: 1px solid var(--cg-sand);
  border-radius: 4px;
  box-shadow: 0 2px 8px rgba(74, 68, 64, 0.06);
  display: inline-block;
}

.cg-framed-image img {
  display: block;
  border-radius: 2px;
  width: 100%;
}
```

### Blockquote / Pull Quote

```css
.cg-blockquote {
  font-family: 'Cormorant Garamond', serif;
  font-style: italic;
  font-size: 1.4rem;
  line-height: 1.7;
  color: var(--cg-driftwood);
  border-left: 2px solid var(--cg-sand);
  padding: 1rem 0 1rem 2rem;
  margin: 2.5rem 0;
  max-width: 600px;
}

.cg-blockquote cite {
  display: block;
  font-family: 'Nunito Sans', sans-serif;
  font-style: normal;
  font-size: 0.75rem;
  font-weight: 600;
  letter-spacing: 0.1em;
  text-transform: uppercase;
  color: var(--cg-sand);
  margin-top: 1rem;
}
```

### Footer

```css
.cg-footer {
  background: var(--cg-oatmeal);
  border-top: 1px solid var(--cg-sand);
  padding: 3rem 2.5rem;
  text-align: center;
}

.cg-footer p {
  font-family: 'Nunito Sans', sans-serif;
  font-size: 0.8rem;
  color: var(--cg-driftwood);
  letter-spacing: 0.05em;
}

.cg-footer a {
  color: var(--cg-hydrangea);
  text-decoration: none;
  border-bottom: 1px solid transparent;
  transition: border-color 0.2s ease;
}

.cg-footer a:hover {
  border-bottom-color: var(--cg-hydrangea);
}
```

---

## Design Do's and Don'ts

### Do's

- Use warm, cream-based backgrounds (`#FAF6F0`, `#F3EDE4`) instead of pure white for every surface
- Pair classic serif headings with readable serif or light sans-serif body text for quiet sophistication
- Apply generous whitespace -- let layouts breathe like a sunlit room with high ceilings
- Use subtle, warm-tinted box-shadows (`rgba(74, 68, 64, 0.05)`) rather than cool or black shadows
- Incorporate linen and woven textures through CSS patterns at very low opacity
- Keep the color palette restrained -- rely on neutral shifts for hierarchy, with accent colors used sparingly
- Choose photography with natural light, neutral tones, and domestic subjects (table settings, gardens, open windows)
- Use thin, elegant borders and dividers; ornament should feel like a fine pen stroke, not a heavy brush
- Maintain consistent vertical rhythm and predictable spacing scales
- Design for reading comfort above all else -- long-form content should be a pleasure to consume

### Don'ts

- Avoid pure white (`#FFFFFF`) as a primary background; it reads as clinical rather than warm
- Avoid saturated, bright colors or neon accents -- nothing should feel loud or urgent
- Do not use heavy sans-serif fonts (Impact, Bebas Neue) or tech-forward geometric typefaces
- Avoid dark mode color schemes; the aesthetic is fundamentally about warmth and light
- Do not use glossy gradients, metallic effects, drop shadows with hard edges, or any "digital-native" flourishes
- Avoid cluttered layouts or dense information grids -- Coastal Grandmother is about editing down, not adding more
- Do not use generic stock photography of beaches, surfboards, or tropical scenes; this is not a vacation aesthetic
- Avoid animation beyond subtle hover transitions; the pace should be calm and unhurried
- Do not use heavy borders or outlined containers; keep structural elements whisper-thin
- Avoid all-caps body text or aggressive typographic hierarchy; the voice should be measured and conversational

---

## Related Aesthetics

| Aesthetic | Relationship |
|-----------|-------------|
| **Coastal Style** | Parent aesthetic; Coastal Grandmother is a refined, domestically-focused subset that emphasizes warmth and maturity over nautical motifs |
| **Grandmillennial** | Shares the appreciation for traditional, "grandmother-coded" design but Grandmillennial is more maximalist with pattern layering and chintz |
| **Cottagecore** | Both celebrate a slower, nature-adjacent life, but Cottagecore is rural and meadow-inflected while Coastal Grandmother is seaside and sophisticated |
| **Hygge** | Overlapping emphasis on comfort, warmth, and domestic coziness; Hygge is Scandinavian and darker-toned, Coastal Grandmother is lighter and American |
| **Japandi** | Shares the restrained, natural-material palette and quiet minimalism, but Japandi leans cooler and more austere |
| **Light Academia** | Both favor warm neutrals, classic serifs, and an intellectual sensibility, but Light Academia adds scholarly and European architectural references |
| **French Provincial Style** | Overlapping warmth, linen textures, and refined domesticity; French Provincial is more ornate and historically European |
| **Frasurbane** | Both channel a sophisticated, upper-middle-class comfort aesthetic from the late 1990s and early 2000s |

---

## Quick-Start HTML Template

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Coastal Grandmother</title>
  <link href="https://fonts.googleapis.com/css2?family=Cormorant+Garamond:ital,wght@0,300;0,400;0,500;1,400&family=Source+Serif+4:ital,wght@0,300;0,400;0,600;1,400&family=Nunito+Sans:wght@300;400;600&display=swap" rel="stylesheet">
  <style>
    :root {
      --cg-linen: #FAF6F0;
      --cg-cream: #F3EDE4;
      --cg-oatmeal: #E8DFD2;
      --cg-porcelain: #FFFFFF;
      --cg-sand: #D5C9B5;
      --cg-driftwood: #A69882;
      --cg-cashmere: #8C7E6D;
      --cg-charcoal: #4A4440;
      --cg-sage: #9EAD94;
      --cg-hydrangea: #8FA3B0;
      --cg-chambray: #B5C4CE;
      --cg-sky: #D8E2E8;
      --cg-terracotta: #BF9B7A;
      --cg-lavender: #B0A4B8;
    }

    *, *::before, *::after {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body {
      font-family: 'Source Serif 4', Georgia, serif;
      font-size: 1.08rem;
      line-height: 1.85;
      color: var(--cg-cashmere);
      background-color: var(--cg-linen);
      background-image:
        repeating-linear-gradient(
          0deg, transparent, transparent 3px,
          rgba(74,68,64,0.015) 3px, rgba(74,68,64,0.015) 4px
        ),
        repeating-linear-gradient(
          90deg, transparent, transparent 3px,
          rgba(74,68,64,0.01) 3px, rgba(74,68,64,0.01) 4px
        );
      -webkit-font-smoothing: antialiased;
    }

    /* ---- Navigation ---- */

    nav {
      background: var(--cg-linen);
      border-bottom: 1px solid var(--cg-sand);
      padding: 1.25rem 2.5rem;
      display: flex;
      align-items: center;
      justify-content: space-between;
      position: sticky;
      top: 0;
      z-index: 100;
    }

    .nav-brand {
      font-family: 'Cormorant Garamond', serif;
      font-size: 1.5rem;
      font-weight: 400;
      color: var(--cg-charcoal);
      text-decoration: none;
      letter-spacing: 0.04em;
    }

    .nav-links {
      display: flex;
      gap: 2rem;
      list-style: none;
    }

    .nav-links a {
      font-family: 'Nunito Sans', sans-serif;
      font-size: 0.78rem;
      font-weight: 600;
      letter-spacing: 0.1em;
      text-transform: uppercase;
      color: var(--cg-cashmere);
      text-decoration: none;
      padding-bottom: 0.3rem;
      border-bottom: 1.5px solid transparent;
      transition: color 0.2s ease, border-color 0.2s ease;
    }

    .nav-links a:hover {
      color: var(--cg-charcoal);
      border-bottom-color: var(--cg-terracotta);
    }

    /* ---- Hero ---- */

    .hero {
      background: linear-gradient(180deg, var(--cg-sky) 0%, var(--cg-cream) 55%, var(--cg-linen) 100%);
      text-align: center;
      padding: 7rem 2rem 5rem;
    }

    .hero-tagline {
      font-family: 'Nunito Sans', sans-serif;
      font-size: 0.78rem;
      font-weight: 600;
      letter-spacing: 0.18em;
      text-transform: uppercase;
      color: var(--cg-driftwood);
      margin-bottom: 1rem;
    }

    .hero h1 {
      font-family: 'Cormorant Garamond', serif;
      font-size: clamp(2.4rem, 5.5vw, 4rem);
      font-weight: 300;
      color: var(--cg-charcoal);
      letter-spacing: 0.03em;
      line-height: 1.2;
      margin-bottom: 1.25rem;
    }

    .hero p {
      font-size: 1.12rem;
      color: var(--cg-cashmere);
      max-width: 540px;
      margin: 0 auto 2.5rem;
      line-height: 1.85;
    }

    .btn {
      display: inline-block;
      background: var(--cg-terracotta);
      color: var(--cg-linen);
      border: none;
      border-radius: 4px;
      padding: 0.8rem 2.2rem;
      font-family: 'Nunito Sans', sans-serif;
      font-size: 0.82rem;
      font-weight: 600;
      letter-spacing: 0.1em;
      text-transform: uppercase;
      text-decoration: none;
      cursor: pointer;
      transition: background 0.3s ease, transform 0.15s ease;
    }

    .btn:hover {
      background: #A8855F;
      transform: translateY(-1px);
    }

    .btn-outline {
      background: transparent;
      color: var(--cg-cashmere);
      border: 1.5px solid var(--cg-sand);
      margin-left: 1rem;
    }

    .btn-outline:hover {
      border-color: var(--cg-cashmere);
      background: var(--cg-oatmeal);
      color: var(--cg-charcoal);
    }

    /* ---- Sections ---- */

    .section {
      max-width: 780px;
      margin: 0 auto;
      padding: 5rem 2rem;
    }

    .section-wide {
      max-width: 1080px;
      margin: 0 auto;
      padding: 5rem 2rem;
    }

    .section h2 {
      font-family: 'Cormorant Garamond', serif;
      font-size: clamp(1.6rem, 3vw, 2.2rem);
      font-weight: 400;
      color: var(--cg-charcoal);
      margin-bottom: 1rem;
      letter-spacing: 0.02em;
    }

    .section h3 {
      font-family: 'Cormorant Garamond', serif;
      font-size: 1.3rem;
      font-weight: 500;
      color: var(--cg-charcoal);
      margin-bottom: 0.6rem;
    }

    .bg-cream { background-color: var(--cg-cream); }
    .bg-oatmeal { background-color: var(--cg-oatmeal); }

    /* ---- Divider ---- */

    .divider {
      text-align: center;
      margin: 0;
      padding: 2rem 0;
      color: var(--cg-sand);
      font-size: 0.7rem;
      letter-spacing: 0.8em;
    }

    /* ---- Card Grid ---- */

    .card-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
      gap: 2rem;
      margin-top: 2rem;
    }

    .card {
      background: var(--cg-cream);
      border: 1px solid var(--cg-sand);
      border-radius: 8px;
      padding: 2rem 2.25rem;
      box-shadow: 0 1px 4px rgba(74,68,64,0.04), 0 4px 16px rgba(74,68,64,0.03);
      transition: box-shadow 0.3s ease, transform 0.3s ease;
    }

    .card:hover {
      box-shadow: 0 2px 8px rgba(74,68,64,0.06), 0 8px 24px rgba(74,68,64,0.05);
      transform: translateY(-2px);
    }

    .card h3 {
      font-family: 'Cormorant Garamond', serif;
      font-size: 1.35rem;
      font-weight: 500;
      color: var(--cg-charcoal);
      margin-bottom: 0.75rem;
    }

    .card p {
      color: var(--cg-cashmere);
      line-height: 1.8;
      font-size: 1rem;
    }

    .card-tag {
      display: inline-block;
      font-family: 'Nunito Sans', sans-serif;
      font-size: 0.7rem;
      font-weight: 600;
      letter-spacing: 0.08em;
      text-transform: uppercase;
      color: var(--cg-hydrangea);
      margin-bottom: 0.75rem;
    }

    /* ---- Blockquote ---- */

    blockquote {
      font-family: 'Cormorant Garamond', serif;
      font-style: italic;
      font-size: 1.4rem;
      line-height: 1.7;
      color: var(--cg-driftwood);
      border-left: 2px solid var(--cg-sand);
      padding: 0.5rem 0 0.5rem 2rem;
      margin: 2.5rem 0;
      max-width: 600px;
    }

    blockquote cite {
      display: block;
      font-family: 'Nunito Sans', sans-serif;
      font-style: normal;
      font-size: 0.72rem;
      font-weight: 600;
      letter-spacing: 0.1em;
      text-transform: uppercase;
      color: var(--cg-sand);
      margin-top: 0.75rem;
    }

    /* ---- Feature Row ---- */

    .feature-row {
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 3rem;
      align-items: center;
      margin: 2.5rem 0;
    }

    .feature-image {
      width: 100%;
      height: 320px;
      background: linear-gradient(135deg, var(--cg-chambray) 0%, var(--cg-sky) 100%);
      border-radius: 6px;
      box-shadow: 0 4px 16px rgba(74,68,64,0.08);
      display: flex;
      align-items: center;
      justify-content: center;
      color: var(--cg-driftwood);
      font-family: 'Nunito Sans', sans-serif;
      font-size: 0.75rem;
      letter-spacing: 0.08em;
      text-transform: uppercase;
    }

    /* ---- Footer ---- */

    footer {
      background: var(--cg-oatmeal);
      border-top: 1px solid var(--cg-sand);
      padding: 3rem 2.5rem;
      text-align: center;
    }

    footer p {
      font-family: 'Nunito Sans', sans-serif;
      font-size: 0.78rem;
      color: var(--cg-driftwood);
      letter-spacing: 0.04em;
    }

    footer a {
      color: var(--cg-hydrangea);
      text-decoration: none;
      border-bottom: 1px solid transparent;
      transition: border-color 0.2s ease;
    }

    footer a:hover {
      border-bottom-color: var(--cg-hydrangea);
    }

    /* ---- Responsive ---- */

    @media (max-width: 768px) {
      nav {
        padding: 1rem 1.5rem;
      }

      .nav-links {
        gap: 1.25rem;
      }

      .hero {
        padding: 5rem 1.5rem 3.5rem;
      }

      .section, .section-wide {
        padding: 3.5rem 1.5rem;
      }

      .feature-row {
        grid-template-columns: 1fr;
        gap: 2rem;
      }

      .card-grid {
        grid-template-columns: 1fr;
      }

      .btn-outline {
        margin-left: 0;
        margin-top: 0.75rem;
      }
    }
  </style>
</head>
<body>

  <!-- Navigation -->
  <nav>
    <a href="#" class="nav-brand">The Coastal Table</a>
    <ul class="nav-links">
      <li><a href="#">Home</a></li>
      <li><a href="#">Journal</a></li>
      <li><a href="#">Recipes</a></li>
      <li><a href="#">About</a></li>
    </ul>
  </nav>

  <!-- Hero Section -->
  <section class="hero">
    <p class="hero-tagline">Linen &middot; Sea Air &middot; Simple Pleasures</p>
    <h1>A Life Well Seasoned</h1>
    <p>Celebrating the quiet art of slow mornings, farmers' market bouquets, and the kind of elegance that only comes with time.</p>
    <div>
      <a href="#" class="btn">Explore the Journal</a>
      <a href="#" class="btn btn-outline">Our Recipes</a>
    </div>
  </section>

  <!-- Divider -->
  <div class="divider">&bull; &bull; &bull;</div>

  <!-- Introduction Section -->
  <section class="section">
    <h2>The Art of Unhurried Living</h2>
    <p>There is a particular kind of morning that stays with you -- coffee in a ceramic mug, the sound of waves through an open window, a novel face-down on a linen tablecloth. This is not about perfection. It is about choosing fewer, better things and giving them room to breathe.</p>

    <blockquote>
      The best things in life are the people you love, the places you've been, and the memories you've made along the way.
      <cite>A sentiment, not a source</cite>
    </blockquote>
  </section>

  <!-- Feature Section on cream background -->
  <div class="bg-cream">
    <section class="section-wide">
      <h2>Seasonal Gatherings</h2>
      <p>Every season brings its own table. Spring asparagus with lemon. Summer tomatoes still warm from the garden. Autumn squash roasted in good olive oil. Winter citrus arranged in a ceramic bowl.</p>

      <div class="feature-row">
        <div class="feature-image">Image Placeholder</div>
        <div>
          <h3>From the Market</h3>
          <p>Saturday mornings begin with a wicker basket and a walk through the stalls. The best meals start not with a recipe but with whatever the season offers -- stone fruit in July, root vegetables in November, fresh herbs year-round.</p>
          <br>
          <a href="#" class="btn">Seasonal Guide</a>
        </div>
      </div>
    </section>
  </div>

  <!-- Divider -->
  <div class="divider">&bull; &bull; &bull;</div>

  <!-- Card Grid Section -->
  <section class="section-wide">
    <h2>From the Journal</h2>
    <p>Notes on living well, gathered slowly over many seasons.</p>

    <div class="card-grid">
      <div class="card">
        <span class="card-tag">Home</span>
        <h3>Setting a Simple Table</h3>
        <p>Linen napkins, mismatched ceramics, and a small jar of garden clippings. The most inviting tables are never the most elaborate ones.</p>
      </div>
      <div class="card">
        <span class="card-tag">Kitchen</span>
        <h3>The Case for One Good Knife</h3>
        <p>A well-maintained kitchen begins with restraint. One beautiful knife, sharpened often, will outlast and outperform a drawer full of gadgets.</p>
      </div>
      <div class="card">
        <span class="card-tag">Reading</span>
        <h3>A Porch Bookshelf</h3>
        <p>The books we return to say more than the ones we finish. A curated shelf by the door -- part intention, part invitation.</p>
      </div>
    </div>
  </section>

  <!-- Closing Section on oatmeal background -->
  <div class="bg-oatmeal">
    <section class="section" style="text-align: center;">
      <h2>Stay a While</h2>
      <p>Join a small community of readers who appreciate linen tablecloths, handwritten notes, and the long way home from the farmers' market.</p>
      <br>
      <a href="#" class="btn">Subscribe to the Letter</a>
    </section>
  </div>

  <!-- Footer -->
  <footer>
    <p>&copy; 2025 The Coastal Table &middot; Made with care and good olive oil</p>
  </footer>

</body>
</html>
```
