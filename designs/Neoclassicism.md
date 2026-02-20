# Neoclassicism Design Reference

## Overview

Neoclassicism is a design movement rooted in the revival of ancient Greek and Roman classical ideals, emerging in the mid-18th century as a reaction against the ornamental excess of Baroque and Rococo styles. Fueled by Enlightenment rationalism and the rediscovery of Pompeii and Herculaneum, it championed symmetry, balanced proportions, geometric clarity, and restrained ornamentation as expressions of order, reason, and civic virtue. The aesthetic dominated European architecture, furniture, and graphic arts from roughly 1750 through the 1830s, producing landmarks from the Pantheon in Paris to the United States Capitol. In web and UI design, Neoclassicism translates to rigidly symmetrical layouts, classical serif typography with high stroke contrast, column and pediment motifs, marble and stone textures, gold and ivory color palettes, and a pervasive sense of dignified restraint. Where Brutalism strips away all decoration and Maximalism piles it on, Neoclassical web design applies ornamentation sparingly and structurally -- every flourish (a Greek key border, a laurel wreath divider, a fluted column sidebar) must serve the composition's balance and hierarchy rather than exist for its own sake.

---

## Visual Characteristics

### Core Design Traits

- **Strict bilateral symmetry**: Layouts are organized around a central vertical axis with mirrored elements on either side, reflecting the axial planning of classical temples and civic buildings
- **Column and pilaster motifs**: Vertical structural elements inspired by the Doric, Ionic, and Corinthian orders are used as sidebar frames, dividers, or decorative accents to evoke classical architecture
- **Pediment and entablature references**: Triangular pediment shapes appear in header areas, card tops, or section dividers, echoing the roofline structures of Greek temples
- **Greek key (meander) borders**: The continuous right-angled spiral pattern from ancient Greek pottery and architecture is used as decorative borders, section dividers, and frame accents
- **Laurel wreath and acanthus ornaments**: Classical botanical motifs are used sparingly as dividers, icons, or accent decorations to signal achievement, honor, or structural punctuation
- **Marble and stone textures**: Backgrounds and surfaces employ subtle marble veining, limestone grain, or travertine textures to evoke the materiality of classical buildings and sculpture
- **High-contrast serif typography**: Transitional and Didone typefaces with dramatic thick-thin stroke contrast reference the letterforms carved into Roman monuments and printed during the Neoclassical era
- **Balanced whitespace and golden proportions**: Generous, symmetrical margins and padding follow classical proportional systems, with the golden ratio (1:1.618) guiding spacing and element sizing
- **Restrained color palette**: Muted neutrals (ivory, cream, warm gray, stone) dominate, with gold, deep navy, and classical red used as deliberate accents rather than broad fills
- **Medallion and cameo elements**: Circular or oval framing devices containing portraits, monograms, or icons reference classical cameos, coins, and relief sculpture

### Design Principles

- **Order over expression**: Every element occupies a deliberate position within a structured grid; asymmetry and randomness are antithetical to the aesthetic
- **Ornament serves structure**: Decorative elements (borders, flourishes, motifs) must reinforce the visual hierarchy and compositional balance rather than exist as pure embellishment
- **Proportion governs scale**: Element sizes relate to each other through classical proportional systems -- the golden ratio, the classical orders, and modular grids derived from a base unit
- **Material honesty through texture**: Surfaces reference noble materials (marble, stone, bronze, parchment) to convey permanence and gravitas without resorting to gratuitous skeuomorphism
- **Hierarchy through typographic contrast**: Information hierarchy is established primarily through type size, weight, and style contrast within a limited family of classical serifs, not through color or imagery
- **Restraint as sophistication**: The deliberate withholding of decoration signals confidence and refinement; every element that could be removed but is kept must justify its presence
- **Civic dignity and timelessness**: The overall impression should be one of enduring authority and considered elegance, suitable for institutions, cultural organizations, and premium brands

---

## Color Palette

The Neoclassical color palette draws from the materials and patinas of Greco-Roman architecture: white marble, warm limestone, aged bronze, gilded surfaces, and the deep pigments found in Pompeian frescoes. Colors are muted and dignified, with metallic accents providing controlled moments of luxury.

| Swatch | Hex | Role / Usage |
|--------|-----|-------------|
| ![#FAF6F0](https://via.placeholder.com/20/FAF6F0/FAF6F0) | `#FAF6F0` | Primary background -- warm parchment white |
| ![#F2EDE4](https://via.placeholder.com/20/F2EDE4/F2EDE4) | `#F2EDE4` | Secondary background -- aged ivory |
| ![#E8E0D4](https://via.placeholder.com/20/E8E0D4/E8E0D4) | `#E8E0D4` | Tertiary surface -- warm limestone |
| ![#D4C9B8](https://via.placeholder.com/20/D4C9B8/D4C9B8) | `#D4C9B8` | Borders, dividers -- sandstone |
| ![#B8A99A](https://via.placeholder.com/20/B8A99A/B8A99A) | `#B8A99A` | Muted text, captions -- weathered stone |
| ![#8C7B6B](https://via.placeholder.com/20/8C7B6B/8C7B6B) | `#8C7B6B` | Secondary text -- aged bronze |
| ![#4A3C2E](https://via.placeholder.com/20/4A3C2E/4A3C2E) | `#4A3C2E` | Primary text -- dark walnut |
| ![#2C1E10](https://via.placeholder.com/20/2C1E10/2C1E10) | `#2C1E10` | Display headings -- near-black sepia |
| ![#C6A96C](https://via.placeholder.com/20/C6A96C/C6A96C) | `#C6A96C` | Primary accent -- classical gold |
| ![#D4AF37](https://via.placeholder.com/20/D4AF37/D4AF37) | `#D4AF37` | Metallic accent -- polished gold |
| ![#1B3A4B](https://via.placeholder.com/20/1B3A4B/1B3A4B) | `#1B3A4B` | Deep accent -- Pompeian blue |
| ![#8B2332](https://via.placeholder.com/20/8B2332/8B2332) | `#8B2332` | Warm accent -- Pompeian red |
| ![#4A6741](https://via.placeholder.com/20/4A6741/4A6741) | `#4A6741` | Organic accent -- laurel green |
| ![#F5F0E8](https://via.placeholder.com/20/F5F0E8/F5F0E8) | `#F5F0E8` | Card surfaces -- polished marble |
| ![#FFFFFF](https://via.placeholder.com/20/FFFFFF/FFFFFF) | `#FFFFFF` | Pure white -- sculptural highlights |

### CSS Custom Properties

```css
:root {
  /* Marble and Stone Neutrals */
  --neo-parchment: #faf6f0;
  --neo-ivory: #f2ede4;
  --neo-limestone: #e8e0d4;
  --neo-sandstone: #d4c9b8;
  --neo-weathered: #b8a99a;
  --neo-bronze: #8c7b6b;
  --neo-walnut: #4a3c2e;
  --neo-sepia: #2c1e10;

  /* Classical Accents */
  --neo-gold: #c6a96c;
  --neo-gold-bright: #d4af37;
  --neo-blue: #1b3a4b;
  --neo-red: #8b2332;
  --neo-green: #4a6741;

  /* Surface Colors */
  --neo-marble: #f5f0e8;
  --neo-white: #ffffff;

  /* Functional Tokens */
  --neo-bg: var(--neo-parchment);
  --neo-bg-alt: var(--neo-ivory);
  --neo-surface: var(--neo-marble);
  --neo-text: var(--neo-walnut);
  --neo-text-display: var(--neo-sepia);
  --neo-text-muted: var(--neo-bronze);
  --neo-border: var(--neo-sandstone);
  --neo-border-strong: var(--neo-bronze);
  --neo-accent: var(--neo-gold);
  --neo-accent-hover: var(--neo-gold-bright);
  --neo-link: var(--neo-blue);
  --neo-link-hover: var(--neo-red);
}
```

---

## Typography

Neoclassical typography favors transitional and Didone serif typefaces that emerged during the 18th and early 19th centuries. These faces are characterized by high stroke contrast (thick verticals, thin horizontals), refined serifs, and vertical stress axes -- qualities that echo the precision of Roman inscriptional lettering. Display text is often set in all-caps with generous letter-spacing to evoke carved stone inscriptions.

### Recommended Google Fonts

| Font | Weight(s) | Usage | Link |
|------|-----------|-------|------|
| Playfair Display | 400, 500, 700, 900 | Display headings, hero titles -- high-contrast Didone elegance | [fonts.google.com/specimen/Playfair+Display](https://fonts.google.com/specimen/Playfair+Display) |
| Cormorant Garamond | 300, 400, 500, 600, 700 | Body text, subheadings -- refined calligraphic serif | [fonts.google.com/specimen/Cormorant+Garamond](https://fonts.google.com/specimen/Cormorant+Garamond) |
| Libre Baskerville | 400, 700 | Body text, editorial content -- sturdy transitional serif | [fonts.google.com/specimen/Libre+Baskerville](https://fonts.google.com/specimen/Libre+Baskerville) |
| Cinzel | 400, 500, 600, 700, 800, 900 | All-caps display, inscriptions -- Roman capital letterforms | [fonts.google.com/specimen/Cinzel](https://fonts.google.com/specimen/Cinzel) |
| Cinzel Decorative | 400, 700, 900 | Ornamental display, monograms -- decorated Roman capitals | [fonts.google.com/specimen/Cinzel+Decorative](https://fonts.google.com/specimen/Cinzel+Decorative) |
| EB Garamond | 400, 500, 600, 700 | Long-form body text -- classic old-style for readability | [fonts.google.com/specimen/EB+Garamond](https://fonts.google.com/specimen/EB+Garamond) |
| Italiana | 400 | Elegant display, subtitles -- Didone-inspired Italian letterforms | [fonts.google.com/specimen/Italiana](https://fonts.google.com/specimen/Italiana) |
| GFS Didot | 400 | Display text, titles -- authentic Didone typeface from Greek Font Society | [fonts.google.com/specimen/GFS+Didot](https://fonts.google.com/specimen/GFS+Didot) |

### Font Pairing Suggestions

| Heading | Body | Vibe |
|---------|------|------|
| Cinzel (700) | Cormorant Garamond (400) | Carved Roman inscription meets refined calligraphy -- the quintessential neoclassical pairing |
| Playfair Display (700) | Libre Baskerville (400) | High-contrast Didone drama with sturdy transitional readability -- editorial elegance |
| Cinzel Decorative (700) | EB Garamond (400) | Ornamental grandeur paired with the most readable classical serif -- formal institutions |
| GFS Didot (400) | Cormorant Garamond (300) | Greek typographic heritage meets refined French calligraphy -- art and cultural contexts |
| Italiana (400) | Libre Baskerville (400) | Italian Didone sophistication with English transitional stability -- luxury and fashion |

### CSS Example

```css
@import url('https://fonts.googleapis.com/css2?family=Cinzel:wght@400;500;700;900&family=Cormorant+Garamond:ital,wght@0,300;0,400;0,500;0,600;0,700;1,400;1,500&display=swap');

/* === Base Typography === */
body {
  font-family: 'Cormorant Garamond', 'Georgia', 'Times New Roman', serif;
  font-size: 18px;
  line-height: 1.75;
  color: var(--neo-text);
  background-color: var(--neo-bg);
  font-weight: 400;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}

h1, h2, h3, h4, h5, h6 {
  font-family: 'Cinzel', 'Georgia', serif;
  font-weight: 700;
  color: var(--neo-text-display);
  line-height: 1.2;
  margin: 0 0 0.75em 0;
}

h1 {
  font-size: clamp(2.5rem, 5vw, 4.5rem);
  letter-spacing: 0.08em;
  text-transform: uppercase;
}

h2 {
  font-size: clamp(1.75rem, 3.5vw, 3rem);
  letter-spacing: 0.06em;
  text-transform: uppercase;
}

h3 {
  font-size: clamp(1.25rem, 2.5vw, 2rem);
  letter-spacing: 0.04em;
}

h4 {
  font-size: clamp(1.1rem, 2vw, 1.5rem);
  font-weight: 500;
  letter-spacing: 0.03em;
}

p {
  margin-bottom: 1.25em;
  max-width: 65ch;
}

a {
  color: var(--neo-link);
  text-decoration: none;
  border-bottom: 1px solid transparent;
  transition: border-color 0.3s ease, color 0.3s ease;
}

a:hover {
  color: var(--neo-link-hover);
  border-bottom-color: var(--neo-link-hover);
}

blockquote {
  font-style: italic;
  font-size: 1.15em;
  border-left: 3px solid var(--neo-gold);
  margin: 2em 0;
  padding: 1em 1.5em;
  color: var(--neo-text-muted);
}

.small-caps {
  font-variant: small-caps;
  letter-spacing: 0.05em;
}

.inscription {
  font-family: 'Cinzel', serif;
  text-transform: uppercase;
  letter-spacing: 0.15em;
  font-size: 0.85em;
}
```

---

## Layout Principles

- **Symmetrical grid structure**: Use a centered, symmetrical grid (commonly 12-column) where content blocks mirror each other across the central axis; avoid asymmetrical or off-center compositions
- **Central axis alignment**: Key elements (headings, hero content, logos, ornamental dividers) should be centered on the page's vertical axis, reinforcing the classical emphasis on bilateral symmetry
- **Golden ratio proportions**: Apply the golden ratio (1:1.618) to column widths, margin ratios, and vertical spacing to achieve the balanced proportions found in classical architecture
- **Generous, structured whitespace**: Use ample margins and padding, but keep them consistent and proportional; whitespace should feel deliberate and architectural, not loose or arbitrary
- **Clear horizontal bands**: Organize the page into distinct horizontal sections (header/entablature, content columns, footer/base) that reference the tripartite structure of classical buildings
- **Contained max-width**: Content should not span the full viewport width; use a max-width container (900-1100px) centered on the page to create a dignified, framed composition like a classical facade
- **Visual weight at the center**: Place the most important content at or near the central axis; secondary elements flank the primary content symmetrically, drawing the eye inward
- **Vertical rhythm through consistent spacing**: Establish a base spacing unit (e.g., 8px or based on body line-height) and derive all vertical margins and padding from multiples of that unit

---

## CSS / Design Techniques

### Neoclassical Card

A content card with subtle marble texture, refined borders, and classical proportions. The card conveys permanence and structure through restrained styling.

```css
.neo-card {
  background-color: var(--neo-surface);
  border: 1px solid var(--neo-border);
  padding: 2.5rem 2rem;
  margin: 1.5rem 0;
  text-align: center;
  position: relative;
  transition: box-shadow 0.3s ease, border-color 0.3s ease;
}

.neo-card::before {
  content: '';
  position: absolute;
  top: 6px;
  left: 6px;
  right: 6px;
  bottom: 6px;
  border: 1px solid var(--neo-border);
  pointer-events: none;
}

.neo-card:hover {
  border-color: var(--neo-gold);
  box-shadow: 0 4px 20px rgba(74, 60, 46, 0.08);
}

.neo-card h3 {
  font-family: 'Cinzel', serif;
  font-size: 1.25rem;
  letter-spacing: 0.1em;
  text-transform: uppercase;
  margin-bottom: 1rem;
  color: var(--neo-text-display);
}

.neo-card p {
  font-family: 'Cormorant Garamond', serif;
  font-size: 1rem;
  line-height: 1.7;
  color: var(--neo-text-muted);
  margin: 0 auto;
  max-width: 40ch;
}
```

### Classical Button

Buttons with refined borders, gold accents, and uppercase inscriptional lettering. Hover states introduce a dignified color shift rather than aggressive visual changes.

```css
.neo-button {
  display: inline-block;
  font-family: 'Cinzel', serif;
  font-size: 0.8rem;
  font-weight: 700;
  text-transform: uppercase;
  letter-spacing: 0.2em;
  padding: 0.875rem 2.5rem;
  border: 1px solid var(--neo-gold);
  background-color: transparent;
  color: var(--neo-gold);
  cursor: pointer;
  text-decoration: none;
  transition: all 0.3s ease;
  position: relative;
}

.neo-button:hover {
  background-color: var(--neo-gold);
  color: var(--neo-white);
  border-color: var(--neo-gold);
}

.neo-button:active {
  background-color: var(--neo-gold-bright);
  border-color: var(--neo-gold-bright);
}

.neo-button--filled {
  background-color: var(--neo-gold);
  color: var(--neo-white);
}

.neo-button--filled:hover {
  background-color: var(--neo-gold-bright);
  border-color: var(--neo-gold-bright);
  color: var(--neo-white);
}

.neo-button--dark {
  border-color: var(--neo-text-display);
  color: var(--neo-text-display);
}

.neo-button--dark:hover {
  background-color: var(--neo-text-display);
  color: var(--neo-parchment);
}
```

### Navigation Bar

A classically inspired navigation bar with centered links, subtle gold underline accents, and inscriptional typography. The structure mirrors the entablature of a classical building.

```css
.neo-nav {
  background-color: var(--neo-bg);
  border-bottom: 1px solid var(--neo-border);
  padding: 1.25rem 2rem;
  text-align: center;
  position: relative;
}

.neo-nav::after {
  content: '';
  display: block;
  width: 60%;
  height: 1px;
  background: linear-gradient(to right, transparent, var(--neo-gold), transparent);
  margin: 0 auto;
  position: absolute;
  bottom: -1px;
  left: 20%;
}

.neo-nav ul {
  list-style: none;
  padding: 0;
  margin: 0;
  display: flex;
  justify-content: center;
  gap: 2.5rem;
}

.neo-nav a {
  font-family: 'Cinzel', serif;
  font-size: 0.75rem;
  font-weight: 500;
  text-transform: uppercase;
  letter-spacing: 0.2em;
  color: var(--neo-text);
  text-decoration: none;
  padding: 0.5rem 0;
  border-bottom: 2px solid transparent;
  transition: color 0.3s ease, border-color 0.3s ease;
}

.neo-nav a:hover {
  color: var(--neo-gold);
  border-bottom-color: var(--neo-gold);
}

.neo-nav a.active {
  color: var(--neo-gold);
  border-bottom-color: var(--neo-gold);
}
```

### Hero Section

A stately hero section with centered text, classical typography hierarchy, and a subtle marble texture background. The layout evokes the facade of a temple with content centered beneath a metaphorical pediment.

```css
.neo-hero {
  min-height: 85vh;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  text-align: center;
  padding: 4rem 2rem;
  background-color: var(--neo-bg);
  background-image:
    radial-gradient(ellipse at 20% 50%, rgba(198, 169, 108, 0.03) 0%, transparent 50%),
    radial-gradient(ellipse at 80% 50%, rgba(198, 169, 108, 0.03) 0%, transparent 50%);
  position: relative;
}

.neo-hero::before,
.neo-hero::after {
  content: '';
  display: block;
  width: 120px;
  height: 1px;
  background-color: var(--neo-gold);
  margin: 0 auto;
}

.neo-hero::before {
  position: absolute;
  top: 3rem;
  left: 50%;
  transform: translateX(-50%);
}

.neo-hero::after {
  position: absolute;
  bottom: 3rem;
  left: 50%;
  transform: translateX(-50%);
}

.neo-hero h1 {
  font-family: 'Cinzel', serif;
  font-size: clamp(2.5rem, 6vw, 5rem);
  font-weight: 700;
  letter-spacing: 0.12em;
  text-transform: uppercase;
  color: var(--neo-text-display);
  margin: 0;
  line-height: 1.15;
}

.neo-hero .subtitle {
  font-family: 'Cormorant Garamond', serif;
  font-size: clamp(1rem, 2vw, 1.4rem);
  font-style: italic;
  color: var(--neo-text-muted);
  margin-top: 1.25rem;
  letter-spacing: 0.03em;
}

.neo-hero .divider-ornament {
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 1rem;
  margin: 2rem 0;
  color: var(--neo-gold);
  font-size: 1.2rem;
}

.neo-hero .divider-ornament::before,
.neo-hero .divider-ornament::after {
  content: '';
  width: 60px;
  height: 1px;
  background-color: var(--neo-gold);
}
```

### Greek Key Border

A CSS-only Greek key (meander) border pattern using repeating linear gradients. This technique creates the iconic right-angled spiral motif without any images.

```css
.greek-key-border {
  --gk-color: var(--neo-gold);
  --gk-bg: var(--neo-bg);
  --gk-size: 20px;
  --gk-weight: 3px;

  position: relative;
  padding: 2rem;
  border: var(--gk-weight) solid var(--gk-color);
}

.greek-key-border::before {
  content: '';
  position: absolute;
  top: calc(var(--gk-weight) + 4px);
  left: calc(var(--gk-weight) + 4px);
  right: calc(var(--gk-weight) + 4px);
  bottom: calc(var(--gk-weight) + 4px);
  border: 1px solid var(--gk-color);
  pointer-events: none;
}

/* Simplified Greek Key top/bottom strip using SVG data URI */
.greek-key-top,
.greek-key-bottom {
  width: 100%;
  height: 20px;
  background-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='40' height='20'%3E%3Cpath d='M0,10 L10,10 L10,0 L30,0 L30,10 L40,10 L40,20 L20,20 L20,10 L0,10 Z' fill='none' stroke='%23c6a96c' stroke-width='1.5'/%3E%3C/svg%3E");
  background-repeat: repeat-x;
  background-size: 40px 20px;
}

.greek-key-bottom {
  transform: rotate(180deg);
}

/* Alternative: simple stepped border using box-shadow */
.greek-key-simple {
  border-top: 3px solid var(--neo-gold);
  border-bottom: 3px solid var(--neo-gold);
  box-shadow:
    inset 0 6px 0 0 var(--neo-bg),
    inset 0 9px 0 0 var(--neo-gold),
    inset 0 -6px 0 0 var(--neo-bg),
    inset 0 -9px 0 0 var(--neo-gold);
  padding: 1.5rem 2rem;
}
```

### Column Frame

A decorative column-inspired sidebar or content frame using CSS to evoke the fluted columns of classical architecture. The vertical grooves are created with repeating gradients.

```css
.column-frame {
  display: flex;
  gap: 0;
}

.column-frame .pilaster {
  width: 40px;
  flex-shrink: 0;
  background: repeating-linear-gradient(
    to right,
    var(--neo-limestone) 0px,
    var(--neo-ivory) 2px,
    var(--neo-limestone) 4px,
    var(--neo-sandstone) 5px,
    var(--neo-limestone) 6px,
    var(--neo-ivory) 8px
  );
  position: relative;
}

/* Capital (top ornament) */
.column-frame .pilaster::before {
  content: '';
  position: absolute;
  top: 0;
  left: -4px;
  right: -4px;
  height: 24px;
  background-color: var(--neo-limestone);
  border-bottom: 2px solid var(--neo-sandstone);
  border-top: 2px solid var(--neo-sandstone);
}

/* Base (bottom ornament) */
.column-frame .pilaster::after {
  content: '';
  position: absolute;
  bottom: 0;
  left: -4px;
  right: -4px;
  height: 16px;
  background-color: var(--neo-limestone);
  border-top: 2px solid var(--neo-sandstone);
}

.column-frame .content-area {
  flex: 1;
  padding: 2.5rem;
  border-top: 2px solid var(--neo-sandstone);
  border-bottom: 2px solid var(--neo-sandstone);
  background-color: var(--neo-surface);
}
```

### Laurel Wreath Divider

A decorative section divider using CSS and a unicode/SVG laurel wreath motif to separate content sections with classical elegance.

```css
.laurel-divider {
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 1.5rem;
  margin: 3rem auto;
  max-width: 500px;
  color: var(--neo-gold);
}

.laurel-divider::before,
.laurel-divider::after {
  content: '';
  flex: 1;
  height: 1px;
  background: linear-gradient(to var(--dir, right), var(--neo-gold), transparent);
}

.laurel-divider::after {
  --dir: left;
}

.laurel-divider .ornament {
  font-size: 1.5rem;
  line-height: 1;
  opacity: 0.8;
}

/* Variant with double lines */
.laurel-divider--double::before,
.laurel-divider--double::after {
  height: 0;
  border-top: 1px solid var(--neo-gold);
  border-bottom: 1px solid var(--neo-gold);
  padding-top: 3px;
  background: none;
}

/* Variant with diamond ornament */
.laurel-divider--diamond .ornament {
  width: 10px;
  height: 10px;
  background-color: var(--neo-gold);
  transform: rotate(45deg);
  font-size: 0;
}

/* Star ornament variant */
.laurel-divider--star .ornament::before {
  content: '✦';
}
```

### Marble Texture Background

A pure-CSS marble texture using layered radial and linear gradients to simulate the veined appearance of classical marble without external images.

```css
.marble-surface {
  background-color: #f5f0e8;
  background-image:
    /* Primary veining */
    radial-gradient(ellipse at 15% 25%, rgba(180, 170, 155, 0.15) 0%, transparent 50%),
    radial-gradient(ellipse at 75% 60%, rgba(180, 170, 155, 0.12) 0%, transparent 45%),
    radial-gradient(ellipse at 45% 80%, rgba(160, 150, 135, 0.1) 0%, transparent 40%),
    /* Secondary veining */
    linear-gradient(135deg, transparent 20%, rgba(212, 201, 184, 0.08) 25%, transparent 30%),
    linear-gradient(225deg, transparent 40%, rgba(212, 201, 184, 0.06) 45%, transparent 50%),
    linear-gradient(315deg, transparent 60%, rgba(212, 201, 184, 0.08) 65%, transparent 70%),
    /* Subtle grain */
    repeating-linear-gradient(
      90deg,
      transparent,
      transparent 2px,
      rgba(200, 190, 175, 0.02) 2px,
      rgba(200, 190, 175, 0.02) 4px
    );
}

/* Darker marble variant for contrast sections */
.marble-surface--dark {
  background-color: var(--neo-text-display);
  background-image:
    radial-gradient(ellipse at 20% 30%, rgba(255, 255, 255, 0.03) 0%, transparent 50%),
    radial-gradient(ellipse at 70% 70%, rgba(255, 255, 255, 0.02) 0%, transparent 45%),
    linear-gradient(135deg, transparent 30%, rgba(255, 255, 255, 0.02) 35%, transparent 40%);
  color: var(--neo-ivory);
}
```

---

## Design Do's and Don'ts

### Do's

- **Maintain strict symmetry** in all major layout decisions; center headings, balance columns, and mirror decorative elements across the central axis
- **Use classical serif typefaces** with high stroke contrast (Didone, transitional) for headings and refined old-style serifs for body text to evoke inscriptional and printed classical letterforms
- **Apply gold accents sparingly** for borders, dividers, hover states, and ornamental details; gold should punctuate the composition, not overwhelm it
- **Employ generous whitespace** with consistent proportional relationships; every margin and padding value should relate to a base unit or the golden ratio
- **Reference classical architectural elements** (columns, pediments, entablatures, medallions) through subtle CSS techniques rather than literal illustrations
- **Keep the color palette restrained** with warm neutrals dominating and only two or three accent colors used across the entire design
- **Use uppercase letter-spaced text** for navigation, labels, and section headings to evoke the inscriptional quality of Roman carved lettering
- **Add subtle texture** through CSS gradients (marble veining, parchment grain) to convey material richness without heavy image files
- **Design for timelessness** by avoiding trendy elements; the composition should feel as appropriate in five years as it does today

### Don'ts

- **Don't use asymmetrical or broken-grid layouts** -- off-center compositions, overlapping elements, and deliberately irregular grids contradict the classical emphasis on order
- **Don't use sans-serif fonts for primary text** -- geometric or grotesque sans-serifs belong to Modernist and Minimalist aesthetics; Neoclassicism demands serifs with visible stroke modulation
- **Don't apply bright, saturated colors** -- neon, electric blue, hot pink, and other high-chroma hues are anachronistic; keep the palette muted, warm, and grounded in natural material tones
- **Don't use rounded corners with large radii** -- if border-radius is used at all, keep it minimal (2-4px) or use it only for circular medallion elements; sharp or very slightly softened corners suit the aesthetic
- **Don't overload with ornament** -- the Rococo excess that Neoclassicism reacted against should not creep back in; each decorative element must serve a structural or hierarchical purpose
- **Don't use playful or casual animations** -- if motion is used, it should be slow, dignified fades and subtle transitions (300-500ms ease) rather than bounces, wobbles, or particle effects
- **Don't mix too many typefaces** -- stick to a maximum of two font families (one for display, one for body) to maintain the disciplined typographic hierarchy that defines the style
- **Don't use dark mode as default** -- the Neoclassical palette is built around light marble and parchment tones; a dark variant can exist but should feel like a moonlit gallery, not a tech interface

---

## Related Aesthetics

| Aesthetic | Relationship |
|-----------|-------------|
| [Art Deco](Art_Deco.md) | Shares geometric ornament and gold accents but pushes toward Modernist abstraction with zigzag patterns, sunburst motifs, and streamlined geometry that Neoclassicism would consider excessive |
| [Light Academia](Light_Academia.md) | Draws from similar classical and scholarly visual language -- warm neutrals, serif typography, parchment textures -- but applies them with a softer, more romantic and nostalgic sensibility |
| [Editorial Magazine Layout](Editorial_Magazine_Layout.md) | Shares the emphasis on typographic hierarchy, structured grids, and restrained elegance, though Editorial design allows more asymmetry and photographic content |
| [Material Design](Material_Design.md) | Both pursue systematic order and consistent spatial rules, but Material Design's geometric sans-serifs and flat color system are distinctly Modernist rather than classical |
| [Minimalism](Minimalism.md) | Shares the principle of restraint and whitespace, but Minimalism strips away all ornament while Neoclassicism retains deliberate, structural decoration |
| [Wes Anderson](Wes_Anderson.md) | Both use symmetrical composition and warm muted palettes, but Wes Anderson applies these with whimsical irony and pastel eccentricity foreign to Neoclassical gravity |

---

## Quick-Start HTML Template

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Neoclassicism Design Template</title>
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Cinzel:wght@400;500;700;900&family=Cormorant+Garamond:ital,wght@0,300;0,400;0,500;0,600;0,700;1,400;1,500&display=swap" rel="stylesheet">
  <style>
    /* --- Custom Properties --- */
    :root {
      --neo-parchment: #faf6f0;
      --neo-ivory: #f2ede4;
      --neo-limestone: #e8e0d4;
      --neo-sandstone: #d4c9b8;
      --neo-weathered: #b8a99a;
      --neo-bronze: #8c7b6b;
      --neo-walnut: #4a3c2e;
      --neo-sepia: #2c1e10;
      --neo-gold: #c6a96c;
      --neo-gold-bright: #d4af37;
      --neo-blue: #1b3a4b;
      --neo-red: #8b2332;
      --neo-green: #4a6741;
      --neo-marble: #f5f0e8;
      --neo-white: #ffffff;

      --neo-bg: var(--neo-parchment);
      --neo-bg-alt: var(--neo-ivory);
      --neo-surface: var(--neo-marble);
      --neo-text: var(--neo-walnut);
      --neo-text-display: var(--neo-sepia);
      --neo-text-muted: var(--neo-bronze);
      --neo-border: var(--neo-sandstone);
      --neo-accent: var(--neo-gold);
    }

    /* --- Reset & Base --- */
    *, *::before, *::after {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
    }

    html {
      scroll-behavior: smooth;
    }

    body {
      font-family: 'Cormorant Garamond', 'Georgia', 'Times New Roman', serif;
      font-size: 18px;
      line-height: 1.75;
      color: var(--neo-text);
      background-color: var(--neo-bg);
      -webkit-font-smoothing: antialiased;
      -moz-osx-font-smoothing: grayscale;
    }

    /* --- Typography --- */
    h1, h2, h3, h4 {
      font-family: 'Cinzel', 'Georgia', serif;
      font-weight: 700;
      color: var(--neo-text-display);
      line-height: 1.2;
    }

    h1 {
      font-size: clamp(2.5rem, 6vw, 5rem);
      letter-spacing: 0.12em;
      text-transform: uppercase;
    }

    h2 {
      font-size: clamp(1.5rem, 3.5vw, 2.5rem);
      letter-spacing: 0.08em;
      text-transform: uppercase;
    }

    h3 {
      font-size: clamp(1.1rem, 2vw, 1.5rem);
      letter-spacing: 0.06em;
      text-transform: uppercase;
    }

    p {
      max-width: 65ch;
      margin-bottom: 1.25em;
    }

    a {
      color: var(--neo-blue);
      text-decoration: none;
      border-bottom: 1px solid transparent;
      transition: color 0.3s ease, border-color 0.3s ease;
    }

    a:hover {
      color: var(--neo-red);
      border-bottom-color: var(--neo-red);
    }

    img {
      max-width: 100%;
      height: auto;
    }

    /* --- Navigation --- */
    .nav {
      background-color: var(--neo-bg);
      border-bottom: 1px solid var(--neo-border);
      padding: 1.25rem 2rem;
      text-align: center;
      position: sticky;
      top: 0;
      z-index: 100;
    }

    .nav::after {
      content: '';
      display: block;
      width: 50%;
      height: 1px;
      background: linear-gradient(to right, transparent, var(--neo-gold), transparent);
      margin: 0 auto;
      position: absolute;
      bottom: -1px;
      left: 25%;
    }

    .nav ul {
      list-style: none;
      display: flex;
      justify-content: center;
      flex-wrap: wrap;
      gap: 2rem;
    }

    .nav a {
      font-family: 'Cinzel', serif;
      font-size: 0.7rem;
      font-weight: 500;
      text-transform: uppercase;
      letter-spacing: 0.2em;
      color: var(--neo-text);
      padding: 0.5rem 0;
      border-bottom: 2px solid transparent;
    }

    .nav a:hover,
    .nav a.active {
      color: var(--neo-gold);
      border-bottom-color: var(--neo-gold);
    }

    /* --- Hero --- */
    .hero {
      min-height: 85vh;
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      text-align: center;
      padding: 5rem 2rem;
      position: relative;
      background-image:
        radial-gradient(ellipse at 20% 50%, rgba(198, 169, 108, 0.03) 0%, transparent 50%),
        radial-gradient(ellipse at 80% 50%, rgba(198, 169, 108, 0.03) 0%, transparent 50%);
    }

    .hero h1 {
      margin: 0;
    }

    .hero .subtitle {
      font-family: 'Cormorant Garamond', serif;
      font-size: clamp(1rem, 2vw, 1.35rem);
      font-style: italic;
      color: var(--neo-text-muted);
      margin-top: 1rem;
      letter-spacing: 0.02em;
    }

    .hero .btn-row {
      margin-top: 2.5rem;
      display: flex;
      gap: 1.25rem;
      flex-wrap: wrap;
      justify-content: center;
    }

    /* --- Ornamental Divider --- */
    .ornament-divider {
      display: flex;
      align-items: center;
      justify-content: center;
      gap: 1.25rem;
      margin: 2.5rem auto;
      max-width: 400px;
      color: var(--neo-gold);
    }

    .ornament-divider::before,
    .ornament-divider::after {
      content: '';
      flex: 1;
      height: 1px;
      background: linear-gradient(to var(--dir, right), var(--neo-gold), transparent);
    }

    .ornament-divider::after {
      --dir: left;
    }

    .ornament-divider span {
      font-size: 1.25rem;
      line-height: 1;
    }

    /* --- Greek Key Strip --- */
    .greek-key-strip {
      width: 100%;
      height: 20px;
      background-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='40' height='20' viewBox='0 0 40 20'%3E%3Crect x='1' y='1' width='18' height='8' fill='none' stroke='%23c6a96c' stroke-width='1.2'/%3E%3Crect x='21' y='11' width='18' height='8' fill='none' stroke='%23c6a96c' stroke-width='1.2'/%3E%3Cline x1='10' y1='9' x2='10' y2='20' stroke='%23c6a96c' stroke-width='1.2'/%3E%3Cline x1='30' y1='0' x2='30' y2='11' stroke='%23c6a96c' stroke-width='1.2'/%3E%3C/svg%3E");
      background-repeat: repeat-x;
      background-size: 40px 20px;
      margin: 0 auto;
    }

    /* --- Buttons --- */
    .btn {
      display: inline-block;
      font-family: 'Cinzel', serif;
      font-size: 0.75rem;
      font-weight: 700;
      text-transform: uppercase;
      letter-spacing: 0.2em;
      padding: 0.875rem 2.25rem;
      border: 1px solid var(--neo-gold);
      background-color: transparent;
      color: var(--neo-gold);
      cursor: pointer;
      text-decoration: none;
      transition: all 0.3s ease;
    }

    .btn:hover {
      background-color: var(--neo-gold);
      color: var(--neo-white);
      border-bottom-color: var(--neo-gold);
    }

    .btn--filled {
      background-color: var(--neo-gold);
      color: var(--neo-white);
    }

    .btn--filled:hover {
      background-color: var(--neo-gold-bright);
      border-color: var(--neo-gold-bright);
      color: var(--neo-white);
    }

    /* --- Section Container --- */
    .section {
      padding: 5rem 2rem;
      max-width: 1100px;
      margin: 0 auto;
      text-align: center;
    }

    .section h2 {
      margin-bottom: 0.5rem;
    }

    .section .section-subtitle {
      font-style: italic;
      color: var(--neo-text-muted);
      margin-bottom: 3rem;
      font-size: 1.05rem;
    }

    .section p {
      margin-left: auto;
      margin-right: auto;
    }

    /* --- Card Grid --- */
    .card-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
      gap: 2rem;
      margin-top: 2rem;
    }

    .card {
      background-color: var(--neo-surface);
      border: 1px solid var(--neo-border);
      padding: 2.5rem 2rem;
      text-align: center;
      position: relative;
      transition: box-shadow 0.3s ease, border-color 0.3s ease;
    }

    .card::before {
      content: '';
      position: absolute;
      top: 6px;
      left: 6px;
      right: 6px;
      bottom: 6px;
      border: 1px solid var(--neo-border);
      pointer-events: none;
      transition: border-color 0.3s ease;
    }

    .card:hover {
      border-color: var(--neo-gold);
      box-shadow: 0 4px 24px rgba(74, 60, 46, 0.08);
    }

    .card:hover::before {
      border-color: var(--neo-gold);
    }

    .card .card-icon {
      font-size: 2rem;
      color: var(--neo-gold);
      margin-bottom: 1.25rem;
      display: block;
    }

    .card h3 {
      margin-bottom: 1rem;
    }

    .card p {
      font-size: 0.95rem;
      color: var(--neo-text-muted);
      line-height: 1.7;
      margin: 0 auto;
    }

    /* --- Feature Section with Column Frame --- */
    .column-section {
      background-color: var(--neo-bg-alt);
      border-top: 1px solid var(--neo-border);
      border-bottom: 1px solid var(--neo-border);
    }

    .column-frame {
      display: flex;
      max-width: 1100px;
      margin: 0 auto;
      min-height: 400px;
    }

    .pilaster {
      width: 36px;
      flex-shrink: 0;
      background: repeating-linear-gradient(
        to right,
        var(--neo-limestone) 0px,
        var(--neo-ivory) 2px,
        var(--neo-limestone) 4px,
        var(--neo-sandstone) 5px,
        var(--neo-limestone) 6px,
        var(--neo-ivory) 8px
      );
      position: relative;
    }

    .pilaster::before {
      content: '';
      position: absolute;
      top: 0;
      left: -3px;
      right: -3px;
      height: 20px;
      background-color: var(--neo-limestone);
      border-bottom: 2px solid var(--neo-sandstone);
      border-top: 2px solid var(--neo-sandstone);
    }

    .pilaster::after {
      content: '';
      position: absolute;
      bottom: 0;
      left: -3px;
      right: -3px;
      height: 14px;
      background-color: var(--neo-limestone);
      border-top: 2px solid var(--neo-sandstone);
    }

    .column-content {
      flex: 1;
      padding: 4rem 3.5rem;
      display: flex;
      flex-direction: column;
      justify-content: center;
      text-align: center;
    }

    .column-content blockquote {
      font-style: italic;
      font-size: 1.3rem;
      line-height: 1.8;
      color: var(--neo-text-muted);
      border: none;
      padding: 0;
      margin: 1.5rem auto;
      max-width: 55ch;
    }

    .column-content .attribution {
      font-family: 'Cinzel', serif;
      font-size: 0.8rem;
      letter-spacing: 0.15em;
      text-transform: uppercase;
      color: var(--neo-gold);
      margin-top: 0.75rem;
    }

    /* --- Marble Band --- */
    .marble-band {
      padding: 5rem 2rem;
      text-align: center;
      background-color: var(--neo-marble);
      background-image:
        radial-gradient(ellipse at 15% 25%, rgba(180, 170, 155, 0.12) 0%, transparent 50%),
        radial-gradient(ellipse at 75% 60%, rgba(180, 170, 155, 0.1) 0%, transparent 45%),
        radial-gradient(ellipse at 50% 80%, rgba(160, 150, 135, 0.08) 0%, transparent 40%),
        linear-gradient(135deg, transparent 20%, rgba(212, 201, 184, 0.06) 25%, transparent 30%),
        linear-gradient(225deg, transparent 40%, rgba(212, 201, 184, 0.05) 45%, transparent 50%);
    }

    .marble-band h2 {
      margin-bottom: 1rem;
    }

    .marble-band p {
      margin-left: auto;
      margin-right: auto;
      color: var(--neo-text-muted);
    }

    .stats-row {
      display: flex;
      justify-content: center;
      gap: 4rem;
      margin-top: 3rem;
      flex-wrap: wrap;
    }

    .stat {
      text-align: center;
    }

    .stat .stat-number {
      font-family: 'Cinzel', serif;
      font-size: clamp(2rem, 4vw, 3.5rem);
      font-weight: 700;
      color: var(--neo-gold);
      display: block;
      line-height: 1.1;
    }

    .stat .stat-label {
      font-family: 'Cinzel', serif;
      font-size: 0.65rem;
      text-transform: uppercase;
      letter-spacing: 0.2em;
      color: var(--neo-text-muted);
      margin-top: 0.5rem;
      display: block;
    }

    /* --- Dark Contrast Section --- */
    .dark-section {
      background-color: var(--neo-sepia);
      background-image:
        radial-gradient(ellipse at 20% 30%, rgba(255, 255, 255, 0.02) 0%, transparent 50%),
        radial-gradient(ellipse at 70% 70%, rgba(255, 255, 255, 0.015) 0%, transparent 45%);
      color: var(--neo-ivory);
      padding: 5rem 2rem;
      text-align: center;
    }

    .dark-section h2 {
      color: var(--neo-ivory);
    }

    .dark-section p {
      color: var(--neo-weathered);
      margin-left: auto;
      margin-right: auto;
    }

    .dark-section .ornament-divider {
      color: var(--neo-gold);
    }

    .dark-section .ornament-divider::before {
      background: linear-gradient(to right, var(--neo-gold), transparent);
    }

    .dark-section .ornament-divider::after {
      background: linear-gradient(to left, var(--neo-gold), transparent);
    }

    .dark-section .btn {
      border-color: var(--neo-gold);
      color: var(--neo-gold);
    }

    .dark-section .btn:hover {
      background-color: var(--neo-gold);
      color: var(--neo-sepia);
    }

    /* --- Footer --- */
    .footer {
      background-color: var(--neo-bg-alt);
      border-top: 1px solid var(--neo-border);
      padding: 3rem 2rem;
      text-align: center;
    }

    .footer .footer-brand {
      font-family: 'Cinzel', serif;
      font-size: 1.1rem;
      font-weight: 700;
      letter-spacing: 0.15em;
      text-transform: uppercase;
      color: var(--neo-text-display);
      margin-bottom: 1rem;
    }

    .footer p {
      font-size: 0.85rem;
      color: var(--neo-text-muted);
      margin: 0.5rem auto;
    }

    .footer-links {
      list-style: none;
      display: flex;
      justify-content: center;
      gap: 2rem;
      margin-top: 1.5rem;
      flex-wrap: wrap;
    }

    .footer-links a {
      font-family: 'Cinzel', serif;
      font-size: 0.65rem;
      font-weight: 500;
      text-transform: uppercase;
      letter-spacing: 0.15em;
      color: var(--neo-text-muted);
    }

    .footer-links a:hover {
      color: var(--neo-gold);
      border-bottom-color: var(--neo-gold);
    }

    .footer .copyright {
      margin-top: 2rem;
      font-size: 0.75rem;
      color: var(--neo-weathered);
    }

    /* --- Responsive --- */
    @media (max-width: 768px) {
      .hero {
        min-height: 70vh;
        padding: 4rem 1.5rem;
      }

      .section {
        padding: 3.5rem 1.5rem;
      }

      .nav ul {
        gap: 1rem;
      }

      .nav a {
        font-size: 0.6rem;
        letter-spacing: 0.12em;
      }

      .card-grid {
        grid-template-columns: 1fr;
      }

      .pilaster {
        display: none;
      }

      .column-content {
        padding: 3rem 1.5rem;
      }

      .stats-row {
        gap: 2rem;
      }

      .hero .btn-row {
        flex-direction: column;
        align-items: center;
      }
    }
  </style>
</head>
<body>

  <!-- NAVIGATION -->
  <nav class="nav">
    <ul>
      <li><a href="#about" class="active">About</a></li>
      <li><a href="#virtues">Virtues</a></li>
      <li><a href="#philosophy">Philosophy</a></li>
      <li><a href="#legacy">Legacy</a></li>
      <li><a href="#contact">Contact</a></li>
    </ul>
  </nav>

  <!-- HERO -->
  <section class="hero" id="about">
    <div class="ornament-divider">
      <span>&#9753;</span>
    </div>
    <h1>Ars Longa<br>Vita Brevis</h1>
    <p class="subtitle">A celebration of order, proportion, and the enduring ideals of classical design</p>
    <div class="btn-row">
      <a href="#virtues" class="btn">Explore Virtues</a>
      <a href="#legacy" class="btn btn--filled">View Legacy</a>
    </div>
    <div class="ornament-divider" style="margin-top: 3rem;">
      <span>&#9753;</span>
    </div>
  </section>

  <!-- GREEK KEY STRIP -->
  <div class="greek-key-strip"></div>

  <!-- VIRTUES (CARD GRID) -->
  <section class="section" id="virtues">
    <h2>Classical Virtues</h2>
    <p class="section-subtitle">The pillars upon which enduring design is built</p>
    <div class="card-grid">
      <div class="card">
        <span class="card-icon">&#9878;</span>
        <h3>Symmetry</h3>
        <p>Balance in all things. Every element finds its mirror, creating compositions of serene equilibrium and visual harmony.</p>
      </div>
      <div class="card">
        <span class="card-icon">&#9041;</span>
        <h3>Proportion</h3>
        <p>The golden ratio governs scale and spacing, ensuring that each part relates harmoniously to the whole.</p>
      </div>
      <div class="card">
        <span class="card-icon">&#10038;</span>
        <h3>Restraint</h3>
        <p>Every ornament must justify its presence. Decoration serves structure, never overwhelming the composition it adorns.</p>
      </div>
    </div>
  </section>

  <!-- GREEK KEY STRIP -->
  <div class="greek-key-strip"></div>

  <!-- PHILOSOPHY (COLUMN FRAME SECTION) -->
  <section class="column-section" id="philosophy">
    <div class="column-frame">
      <div class="pilaster"></div>
      <div class="column-content">
        <h2>Philosophy</h2>
        <div class="ornament-divider">
          <span>&#10043;</span>
        </div>
        <blockquote>
          True elegance is not the accumulation of ornament, but the
          perfection of proportion. In restraint, we discover refinement.
          In order, we find beauty that endures beyond the fashions of any age.
        </blockquote>
        <p class="attribution">On Classical Design</p>
      </div>
      <div class="pilaster"></div>
    </div>
  </section>

  <!-- MARBLE BAND (STATISTICS) -->
  <section class="marble-band" id="legacy">
    <h2>Enduring Legacy</h2>
    <p class="section-subtitle" style="font-style: italic; color: var(--neo-text-muted);">
      Neoclassical design has shaped the built world for centuries
    </p>
    <div class="stats-row">
      <div class="stat">
        <span class="stat-number">1750</span>
        <span class="stat-label">Year of Origin</span>
      </div>
      <div class="stat">
        <span class="stat-number">III</span>
        <span class="stat-label">Classical Orders</span>
      </div>
      <div class="stat">
        <span class="stat-number">1.618</span>
        <span class="stat-label">Golden Ratio</span>
      </div>
      <div class="stat">
        <span class="stat-number">&#8734;</span>
        <span class="stat-label">Timelessness</span>
      </div>
    </div>
  </section>

  <!-- GREEK KEY STRIP -->
  <div class="greek-key-strip"></div>

  <!-- DARK CONTRAST SECTION (CTA) -->
  <section class="dark-section" id="contact">
    <h2>Begin Your Journey</h2>
    <div class="ornament-divider">
      <span>&#9753;</span>
    </div>
    <p>
      Embrace the clarity of classical design. Let symmetry guide your compositions,
      proportion govern your spaces, and restraint refine your craft.
    </p>
    <div style="margin-top: 2rem;">
      <a href="#about" class="btn">Return to the Beginning</a>
    </div>
  </section>

  <!-- FOOTER -->
  <footer class="footer">
    <div class="footer-brand">Neoclassicism</div>
    <p>Order, proportion, and enduring elegance in design.</p>
    <ul class="footer-links">
      <li><a href="#about">About</a></li>
      <li><a href="#virtues">Virtues</a></li>
      <li><a href="#philosophy">Philosophy</a></li>
      <li><a href="#legacy">Legacy</a></li>
    </ul>
    <p class="copyright">&copy; MMXXVI &middot; Designed in the classical tradition</p>
  </footer>

</body>
</html>
```

---

## Implementation Tips

- **Start with the golden ratio**: Establish a base spacing unit (e.g., 8px) and derive all padding, margin, and gap values from multiples of that unit that approximate golden ratio relationships (1, 1.618, 2.618, 4.236, etc.), then round to whole pixel values for consistency
- **Use CSS custom properties for the full palette**: Define all colors as custom properties from the start so that creating a dark variant (think moonlit marble gallery) or an alternate accent scheme (silver instead of gold, Pompeian red instead of blue) requires changing only the root variables
- **Test symmetry by mirroring**: Flip your layout horizontally in browser DevTools; if the composition looks identical (or intentionally identical where content differs), your symmetry is working; if elements feel unbalanced when mirrored, adjust their positioning
- **Layer subtle textures with CSS gradients**: Use multiple radial-gradient and linear-gradient layers at very low opacity (0.02-0.08) to simulate marble veining and parchment grain without any image requests; this keeps the page lightweight while adding material richness
- **Set up a typographic scale**: Use a 1.25 (major third) or 1.333 (perfect fourth) typographic scale to derive heading sizes from the body font size; this creates the orderly size hierarchy that Neoclassical design demands
- **Keep ornamental SVGs inline**: Greek key borders, laurel wreaths, and acanthus motifs should be embedded as SVG data URIs in CSS rather than loaded as external files; this eliminates extra HTTP requests and ensures the ornaments scale crisply at any resolution
- **Reserve gold for interaction and emphasis**: The gold accent color (#C6A96C) should appear primarily on hover states, active navigation indicators, divider ornaments, and key headings; overusing it dilutes its impact and shifts the aesthetic toward gaudy rather than refined
