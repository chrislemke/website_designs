# Maximalism Design Reference

Maximalism is an aesthetic philosophy built on the principle **"more is more"** -- the deliberate embrace of excess, abundance, bold color, dense pattern, and layered ornamentation as a form of self-expression. It directly opposes minimalist restraint. The guiding concept is **horror vacui** (fear of empty space): every surface, every region of the composition should be filled with pattern, texture, color, or decorative detail. Drawing from historical movements like Baroque, Rococo, Victorian, and Gothic design, Maximalism celebrates **visual richness, clashing combinations, emotional intensity, and unapologetic exuberance**.

---

## Visual Characteristics

### Core Motifs and Patterns

- **Dense layered patterns** -- multiple prints, textures, and motifs stacked and overlapping simultaneously
- **Ornamental excess** -- elaborate borders, decorative fills, gilded accents, and embellishments on every surface
- **Mixed prints** -- florals, geometrics, animal prints, damask, paisley, and abstract patterns combined freely
- **Wallpaper-like repetition** -- rich repeating surface patterns covering entire backgrounds
- **Textile references** -- rugs, tapestries, brocade, velvet textures rendered as visual elements
- **Metallic accents** -- gold, bronze, copper, and chrome used generously for shimmer and opulence
- **Sculptural / three-dimensional ornamentation** -- elements that appear to project from the surface via shadows and depth
- **Mixed historical references** -- Baroque scrollwork, Rococo shells, Victorian filigree, Gothic tracery combined eclectically
- **Bold graphic elements** -- oversized typography, vivid illustrations, saturated photography
- **Clutter as composition** -- intentional visual density where "empty" space is treated as waste

### Design Principles

- **Horror vacui** -- fill every available space; negative space is the enemy
- **More is more** -- when in doubt, add another layer, pattern, or decorative element
- **Self-expression over restraint** -- personal, emotional, eclectic choices over curated minimalism
- **Experimentation** -- clash colors, mix periods, break conventional rules of harmony
- **Controlled chaos** -- abundance is intentional, not accidental; compositions should feel exuberant, not sloppy
- **Layered depth** -- multiple visual planes overlapping, creating dimensional richness
- **Exaggerated hierarchy** -- dramatically oversized headline text juxtaposed with much smaller body text
- **Pattern mixing** -- at least 2-3 different patterns visible in any given section
- **Saturated color throughout** -- no muted, desaturated palettes; everything is vivid and bold
- **Eclecticism** -- borrow freely from any era, culture, or style; coherence comes from commitment to abundance

---

## Color Palette

### Primary Scheme

| Role | Colors |
|------|--------|
| **Base / Backgrounds** | Deep jewel tones, saturated darks, or bold vivid backgrounds |
| **Primary accents** | Hot magenta, electric teal, burnished gold, vivid emerald |
| **Contrast / Energy** | Clashing complementaries and unexpected combinations |

### Full Palette

| Color | Hex (suggested) | Usage |
|-------|-----------------|-------|
| Deep Magenta | `#B60059`, `#D4145A` | Primary accent, headers, dramatic panels |
| Dark Forest Green | `#00522E`, `#1B4332` | Rich backgrounds, contrast panels |
| Golden Yellow | `#D5B800`, `#D4A017` | Metallic accents, borders, ornamental highlights |
| Teal / Cyan | `#00A1A1`, `#05878A` | Vibrant accent, links, secondary highlights |
| Deep Navy | `#06034D`, `#0A0A3E` | Dark backgrounds, depth layers |
| Ruby Red | `#9B1B30`, `#C41E3A` | Bold accent, call-to-action, dramatic elements |
| Amethyst Purple | `#5A175D`, `#7B2D8E` | Rich accent, decorative highlights, gradients |
| Sapphire Blue | `#074E67`, `#1A5276` | Cool contrast, information panels |
| Emerald Green | `#006B3C`, `#00875A` | Lush accent, nature motifs, secondary panels |
| Burnt Orange | `#CC5500`, `#E07020` | Warm accent, energy, playful elements |
| Hot Pink | `#FF1493`, `#FF69B4` | Pop accents, Gen Z Maximalism variant |
| Ivory / Cream | `#FFF8E7`, `#FFFFF0` | Light text on dark backgrounds, relief areas |
| Rich Black | `#0A0A0A`, `#1A1009` | Deepest backgrounds, shadow areas |

### Suggested CSS Custom Properties

```css
:root {
  /* Base */
  --max-black: #0a0a0a;
  --max-dark-navy: #06034d;
  --max-forest: #00522e;
  --max-ivory: #fff8e7;
  --max-cream: #fffff0;

  /* Jewel Tones */
  --max-magenta: #b60059;
  --max-ruby: #9b1b30;
  --max-amethyst: #5a175d;
  --max-sapphire: #074e67;
  --max-emerald: #006b3c;
  --max-teal: #00a1a1;

  /* Warm Accents */
  --max-gold: #d5b800;
  --max-gold-burnished: #d4a017;
  --max-orange: #cc5500;
  --max-hot-pink: #ff1493;

  /* Extended Brights */
  --max-electric-blue: #0066ff;
  --max-vivid-red: #e60023;
  --max-lime: #a4c639;
  --max-violet: #8b00ff;

  /* Functional */
  --max-bg-primary: var(--max-dark-navy);
  --max-bg-secondary: var(--max-forest);
  --max-bg-accent: var(--max-magenta);
  --max-text-primary: var(--max-ivory);
  --max-text-accent: var(--max-gold);
  --max-border-primary: var(--max-gold);
  --max-border-accent: var(--max-teal);
}
```

### Color Approaches

- **Jewel tone foundation** -- emerald, sapphire, ruby, amethyst as primary palette, inspired by precious stones; creates opulent depth
- **Clashing complementaries** -- magenta + teal, orange + navy, purple + gold; unexpected pairings that vibrate with energy
- **Rainbow saturation** -- all hues welcome, saturated to maximum; avoid pastels and muted tones
- **Metallic through-line** -- gold, bronze, or chrome accents unify otherwise chaotic palettes
- **Dark base, vivid overlay** -- deep navy or black backgrounds allow jewel tones and brights to pop dramatically
- **No color is off-limits** -- the only rule is saturation; every color should be turned up to full intensity

---

## Typography

### Typeface Characteristics

Maximalist typography features:

- **Exaggerated scale contrast** -- dramatically oversized display text (headline) juxtaposed with small body text
- **Ornate serif display faces** -- high-contrast, decorative serifs for impact headings
- **Mixed typeface families** -- combine serif, sans-serif, script, and display in a single composition
- **Decorative / swash capitals** -- flourishes, ligatures, and ornamental letterforms
- **Bold weights by default** -- regular weight is the exception, not the rule
- **Layered text effects** -- shadows, outlines, gradients, textures applied to type
- **Variable sizing** -- text at many different scales within the same section
- **Pattern-filled or gradient type** -- text as a vessel for additional visual information

### Recommended Web Fonts (Google Fonts)

| Font | Style | Usage |
|------|-------|-------|
| **Playfair Display** | High-contrast transitional serif | Display headlines, dramatic titles |
| **Abril Fatface** | Bold 19th-century display serif | Hero text, oversized headings |
| **Cinzel Decorative** | Ornamental Roman capitals | Feature titles, section openers |
| **Lobster** | Bold connected script | Playful accent headings |
| **Cormorant Garamond** | Elegant old-style serif | Subheadings, refined body text |
| **Libre Baskerville** | Refined transitional serif | Body copy, readable text |
| **Montserrat** | Geometric sans-serif | Body text, UI elements, contrast against serifs |
| **Great Vibes** | Calligraphic script | Decorative accents, quotes |
| **Permanent Marker** | Hand-drawn display | Informal accents, Gen Z Maximalism variant |
| **Bungee** | Chromatic display | Bold block headings, layered color effects |
| **Righteous** | Retro display | Energetic, pop-culture headings |

### Typography CSS Example

```css
/* Display / Hero text -- oversized, ornate, layered */
.max-hero-text {
  font-family: 'Abril Fatface', 'Playfair Display', serif;
  font-size: clamp(4rem, 12vw, 10rem);
  letter-spacing: -0.02em;
  line-height: 0.95;
  background: linear-gradient(
    135deg,
    var(--max-magenta),
    var(--max-gold),
    var(--max-teal),
    var(--max-amethyst)
  );
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  background-clip: text;
  text-shadow: none; /* required when using background-clip */
}

/* Section headings -- bold, vivid */
h1, h2, h3 {
  font-family: 'Playfair Display', 'Cinzel Decorative', serif;
  font-weight: 900;
  letter-spacing: 0.03em;
  color: var(--max-gold);
  text-shadow:
    3px 3px 0px var(--max-magenta),
    6px 6px 0px rgba(0, 0, 0, 0.3);
}

/* Body text -- readable but still characterful */
body {
  font-family: 'Montserrat', 'Libre Baskerville', sans-serif;
  font-weight: 400;
  font-size: 1rem;
  letter-spacing: 0.01em;
  line-height: 1.7;
  color: var(--max-ivory);
}

/* Script accent -- for decorative labels, quotes */
.max-script {
  font-family: 'Great Vibes', 'Lobster', cursive;
  font-size: 2em;
  color: var(--max-hot-pink);
  text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.5);
}

/* Exaggerated hierarchy -- tiny caption under massive heading */
.max-caption {
  font-family: 'Montserrat', sans-serif;
  font-size: 0.65rem;
  text-transform: uppercase;
  letter-spacing: 0.3em;
  color: var(--max-teal);
}
```

---

## Layout Principles

### Grid and Structure

- **No negative space** -- fill the viewport; backgrounds, patterns, and content should cover every pixel
- **Asymmetric, organic layouts** -- avoid rigid symmetry; let content flow dynamically and overlap
- **Layered, overlapping elements** -- cards, images, and text blocks that partially cover one another
- **Multiple column widths** -- vary grid columns within a single page; mix full-width, narrow, and offset sections
- **Dense content grids** -- tightly packed masonry or collage-style arrangements
- **Full-bleed backgrounds** -- every section has its own bold background color or pattern
- **Mixed media zones** -- combine images, illustrations, patterns, and typography in the same visual area
- **Broken grid** -- elements that intentionally break out of grid lines for energetic, unpredictable composition

### Section Organization

- Use **bold, contrasting section backgrounds** -- each section should feel like a different room
- Apply **ornate dividers** between sections (decorative borders, pattern strips, colored bands)
- Create **overwhelming hero sections** -- oversized type, layered patterns, multiple visual elements stacked
- Employ **collage-style containers** -- overlapping cards, rotated elements, varied border styles
- Use **pattern borders and fills** -- stripes, dots, zigzags, chevrons as section boundaries
- Mix **full-width and contained sections** -- some content bleeds edge to edge, some is boxed
- Apply **generous decoration to every container** -- borders, shadows, gradients, corner ornaments, background patterns

---

## CSS/Design Techniques

### Multi-Pattern Layered Background

```css
/* Stack multiple patterns using CSS gradients */
.max-pattern-bg {
  background-color: var(--max-dark-navy);
  background-image:
    /* Diagonal stripes */
    repeating-linear-gradient(
      45deg,
      transparent,
      transparent 20px,
      rgba(182, 0, 89, 0.08) 20px,
      rgba(182, 0, 89, 0.08) 22px
    ),
    /* Polka dots */
    radial-gradient(
      circle 8px at 30px 30px,
      rgba(213, 184, 0, 0.1) 0%,
      transparent 100%
    ),
    /* Large radial glow */
    radial-gradient(
      ellipse at 50% 50%,
      rgba(0, 161, 161, 0.1) 0%,
      transparent 60%
    );
  background-size: 40px 40px, 60px 60px, 100% 100%;
}
```

### Ornate Multi-Border Frame

```css
/* Layered borders for maximalist framing */
.max-frame {
  border: 4px solid var(--max-gold);
  outline: 3px solid var(--max-magenta);
  outline-offset: 6px;
  box-shadow:
    0 0 0 12px var(--max-dark-navy),
    0 0 0 15px var(--max-teal),
    0 8px 32px rgba(0, 0, 0, 0.5);
  padding: 2.5rem;
  position: relative;
}

/* Corner flourishes */
.max-frame::before,
.max-frame::after {
  content: '\2726'; /* four-pointed star */
  position: absolute;
  font-size: 1.8rem;
  color: var(--max-gold);
  text-shadow: 0 0 8px rgba(213, 184, 0, 0.5);
}

.max-frame::before {
  top: -16px;
  left: -16px;
}

.max-frame::after {
  bottom: -16px;
  right: -16px;
  transform: rotate(45deg);
}
```

### Bold Gradient Cards

```css
.max-card {
  background: linear-gradient(
    135deg,
    var(--max-magenta) 0%,
    var(--max-amethyst) 50%,
    var(--max-dark-navy) 100%
  );
  border: 3px solid var(--max-gold);
  border-radius: 0; /* sharp corners for impact */
  padding: 2rem;
  position: relative;
  overflow: hidden;
  box-shadow:
    8px 8px 0px var(--max-teal),
    16px 16px 0px rgba(0, 0, 0, 0.3);
  transition: transform 0.3s ease, box-shadow 0.3s ease;
}

.max-card:hover {
  transform: translate(-4px, -4px);
  box-shadow:
    12px 12px 0px var(--max-teal),
    20px 20px 0px rgba(0, 0, 0, 0.3);
}

/* Internal pattern overlay */
.max-card::before {
  content: '';
  position: absolute;
  inset: 0;
  background: repeating-linear-gradient(
    -45deg,
    transparent,
    transparent 10px,
    rgba(255, 255, 255, 0.03) 10px,
    rgba(255, 255, 255, 0.03) 12px
  );
  pointer-events: none;
}
```

### Collage / Overlapping Layout

```css
/* Overlapping grid for collage effect */
.max-collage {
  display: grid;
  grid-template-columns: repeat(12, 1fr);
  grid-auto-rows: 80px;
  gap: 0;
  padding: 2rem;
}

.max-collage-item:nth-child(1) {
  grid-column: 1 / 7;
  grid-row: 1 / 5;
  z-index: 1;
  transform: rotate(-2deg);
}

.max-collage-item:nth-child(2) {
  grid-column: 5 / 11;
  grid-row: 2 / 6;
  z-index: 2;
  transform: rotate(1.5deg);
}

.max-collage-item:nth-child(3) {
  grid-column: 8 / 13;
  grid-row: 1 / 4;
  z-index: 3;
  transform: rotate(-1deg);
}

.max-collage-item {
  border: 3px solid var(--max-gold);
  box-shadow: 4px 4px 0px var(--max-magenta);
  overflow: hidden;
}
```

### Exaggerated Typography Hierarchy

```css
/* Massive heading with tiny subtitle */
.max-heading-group {
  text-align: center;
  padding: 4rem 2rem;
}

.max-heading-group h1 {
  font-family: 'Abril Fatface', serif;
  font-size: clamp(5rem, 15vw, 12rem);
  line-height: 0.9;
  margin: 0;
  background: linear-gradient(
    180deg,
    var(--max-gold) 0%,
    var(--max-magenta) 50%,
    var(--max-teal) 100%
  );
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  background-clip: text;
}

.max-heading-group .subtitle {
  font-family: 'Montserrat', sans-serif;
  font-size: 0.6rem;
  text-transform: uppercase;
  letter-spacing: 0.5em;
  color: var(--max-teal);
  margin-top: 1rem;
}
```

### Animated Pattern Border

```css
/* Moving gradient border using background animation */
.max-animated-border {
  --border-width: 4px;
  position: relative;
  background: var(--max-dark-navy);
  padding: 2rem;
}

.max-animated-border::before {
  content: '';
  position: absolute;
  inset: 0;
  padding: var(--border-width);
  background: linear-gradient(
    90deg,
    var(--max-magenta),
    var(--max-gold),
    var(--max-teal),
    var(--max-amethyst),
    var(--max-ruby),
    var(--max-magenta)
  );
  background-size: 300% 100%;
  -webkit-mask:
    linear-gradient(#fff 0 0) content-box,
    linear-gradient(#fff 0 0);
  -webkit-mask-composite: xor;
  mask-composite: exclude;
  animation: max-border-flow 4s linear infinite;
}

@keyframes max-border-flow {
  0% { background-position: 0% 50%; }
  100% { background-position: 300% 50%; }
}
```

### Maximalist Divider / Section Break

```css
/* Bold multi-colored divider strip */
.max-divider {
  height: 8px;
  border: none;
  margin: 0;
  background: linear-gradient(
    90deg,
    var(--max-magenta) 0%,
    var(--max-gold) 20%,
    var(--max-teal) 40%,
    var(--max-amethyst) 60%,
    var(--max-ruby) 80%,
    var(--max-emerald) 100%
  );
}

/* Ornamental pattern strip */
.max-pattern-strip {
  height: 40px;
  background:
    repeating-linear-gradient(
      90deg,
      var(--max-magenta) 0px,
      var(--max-magenta) 20px,
      var(--max-gold) 20px,
      var(--max-gold) 40px,
      var(--max-teal) 40px,
      var(--max-teal) 60px,
      var(--max-amethyst) 60px,
      var(--max-amethyst) 80px
    );
}
```

### Dense Background Texture Overlay

```css
/* Noise-like texture for visual richness */
.max-texture {
  position: relative;
}

.max-texture::after {
  content: '';
  position: absolute;
  inset: 0;
  background-image: url("data:image/svg+xml,%3Csvg width='6' height='6' xmlns='http://www.w3.org/2000/svg'%3E%3Ccircle cx='1' cy='1' r='0.6' fill='%23ffffff' opacity='0.04'/%3E%3Ccircle cx='4' cy='4' r='0.4' fill='%23d5b800' opacity='0.03'/%3E%3C/svg%3E");
  pointer-events: none;
}

/* Damask-inspired SVG pattern overlay */
.max-damask {
  background-color: var(--max-dark-navy);
  background-image: url("data:image/svg+xml,%3Csvg width='40' height='40' xmlns='http://www.w3.org/2000/svg'%3E%3Cpath d='M20 0 L40 20 L20 40 L0 20 Z' fill='none' stroke='%23d5b800' stroke-width='0.5' opacity='0.06'/%3E%3Ccircle cx='20' cy='20' r='3' fill='none' stroke='%23b60059' stroke-width='0.4' opacity='0.05'/%3E%3C/svg%3E");
}
```

---

## Materials and Textures (Visual Metaphors for Web)

Physical Maximalist materials and their web equivalents:

| Physical Material | Web Equivalent |
|-------------------|----------------|
| Layered textiles (rugs, tapestries, brocade) | Stacked CSS gradient patterns, repeating SVG backgrounds |
| Gold leaf / Gilding | Warm gold gradients (`#D5B800` to `#D4A017`), metallic text effects |
| Velvet and damask | Deep jewel-tone backgrounds with subtle pattern overlays |
| Mixed printed fabrics | Multiple `background-image` layers with different pattern types |
| Lacquered surfaces | High-contrast glossy gradients with bright highlights |
| Mosaic and tile | CSS grid or repeating patterns with many small colored cells |
| Wallpaper | Full-coverage repeating CSS patterns, no exposed base color |
| Stained glass | Vivid, saturated color blocks with dark borders (box-shadow, outline) |
| Embroidery and beadwork | Small, detailed SVG pattern elements with metallic colors |
| Collaged paper and ephemera | Overlapping rotated containers, mixed border styles, varied backgrounds |

---

## Sub-Styles and Variants

### Gen Z Maximalism
- **Hyper-saturated rainbow palette** -- every color at full saturation, deliberate clashing
- **Memphis Design influences** -- geometric shapes, bold primary colors, squiggly lines
- **Digital-native patterns** -- emojis, pixel art, gradient meshes, sticker-like elements
- **TikTok/Instagram aesthetic** -- designed for screens, quick visual impact
- **Kidcore and Decora crossover** -- playful, youth-oriented, accessory-heavy
- Suggested accents: `#FF1493` (hot pink), `#00BFFF` (deep sky blue), `#FFD700` (gold), `#FF4500` (orange red), `#7FFF00` (chartreuse)

### Grandmillennial Maximalism
- **Chintz florals and toile** -- traditional prints in dense, layered arrangements
- **Warm, muted jewel tones** -- slightly desaturated compared to pure Maximalism
- **Vintage and antique references** -- needlepoint, porcelain, wallpaper, lace
- **Curated clutter** -- abundance that feels inherited rather than chaotic

### Hollywood Regency Maximalism
- **Glamorous, high-contrast palette** -- black, white, gold, emerald, hot pink
- **Lacquer and mirror finishes** -- glossy, reflective surfaces
- **Bold geometric patterns** -- Greek key, chevrons, sunbursts
- **Luxury signifiers** -- velvet, crystal, brass, marble textures

### Mob Wife / Opulent Maximalism
- **Dark, rich palette** -- burgundy, gold, leopard print, black, deep red
- **Animal prints** -- leopard, zebra, snakeskin as core pattern elements
- **Heavy metallic gold** -- dominant accent color, applied generously
- **Baroque and Rococo ornament** -- scrollwork, cherubs, ornate frames

---

## Related Aesthetics

| Aesthetic | Relationship to Maximalism |
|-----------|---------------------------|
| **Minimalism** | Direct opposite; Maximalism exists as a rejection of minimalist restraint |
| **Baroque** | Historical ancestor; shares horror vacui, gilded ornament, dramatic intensity |
| **Rococo** | Historical ancestor; lighter, more playful ornamental excess |
| **Camp** | Overlapping sensibility; both celebrate exaggeration, artifice, and theatricality |
| **Cluttercore** | Modern variant; celebrates material abundance and collected objects |
| **Dopamine Dressing** | Overlapping concept; uses bold color and pattern for emotional stimulation |
| **Avant Basic** | Contemporary variant; maximalism applied to trendy, accessible fashion and decor |
| **Gen Z Maximalism** | Youth-oriented digital variant; hyper-saturated, screen-native, meme-influenced |
| **Grandmillennial** | Curated, vintage-inflected variant; traditional patterns in dense arrangements |
| **Hollywood Regency** | Glamorous, high-contrast variant; luxury and drama in black/white/gold |
| **Mob Wife** | Dark, opulent variant; animal prints, gold, baroque ornament |
| **Grocery Girl Fall** | Niche seasonal variant; maximalist layering applied to cozy fall aesthetics |
| **Victorian** | Historical parallel; shared love of ornament, pattern, and filled surfaces |
| **Gothic** | Shares dramatic intensity and ornamental excess, but in darker palette |
| **Chinoiserie** | Historical decorative style often incorporated into maximalist compositions |
| **Memphis Design** | 1980s movement sharing bold color, geometric pattern, and anti-minimalism |

---

## Quick-Start: Minimal Maximalism Page Template

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Maximalism Page</title>
  <link href="https://fonts.googleapis.com/css2?family=Abril+Fatface&family=Playfair+Display:wght@700;900&family=Montserrat:wght@400;700&family=Great+Vibes&display=swap" rel="stylesheet">
  <style>
    :root {
      --max-black: #0a0a0a;
      --max-dark-navy: #06034d;
      --max-magenta: #b60059;
      --max-gold: #d5b800;
      --max-teal: #00a1a1;
      --max-amethyst: #5a175d;
      --max-ruby: #9b1b30;
      --max-emerald: #006b3c;
      --max-ivory: #fff8e7;
    }

    * { margin: 0; padding: 0; box-sizing: border-box; }

    body {
      background: var(--max-dark-navy);
      color: var(--max-ivory);
      font-family: 'Montserrat', sans-serif;
      font-size: 1rem;
      line-height: 1.7;
    }

    /* Hero -- overwhelming, layered, dense */
    .hero {
      text-align: center;
      padding: 6rem 2rem;
      position: relative;
      overflow: hidden;
      background:
        repeating-linear-gradient(
          45deg,
          transparent,
          transparent 20px,
          rgba(182, 0, 89, 0.06) 20px,
          rgba(182, 0, 89, 0.06) 22px
        ),
        radial-gradient(
          ellipse at 30% 50%,
          rgba(0, 161, 161, 0.15) 0%,
          transparent 50%
        ),
        radial-gradient(
          ellipse at 70% 30%,
          rgba(213, 184, 0, 0.12) 0%,
          transparent 50%
        ),
        var(--max-dark-navy);
    }

    .hero h1 {
      font-family: 'Abril Fatface', serif;
      font-size: clamp(4rem, 12vw, 10rem);
      line-height: 0.95;
      background: linear-gradient(
        135deg,
        var(--max-magenta),
        var(--max-gold),
        var(--max-teal)
      );
      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent;
      background-clip: text;
    }

    .hero .subtitle {
      font-family: 'Montserrat', sans-serif;
      font-size: 0.65rem;
      text-transform: uppercase;
      letter-spacing: 0.5em;
      color: var(--max-teal);
      margin-top: 1.5rem;
    }

    /* Bold gradient divider */
    .max-divider {
      height: 6px;
      border: none;
      background: linear-gradient(
        90deg,
        var(--max-magenta),
        var(--max-gold),
        var(--max-teal),
        var(--max-amethyst),
        var(--max-ruby),
        var(--max-emerald)
      );
    }

    /* Content section with pattern background */
    section {
      max-width: 1000px;
      margin: 0 auto;
      padding: 4rem 2rem;
    }

    h2 {
      font-family: 'Playfair Display', serif;
      font-weight: 900;
      font-size: 2.5rem;
      color: var(--max-gold);
      text-shadow:
        3px 3px 0px var(--max-magenta),
        6px 6px 0px rgba(0, 0, 0, 0.2);
      margin-bottom: 1.5rem;
    }

    /* Maximalist card with offset shadow and pattern */
    .max-card {
      background: linear-gradient(
        135deg,
        var(--max-magenta) 0%,
        var(--max-amethyst) 100%
      );
      border: 3px solid var(--max-gold);
      padding: 2rem;
      margin: 2rem 0;
      position: relative;
      box-shadow:
        8px 8px 0px var(--max-teal),
        16px 16px 0px rgba(0, 0, 0, 0.3);
    }

    .max-card::before {
      content: '';
      position: absolute;
      inset: 0;
      background: repeating-linear-gradient(
        -45deg,
        transparent,
        transparent 10px,
        rgba(255, 255, 255, 0.03) 10px,
        rgba(255, 255, 255, 0.03) 12px
      );
      pointer-events: none;
    }

    /* Decorative script accent */
    .script-accent {
      font-family: 'Great Vibes', cursive;
      font-size: 2em;
      color: var(--max-gold);
    }
  </style>
</head>
<body>
  <div class="hero">
    <h1>Title Here</h1>
    <p class="subtitle">A subtitle in tracked-out Montserrat</p>
  </div>
  <hr class="max-divider">
  <section>
    <h2>Section Heading</h2>
    <div class="max-card">
      <p>Content within a boldly styled Maximalist panel.
         Every surface is filled. Every color is vivid.
         More is more.</p>
    </div>
    <p class="script-accent">Ornamental accent text</p>
  </section>
</body>
</html>
```
