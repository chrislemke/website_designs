# Cluttercore Design Reference

Cluttercore is a maximalist interior and lifestyle aesthetic that emerged on TikTok around 2020, gaining traction during the COVID-19 pandemic. It celebrates the **"beautiful mess"** -- densely curated, deeply personal spaces where every surface becomes a display canvas for collections, memorabilia, and sentimental objects. Unlike traditional maximalism, which aims for bold but *cohesive* design, Cluttercore prioritizes **emotional resonance and personal expression** over aesthetic harmony, creating spaces that feel organically evolved and intimately lived-in.

---

## Visual Characteristics

### Core Motifs and Patterns

- **Dense, layered collections** -- books, figurines, vintage cameras, trinkets, and curiosities filling every shelf and surface
- **Gallery walls** -- walls comprehensively covered with art, photographs, postcards, prints in mismatched frames
- **Overflowing bookshelves** -- books stacked horizontally, vertically, and double-layered with objects tucked between them
- **Abundant houseplants** -- trailing vines, potted succulents, and hanging planters woven through the clutter
- **Mixed textiles and patterns** -- layered fabrics combining florals, plaids, geometric prints, and ethnic patterns with no concern for matching
- **Eclectic, mismatched furniture** -- antique dressers next to modern shelving next to thrifted side tables
- **Sentimental objects as decor** -- travel souvenirs, inherited items, childhood keepsakes prominently displayed
- **Blank walls are rare** -- every vertical and horizontal surface serves as a curated display area

### Design Principles

- **Intentional accumulation** -- the clutter is curated, not careless; every object tells a story
- **Personal narrative over design rules** -- spaces reflect the inhabitant's journey, passions, and memories
- **Chromatic diversity** -- highly saturated and varied colors coexist without a unifying scheme
- **Textural richness** -- velvet, wool, wicker, ceramic, brass, wood, and paper layered together
- **Warmth and comfort** -- the overall effect should feel like an "emotional security blanket"
- **Organic arrangement** -- objects are grouped by meaning or association rather than visual symmetry
- **Visual density with navigable paths** -- packed spaces that still feel inviting, not claustrophobic
- **Nostalgia and authenticity** -- handmade, vintage, and well-worn items valued over new and pristine

---

## Color Palette

### Primary Scheme

| Role | Colors |
|------|--------|
| **Base / Background** | Warm cream, aged paper, soft ivory |
| **Warm accents** | Terracotta, mustard yellow, burnt orange, dusty rose |
| **Cool accents** | Teal, sage green, periwinkle blue, plum purple |
| **Rich tones** | Burgundy, forest green, navy blue, ochre |
| **Bright pops** | Cherry red, sunflower yellow, cobalt blue, magenta |

### Detailed Palette

| Color | Hex (suggested) | Usage |
|-------|-----------------|-------|
| Warm Cream | `#F5F0E6`, `#FFF8EE` | Primary background, base surface |
| Aged Paper | `#EDE4D3`, `#E8DCCA` | Secondary backgrounds, card surfaces |
| Terracotta | `#C8614C`, `#D4735E` | Primary warm accent, highlights |
| Mustard Yellow | `#D4A843`, `#E5B94E` | Accent elements, badges, tags |
| Sage Green | `#8DA47E`, `#9BB08E` | Nature/plant accents, secondary elements |
| Dusty Rose | `#C48B8B`, `#D1A0A0` | Soft warm accent, borders, hover states |
| Teal | `#3D8B8B`, `#4A9E9E` | Cool accent, links, interactive elements |
| Plum Purple | `#7B5078`, `#8E6088` | Feature accents, headings |
| Burgundy | `#803040`, `#943A4A` | Deep accent, emphasis text |
| Forest Green | `#2E5E3E`, `#3A7050` | Rich accent, section backgrounds |
| Burnt Orange | `#CC6B30`, `#D87A3E` | Call-to-action, warm highlight |
| Navy | `#2A3A5C`, `#354770` | Dark accent, contrast backgrounds |
| Cobalt Blue | `#2E5BA8`, `#3A6CBC` | Bright pop accent |
| Cherry Red | `#B83240`, `#CC3D4C` | Bright pop accent |
| Rich Brown | `#5C3D2E`, `#6B4A3A` | Borders, frames, grounding color |

### Suggested CSS Custom Properties

```css
:root {
  /* Warm base tones */
  --clutter-cream: #f5f0e6;
  --clutter-ivory: #fff8ee;
  --clutter-paper: #ede4d3;
  --clutter-parchment: #e8dcca;

  /* Warm accents */
  --clutter-terracotta: #c8614c;
  --clutter-mustard: #d4a843;
  --clutter-burnt-orange: #cc6b30;
  --clutter-dusty-rose: #c48b8b;

  /* Cool accents */
  --clutter-teal: #3d8b8b;
  --clutter-sage: #8da47e;
  --clutter-periwinkle: #7080b8;
  --clutter-plum: #7b5078;

  /* Rich / deep tones */
  --clutter-burgundy: #803040;
  --clutter-forest: #2e5e3e;
  --clutter-navy: #2a3a5c;
  --clutter-brown: #5c3d2e;

  /* Bright pops */
  --clutter-cherry: #b83240;
  --clutter-cobalt: #2e5ba8;
  --clutter-sunflower: #e5c040;
  --clutter-magenta: #b8388e;

  /* Functional mappings */
  --clutter-bg-primary: var(--clutter-cream);
  --clutter-bg-secondary: var(--clutter-paper);
  --clutter-bg-card: var(--clutter-ivory);
  --clutter-text-primary: var(--clutter-brown);
  --clutter-text-secondary: #6b5a4a;
  --clutter-text-heading: var(--clutter-burgundy);
  --clutter-accent: var(--clutter-teal);
  --clutter-accent-warm: var(--clutter-terracotta);
  --clutter-border: var(--clutter-dusty-rose);
  --clutter-link: var(--clutter-teal);
  --clutter-link-hover: var(--clutter-plum);
}
```

### Approaches

- **No single dominant color** -- embrace chromatic variety; each section or card can have its own accent
- **Warm neutral base with saturated pops** -- cream/paper backgrounds keep the density from feeling heavy
- **Random-feeling but curated palette** -- colors should feel collected over time, not chosen from a single swatch
- **Earthy warmth as the unifying thread** -- even bright pops are slightly muted or warm-shifted
- **High saturation tolerance** -- colors that would clash in minimalist design feel natural here

---

## Typography

### Typeface Characteristics

Cluttercore typography reflects its eclectic, personal, handmade ethos:

- **Mix of typeface styles** -- a serif heading with a handwritten accent and a clean body font is perfectly appropriate
- **Warm, characterful serifs** -- not cold or corporate; think vintage book typography
- **Handwritten or script accents** -- labels, annotations, and decorative text
- **Rounded, friendly sans-serifs for body text** -- approachable and readable
- **Varied weights and sizes** -- visual hierarchy through deliberate typographic contrast
- **Slight imperfection is a feature** -- decorative or quirky letterforms over geometric precision

### Recommended Web Fonts (Google Fonts / Free)

| Font | Style | Usage |
|------|-------|-------|
| **Playfair Display** | Elegant, high-contrast serif | Headlines, section titles |
| **Lora** | Warm, calligraphic serif | Subheadings, pull quotes |
| **Merriweather** | Sturdy, readable serif | Body text alternative |
| **Nunito** | Rounded, friendly sans-serif | Body text, UI elements |
| **Quicksand** | Rounded geometric sans-serif | Labels, navigation, tags |
| **Caveat** | Handwritten, natural | Annotations, decorative labels, captions |
| **Patrick Hand** | Handwritten, casual | Accent text, callouts |
| **Crimson Pro** | Classic, book-style serif | Long-form body text |
| **Indie Flower** | Handwritten, whimsical | Decorative accents, stickers |
| **DM Serif Display** | Bold, characterful display serif | Hero headlines |

### Typography CSS Example

```css
/* Headlines -- characterful serif */
h1, h2, h3 {
  font-family: 'Playfair Display', 'DM Serif Display', Georgia, serif;
  font-weight: 700;
  color: var(--clutter-text-heading);
  line-height: 1.2;
}

h1 { font-size: clamp(2.2rem, 5vw, 4rem); }
h2 { font-size: clamp(1.6rem, 3.5vw, 2.5rem); }
h3 { font-size: clamp(1.2rem, 2.5vw, 1.8rem); }

/* Body text -- friendly, rounded */
body {
  font-family: 'Nunito', 'Quicksand', sans-serif;
  font-weight: 400;
  font-size: 1rem;
  line-height: 1.7;
  color: var(--clutter-text-primary);
}

/* Handwritten accent text */
.clutter-handwritten {
  font-family: 'Caveat', 'Patrick Hand', cursive;
  font-size: 1.3em;
  color: var(--clutter-terracotta);
  transform: rotate(-2deg);
  display: inline-block;
}

/* Labels and tags */
.clutter-tag {
  font-family: 'Quicksand', 'Nunito', sans-serif;
  font-size: 0.75rem;
  font-weight: 600;
  text-transform: uppercase;
  letter-spacing: 0.08em;
  color: var(--clutter-text-secondary);
}

/* Decorative pull quote */
.clutter-quote {
  font-family: 'Lora', 'Crimson Pro', serif;
  font-style: italic;
  font-size: 1.4rem;
  line-height: 1.5;
  color: var(--clutter-plum);
  border-left: 4px solid var(--clutter-dusty-rose);
  padding-left: 1.5rem;
}
```

---

## Layout Principles

### Grid and Structure

- **Asymmetric, organic grid layouts** -- avoid rigid symmetry; let elements feel casually placed
- **CSS Grid with varied track sizes** -- columns and rows of different widths to avoid uniformity
- **Masonry-style arrangements** -- items of different heights packed together like a shelf display
- **Overlapping elements** -- slight overlaps between cards, images, and decorative elements
- **No excessive whitespace** -- surfaces should feel populated, but not unreadable
- **Multiple visual layers** -- background textures, mid-ground content, foreground decorative elements
- **Rotated and tilted elements** -- slight rotations (1-3 degrees) on cards or images, like pinned photos

### Section Organization

- Use **varied section backgrounds** -- alternate between cream, soft colored washes, and textured panels
- Apply **decorative borders** -- hand-drawn style borders, dotted lines, washi-tape motifs
- Create **hierarchy through size and color variety** rather than strict geometric alignment
- Employ **rounded and irregular shapes** for containers -- not everything needs to be a rectangle
- Use **sticker-like labels and annotations** -- scattered decorative elements that break the grid
- Incorporate **shelf and pinboard metaphors** -- sections that look like physical display surfaces

---

## CSS/Design Techniques

### Warm Textured Background

```css
/* Aged paper / cream background with subtle texture */
.clutter-bg {
  background-color: var(--clutter-cream);
  background-image:
    radial-gradient(
      ellipse at 20% 50%,
      rgba(212, 168, 67, 0.06) 0%,
      transparent 50%
    ),
    radial-gradient(
      ellipse at 80% 20%,
      rgba(141, 164, 126, 0.06) 0%,
      transparent 50%
    ),
    radial-gradient(
      ellipse at 50% 80%,
      rgba(196, 139, 139, 0.06) 0%,
      transparent 50%
    );
}

/* Paper grain texture overlay */
.clutter-grain::before {
  content: '';
  position: absolute;
  inset: 0;
  background-image: url("data:image/svg+xml,%3Csvg viewBox='0 0 256 256' xmlns='http://www.w3.org/2000/svg'%3E%3Cfilter id='noise'%3E%3CfeTurbulence type='fractalNoise' baseFrequency='0.9' numOctaves='4' stitchTiles='stitch'/%3E%3C/filter%3E%3Crect width='100%25' height='100%25' filter='url(%23noise)' opacity='0.03'/%3E%3C/svg%3E");
  pointer-events: none;
  z-index: 0;
}
```

### Masonry / Shelf Grid Layout

```css
/* CSS Grid masonry approximation */
.clutter-grid {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(220px, 1fr));
  gap: 1rem;
  padding: 1rem;
}

/* Varied card sizes for organic feel */
.clutter-grid > :nth-child(3n+1) { grid-row: span 2; }
.clutter-grid > :nth-child(5n+2) { grid-column: span 2; }

/* True masonry with columns (fallback approach) */
.clutter-masonry {
  columns: 3 280px;
  column-gap: 1.2rem;
  padding: 1rem;
}

.clutter-masonry > * {
  break-inside: avoid;
  margin-bottom: 1.2rem;
  display: inline-block;
  width: 100%;
}
```

### Eclectic Card Styles

```css
/* Base clutter card -- warm, slightly tilted */
.clutter-card {
  background: var(--clutter-bg-card);
  border: 2px solid var(--clutter-dusty-rose);
  border-radius: 4px;
  padding: 1.5rem;
  position: relative;
  transition: transform 0.3s ease, box-shadow 0.3s ease;
  box-shadow: 2px 3px 8px rgba(92, 61, 46, 0.12);
}

/* Random-feeling rotations */
.clutter-card:nth-child(odd) { transform: rotate(-1.2deg); }
.clutter-card:nth-child(even) { transform: rotate(0.8deg); }
.clutter-card:nth-child(3n) { transform: rotate(-0.5deg); }

.clutter-card:hover {
  transform: rotate(0deg) translateY(-4px);
  box-shadow: 3px 6px 16px rgba(92, 61, 46, 0.2);
  z-index: 2;
}

/* Polaroid-style image card */
.clutter-polaroid {
  background: #fff;
  padding: 0.8rem 0.8rem 2.5rem;
  border: 1px solid #ddd;
  box-shadow: 2px 3px 10px rgba(0, 0, 0, 0.1);
}

.clutter-polaroid img {
  width: 100%;
  display: block;
}

.clutter-polaroid .caption {
  font-family: 'Caveat', cursive;
  font-size: 1.1rem;
  color: var(--clutter-text-secondary);
  text-align: center;
  margin-top: 0.5rem;
}
```

### Washi Tape / Decorative Tape Effect

```css
/* Washi tape strip (decorative element) */
.clutter-tape {
  position: absolute;
  width: 120px;
  height: 28px;
  background: var(--clutter-mustard);
  opacity: 0.7;
  transform: rotate(-5deg);
  top: -12px;
  left: calc(50% - 60px);
  z-index: 3;
}

/* Variant tape colors */
.clutter-tape--rose { background: var(--clutter-dusty-rose); }
.clutter-tape--sage { background: var(--clutter-sage); }
.clutter-tape--teal {
  background: repeating-linear-gradient(
    90deg,
    var(--clutter-teal),
    var(--clutter-teal) 4px,
    rgba(255,255,255,0.4) 4px,
    rgba(255,255,255,0.4) 8px
  );
}
```

### Pinboard / Corkboard Section

```css
/* Corkboard-textured section background */
.clutter-pinboard {
  background-color: #c4a56e;
  background-image:
    radial-gradient(circle at 15% 25%, rgba(180, 140, 80, 0.4) 0%, transparent 40%),
    radial-gradient(circle at 85% 75%, rgba(160, 120, 60, 0.3) 0%, transparent 40%),
    repeating-linear-gradient(
      45deg,
      transparent,
      transparent 3px,
      rgba(0,0,0,0.02) 3px,
      rgba(0,0,0,0.02) 4px
    );
  padding: 3rem 2rem;
  position: relative;
  border: 8px solid var(--clutter-brown);
  border-radius: 2px;
}

/* Push pin decoration */
.clutter-pin {
  position: absolute;
  width: 16px;
  height: 16px;
  background: radial-gradient(circle at 40% 40%, #e85050, #c03030);
  border-radius: 50%;
  box-shadow:
    0 2px 4px rgba(0,0,0,0.3),
    inset 0 -1px 2px rgba(0,0,0,0.2),
    inset 0 1px 1px rgba(255,255,255,0.3);
  z-index: 4;
}
```

### Shelf Display Section

```css
/* Wooden shelf effect */
.clutter-shelf {
  position: relative;
  padding: 2rem 2rem 3rem;
  margin-bottom: 2rem;
}

.clutter-shelf::after {
  content: '';
  position: absolute;
  bottom: 0;
  left: 0;
  right: 0;
  height: 20px;
  background: linear-gradient(
    180deg,
    #8b6b4a 0%,
    #7a5c3c 40%,
    #6b4d30 100%
  );
  border-radius: 0 0 3px 3px;
  box-shadow:
    0 4px 8px rgba(0,0,0,0.2),
    inset 0 1px 0 rgba(255,255,255,0.15);
}

.clutter-shelf-items {
  display: flex;
  gap: 1rem;
  align-items: flex-end;
  justify-content: center;
  flex-wrap: wrap;
}
```

### Sticker / Badge Labels

```css
/* Decorative sticker label */
.clutter-sticker {
  display: inline-block;
  padding: 0.3rem 0.8rem;
  font-family: 'Quicksand', sans-serif;
  font-size: 0.75rem;
  font-weight: 700;
  text-transform: uppercase;
  letter-spacing: 0.05em;
  border-radius: 100px;
  transform: rotate(-3deg);
  box-shadow: 1px 2px 4px rgba(0,0,0,0.1);
}

.clutter-sticker--warm {
  background: var(--clutter-terracotta);
  color: #fff;
}

.clutter-sticker--cool {
  background: var(--clutter-teal);
  color: #fff;
}

.clutter-sticker--bright {
  background: var(--clutter-sunflower);
  color: var(--clutter-brown);
}

.clutter-sticker--outlined {
  background: transparent;
  border: 2px dashed var(--clutter-dusty-rose);
  color: var(--clutter-dusty-rose);
}
```

### Handwritten Underline / Annotation

```css
/* Wavy hand-drawn underline */
.clutter-underline {
  text-decoration: none;
  background-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 100 8'%3E%3Cpath d='M0 6 Q12.5 0 25 6 T50 6 T75 6 T100 6' fill='none' stroke='%23c8614c' stroke-width='2' stroke-linecap='round'/%3E%3C/svg%3E");
  background-repeat: repeat-x;
  background-position: bottom;
  background-size: 100px 8px;
  padding-bottom: 6px;
}

/* Scribble circle highlight */
.clutter-circle-highlight {
  position: relative;
}

.clutter-circle-highlight::after {
  content: '';
  position: absolute;
  inset: -8px -12px;
  border: 2.5px solid var(--clutter-terracotta);
  border-radius: 50% 45% 55% 48%;
  opacity: 0.6;
  transform: rotate(-2deg);
  pointer-events: none;
}
```

### Layered Textile / Pattern Background

```css
/* Patchwork quilt-inspired section */
.clutter-patchwork {
  background:
    linear-gradient(45deg, rgba(200, 97, 76, 0.08) 25%, transparent 25%),
    linear-gradient(-45deg, rgba(141, 164, 126, 0.08) 25%, transparent 25%),
    linear-gradient(45deg, transparent 75%, rgba(123, 80, 120, 0.08) 75%),
    linear-gradient(-45deg, transparent 75%, rgba(61, 139, 139, 0.08) 75%),
    var(--clutter-cream);
  background-size: 60px 60px;
  background-position: 0 0, 0 30px, 30px -30px, 30px 0;
}

/* Floral wallpaper hint */
.clutter-floral-bg {
  background-color: var(--clutter-paper);
  background-image:
    radial-gradient(circle at 20% 30%, rgba(196, 139, 139, 0.15) 8px, transparent 8px),
    radial-gradient(circle at 60% 70%, rgba(141, 164, 126, 0.12) 6px, transparent 6px),
    radial-gradient(circle at 80% 20%, rgba(212, 168, 67, 0.1) 5px, transparent 5px),
    radial-gradient(circle at 40% 80%, rgba(123, 80, 120, 0.1) 7px, transparent 7px);
  background-size: 200px 200px;
}
```

### Gallery Wall / Collage Layout

```css
/* Dense gallery wall with overlapping frames */
.clutter-gallery {
  display: grid;
  grid-template-columns: repeat(12, 1fr);
  grid-auto-rows: 60px;
  gap: 0.5rem;
  padding: 2rem;
  position: relative;
}

.clutter-gallery-item {
  border: 3px solid var(--clutter-brown);
  background: #fff;
  padding: 4px;
  box-shadow: 2px 3px 8px rgba(0,0,0,0.15);
  overflow: hidden;
  z-index: 1;
  transition: z-index 0s, transform 0.3s ease;
}

/* Varied frame sizes */
.clutter-gallery-item:nth-child(1) { grid-column: 1 / 5; grid-row: 1 / 4; transform: rotate(-2deg); }
.clutter-gallery-item:nth-child(2) { grid-column: 4 / 8; grid-row: 1 / 5; transform: rotate(1deg); }
.clutter-gallery-item:nth-child(3) { grid-column: 7 / 10; grid-row: 1 / 3; transform: rotate(-1deg); }
.clutter-gallery-item:nth-child(4) { grid-column: 9 / 13; grid-row: 1 / 5; transform: rotate(2deg); }
.clutter-gallery-item:nth-child(5) { grid-column: 1 / 4; grid-row: 3 / 7; transform: rotate(1.5deg); }
.clutter-gallery-item:nth-child(6) { grid-column: 3 / 7; grid-row: 4 / 7; transform: rotate(-0.5deg); }

.clutter-gallery-item:hover {
  transform: rotate(0deg) scale(1.05);
  z-index: 10;
  box-shadow: 4px 6px 20px rgba(0,0,0,0.25);
}

/* Ornate frame variant */
.clutter-gallery-item--ornate {
  border: 6px solid var(--clutter-brown);
  box-shadow:
    inset 0 0 0 2px var(--clutter-mustard),
    2px 3px 8px rgba(0,0,0,0.15);
}
```

### Scattered Decorative Elements

```css
/* Floating decorative objects (stars, hearts, flowers) */
.clutter-scatter {
  position: relative;
}

.clutter-scatter::before,
.clutter-scatter::after {
  position: absolute;
  font-size: 1.2rem;
  opacity: 0.4;
  pointer-events: none;
}

.clutter-scatter--stars::before { content: '\2728'; top: -10px; left: 5%; }
.clutter-scatter--stars::after { content: '\2B50'; bottom: -8px; right: 8%; }
.clutter-scatter--hearts::before { content: '\2764'; top: -8px; right: 10%; }
.clutter-scatter--plants::before { content: '\1F33F'; top: -12px; left: 8%; }
.clutter-scatter--plants::after { content: '\1F33A'; bottom: -10px; right: 5%; }
```

---

## Materials and Textures (Visual Metaphors for Web)

Physical Cluttercore materials and their web equivalents:

| Physical Material | Web Equivalent |
|-------------------|----------------|
| Cork board | Warm tan background with subtle noise texture and pinned elements |
| Washi tape | Colored semi-transparent strips with repeating patterns, positioned over edges |
| Picture frames | Thick colored borders with box-shadow, slight rotation transforms |
| Fabric / textiles | CSS patterns using repeating gradients (plaids, dots, stripes) |
| Aging paper / parchment | Cream/ivory backgrounds with radial gradient warm spots and noise overlay |
| Wooden shelves | Horizontal gradient bars with grain-like repeating gradients |
| Ceramic and pottery | Rounded border-radius containers with warm, earthy solid colors |
| Stickers and labels | Pill-shaped badges with slight rotation and drop shadows |
| Plants and greenery | Sage/forest green accent colors; leaf emoji as decorative pseudo-elements |
| String lights | Dotted border or repeated radial gradient circles along a curved path |

---

## Key Differences from Maximalism

| Aspect | Traditional Maximalism | Cluttercore |
|--------|----------------------|-------------|
| **Color approach** | Bold but cohesive, often with a unifying palette | Any colors, no unifying scheme required |
| **Material quality** | Luxurious, rich materials (velvet, gold, marble) | Eclectic mix of high and low, thrifted and handmade |
| **Organization** | Intentionally designed; follows design principles | Organically evolved; follows personal meaning |
| **Emotional goal** | Impressive, dramatic, curated | Comforting, personal, nostalgic |
| **Overall feel** | Magazine editorial | Lived-in home |

---

## Related Aesthetics

| Aesthetic | Relationship to Cluttercore |
|-----------|----------------------------|
| **Maximalism** | Parent aesthetic; Cluttercore is a personal, comfort-oriented subset |
| **Cottagecore** | Shares warmth, handmade values, and cozy interiors; Cottagecore is more rural and curated |
| **Goblincore** | Shares collecting instinct and appreciation for unconventional objects |
| **Grandmacore** | Overlaps in nostalgia, inherited objects, doilies, and vintage decor |
| **Cacareco Girl** | Related Brazilian aesthetic celebrating eclectic accumulation |

---

## Quick-Start: Minimal Cluttercore Page Template

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Cluttercore Page</title>
  <link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@400;700&family=Nunito:wght@400;600&family=Caveat:wght@400;700&family=Quicksand:wght@500;700&display=swap" rel="stylesheet">
  <style>
    :root {
      --clutter-cream: #f5f0e6;
      --clutter-ivory: #fff8ee;
      --clutter-paper: #ede4d3;
      --clutter-terracotta: #c8614c;
      --clutter-mustard: #d4a843;
      --clutter-sage: #8da47e;
      --clutter-teal: #3d8b8b;
      --clutter-dusty-rose: #c48b8b;
      --clutter-plum: #7b5078;
      --clutter-burgundy: #803040;
      --clutter-brown: #5c3d2e;
    }

    * { margin: 0; padding: 0; box-sizing: border-box; }

    body {
      background: var(--clutter-cream);
      color: var(--clutter-brown);
      font-family: 'Nunito', sans-serif;
      font-weight: 400;
      line-height: 1.7;
    }

    h1, h2, h3 {
      font-family: 'Playfair Display', Georgia, serif;
      font-weight: 700;
      color: var(--clutter-burgundy);
      line-height: 1.2;
    }

    .hero {
      text-align: center;
      padding: 5rem 2rem 3rem;
      background: var(--clutter-paper);
      position: relative;
      overflow: hidden;
    }

    .hero h1 {
      font-size: clamp(2.5rem, 5vw, 4.5rem);
      margin-bottom: 0.5rem;
    }

    .hero .subtitle {
      font-family: 'Caveat', cursive;
      font-size: 1.6rem;
      color: var(--clutter-terracotta);
      transform: rotate(-2deg);
      display: inline-block;
    }

    .clutter-grid {
      display: grid;
      grid-template-columns: repeat(auto-fill, minmax(260px, 1fr));
      gap: 1.5rem;
      max-width: 1100px;
      margin: 0 auto;
      padding: 3rem 2rem;
    }

    .clutter-card {
      background: var(--clutter-ivory);
      border: 2px solid var(--clutter-dusty-rose);
      border-radius: 4px;
      padding: 1.5rem;
      box-shadow: 2px 3px 8px rgba(92, 61, 46, 0.12);
      position: relative;
      transition: transform 0.3s ease, box-shadow 0.3s ease;
    }

    .clutter-card:nth-child(odd) { transform: rotate(-1.2deg); }
    .clutter-card:nth-child(even) { transform: rotate(0.8deg); }

    .clutter-card:hover {
      transform: rotate(0deg) translateY(-4px);
      box-shadow: 3px 6px 16px rgba(92, 61, 46, 0.2);
      z-index: 2;
    }

    .clutter-card h3 {
      font-size: 1.3rem;
      margin-bottom: 0.5rem;
    }

    .tag {
      display: inline-block;
      padding: 0.2rem 0.6rem;
      font-family: 'Quicksand', sans-serif;
      font-size: 0.7rem;
      font-weight: 700;
      text-transform: uppercase;
      border-radius: 100px;
      margin-bottom: 0.8rem;
    }

    .tag--terracotta { background: var(--clutter-terracotta); color: #fff; }
    .tag--teal { background: var(--clutter-teal); color: #fff; }
    .tag--mustard { background: var(--clutter-mustard); color: var(--clutter-brown); }
    .tag--sage { background: var(--clutter-sage); color: #fff; }
  </style>
</head>
<body>
  <div class="hero">
    <h1>My Beautiful Mess</h1>
    <span class="subtitle">a curated collection of everything</span>
  </div>
  <section class="clutter-grid">
    <div class="clutter-card">
      <span class="tag tag--terracotta">Memories</span>
      <h3>Grandma's Teacups</h3>
      <p>A mismatched set collected from flea markets across three countries, each with its own story.</p>
    </div>
    <div class="clutter-card">
      <span class="tag tag--teal">Collection</span>
      <h3>Vintage Cameras</h3>
      <p>From Kodak Brownies to Polaroid SX-70s, arranged on the bookshelf between travel guides.</p>
    </div>
    <div class="clutter-card">
      <span class="tag tag--mustard">Reading</span>
      <h3>The Overflowing Shelf</h3>
      <p>Books stacked two-deep with postcards marking favorite passages and plants filling the gaps.</p>
    </div>
    <div class="clutter-card">
      <span class="tag tag--sage">Growing</span>
      <h3>Plant Corner</h3>
      <p>Seventeen plants and counting, trailing across the windowsill and climbing up the wall.</p>
    </div>
  </section>
</body>
</html>
```
