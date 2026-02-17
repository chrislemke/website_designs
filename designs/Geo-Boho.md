# Geo-Boho Design Reference

Geo-Boho is a hybrid aesthetic that merges the free-spirited, naturalistic sensibility of Bohemian design with rigorous geometric structure. It replaces the traditional organic looseness of boho with triangular grids, vector line-work, and mathematically precise patterning -- while retaining the earthy warmth, muted tones, and handcrafted feel of its bohemian roots. The result is a design language that feels simultaneously structured and soulful, modern and ancient, precise and organic. It rose to prominence alongside the broader hipster movement, borrowing visual language from Native American, Indian, and Buddhist iconography, reinterpreting it through clean geometric abstraction.

---

## Visual Characteristics

### Core Design Traits

- **Triangle-obsessed geometry** -- triangles are the foundational shape, used as grids, frames, decorative elements, and organizational structures; squares and rectangles are deliberately de-emphasized
- **Line-based vector aesthetics** -- designs emphasize strokes and outlines over filled surfaces; thin, precise lines create intricate patterns that feel hand-drawn but mathematically composed
- **Non-traditional grid organization** -- triangular and circular grids replace conventional square/rectangular layouts, creating dynamic, angular compositions
- **Muted, naturalistic color palette** -- airy whites, soft greys, warm beiges, and dusty pastels dominate; color is understated, never saturated or aggressive
- **Lo-fi photographic filters** -- imagery uses desaturated, analog-style treatments (lo-mo filters, soft focus, muted contrast) that evoke film photography
- **Geometric letterforms** -- typography features elongated sans-serifs with additional parallel lines, crossbars, and geometric embellishments integrated into the letterforms
- **Cultural iconography** -- dreamcatchers, mandalas, paisley, henna-style patterns, yin-yang symbols, Om glyphs, and feather motifs, all rendered through geometric abstraction
- **Wild animal illustration** -- deer, wolves, bears, and birds depicted in geometric/polygonal wireframe style rather than realistic illustration
- **Macrame and rope textures** -- woven, knotted visual references suggesting handcraft and natural materials
- **Pale, undyed materials** -- natural wood, raw linen, unbleached cotton textures as backgrounds and accents
- **Watercolor and collage effects** -- traditional media simulation blended with precise geometric overlays

### Design Principles

- Fuse the mathematical precision of geometry with the organic warmth of bohemian naturalism
- Use line weight and stroke style (not color intensity) to create visual hierarchy
- Layer geometric patterns over soft, muted backgrounds to create depth without shadows
- Embrace asymmetry within geometric frameworks -- structured but never rigid
- Favor SVG line art and thin-stroke illustrations over photographic imagery
- Let negative space breathe; compositions should feel airy, not dense
- Blend cultural motifs respectfully, abstracting them into geometric pattern language
- Simulate handcrafted quality through subtle imperfections in otherwise precise geometry
- Use desaturation and muted tones to unify diverse visual elements into a cohesive palette
- Balance digital precision with analog warmth -- every vector line should feel like it could have been drawn by hand

---

## Color Palette

### Primary Geo-Boho Palette

The core palette draws from natural, undyed materials and desert landscapes -- warm but never hot, muted but never dull. Every color feels sun-bleached and lived-in.

| Color Name | Hex | Role / Usage |
|------------|-----|-------------|
| **Parchment White** | `#F2EFEB` | Primary background, breathing space, page canvas |
| **Desert Sand** | `#D9C7C1` | Secondary backgrounds, card surfaces, soft fills |
| **Warm Clay** | `#BF8D7A` | Accent elements, borders, decorative lines |
| **Terracotta** | `#A65C32` | Primary accent, CTAs, headings, key interactive elements |
| **Deep Sienna** | `#734E40` | Dark text, strong headings, high-contrast elements |
| **Charcoal Earth** | `#401D09` | Deepest text, footer backgrounds, maximum contrast |

### Accent Colors

| Color Name | Hex | Role / Usage |
|------------|-----|-------------|
| **Sage Green** | `#728C82` | Secondary accent, nature references, success states |
| **Dusty Teal** | `#4A7C6F` | Links, interactive highlights, geometric line fills |
| **Amber Gold** | `#BF9039` | Highlights, stars, warmth accents, hover states |
| **Muted Rose** | `#BF8085` | Soft accent, feminine touches, decorative fills |
| **Faded Plum** | `#73516A` | Tertiary accent, tags, badges, subtle differentiation |
| **Storm Grey** | `#687372` | Muted text, captions, secondary information |

### Neutral Scale

| Color Name | Hex | Role / Usage |
|------------|-----|-------------|
| **Raw Linen** | `#F5F0E8` | Lightest background, near-white warmth |
| **Bleached Sand** | `#E7DDD3` | Alternate section backgrounds |
| **Driftwood** | `#C9B5AE` | Borders, dividers, subtle separators |
| **Weathered Stone** | `#A09890` | Placeholder text, disabled states |
| **Ash Brown** | `#8C8080` | Secondary text, captions |
| **Dark Earth** | `#595456` | Body text on light backgrounds |

### CSS Custom Properties

```css
:root {
  /* Primary palette */
  --geo-parchment: #f2efeb;
  --geo-desert-sand: #d9c7c1;
  --geo-warm-clay: #bf8d7a;
  --geo-terracotta: #a65c32;
  --geo-sienna: #734e40;
  --geo-charcoal: #401d09;

  /* Accent colors */
  --geo-sage: #728c82;
  --geo-teal: #4a7c6f;
  --geo-amber: #bf9039;
  --geo-rose: #bf8085;
  --geo-plum: #73516a;
  --geo-storm: #687372;

  /* Neutrals */
  --geo-linen: #f5f0e8;
  --geo-bleached: #e7ddd3;
  --geo-driftwood: #c9b5ae;
  --geo-weathered: #a09890;
  --geo-ash: #8c8080;
  --geo-dark-earth: #595456;

  /* Semantic */
  --geo-bg-primary: #f2efeb;
  --geo-bg-secondary: #f5f0e8;
  --geo-bg-accent: #e7ddd3;
  --geo-bg-dark: #401d09;
  --geo-text-primary: #401d09;
  --geo-text-secondary: #734e40;
  --geo-text-muted: #8c8080;
  --geo-text-light: #f2efeb;
  --geo-accent-primary: #a65c32;
  --geo-accent-secondary: #728c82;
  --geo-border: #c9b5ae;
}
```

### Color Usage Guidelines

- **Backgrounds should always be warm** -- never use pure white (`#ffffff`) or cool greys; even the lightest shade should carry warmth
- **Limit saturated colors** to small accent touches -- geometric line patterns, borders, CTAs; large surfaces stay muted
- **Terracotta is the hero color** -- use it for primary actions, key headings, and focal geometric elements
- **Sage and teal provide contrast** without breaking the earthy palette; use for links, icons, and secondary interactive elements
- **Layer opacity** on geometric patterns; use `0.06 - 0.15` opacity fills behind dense line-work to add depth without weight
- **Amber gold** works as a highlight and hover state; it should feel like sunlight catching a surface
- **Avoid pure black** for text; use Charcoal Earth (`#401d09`) or Dark Earth (`#595456`) for warmth
- **Photography should be desaturated** 20-40% and warmed with an amber overlay to match the palette

---

## Typography

### Typeface Characteristics

Geo-Boho typography is:

- **Elongated geometric sans-serif** -- letterforms emphasize vertical proportions with geometric construction
- **Thin to medium weight** -- matching the line-art aesthetic; heavy weights feel too solid for this style
- **Occasionally embellished** -- decorative parallel lines, crossbars, or geometric additions to display text (achieved through CSS or SVG)
- **Mixed with hand-lettered accents** -- script or hand-drawn fonts for secondary/decorative text to add warmth
- **Generous letter-spacing on uppercase** -- wide-tracked uppercase text in navigation and labels evokes craft branding
- **Soft and warm in body text** -- highly readable with generous line height, never clinical

### Recommended Web Fonts (Google Fonts)

| Font | Style | Best For |
|------|-------|----------|
| **Josefin Sans** | Geometric, elegant, thin stems | Display headings, hero text -- its geometric purity is quintessentially Geo-Boho |
| **Poiret One** | Art Deco geometric, ultra-thin | Large display text, decorative titles, section headers |
| **Quicksand** | Rounded geometric sans | Body text, UI elements -- friendly and warm yet geometric |
| **Comfortaa** | Rounded, geometric, wide | Secondary headings, navigation labels |
| **Philosopher** | Humanist with geometric touches | Body text, longer reads -- warm without losing structure |
| **Cormorant Garamond** | Elegant serif with fine strokes | Pull quotes, editorial accents -- adds bohemian refinement |
| **Amatic SC** | Hand-drawn, narrow | Decorative labels, sub-headings, craft-style accents |
| **Caveat** | Natural handwriting | Annotations, callouts, personal-touch elements |
| **Nunito** | Rounded terminals, soft geometry | Body text alternative, approachable and warm |
| **Marcellus** | Sharp serif, geometric elegance | Headlines alternative for a more editorial Geo-Boho feel |

### Font Pairing Suggestions

| Heading Font | Body Font | Character |
|-------------|-----------|-----------|
| **Josefin Sans** (300/400) | **Quicksand** (400) | Pure Geo-Boho: geometric precision meets soft warmth |
| **Poiret One** (400) | **Philosopher** (400) | Elegant, editorial: fine geometric lines with humanist reading |
| **Josefin Sans** (600) | **Nunito** (400) | Modern, accessible: structured headings, friendly body |
| **Marcellus** (400) | **Quicksand** (400) | Refined bohemian: sharp serif display, soft geometric body |
| **Comfortaa** (600) | **Philosopher** (400) | Warm throughout: rounded headings, warm body text |

### Typography CSS Example

```css
/* Import fonts */
@import url('https://fonts.googleapis.com/css2?family=Josefin+Sans:wght@300;400;600&family=Quicksand:wght@400;500;600&family=Amatic+SC:wght@400;700&display=swap');

/* Headings */
h1, h2, h3, h4, h5, h6 {
  font-family: 'Josefin Sans', 'Quicksand', sans-serif;
  font-weight: 300;
  color: var(--geo-text-primary);
  line-height: 1.2;
  letter-spacing: 0.02em;
}

/* Display / Hero text */
.geo-display {
  font-family: 'Josefin Sans', sans-serif;
  font-size: clamp(2.5rem, 6vw, 5rem);
  font-weight: 300;
  letter-spacing: 0.06em;
  line-height: 1.1;
  text-transform: uppercase;
}

/* Body text */
body {
  font-family: 'Quicksand', 'Nunito', sans-serif;
  font-weight: 400;
  font-size: 1rem;
  line-height: 1.8;
  color: var(--geo-dark-earth);
}

/* Decorative / hand-lettered accent text */
.geo-handwritten {
  font-family: 'Amatic SC', cursive;
  font-size: 1.5rem;
  font-weight: 700;
  letter-spacing: 0.08em;
  color: var(--geo-terracotta);
}

/* Navigation labels */
.geo-nav-label {
  font-family: 'Josefin Sans', sans-serif;
  font-weight: 400;
  font-size: 0.85rem;
  letter-spacing: 0.14em;
  text-transform: uppercase;
}

/* Captions / subtext */
.geo-caption {
  font-family: 'Quicksand', sans-serif;
  font-weight: 400;
  font-size: 0.85rem;
  color: var(--geo-text-muted);
  line-height: 1.6;
}
```

---

## Layout Principles

### Grid and Structure

- **Triangular and diamond motifs in layout** -- use CSS clip-path, rotated elements, and diagonal dividers to break away from strictly rectangular composition
- **Centered, constrained containers** -- max-width of 1000-1100px for content; narrower than typical flat design to maintain intimacy and readability
- **Generous whitespace with warmth** -- sections separated by 80-120px of vertical space; the breathing room should feel intentional and meditative, not clinical
- **Layered geometric backgrounds** -- thin SVG line patterns (triangular grids, diamond tessellations) at very low opacity behind content
- **Asymmetric balance** -- content blocks can be offset from center; the grid provides structure but allows bohemian looseness
- **Section dividers as geometric art** -- instead of simple horizontal lines, use SVG triangle waves, diamond chains, or zigzag patterns
- **Natural texture backgrounds** -- subtle linen, paper, or wood-grain textures at low opacity to add tactile warmth
- **Mixed-media sections** -- combine photography (desaturated), SVG line-art, and geometric pattern in the same composition

### Section Organization

- **Navigation**: Minimal top bar with wide-tracked uppercase links; thin geometric line separator below; optional small geometric motif as logo
- **Hero**: Large thin-weight geometric type + geometric line-art illustration or desaturated photography with geometric overlay; soft, warm background
- **Pattern divider**: SVG geometric border (triangles, diamonds, zigzag) between major sections
- **Features**: 3-column grid with geometric icons (line-art style, thin strokes); ample spacing between items
- **Content rows**: Text paired with geometric illustrations or filtered photography; asymmetric placement encouraged
- **Pull quote**: Large decorative text in hand-lettered font, framed by geometric border elements
- **Gallery / portfolio**: Masonry or offset grid with geometric frame overlays on images
- **CTA section**: Warm background color with geometric pattern overlay at low opacity; centered text and button
- **Footer**: Dark warm background, thin geometric line-art decorations, organized in columns with wide-tracked labels

### Responsive Approach

- Stack to single column below 768px; maintain generous padding (minimum 24px side padding)
- Geometric background patterns should scale or simplify on mobile -- reduce density to avoid visual noise
- Typography scales fluidly with `clamp()`; display text can be dramatically larger on desktop
- Section dividers simplify to thinner, less complex patterns on mobile
- Touch targets minimum 48px; interactive elements should have visible geometric borders for clarity

---

## CSS / Design Techniques

### Geometric Background Pattern (SVG + CSS)

```css
/* Triangular grid pattern background */
.geo-pattern-bg {
  position: relative;
  background-color: var(--geo-bg-primary);
}

.geo-pattern-bg::before {
  content: '';
  position: absolute;
  inset: 0;
  background-image: url("data:image/svg+xml,%3Csvg width='60' height='52' viewBox='0 0 60 52' xmlns='http://www.w3.org/2000/svg'%3E%3Cpath d='M30 0 L60 52 L0 52 Z' fill='none' stroke='%23c9b5ae' stroke-width='0.5'/%3E%3C/svg%3E");
  background-size: 60px 52px;
  opacity: 0.15;
  pointer-events: none;
}

/* Diamond tessellation pattern */
.geo-diamond-bg::before {
  content: '';
  position: absolute;
  inset: 0;
  background-image: url("data:image/svg+xml,%3Csvg width='40' height='40' viewBox='0 0 40 40' xmlns='http://www.w3.org/2000/svg'%3E%3Cpath d='M20 0 L40 20 L20 40 L0 20 Z' fill='none' stroke='%23bf8d7a' stroke-width='0.5'/%3E%3C/svg%3E");
  background-size: 40px 40px;
  opacity: 0.1;
  pointer-events: none;
}
```

### Geometric Section Divider

```css
/* Triangle wave divider */
.geo-divider {
  width: 100%;
  height: 24px;
  margin: 0 auto;
  max-width: 600px;
  background-image: url("data:image/svg+xml,%3Csvg width='48' height='24' viewBox='0 0 48 24' xmlns='http://www.w3.org/2000/svg'%3E%3Cpath d='M0 24 L12 0 L24 24 L36 0 L48 24' fill='none' stroke='%23c9b5ae' stroke-width='1'/%3E%3C/svg%3E");
  background-repeat: repeat-x;
  background-position: center;
}

/* Diamond chain divider */
.geo-divider--diamond {
  width: 100%;
  height: 20px;
  margin: 40px auto;
  max-width: 400px;
  background-image: url("data:image/svg+xml,%3Csvg width='20' height='20' viewBox='0 0 20 20' xmlns='http://www.w3.org/2000/svg'%3E%3Cpath d='M10 0 L20 10 L10 20 L0 10 Z' fill='none' stroke='%23a65c32' stroke-width='0.8'/%3E%3C/svg%3E");
  background-repeat: repeat-x;
  background-position: center;
  background-size: 20px 20px;
}

/* Centered mandala-style dot divider */
.geo-divider--dots {
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 12px;
  padding: 40px 0;
}

.geo-divider--dots::before,
.geo-divider--dots::after {
  content: '';
  width: 80px;
  height: 1px;
  background: var(--geo-driftwood);
}

.geo-divider--dots span {
  width: 8px;
  height: 8px;
  background: var(--geo-terracotta);
  transform: rotate(45deg);
}
```

### Geo-Boho Card Component

```css
.geo-card {
  background: var(--geo-bg-primary);
  border: 1px solid var(--geo-driftwood);
  padding: 36px;
  position: relative;
  /* Subtle warm shadow -- not flat, but not heavy; a soft, diffused glow */
  box-shadow: 0 2px 20px rgba(64, 29, 9, 0.06);
  transition: box-shadow 0.3s ease, transform 0.3s ease;
}

.geo-card:hover {
  box-shadow: 0 4px 30px rgba(64, 29, 9, 0.1);
  transform: translateY(-2px);
}

/* Geometric corner accents */
.geo-card::before,
.geo-card::after {
  content: '';
  position: absolute;
  width: 24px;
  height: 24px;
  border-color: var(--geo-warm-clay);
  border-style: solid;
  border-width: 0;
}

.geo-card::before {
  top: 8px;
  left: 8px;
  border-top-width: 1px;
  border-left-width: 1px;
}

.geo-card::after {
  bottom: 8px;
  right: 8px;
  border-bottom-width: 1px;
  border-right-width: 1px;
}

/* Card grid */
.geo-card-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
  gap: 32px;
}
```

### Geo-Boho Button

```css
.geo-button {
  display: inline-flex;
  align-items: center;
  justify-content: center;
  gap: 8px;
  background: transparent;
  color: var(--geo-terracotta);
  border: 1.5px solid var(--geo-terracotta);
  padding: 12px 36px;
  font-family: 'Josefin Sans', sans-serif;
  font-weight: 400;
  font-size: 0.85rem;
  letter-spacing: 0.12em;
  text-transform: uppercase;
  cursor: pointer;
  transition: all 0.3s ease;
  text-decoration: none;
  position: relative;
}

.geo-button:hover {
  background: var(--geo-terracotta);
  color: var(--geo-text-light);
}

/* Filled variant */
.geo-button--filled {
  background: var(--geo-terracotta);
  color: var(--geo-text-light);
}

.geo-button--filled:hover {
  background: var(--geo-sienna);
  border-color: var(--geo-sienna);
}

/* With geometric arrow */
.geo-button--arrow::after {
  content: '';
  width: 0;
  height: 0;
  border-left: 5px solid currentColor;
  border-top: 4px solid transparent;
  border-bottom: 4px solid transparent;
  transition: transform 0.3s ease;
}

.geo-button--arrow:hover::after {
  transform: translateX(3px);
}

/* Sage variant */
.geo-button--sage {
  color: var(--geo-teal);
  border-color: var(--geo-teal);
}

.geo-button--sage:hover {
  background: var(--geo-teal);
  color: var(--geo-text-light);
}
```

### Navigation Bar

```css
.geo-nav {
  display: flex;
  align-items: center;
  justify-content: space-between;
  max-width: 1100px;
  margin: 0 auto;
  padding: 24px 40px;
  border-bottom: 1px solid var(--geo-driftwood);
}

.geo-nav__logo {
  font-family: 'Josefin Sans', sans-serif;
  font-weight: 300;
  font-size: 1.5rem;
  color: var(--geo-text-primary);
  text-decoration: none;
  letter-spacing: 0.08em;
  text-transform: uppercase;
}

.geo-nav__links {
  display: flex;
  gap: 36px;
  list-style: none;
  margin: 0;
  padding: 0;
}

.geo-nav__links a {
  font-family: 'Josefin Sans', sans-serif;
  font-weight: 400;
  font-size: 0.8rem;
  letter-spacing: 0.14em;
  text-transform: uppercase;
  color: var(--geo-text-muted);
  text-decoration: none;
  transition: color 0.3s ease;
  position: relative;
}

.geo-nav__links a::after {
  content: '';
  position: absolute;
  bottom: -4px;
  left: 50%;
  width: 0;
  height: 1px;
  background: var(--geo-terracotta);
  transition: width 0.3s ease, left 0.3s ease;
}

.geo-nav__links a:hover {
  color: var(--geo-terracotta);
}

.geo-nav__links a:hover::after {
  width: 100%;
  left: 0;
}
```

### Hero Section

```css
.geo-hero {
  display: flex;
  align-items: center;
  justify-content: center;
  flex-direction: column;
  text-align: center;
  max-width: 1100px;
  margin: 0 auto;
  padding: 100px 40px 80px;
  position: relative;
}

.geo-hero h1 {
  font-family: 'Josefin Sans', sans-serif;
  font-weight: 300;
  font-size: clamp(2.5rem, 6vw, 4.5rem);
  letter-spacing: 0.08em;
  text-transform: uppercase;
  margin-bottom: 1.5rem;
  color: var(--geo-text-primary);
}

.geo-hero p {
  font-family: 'Quicksand', sans-serif;
  font-size: 1.1rem;
  color: var(--geo-text-muted);
  max-width: 560px;
  margin: 0 auto 2.5rem;
  line-height: 1.8;
}

/* Decorative triangle frame around hero */
.geo-hero::before {
  content: '';
  position: absolute;
  top: 40px;
  left: 50%;
  transform: translateX(-50%);
  width: 0;
  height: 0;
  border-left: 200px solid transparent;
  border-right: 200px solid transparent;
  border-bottom: 340px solid transparent;
  border-bottom-color: rgba(166, 92, 50, 0.04);
  pointer-events: none;
}

@media (max-width: 768px) {
  .geo-hero {
    padding: 60px 24px 40px;
  }

  .geo-hero::before {
    display: none;
  }
}
```

### Diagonal / Angled Section Transition

```css
/* Angled section break -- a signature Geo-Boho technique */
.geo-section--angled {
  position: relative;
  padding: 100px 0 80px;
  background: var(--geo-bg-accent);
}

.geo-section--angled::before {
  content: '';
  position: absolute;
  top: -40px;
  left: 0;
  right: 0;
  height: 80px;
  background: var(--geo-bg-accent);
  clip-path: polygon(0 50%, 100% 0, 100% 100%, 0 100%);
}

.geo-section--angled::after {
  content: '';
  position: absolute;
  bottom: -40px;
  left: 0;
  right: 0;
  height: 80px;
  background: var(--geo-bg-accent);
  clip-path: polygon(0 0, 100% 0, 100% 50%, 0 100%);
  z-index: 1;
}
```

### Geometric Icon Style

```css
/* Line-art geometric icons -- thin strokes, no fills */
.geo-icon {
  stroke: var(--geo-terracotta);
  stroke-width: 1.5;
  fill: none;
  width: 48px;
  height: 48px;
}

/* Icon in a geometric frame */
.geo-icon-frame {
  display: inline-flex;
  align-items: center;
  justify-content: center;
  width: 72px;
  height: 72px;
  border: 1px solid var(--geo-driftwood);
  transform: rotate(45deg);
}

.geo-icon-frame .geo-icon {
  transform: rotate(-45deg);
}

/* Circular icon container with geometric border */
.geo-icon-circle {
  display: inline-flex;
  align-items: center;
  justify-content: center;
  width: 64px;
  height: 64px;
  border-radius: 50%;
  border: 1.5px solid var(--geo-warm-clay);
  position: relative;
}

/* Decorative dots around circle */
.geo-icon-circle::before,
.geo-icon-circle::after {
  content: '';
  position: absolute;
  width: 4px;
  height: 4px;
  background: var(--geo-warm-clay);
  border-radius: 50%;
}

.geo-icon-circle::before { top: -2px; }
.geo-icon-circle::after { bottom: -2px; }
```

### Geometric Image Frame

```css
/* Photo with geometric overlay border */
.geo-image-frame {
  position: relative;
  display: inline-block;
}

.geo-image-frame img {
  display: block;
  width: 100%;
  filter: saturate(0.7) sepia(0.15);
  transition: filter 0.4s ease;
}

.geo-image-frame:hover img {
  filter: saturate(0.85) sepia(0.08);
}

/* Offset geometric border */
.geo-image-frame::after {
  content: '';
  position: absolute;
  top: 12px;
  left: 12px;
  right: -12px;
  bottom: -12px;
  border: 1px solid var(--geo-warm-clay);
  pointer-events: none;
}

/* Triangular clip-path for images */
.geo-image--triangle {
  clip-path: polygon(50% 0%, 0% 100%, 100% 100%);
}

/* Hexagonal clip-path */
.geo-image--hexagon {
  clip-path: polygon(25% 0%, 75% 0%, 100% 50%, 75% 100%, 25% 100%, 0% 50%);
}

/* Diamond clip-path */
.geo-image--diamond {
  clip-path: polygon(50% 0%, 100% 50%, 50% 100%, 0% 50%);
}
```

### Mandala / Geometric Decorative Element

```css
/* Rotating mandala-style decoration (pure CSS) */
.geo-mandala {
  width: 200px;
  height: 200px;
  position: relative;
  margin: 40px auto;
}

.geo-mandala span {
  position: absolute;
  inset: 0;
  border: 1px solid var(--geo-driftwood);
  border-radius: 50%;
}

.geo-mandala span:nth-child(2) {
  inset: 15px;
  border-color: var(--geo-warm-clay);
}

.geo-mandala span:nth-child(3) {
  inset: 30px;
  border-color: var(--geo-terracotta);
  border-radius: 0;
  transform: rotate(45deg);
}

.geo-mandala span:nth-child(4) {
  inset: 45px;
  border-color: var(--geo-sage);
  border-radius: 0;
  transform: rotate(22.5deg);
}

.geo-mandala span:nth-child(5) {
  inset: 55px;
  border-color: var(--geo-driftwood);
  border-radius: 50%;
}
```

### Pull Quote

```css
.geo-quote {
  text-align: center;
  padding: 60px 40px;
  max-width: 700px;
  margin: 0 auto;
  position: relative;
}

.geo-quote blockquote {
  font-family: 'Cormorant Garamond', 'Philosopher', serif;
  font-size: clamp(1.4rem, 3vw, 2rem);
  font-style: italic;
  color: var(--geo-text-secondary);
  line-height: 1.6;
  margin: 0 0 1rem;
}

/* Geometric quote marks */
.geo-quote::before,
.geo-quote::after {
  content: '';
  position: absolute;
  width: 0;
  height: 0;
}

.geo-quote::before {
  top: 20px;
  left: 20px;
  border-left: 12px solid var(--geo-warm-clay);
  border-top: 8px solid transparent;
  border-bottom: 8px solid transparent;
}

.geo-quote::after {
  bottom: 20px;
  right: 20px;
  border-right: 12px solid var(--geo-warm-clay);
  border-top: 8px solid transparent;
  border-bottom: 8px solid transparent;
}

.geo-quote cite {
  font-family: 'Josefin Sans', sans-serif;
  font-weight: 400;
  font-size: 0.8rem;
  letter-spacing: 0.12em;
  text-transform: uppercase;
  color: var(--geo-text-muted);
  font-style: normal;
}
```

### Footer

```css
.geo-footer {
  background: var(--geo-charcoal);
  color: var(--geo-driftwood);
  padding: 60px 40px 40px;
  position: relative;
}

/* Geometric top border */
.geo-footer::before {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  height: 3px;
  background: repeating-linear-gradient(
    90deg,
    var(--geo-terracotta) 0px,
    var(--geo-terracotta) 20px,
    transparent 20px,
    transparent 24px,
    var(--geo-sage) 24px,
    var(--geo-sage) 44px,
    transparent 44px,
    transparent 48px
  );
}

.geo-footer__content {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
  gap: 40px;
  max-width: 1100px;
  margin: 0 auto;
}

.geo-footer h4 {
  font-family: 'Josefin Sans', sans-serif;
  font-weight: 400;
  font-size: 0.8rem;
  letter-spacing: 0.14em;
  text-transform: uppercase;
  color: var(--geo-warm-clay);
  margin-bottom: 16px;
}

.geo-footer a {
  color: var(--geo-driftwood);
  text-decoration: none;
  font-size: 0.9rem;
  transition: color 0.3s ease;
}

.geo-footer a:hover {
  color: var(--geo-amber);
}

.geo-footer__bottom {
  text-align: center;
  padding-top: 32px;
  margin-top: 32px;
  border-top: 1px solid rgba(201, 181, 174, 0.2);
  font-size: 0.8rem;
  color: var(--geo-ash);
}
```

---

## Design Do's and Don'ts

### Do

- Use triangles, diamonds, and circles as the foundational geometric vocabulary -- avoid relying on rectangles
- Keep line weights thin and consistent (1-2px strokes for patterns, 1-1.5px for borders)
- Layer geometric patterns at very low opacity (0.05-0.15) to add texture without visual noise
- Desaturate photography and warm-shift it to match the earthy palette
- Mix geometric precision with hand-lettered or handwriting fonts for warmth
- Use wide letter-spacing on uppercase navigation and label text
- Create section transitions with diagonal lines, zigzags, or geometric dividers instead of hard horizontal breaks
- Embrace asymmetry within geometric frameworks -- offset elements, uneven margins, loose alignment
- Use CSS `clip-path` for geometric image masks (triangles, hexagons, diamonds)
- Include subtle texture (paper grain, linen weave) at very low opacity on backgrounds
- Use SVG for all decorative geometric elements to ensure crispness at any resolution

### Don't

- Use saturated, neon, or digitally vibrant colors -- Geo-Boho is always muted and warm
- Apply heavy drop shadows or glossy effects -- depth should come from layering and overlap, not shadow
- Use square/rectangular grids exclusively -- triangular and diagonal organization is essential
- Fill geometric shapes with solid color -- prefer outlines and line-art
- Use cold greys or pure white -- every neutral should carry warmth
- Over-clutter with geometric patterns -- the aesthetic should feel airy, not overwhelming
- Use heavy or condensed type weights for body text -- thin-to-regular weights maintain the ethereal quality
- Apply geometric patterns at full opacity -- subtlety is key
- Ignore cultural sensitivity -- geometric abstraction of cultural motifs (dreamcatchers, mandalas, Om symbols) should be respectful and non-appropriative
- Mix Geo-Boho with high-contrast, high-saturation design systems (Material Design, Flat UI) -- the palettes and philosophies conflict

---

## Related Aesthetics

| Aesthetic | Relationship to Geo-Boho |
|-----------|--------------------------|
| **Boho-Chic** | Direct parent; Geo-Boho adds geometric structure and vector precision to the free-flowing, textile-heavy bohemian foundation |
| **Hipster** | Cultural sibling; shares the authenticity-seeking, craft-oriented, analog-nostalgic sensibility but Geo-Boho is more visually structured |
| **Flat Design** | Technical cousin; shares the vector-based, minimal-ornament approach but Geo-Boho replaces digital vibrancy with organic warmth |
| **Vaporwave** | Distant aesthetic relative; both remix cultural imagery through geometric abstraction, but with completely opposite palettes and moods |
| **Tranquil Spa** | Mood ally; shares the calming, muted, naturalistic atmosphere but lacks the geometric structural discipline |
| **Technozen** | Philosophical parallel; both merge technology (geometry, precision) with spiritual/natural aesthetics |
| **Avantropop** | Creative sibling; both mix high-culture precision with folk/popular aesthetics and cultural sampling |
| **Recession Pop** | Contemporaneous aesthetic; both emerged from the same cultural moment of making beauty from constraint and simplicity |
| **Ethnic Chic** | Closely related; both draw from global cultural visual traditions, but Geo-Boho filters them through stricter geometric abstraction |
| **Earth Tones** | Palette parent; Geo-Boho inherits its warm, muted color philosophy directly from the Earth Tones aesthetic |
| **Art Deco** | Historical ancestor of the geometric side; shares the love of geometric precision, triangular forms, and decorative line-work |
| **Sacred Geometry** | Spiritual cousin; both use geometric forms as carriers of deeper meaning, but Sacred Geometry is more mystical and precise |

---

## Quick-Start: Minimal Geo-Boho Page Template

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Geo-Boho Page</title>
  <link href="https://fonts.googleapis.com/css2?family=Josefin+Sans:wght@300;400;600&family=Quicksand:wght@400;500;600&family=Amatic+SC:wght@700&display=swap" rel="stylesheet">
  <style>
    :root {
      --geo-parchment: #f2efeb;
      --geo-desert-sand: #d9c7c1;
      --geo-warm-clay: #bf8d7a;
      --geo-terracotta: #a65c32;
      --geo-sienna: #734e40;
      --geo-charcoal: #401d09;
      --geo-sage: #728c82;
      --geo-teal: #4a7c6f;
      --geo-amber: #bf9039;
      --geo-rose: #bf8085;
      --geo-linen: #f5f0e8;
      --geo-bleached: #e7ddd3;
      --geo-driftwood: #c9b5ae;
      --geo-weathered: #a09890;
      --geo-ash: #8c8080;
      --geo-dark-earth: #595456;
    }

    * { margin: 0; padding: 0; box-sizing: border-box; }

    body {
      background: var(--geo-parchment);
      color: var(--geo-dark-earth);
      font-family: 'Quicksand', sans-serif;
      font-weight: 400;
      line-height: 1.8;
    }

    h1, h2, h3 {
      font-family: 'Josefin Sans', sans-serif;
      font-weight: 300;
      line-height: 1.2;
      color: var(--geo-charcoal);
      letter-spacing: 0.04em;
    }

    /* Navigation */
    nav {
      display: flex;
      align-items: center;
      justify-content: space-between;
      max-width: 1100px;
      margin: 0 auto;
      padding: 24px 40px;
      border-bottom: 1px solid var(--geo-driftwood);
    }

    nav a.logo {
      font-family: 'Josefin Sans', sans-serif;
      font-weight: 300;
      font-size: 1.4rem;
      color: var(--geo-charcoal);
      text-decoration: none;
      letter-spacing: 0.1em;
      text-transform: uppercase;
    }

    nav ul {
      display: flex;
      gap: 32px;
      list-style: none;
    }

    nav ul a {
      color: var(--geo-ash);
      text-decoration: none;
      font-family: 'Josefin Sans', sans-serif;
      font-weight: 400;
      font-size: 0.8rem;
      letter-spacing: 0.14em;
      text-transform: uppercase;
      transition: color 0.3s;
    }

    nav ul a:hover { color: var(--geo-terracotta); }

    /* Hero */
    .hero {
      text-align: center;
      max-width: 800px;
      margin: 0 auto;
      padding: 100px 40px 60px;
      position: relative;
    }

    .hero h1 {
      font-size: clamp(2.2rem, 5.5vw, 4rem);
      letter-spacing: 0.08em;
      text-transform: uppercase;
      margin-bottom: 1.5rem;
    }

    .hero p {
      font-size: 1.05rem;
      color: var(--geo-ash);
      max-width: 520px;
      margin: 0 auto 2.5rem;
    }

    /* Decorative triangle behind hero */
    .hero::before {
      content: '';
      position: absolute;
      top: 50%;
      left: 50%;
      transform: translate(-50%, -50%);
      width: 0;
      height: 0;
      border-left: 180px solid transparent;
      border-right: 180px solid transparent;
      border-bottom: 310px solid rgba(166, 92, 50, 0.03);
      pointer-events: none;
      z-index: -1;
    }

    /* Button */
    .btn {
      display: inline-block;
      background: transparent;
      color: var(--geo-terracotta);
      border: 1.5px solid var(--geo-terracotta);
      padding: 12px 40px;
      font-family: 'Josefin Sans', sans-serif;
      font-weight: 400;
      font-size: 0.8rem;
      letter-spacing: 0.12em;
      text-transform: uppercase;
      text-decoration: none;
      cursor: pointer;
      transition: all 0.3s;
    }

    .btn:hover {
      background: var(--geo-terracotta);
      color: var(--geo-parchment);
    }

    /* Geometric divider */
    .divider {
      display: flex;
      align-items: center;
      justify-content: center;
      gap: 12px;
      padding: 20px 0;
    }

    .divider::before,
    .divider::after {
      content: '';
      width: 60px;
      height: 1px;
      background: var(--geo-driftwood);
    }

    .divider span {
      width: 8px;
      height: 8px;
      background: var(--geo-terracotta);
      transform: rotate(45deg);
    }

    /* Features section */
    .features {
      background: var(--geo-linen);
      padding: 80px 0;
      position: relative;
    }

    /* Triangular background pattern */
    .features::before {
      content: '';
      position: absolute;
      inset: 0;
      background-image: url("data:image/svg+xml,%3Csvg width='60' height='52' viewBox='0 0 60 52' xmlns='http://www.w3.org/2000/svg'%3E%3Cpath d='M30 0 L60 52 L0 52 Z' fill='none' stroke='%23c9b5ae' stroke-width='0.5'/%3E%3C/svg%3E");
      background-size: 60px 52px;
      opacity: 0.1;
      pointer-events: none;
    }

    .features h2 {
      text-align: center;
      font-size: 2rem;
      letter-spacing: 0.06em;
      text-transform: uppercase;
      margin-bottom: 12px;
    }

    .features .subtitle {
      text-align: center;
      font-family: 'Amatic SC', cursive;
      font-size: 1.3rem;
      color: var(--geo-terracotta);
      letter-spacing: 0.08em;
      margin-bottom: 48px;
    }

    .features-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
      gap: 32px;
      max-width: 1100px;
      margin: 0 auto;
      padding: 0 40px;
      position: relative;
      z-index: 1;
    }

    .feature {
      background: var(--geo-parchment);
      border: 1px solid var(--geo-driftwood);
      padding: 36px;
      text-align: center;
      position: relative;
    }

    /* Corner accents */
    .feature::before {
      content: '';
      position: absolute;
      top: 8px;
      left: 8px;
      width: 16px;
      height: 16px;
      border-top: 1px solid var(--geo-warm-clay);
      border-left: 1px solid var(--geo-warm-clay);
    }

    .feature::after {
      content: '';
      position: absolute;
      bottom: 8px;
      right: 8px;
      width: 16px;
      height: 16px;
      border-bottom: 1px solid var(--geo-warm-clay);
      border-right: 1px solid var(--geo-warm-clay);
    }

    .feature-icon {
      width: 64px;
      height: 64px;
      margin: 0 auto 20px;
      display: flex;
      align-items: center;
      justify-content: center;
    }

    .feature h3 {
      margin-bottom: 0.75rem;
      font-size: 1.15rem;
      letter-spacing: 0.03em;
    }

    .feature p {
      color: var(--geo-ash);
      font-size: 0.9rem;
      line-height: 1.7;
    }

    /* CTA section */
    .cta {
      background: var(--geo-bleached);
      text-align: center;
      padding: 80px 40px;
    }

    .cta h2 {
      font-size: clamp(1.8rem, 4vw, 2.5rem);
      letter-spacing: 0.06em;
      text-transform: uppercase;
      margin-bottom: 1rem;
    }

    .cta p {
      font-size: 1rem;
      color: var(--geo-ash);
      margin-bottom: 2rem;
      max-width: 480px;
      margin-left: auto;
      margin-right: auto;
    }

    .cta .btn {
      background: var(--geo-terracotta);
      color: var(--geo-parchment);
      border-color: var(--geo-terracotta);
    }

    .cta .btn:hover {
      background: var(--geo-sienna);
      border-color: var(--geo-sienna);
    }

    /* Footer */
    footer {
      background: var(--geo-charcoal);
      color: var(--geo-driftwood);
      text-align: center;
      padding: 40px;
      font-size: 0.85rem;
      position: relative;
    }

    footer::before {
      content: '';
      position: absolute;
      top: 0;
      left: 0;
      right: 0;
      height: 3px;
      background: repeating-linear-gradient(
        90deg,
        var(--geo-terracotta) 0px,
        var(--geo-terracotta) 20px,
        transparent 20px,
        transparent 24px,
        var(--geo-sage) 24px,
        var(--geo-sage) 44px,
        transparent 44px,
        transparent 48px
      );
    }

    @media (max-width: 768px) {
      .hero {
        padding: 60px 24px 40px;
      }
      .hero::before { display: none; }
      nav { padding: 16px 24px; }
      nav ul { gap: 20px; }
    }
  </style>
</head>
<body>
  <nav>
    <a href="#" class="logo">Geo-Boho</a>
    <ul>
      <li><a href="#">Explore</a></li>
      <li><a href="#">Gallery</a></li>
      <li><a href="#">Journal</a></li>
      <li><a href="#">About</a></li>
    </ul>
  </nav>

  <section class="hero">
    <h1>Where Geometry Meets Soul</h1>
    <p>Structured lines and free-spirited warmth converge in designs that honor both precision and the handcrafted.</p>
    <a href="#" class="btn">Discover More</a>
  </section>

  <div class="divider"><span></span></div>

  <section class="features">
    <h2>Our Principles</h2>
    <div class="subtitle">crafted with intention</div>
    <div class="features-grid">
      <div class="feature">
        <div class="feature-icon">
          <svg width="48" height="48" viewBox="0 0 48 48" fill="none">
            <!-- Triangle icon -->
            <path d="M24 6 L44 42 L4 42 Z" stroke="#a65c32" stroke-width="1.5" fill="none"/>
            <circle cx="24" cy="30" r="6" stroke="#728c82" stroke-width="1" fill="none"/>
          </svg>
        </div>
        <h3>Geometric Foundation</h3>
        <p>Every design begins with triangular grids and precise line-work, creating structure that grounds the composition.</p>
      </div>
      <div class="feature">
        <div class="feature-icon">
          <svg width="48" height="48" viewBox="0 0 48 48" fill="none">
            <!-- Circle with inner pattern -->
            <circle cx="24" cy="24" r="20" stroke="#a65c32" stroke-width="1.5" fill="none"/>
            <circle cx="24" cy="24" r="12" stroke="#bf8d7a" stroke-width="1" fill="none"/>
            <circle cx="24" cy="24" r="4" stroke="#728c82" stroke-width="1" fill="none"/>
            <line x1="24" y1="4" x2="24" y2="44" stroke="#c9b5ae" stroke-width="0.5"/>
            <line x1="4" y1="24" x2="44" y2="24" stroke="#c9b5ae" stroke-width="0.5"/>
          </svg>
        </div>
        <h3>Natural Harmony</h3>
        <p>Warm, earthy palettes and organic textures soften geometric precision into something deeply human.</p>
      </div>
      <div class="feature">
        <div class="feature-icon">
          <svg width="48" height="48" viewBox="0 0 48 48" fill="none">
            <!-- Diamond with lines -->
            <path d="M24 4 L44 24 L24 44 L4 24 Z" stroke="#a65c32" stroke-width="1.5" fill="none"/>
            <path d="M24 12 L36 24 L24 36 L12 24 Z" stroke="#bf8d7a" stroke-width="1" fill="none"/>
          </svg>
        </div>
        <h3>Intentional Craft</h3>
        <p>Each element is placed with purpose, blending the precision of vectors with the soul of handmade artistry.</p>
      </div>
    </div>
  </section>

  <div class="divider"><span></span></div>

  <section class="cta">
    <h2>Begin Your Journey</h2>
    <p>Embrace the balance between structure and spirit, precision and warmth.</p>
    <a href="#" class="btn">Get Started</a>
  </section>

  <footer>
    <p>Crafted with geometric intention and bohemian soul.</p>
  </footer>
</body>
</html>
```
