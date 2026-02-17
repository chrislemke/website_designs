# French Provincial Style

## Overview

French Provincial Style is an aesthetic that embodies "a balance of rustic simplicity and refined elegance," originating from the provincial regions of France outside Paris. It translates the warmth of countryside living into a sophisticated design language characterized by muted color palettes, natural materials, curved ornamental details, and pastoral motifs. When applied to web design, the style evokes an atmosphere of timeless grace, comfort, and understated luxury.

## Visual Characteristics

- **Elegant restraint**: Refined but never ostentatious; luxury expressed through subtlety rather than excess
- **Soft, organic curves**: S-shaped cabriole legs, scrollwork, and scalloped edges inform decorative UI shapes
- **Symmetrical composition**: Balanced, formal layouts with clear visual hierarchy
- **Warm natural textures**: Stone, linen, aged wood, and soft fabrics translated into background textures and surface treatments
- **Distressed and aged finishes**: A patina of age conveyed through subtle texture overlays, muted tones, and soft shadow effects
- **Pastoral and floral ornamentation**: Botanical illustrations, toile patterns, and delicate flourishes used as decorative accents
- **Generous white space**: Open, airy layouts that allow content to breathe, echoing light-filled provincial interiors
- **Arched and rounded elements**: Arched doorways and windows inspire rounded corners, arched frames, and soft UI shapes

## Color Palette

The French Provincial palette draws from the natural landscape of rural France: sun-warmed stone, lavender fields, sage gardens, dusty blue skies, and cream-washed walls.

### Primary Palette

| Role | Color Name | Hex | Usage |
|------|-----------|-----|-------|
| Background | Antique Cream | `#FAF6F0` | Page backgrounds, card surfaces |
| Background Alt | Warm Linen | `#F3EDE4` | Alternate sections, subtle contrast |
| Text Primary | Charcoal Umber | `#2C2A26` | Body text, headings |
| Text Secondary | Warm Grey | `#6B6560` | Captions, secondary text, metadata |

### Accent Palette

| Role | Color Name | Hex | Usage |
|------|-----------|-----|-------|
| Primary Accent | French Blue | `#6B8EAE` | Links, buttons, key interactive elements |
| Secondary Accent | Dusty Sage | `#8E9E82` | Tags, badges, secondary highlights |
| Warm Accent | Terracotta | `#C47A5A` | Call-to-action buttons, alerts, warmth |
| Soft Accent | Lavender Mist | `#B8A9C9` | Decorative borders, hover states |
| Gold Accent | Antique Gold | `#C5A86A` | Ornamental details, icon highlights, dividers |

### Supporting Neutrals

| Role | Color Name | Hex | Usage |
|------|-----------|-----|-------|
| Stone | Pale Stone | `#E8E0D4` | Borders, dividers, card outlines |
| Warm White | Ivory | `#FFFEF9` | Modal backgrounds, overlays |
| Soft Pink | Dusky Rose | `#D4A9A0` | Subtle highlights, decorative flourishes |
| Muted Blue-Grey | Provincial Grey | `#B0ADA8` | Disabled states, muted elements |

### Extended Palette (Seasonal/Decorative)

| Color Name | Hex | Inspiration |
|-----------|-----|-------------|
| Sunflower Gold | `#E8C547` | Provencal sunflower fields |
| Burnt Rust | `#A85A3C` | Aged terracotta tiles |
| Olive Grove | `#7A7A52` | Southern French olive groves |
| Toile Blue | `#4E6E8E` | Classic blue-and-white toile fabric |
| Wisteria | `#9B8FBB` | Climbing wisteria on stone walls |
| Wheat | `#D9C9A5` | Harvested wheat fields |

## Typography

French Provincial typography should balance elegance with readability. Use high-contrast serif typefaces for headings that evoke classical French printing tradition, paired with clean, warm body fonts.

### Recommended Google Fonts

**Headings: Cormorant Garamond**
A refined display serif inspired by Claude Garamond's work. High contrast, elegant proportions, and a distinctly French character.

```
@import url('https://fonts.googleapis.com/css2?family=Cormorant+Garamond:ital,wght@0,300;0,400;0,500;0,600;0,700;1,300;1,400;1,500;1,600;1,700&display=swap');
```

**Subheadings: Playfair Display**
A transitional serif with refined contrast and sophisticated curves, ideal for pull quotes, subtitles, and display text.

```
@import url('https://fonts.googleapis.com/css2?family=Playfair+Display:ital,wght@0,400;0,500;0,600;0,700;1,400;1,500;1,600;1,700&display=swap');
```

**Body: Lora**
A contemporary serif rooted in calligraphy, optimized for screen reading. Warm and inviting with a subtle hand-crafted quality.

```
@import url('https://fonts.googleapis.com/css2?family=Lora:ital,wght@0,400;0,500;0,600;0,700;1,400;1,500;1,600;1,700&display=swap');
```

**Accent/Small Caps: EB Garamond**
For monograms, labels, small-caps navigation, or ornamental text that needs a classic French typographic feel.

```
@import url('https://fonts.googleapis.com/css2?family=EB+Garamond:ital,wght@0,400;0,500;0,600;0,700;1,400;1,500;1,600;1,700&display=swap');
```

**Script/Decorative (sparingly): Great Vibes**
For decorative initials, section dividers, or single-word flourishes. Use very sparingly to avoid kitsch.

```
@import url('https://fonts.googleapis.com/css2?family=Great+Vibes&display=swap');
```

### Type Scale

```css
:root {
  --font-heading: 'Cormorant Garamond', 'Georgia', serif;
  --font-subheading: 'Playfair Display', 'Georgia', serif;
  --font-body: 'Lora', 'Georgia', serif;
  --font-accent: 'EB Garamond', 'Georgia', serif;
  --font-script: 'Great Vibes', cursive;

  --text-xs: 0.75rem;      /* 12px - labels, fine print */
  --text-sm: 0.875rem;     /* 14px - captions, metadata */
  --text-base: 1rem;       /* 16px - body text */
  --text-lg: 1.125rem;     /* 18px - lead paragraphs */
  --text-xl: 1.375rem;     /* 22px - section intros */
  --text-2xl: 1.75rem;     /* 28px - section headings */
  --text-3xl: 2.25rem;     /* 36px - page headings */
  --text-4xl: 3rem;        /* 48px - hero headings */
  --text-5xl: 3.75rem;     /* 60px - display/decorative */

  --leading-tight: 1.2;
  --leading-normal: 1.6;
  --leading-relaxed: 1.8;

  --tracking-tight: -0.02em;
  --tracking-normal: 0;
  --tracking-wide: 0.05em;
  --tracking-widest: 0.12em;
}
```

## Layout Principles

### Symmetry and Balance
French Provincial design is fundamentally symmetrical. Center-align hero content, use evenly spaced grid columns, and maintain balanced whitespace on both sides.

### Generous Margins and Padding
Emulate the airy, spacious feel of provincial interiors with ample whitespace. Content should never feel cramped. Use at least 80-100px vertical section padding.

### Contained Content Width
Keep body content within a comfortable reading width (680-780px for text, 1100-1200px for full layouts) to maintain elegance and readability.

### Layered Depth
Create a sense of depth through subtle layering: soft box shadows, overlapping elements with slight offsets, and background textures that recede behind content.

### Focal Points
Every section should have a clear focal point, much like a fireplace mantel serves as the anchor of a provincial room. Use scale, color, or ornamentation to draw the eye.

### Grid Structure

```css
.provincial-grid {
  display: grid;
  grid-template-columns: repeat(12, 1fr);
  gap: 2rem;
  max-width: 1200px;
  margin: 0 auto;
  padding: 0 2rem;
}

/* Symmetrical two-column layout */
.provincial-two-col {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 3rem;
  align-items: center;
}

/* Content-centered single column */
.provincial-content {
  max-width: 720px;
  margin: 0 auto;
  padding: 0 1.5rem;
}
```

## CSS Implementation

### Design Tokens

```css
:root {
  /* Colors */
  --color-bg: #FAF6F0;
  --color-bg-alt: #F3EDE4;
  --color-text: #2C2A26;
  --color-text-secondary: #6B6560;
  --color-accent-blue: #6B8EAE;
  --color-accent-sage: #8E9E82;
  --color-accent-terracotta: #C47A5A;
  --color-accent-lavender: #B8A9C9;
  --color-accent-gold: #C5A86A;
  --color-stone: #E8E0D4;
  --color-ivory: #FFFEF9;
  --color-rose: #D4A9A0;
  --color-grey: #B0ADA8;

  /* Shadows */
  --shadow-sm: 0 1px 3px rgba(44, 42, 38, 0.06);
  --shadow-md: 0 4px 12px rgba(44, 42, 38, 0.08);
  --shadow-lg: 0 8px 30px rgba(44, 42, 38, 0.10);
  --shadow-soft: 0 2px 20px rgba(44, 42, 38, 0.05);

  /* Borders */
  --border-thin: 1px solid var(--color-stone);
  --border-ornamental: 2px solid var(--color-accent-gold);
  --radius-sm: 4px;
  --radius-md: 8px;
  --radius-lg: 16px;
  --radius-arch: 50% 50% 0 0;

  /* Transitions */
  --transition-gentle: all 0.3s ease;
  --transition-slow: all 0.5s ease;
}
```

### Base Styles

```css
*, *::before, *::after {
  box-sizing: border-box;
}

body {
  font-family: var(--font-body);
  font-size: var(--text-base);
  line-height: var(--leading-normal);
  color: var(--color-text);
  background-color: var(--color-bg);
  -webkit-font-smoothing: antialiased;
}

h1, h2, h3 {
  font-family: var(--font-heading);
  font-weight: 400;
  line-height: var(--leading-tight);
  letter-spacing: var(--tracking-tight);
  color: var(--color-text);
}

h1 { font-size: var(--text-4xl); }
h2 { font-size: var(--text-3xl); }
h3 { font-size: var(--text-2xl); }
h4 {
  font-family: var(--font-subheading);
  font-size: var(--text-xl);
  font-weight: 500;
}

p {
  margin-bottom: 1.5em;
  max-width: 68ch;
}

a {
  color: var(--color-accent-blue);
  text-decoration: none;
  border-bottom: 1px solid transparent;
  transition: var(--transition-gentle);
}

a:hover {
  border-bottom-color: var(--color-accent-blue);
}
```

### Card Component

```css
.provincial-card {
  background: var(--color-ivory);
  border: var(--border-thin);
  border-radius: var(--radius-md);
  padding: 2rem;
  box-shadow: var(--shadow-sm);
  transition: var(--transition-gentle);
}

.provincial-card:hover {
  box-shadow: var(--shadow-md);
  transform: translateY(-2px);
}

/* Card with arched image frame */
.provincial-card--arched .card-image {
  border-radius: var(--radius-arch);
  overflow: hidden;
  margin-bottom: 1.5rem;
}

.provincial-card--arched .card-image img {
  width: 100%;
  height: auto;
  display: block;
  object-fit: cover;
}
```

### Button Styles

```css
.btn-provincial {
  font-family: var(--font-accent);
  font-size: var(--text-sm);
  letter-spacing: var(--tracking-widest);
  text-transform: uppercase;
  padding: 0.875rem 2rem;
  border: 2px solid var(--color-accent-terracotta);
  background: transparent;
  color: var(--color-accent-terracotta);
  border-radius: var(--radius-sm);
  cursor: pointer;
  transition: var(--transition-gentle);
}

.btn-provincial:hover {
  background: var(--color-accent-terracotta);
  color: var(--color-ivory);
}

.btn-provincial--filled {
  background: var(--color-accent-terracotta);
  color: var(--color-ivory);
}

.btn-provincial--filled:hover {
  background: #A85A3C;
  border-color: #A85A3C;
}

.btn-provincial--gold {
  border-color: var(--color-accent-gold);
  color: var(--color-accent-gold);
}

.btn-provincial--gold:hover {
  background: var(--color-accent-gold);
  color: var(--color-ivory);
}
```

### Ornamental Divider

```css
.divider-ornamental {
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 1rem;
  margin: 3rem 0;
  color: var(--color-accent-gold);
}

.divider-ornamental::before,
.divider-ornamental::after {
  content: '';
  flex: 1;
  height: 1px;
  background: linear-gradient(
    to var(--direction, right),
    transparent,
    var(--color-accent-gold),
    transparent
  );
}

.divider-ornamental::before { --direction: right; }
.divider-ornamental::after { --direction: left; }

/* Fleur-de-lis or decorative symbol in center */
.divider-ornamental span {
  font-size: 1.25rem;
  opacity: 0.7;
}
```

### Toile-Inspired Background Pattern

```css
/* Subtle linen texture background */
.bg-linen {
  background-color: var(--color-bg);
  background-image:
    repeating-linear-gradient(
      0deg,
      transparent,
      transparent 2px,
      rgba(44, 42, 38, 0.015) 2px,
      rgba(44, 42, 38, 0.015) 4px
    ),
    repeating-linear-gradient(
      90deg,
      transparent,
      transparent 2px,
      rgba(44, 42, 38, 0.015) 2px,
      rgba(44, 42, 38, 0.015) 4px
    );
}

/* Decorative floral corner accents (using pseudo-elements) */
.provincial-frame {
  position: relative;
  padding: 3rem;
  border: 1px solid var(--color-stone);
}

.provincial-frame::before,
.provincial-frame::after {
  content: '';
  position: absolute;
  width: 40px;
  height: 40px;
  border-color: var(--color-accent-gold);
  border-style: solid;
}

.provincial-frame::before {
  top: 12px;
  left: 12px;
  border-width: 2px 0 0 2px;
}

.provincial-frame::after {
  bottom: 12px;
  right: 12px;
  border-width: 0 2px 2px 0;
}
```

### Arched Section Header

```css
.arch-header {
  text-align: center;
  padding: 4rem 2rem 3rem;
  position: relative;
}

.arch-header::before {
  content: '';
  position: absolute;
  top: 0;
  left: 50%;
  transform: translateX(-50%);
  width: 200px;
  height: 100px;
  border-radius: 100px 100px 0 0;
  border: 2px solid var(--color-stone);
  border-bottom: none;
}

.arch-header h2 {
  margin-bottom: 0.5rem;
}

.arch-header .subtitle {
  font-family: var(--font-accent);
  font-style: italic;
  color: var(--color-text-secondary);
  font-size: var(--text-lg);
  letter-spacing: var(--tracking-wide);
}
```

### Provincial Navigation

```css
.nav-provincial {
  display: flex;
  justify-content: center;
  align-items: center;
  gap: 2.5rem;
  padding: 1.25rem 0;
  border-top: 1px solid var(--color-stone);
  border-bottom: 1px solid var(--color-stone);
}

.nav-provincial a {
  font-family: var(--font-accent);
  font-size: var(--text-sm);
  letter-spacing: var(--tracking-widest);
  text-transform: uppercase;
  color: var(--color-text-secondary);
  text-decoration: none;
  border-bottom: none;
  position: relative;
  padding-bottom: 4px;
}

.nav-provincial a::after {
  content: '';
  position: absolute;
  bottom: 0;
  left: 50%;
  width: 0;
  height: 1px;
  background: var(--color-accent-gold);
  transition: var(--transition-gentle);
  transform: translateX(-50%);
}

.nav-provincial a:hover {
  color: var(--color-text);
}

.nav-provincial a:hover::after {
  width: 100%;
}
```

### Hero Section

```css
.hero-provincial {
  text-align: center;
  padding: 6rem 2rem;
  background: var(--color-bg-alt);
  position: relative;
  overflow: hidden;
}

.hero-provincial .overline {
  font-family: var(--font-accent);
  font-size: var(--text-sm);
  letter-spacing: var(--tracking-widest);
  text-transform: uppercase;
  color: var(--color-accent-gold);
  margin-bottom: 1rem;
  display: block;
}

.hero-provincial h1 {
  font-size: var(--text-5xl);
  font-weight: 300;
  margin-bottom: 1.5rem;
  max-width: 800px;
  margin-left: auto;
  margin-right: auto;
}

.hero-provincial .lead {
  font-family: var(--font-subheading);
  font-style: italic;
  font-size: var(--text-xl);
  color: var(--color-text-secondary);
  max-width: 600px;
  margin: 0 auto 2rem;
  line-height: var(--leading-relaxed);
}
```

### Blockquote / Pull Quote

```css
.quote-provincial {
  font-family: var(--font-subheading);
  font-style: italic;
  font-size: var(--text-xl);
  line-height: var(--leading-relaxed);
  color: var(--color-text-secondary);
  text-align: center;
  max-width: 640px;
  margin: 3rem auto;
  padding: 2rem 3rem;
  position: relative;
}

.quote-provincial::before {
  content: '\201C';
  font-family: var(--font-heading);
  font-size: 4rem;
  color: var(--color-accent-gold);
  position: absolute;
  top: -0.5rem;
  left: 0.5rem;
  line-height: 1;
  opacity: 0.6;
}

.quote-provincial cite {
  display: block;
  margin-top: 1rem;
  font-family: var(--font-accent);
  font-style: normal;
  font-size: var(--text-sm);
  letter-spacing: var(--tracking-wide);
  text-transform: uppercase;
  color: var(--color-grey);
}
```

### Image Presentation

```css
/* Arched image frame, mimicking provincial doorways */
.img-arch {
  border-radius: 50% 50% var(--radius-md) var(--radius-md);
  overflow: hidden;
  box-shadow: var(--shadow-md);
}

.img-arch img {
  width: 100%;
  height: 100%;
  object-fit: cover;
  display: block;
}

/* Framed image with ornamental border */
.img-framed {
  padding: 8px;
  border: 1px solid var(--color-stone);
  background: var(--color-ivory);
  box-shadow: var(--shadow-soft);
}

.img-framed img {
  width: 100%;
  display: block;
}

/* Image with gold ornamental caption bar */
.img-captioned figcaption {
  font-family: var(--font-accent);
  font-size: var(--text-sm);
  font-style: italic;
  color: var(--color-text-secondary);
  text-align: center;
  padding: 0.75rem 0;
  border-bottom: 1px solid var(--color-accent-gold);
  margin-top: 0.75rem;
}
```

### Scrollwork / Decorative SVG Motifs

```css
/* Use as section separators or decorative corners */
.scrollwork {
  display: block;
  margin: 2rem auto;
  width: 120px;
  height: auto;
  opacity: 0.3;
  fill: var(--color-accent-gold);
}

/* Fleur-de-lis accent */
.fleur::before {
  content: '\269C';  /* Unicode fleur-de-lis */
  display: inline-block;
  color: var(--color-accent-gold);
  font-size: 1.25em;
  margin: 0 0.5em;
  opacity: 0.6;
}
```

## Key Motifs and Patterns

### Floral and Botanical
Roses, lavender, wisteria, olive branches, sunflowers, and wildflowers. Use as subtle background patterns, section illustrations, or decorative corner elements. Prefer hand-drawn or watercolor styles over photorealistic renders.

### Toile de Jouy
The iconic French Provincial pattern featuring pastoral or floral scenes in a single color (traditionally blue, red, or sepia) on a cream/white ground. Use as a subtle background pattern at very low opacity, or for decorative borders and section dividers.

### Scrollwork and Flourishes
S-curves, acanthus leaves, and cabriole-inspired decorative elements. Apply to dividers, border treatments, and ornamental corner accents. Keep refined rather than heavy.

### Architectural Elements
Arched windows, symmetrical facades, rustic stone textures, wrought iron details. Translate into arched image frames, symmetrical layouts, stone-textured backgrounds, and thin ornamental line work.

### Fleur-de-lis
A subtle nod to French heritage. Use sparingly as an icon, bullet point, or section divider symbol.

## Design Do's and Don'ts

### Do
- Use a restrained, muted color palette with warm undertones
- Employ generous whitespace and balanced, symmetrical layouts
- Choose high-contrast serif typefaces with classical proportions
- Add subtle texture (linen, stone, paper grain) to backgrounds
- Use ornamental accents (gold dividers, scrollwork, arched frames) with restraint
- Let content breathe; prioritize readability and elegance
- Use soft, warm shadows rather than harsh drop shadows

### Don't
- Use bright, saturated, or neon colors
- Overcrowd layouts or use tight spacing
- Mix too many decorative fonts; keep ornamentation focused
- Use heavy, blocky sans-serif fonts for primary text
- Apply excessive ornamentation that competes with content
- Use stark white (#FFFFFF) as a background; always warm it up
- Use hard edges and sharp geometric shapes exclusively; soften with curves

## Responsive Considerations

- On mobile, reduce heading sizes by approximately 30% and increase line height for body text
- Stack two-column layouts into single columns below 768px
- Maintain generous vertical padding between sections even on mobile
- Arched image frames can simplify to standard rounded corners on small screens
- Navigation should collapse into a clean, centered hamburger menu with the same refined styling
- Ornamental dividers can be simplified or hidden on the smallest screens

## Related Aesthetics

- **Cottagecore** -- Shares the pastoral, rural charm and floral motifs but with a more whimsical, handmade quality
- **Country (French Country)** -- Overlaps significantly; French Provincial is the more refined, furniture-focused subset
- **Gustavian** -- Swedish interpretation of French styles with a cooler, more minimal Nordic palette
- **Grandmillennial** -- Modern revival of traditional and "granny chic" aesthetics, including chintz, toile, and antique styling
- **Shabby Chic** -- Shares the distressed, aged aesthetic and pastel palette but tends toward lighter, more faded treatments
- **Art Nouveau** -- Shares organic curves and floral motifs but with more dramatic, sinuous line work
- **Empire Style** -- A more formal, classical French aesthetic with heavier ornamentation and darker palettes
- **Baroque** -- Shares ornamental richness but at a much grander, more theatrical scale
