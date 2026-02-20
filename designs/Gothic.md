# Gothic Design Reference

Gothic is one of the most influential design movements in Western history, originating in 12th-century France with the construction of the Basilica of Saint-Denis and spreading across Europe for over four centuries. Defined by its dramatic verticality, pointed arches, ribbed vaults, flying buttresses, stained glass windows, and ornate stone tracery, the Gothic style sought to dissolve solid walls into luminous, soaring spaces that directed the eye and spirit upward. In modern web and UI design, the Gothic aesthetic translates into dark, atmospheric palettes built on near-blacks, deep purples, and crimsons; ornate decorative frameworks inspired by tracery and rose windows; blackletter and high-contrast serif typography; pointed arch motifs used as frames and dividers; and stained-glass-inspired color work where jewel tones glow against dark leading lines. The result is design that feels weighty, dramatic, and richly layered -- evoking the grandeur and mystery of medieval cathedrals while remaining functional for modern interfaces.

---

## Visual Characteristics

### Core Design Traits

- **Pointed arch motifs** -- the signature Gothic form; used as frames for cards, navigation elements, hero sections, and decorative borders to establish the aesthetic immediately
- **Dramatic verticality** -- tall, narrow proportions that echo cathedral naves; content is stacked and elongated rather than spread horizontally, creating a sense of upward aspiration
- **Stained glass color work** -- jewel-toned panels (deep blue, ruby red, emerald green, amber gold) set against dark borders that simulate the leading of medieval windows
- **Ornate tracery patterns** -- intricate geometric and curvilinear stone-carved patterns (trefoils, quatrefoils, cinquefoils, mouchettes) adapted as borders, dividers, and background textures
- **Rose window motifs** -- circular, radially symmetric decorative elements used as hero focal points, section dividers, or ornamental backgrounds
- **Dark atmospheric grounding** -- deep, shadowed backgrounds (near-black, dark stone gray, midnight blue) that make illuminated content elements feel as though they glow from within
- **Ribbed vault and fan vault patterns** -- intersecting curved lines radiating from points, used as ceiling-like background patterns or decorative overlays
- **Gargoyle and grotesque ornamentation** -- sculptural, often menacing decorative elements used sparingly as icons, corner embellishments, or illustrative accents
- **Flying buttress structural metaphors** -- visible supporting structures and frameworks; exposed grid lines or sidebar supports that reference this engineering innovation
- **Illuminated manuscript influences** -- ornate initial capitals, vine-scroll borders, gold leaf details, and richly decorated text treatments

### Design Principles

- **Weight and gravitas** -- every element should feel substantial and anchored; avoid lightweight, airy, or floating compositions
- **Upward aspiration** -- compositions lead the eye vertically through pointed forms, tall proportions, and layered vertical stacking
- **Light emerging from darkness** -- bright, jewel-toned accents and gold highlights should feel as though they radiate from within a dark surround, like candlelight through stained glass
- **Structural ornamentation** -- decoration is not applied superficially but integrated into the structure itself; borders, frames, and dividers carry ornamental weight
- **Symmetry and bilateral balance** -- Gothic design favors formal symmetry, particularly in headers, navigation, and decorative frameworks
- **Layered depth and texture** -- multiple visual layers (background texture, structural framework, content, ornamental overlay) create richness and complexity
- **Mystery through shadow** -- strategic use of darkness, vignettes, and obscured areas to create atmosphere and intrigue

---

## Color Palette

| Swatch Name | Hex | Role / Usage |
|-------------|-----|-------------|
| Void Black | `#0C0C0F` | Deepest background, shadow areas |
| Cathedral Stone | `#1A1A22` | Primary dark background |
| Cloister Gray | `#2A2A35` | Card and panel backgrounds |
| Gargoyle Gray | `#4A4A58` | Borders, dividers, secondary elements |
| Ash Stone | `#7A7A8A` | Muted text, subtle UI elements |
| Parchment Light | `#D4CFC0` | Primary text on dark backgrounds |
| Stained Ruby | `#8B1A2B` | Primary warm accent, emphasis |
| Cathedral Blue | `#1A3A6B` | Primary cool accent, depth |
| Rose Window Gold | `#C5A033` | Gold highlights, ornamental borders |
| Liturgical Purple | `#4A1A5E` | Tertiary accent, regal emphasis |
| Emerald Glass | `#1A5A3A` | Stained glass green accent |
| Amber Glow | `#D4A020` | Warm highlights, candlelight effects |
| Bone White | `#E8E0D0` | High-contrast text, bright highlights |
| Dried Blood | `#5A1018` | Deep warm accent, Gothic drama |
| Midnight Blue | `#101828` | Alternative dark background, depth |

### CSS Custom Properties

```css
:root {
  /* Backgrounds */
  --gothic-void: #0C0C0F;
  --gothic-stone: #1A1A22;
  --gothic-cloister: #2A2A35;
  --gothic-midnight: #101828;

  /* Stone and Neutral */
  --gothic-gargoyle: #4A4A58;
  --gothic-ash: #7A7A8A;
  --gothic-parchment: #D4CFC0;
  --gothic-bone: #E8E0D0;

  /* Jewel Accents */
  --gothic-ruby: #8B1A2B;
  --gothic-blood: #5A1018;
  --gothic-blue: #1A3A6B;
  --gothic-purple: #4A1A5E;
  --gothic-emerald: #1A5A3A;

  /* Gold and Warm Light */
  --gothic-gold: #C5A033;
  --gothic-amber: #D4A020;

  /* Functional Aliases */
  --gothic-bg-primary: var(--gothic-void);
  --gothic-bg-surface: var(--gothic-stone);
  --gothic-bg-elevated: var(--gothic-cloister);
  --gothic-text-primary: var(--gothic-parchment);
  --gothic-text-bright: var(--gothic-bone);
  --gothic-accent-primary: var(--gothic-gold);
  --gothic-accent-warm: var(--gothic-ruby);
  --gothic-accent-cool: var(--gothic-blue);
  --gothic-border: var(--gothic-gargoyle);
}
```

---

## Typography

### Recommended Google Fonts

| Font | Style | Weight(s) | Usage |
|------|-------|-----------|-------|
| **UnifrakturMaguntia** | Blackletter / Fraktur | 400 | Display headings, hero titles, decorative text |
| **Cinzel** | Inscriptional serif | 400, 500, 600, 700, 900 | Section headings, navigation labels, formal titles |
| **Cinzel Decorative** | Ornamental inscriptional serif | 400, 700, 900 | Hero display text, ornamental headings |
| **Playfair Display** | High-contrast transitional serif | 400-900 | Subheadings, editorial content |
| **EB Garamond** | Classical old-style serif | 400-800 | Body text, long-form reading |
| **Cormorant** | Refined display serif | 300-700 | Pull quotes, feature text, large subheadings |
| **MedievalSharp** | Medieval-inspired serif | 400 | Decorative labels, accent text, stylized UI elements |
| **Spectral** | Screen-optimized serif | 300-700 | Body copy, readable long-form content |

### Font Pairing Suggestions

| Heading Font | Body Font | Character |
|-------------|-----------|-----------|
| UnifrakturMaguntia 400 | EB Garamond 400 | Pure Gothic: blackletter display with classical readability |
| Cinzel Decorative 700 | Spectral 400 | Architectural gravitas with comfortable reading |
| Cinzel 600 | Cormorant 400 | Monumental headings with refined literary body |
| Playfair Display 700 | EB Garamond 400 | Editorial Gothic: dramatic contrast with old-style elegance |
| MedievalSharp 400 | Spectral 400 | Medieval character with modern screen readability |

### CSS Example

```css
/* Google Fonts import */
@import url('https://fonts.googleapis.com/css2?family=UnifrakturMaguntia&family=Cinzel:wght@400;600;700;900&family=Cinzel+Decorative:wght@400;700;900&family=EB+Garamond:ital,wght@0,400;0,500;0,600;1,400&family=Cormorant:ital,wght@0,400;0,600;1,400&family=Spectral:ital,wght@0,400;0,600;1,400&display=swap');

/* Display / Hero headings -- blackletter */
.gothic-display {
  font-family: 'UnifrakturMaguntia', 'MedievalSharp', cursive;
  font-size: clamp(2.5rem, 8vw, 6rem);
  color: var(--gothic-gold);
  letter-spacing: 0.03em;
  line-height: 1.1;
  text-shadow: 0 2px 12px rgba(197, 160, 51, 0.3);
}

/* Section headings -- inscriptional */
h1, h2, h3 {
  font-family: 'Cinzel', 'Playfair Display', serif;
  font-weight: 600;
  color: var(--gothic-bone);
  letter-spacing: 0.08em;
  text-transform: uppercase;
  line-height: 1.2;
}

h1 { font-size: clamp(2rem, 5vw, 3.5rem); }
h2 { font-size: clamp(1.5rem, 3.5vw, 2.5rem); }
h3 { font-size: clamp(1.2rem, 2.5vw, 1.8rem); }

/* Body text */
body {
  font-family: 'EB Garamond', 'Spectral', 'Cormorant', serif;
  font-weight: 400;
  font-size: 1.1rem;
  line-height: 1.8;
  letter-spacing: 0.02em;
  color: var(--gothic-parchment);
}

/* Decorative accent text */
.gothic-accent-text {
  font-family: 'Cormorant', serif;
  font-style: italic;
  font-size: 1.4em;
  color: var(--gothic-gold);
  letter-spacing: 0.04em;
}

/* Small caps for labels and navigation */
.gothic-small-caps {
  font-family: 'Cinzel', serif;
  font-variant: small-caps;
  font-size: 0.85rem;
  letter-spacing: 0.15em;
  color: var(--gothic-ash);
}
```

---

## Layout Principles

- **Centered, symmetrical compositions** -- Gothic design favors bilateral symmetry; center main content with balanced flanking elements, echoing the symmetry of cathedral facades
- **Tall, narrow containers** -- favor portrait-oriented cards and panels with generous vertical padding; avoid wide, squat layouts
- **Layered z-depth** -- use multiple background layers (dark base, textured overlay, ornamental framework, content) to create cathedral-like visual depth
- **Generous vertical spacing** -- sections should breathe with ample margin, suggesting the soaring height of Gothic interiors
- **Ornamental framing** -- content panels are enclosed in decorative borders with pointed arch tops, tracery corners, or ornamental rules
- **Dark canvas, illuminated content** -- the background is predominantly dark; content areas and accent elements provide the light, like windows in a stone wall
- **Sidebar buttressing** -- secondary navigation or supplementary content in narrow side columns that visually "support" the main content, referencing flying buttresses
- **Grid with gothic proportions** -- use narrow columns with tall rows; a 3-column or 5-column grid with a dominant center column works well
- **Decorative section dividers** -- use ornamental rules, pointed arch separators, or tracery-inspired SVG dividers between sections rather than plain horizontal lines

---

## CSS / Design Techniques

### Gothic Card Component

```css
.gothic-card {
  background: var(--gothic-stone);
  border: 1px solid var(--gothic-gargoyle);
  padding: 2rem 1.5rem 2.5rem;
  position: relative;
  text-align: center;
  overflow: hidden;
  transition: border-color 0.4s ease, box-shadow 0.4s ease;
}

/* Pointed arch top using clip-path */
.gothic-card::before {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  height: 6px;
  background: linear-gradient(90deg,
    transparent 0%,
    var(--gothic-gold) 20%,
    var(--gothic-gold) 80%,
    transparent 100%
  );
  clip-path: polygon(0 100%, 50% 0%, 100% 100%);
}

/* Inner glow effect */
.gothic-card::after {
  content: '';
  position: absolute;
  inset: 0;
  background: radial-gradient(
    ellipse at 50% 0%,
    rgba(197, 160, 51, 0.06) 0%,
    transparent 60%
  );
  pointer-events: none;
}

.gothic-card:hover {
  border-color: var(--gothic-gold);
  box-shadow:
    0 0 20px rgba(197, 160, 51, 0.1),
    0 8px 30px rgba(0, 0, 0, 0.4);
}

.gothic-card h3 {
  font-family: 'Cinzel', serif;
  font-weight: 600;
  letter-spacing: 0.1em;
  text-transform: uppercase;
  color: var(--gothic-gold);
  margin-bottom: 1rem;
}

.gothic-card p {
  font-family: 'EB Garamond', serif;
  color: var(--gothic-parchment);
  line-height: 1.7;
}
```

### Gothic Button Component

```css
.gothic-btn {
  display: inline-block;
  font-family: 'Cinzel', serif;
  font-weight: 600;
  font-size: 0.85rem;
  letter-spacing: 0.15em;
  text-transform: uppercase;
  color: var(--gothic-gold);
  background: transparent;
  border: 1px solid var(--gothic-gold);
  padding: 0.8rem 2.5rem;
  cursor: pointer;
  position: relative;
  overflow: hidden;
  transition: all 0.4s ease;
}

/* Pointed bracket decorations */
.gothic-btn::before,
.gothic-btn::after {
  content: '';
  position: absolute;
  width: 8px;
  height: 8px;
  border: 1px solid var(--gothic-gold);
  transition: all 0.4s ease;
}

.gothic-btn::before {
  top: 4px;
  left: 4px;
  border-right: none;
  border-bottom: none;
}

.gothic-btn::after {
  bottom: 4px;
  right: 4px;
  border-left: none;
  border-top: none;
}

.gothic-btn:hover {
  background: var(--gothic-gold);
  color: var(--gothic-void);
  box-shadow: 0 0 20px rgba(197, 160, 51, 0.25);
}

.gothic-btn:hover::before,
.gothic-btn:hover::after {
  width: 12px;
  height: 12px;
}

/* Ruby variant */
.gothic-btn--ruby {
  color: var(--gothic-ruby);
  border-color: var(--gothic-ruby);
}

.gothic-btn--ruby:hover {
  background: var(--gothic-ruby);
  color: var(--gothic-bone);
  box-shadow: 0 0 20px rgba(139, 26, 43, 0.3);
}
```

### Gothic Navigation Bar

```css
.gothic-nav {
  background: var(--gothic-void);
  border-bottom: 1px solid var(--gothic-gargoyle);
  padding: 0;
  position: sticky;
  top: 0;
  z-index: 100;
}

.gothic-nav-inner {
  max-width: 1200px;
  margin: 0 auto;
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 0;
}

.gothic-nav-brand {
  font-family: 'UnifrakturMaguntia', cursive;
  font-size: 1.6rem;
  color: var(--gothic-gold);
  padding: 1rem 2rem;
  text-decoration: none;
  white-space: nowrap;
}

.gothic-nav-links {
  display: flex;
  list-style: none;
  margin: 0;
  padding: 0;
}

.gothic-nav-links a {
  display: block;
  font-family: 'Cinzel', serif;
  font-size: 0.75rem;
  font-weight: 600;
  letter-spacing: 0.2em;
  text-transform: uppercase;
  color: var(--gothic-ash);
  text-decoration: none;
  padding: 1.5rem 1.5rem;
  position: relative;
  transition: color 0.3s ease;
}

.gothic-nav-links a::after {
  content: '';
  position: absolute;
  bottom: 0;
  left: 50%;
  transform: translateX(-50%);
  width: 0;
  height: 2px;
  background: var(--gothic-gold);
  transition: width 0.3s ease;
}

.gothic-nav-links a:hover {
  color: var(--gothic-gold);
}

.gothic-nav-links a:hover::after {
  width: 60%;
}

/* Ornamental center divider between brand and links */
.gothic-nav-divider {
  width: 1px;
  height: 30px;
  background: linear-gradient(
    to bottom,
    transparent,
    var(--gothic-gargoyle),
    transparent
  );
  margin: 0 1rem;
}
```

### Gothic Hero Section

```css
.gothic-hero {
  background: var(--gothic-void);
  min-height: 100vh;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  text-align: center;
  padding: 4rem 2rem;
  position: relative;
  overflow: hidden;
}

/* Radial vignette overlay */
.gothic-hero::before {
  content: '';
  position: absolute;
  inset: 0;
  background: radial-gradient(
    ellipse at 50% 50%,
    transparent 30%,
    rgba(12, 12, 15, 0.8) 100%
  );
  pointer-events: none;
}

/* Subtle stone texture overlay */
.gothic-hero::after {
  content: '';
  position: absolute;
  inset: 0;
  background-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='4' height='4'%3E%3Crect width='4' height='4' fill='%231A1A22'/%3E%3Crect width='1' height='1' x='1' y='1' fill='%23222230' opacity='0.3'/%3E%3C/svg%3E");
  background-size: 4px 4px;
  opacity: 0.5;
  pointer-events: none;
}

.gothic-hero-content {
  position: relative;
  z-index: 1;
}

.gothic-hero h1 {
  font-family: 'UnifrakturMaguntia', cursive;
  font-size: clamp(3rem, 10vw, 7rem);
  color: var(--gothic-gold);
  text-shadow:
    0 0 40px rgba(197, 160, 51, 0.2),
    0 4px 20px rgba(0, 0, 0, 0.5);
  margin-bottom: 1rem;
}

.gothic-hero .subtitle {
  font-family: 'Cinzel', serif;
  font-size: clamp(0.9rem, 2vw, 1.2rem);
  font-weight: 400;
  letter-spacing: 0.3em;
  text-transform: uppercase;
  color: var(--gothic-ash);
  margin-bottom: 2.5rem;
}

/* Ornamental rule beneath subtitle */
.gothic-hero .ornament {
  width: 120px;
  height: 20px;
  margin: 0 auto 2.5rem;
  background: no-repeat center / contain;
  background-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 120 20'%3E%3Cpath d='M0,10 L50,10 L60,2 L70,10 L120,10' fill='none' stroke='%23C5A033' stroke-width='1'/%3E%3Ccircle cx='60' cy='2' r='2' fill='%23C5A033'/%3E%3Ccircle cx='0' cy='10' r='1.5' fill='%23C5A033'/%3E%3Ccircle cx='120' cy='10' r='1.5' fill='%23C5A033'/%3E%3C/svg%3E");
  opacity: 0.7;
}
```

### Pointed Arch Frame

```css
/* A container with a pointed arch top, suitable for framing
   images, feature content, or decorative sections */
.gothic-arch-frame {
  position: relative;
  max-width: 400px;
  margin: 2rem auto;
  padding: 3rem 2rem 2rem;
  background: var(--gothic-stone);
  border: 1px solid var(--gothic-gargoyle);
  text-align: center;
}

/* Pointed arch top created with borders */
.gothic-arch-frame::before {
  content: '';
  position: absolute;
  top: -40px;
  left: 50%;
  transform: translateX(-50%);
  width: 0;
  height: 0;
  border-left: 200px solid transparent;
  border-right: 200px solid transparent;
  border-bottom: 40px solid var(--gothic-stone);
  filter: drop-shadow(0 -1px 0 var(--gothic-gargoyle));
}

/* Gold keystone accent at the apex */
.gothic-arch-frame::after {
  content: '';
  position: absolute;
  top: -8px;
  left: 50%;
  transform: translateX(-50%);
  width: 12px;
  height: 12px;
  background: var(--gothic-gold);
  clip-path: polygon(50% 0%, 100% 50%, 50% 100%, 0% 50%);
}

/* SVG pointed arch alternative using clip-path */
.gothic-arch-clip {
  clip-path: polygon(
    0% 15%,
    5% 8%,
    15% 3%,
    30% 0.5%,
    50% 0%,
    70% 0.5%,
    85% 3%,
    95% 8%,
    100% 15%,
    100% 100%,
    0% 100%
  );
  background: var(--gothic-stone);
  padding: 4rem 2rem 2rem;
}
```

### Stained Glass Panel Effect

```css
/* Grid of colored panels with dark "leading" borders,
   simulating a stained glass window */
.gothic-stained-glass {
  display: grid;
  grid-template-columns: repeat(4, 1fr);
  grid-template-rows: auto;
  gap: 3px;
  background: var(--gothic-void); /* dark leading between panes */
  padding: 3px;
  border: 2px solid var(--gothic-gargoyle);
  border-radius: 0;
  max-width: 600px;
  margin: 2rem auto;
}

.gothic-stained-glass > * {
  padding: 2rem 1rem;
  text-align: center;
  font-family: 'Cinzel', serif;
  font-size: 0.8rem;
  letter-spacing: 0.1em;
  text-transform: uppercase;
}

/* Jewel-toned glass panes */
.gothic-glass-ruby {
  background: rgba(139, 26, 43, 0.25);
  color: #e8a0a8;
}

.gothic-glass-blue {
  background: rgba(26, 58, 107, 0.3);
  color: #8ab0e0;
}

.gothic-glass-emerald {
  background: rgba(26, 90, 58, 0.25);
  color: #80c8a0;
}

.gothic-glass-amber {
  background: rgba(212, 160, 32, 0.2);
  color: #e8d080;
}

.gothic-glass-purple {
  background: rgba(74, 26, 94, 0.25);
  color: #c090d8;
}

/* Center panel spanning 2 columns for rose window effect */
.gothic-glass-center {
  grid-column: span 2;
  background: radial-gradient(
    circle at 50% 50%,
    rgba(197, 160, 51, 0.15) 0%,
    rgba(139, 26, 43, 0.12) 40%,
    rgba(26, 58, 107, 0.15) 70%,
    transparent 100%
  );
  color: var(--gothic-gold);
}
```

### Rose Window Ornament

```css
/* Decorative rose window motif using layered radial gradients
   and pseudo-elements -- purely ornamental */
.gothic-rose-window {
  width: 200px;
  height: 200px;
  border-radius: 50%;
  margin: 2rem auto;
  position: relative;
  background:
    radial-gradient(circle at 50% 50%,
      var(--gothic-gold) 0%,
      var(--gothic-gold) 4%,
      transparent 4.5%,
      transparent 12%,
      rgba(139, 26, 43, 0.3) 12%,
      rgba(139, 26, 43, 0.3) 18%,
      transparent 18.5%,
      transparent 25%,
      rgba(26, 58, 107, 0.25) 25%,
      rgba(26, 58, 107, 0.25) 32%,
      transparent 32.5%,
      transparent 40%,
      rgba(74, 26, 94, 0.2) 40%,
      rgba(74, 26, 94, 0.2) 48%,
      transparent 48.5%,
      transparent 58%,
      rgba(26, 90, 58, 0.2) 58%,
      rgba(26, 90, 58, 0.2) 66%,
      transparent 66.5%,
      transparent 78%,
      var(--gothic-gargoyle) 78%,
      var(--gothic-gargoyle) 80%,
      transparent 80.5%
    );
  border: 3px solid var(--gothic-gargoyle);
  box-shadow:
    0 0 30px rgba(197, 160, 51, 0.15),
    inset 0 0 20px rgba(0, 0, 0, 0.3);
}

/* Radial "spokes" overlay */
.gothic-rose-window::before {
  content: '';
  position: absolute;
  inset: 0;
  border-radius: 50%;
  background:
    repeating-conic-gradient(
      from 0deg,
      transparent 0deg,
      transparent 14deg,
      rgba(74, 74, 88, 0.3) 14deg,
      rgba(74, 74, 88, 0.3) 16deg
    );
}

/* Center jewel */
.gothic-rose-window::after {
  content: '';
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  width: 14px;
  height: 14px;
  background: var(--gothic-gold);
  border-radius: 50%;
  box-shadow: 0 0 10px rgba(197, 160, 51, 0.5);
}
```

### Tracery Border Ornament

```css
/* Decorative tracery-inspired border using SVG background
   with trefoil and pointed arch patterns */
.gothic-tracery-border {
  border: none;
  height: 40px;
  margin: 2rem 0;
  background: no-repeat center / 100% 100%;
  background-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 600 40'%3E%3C!-- pointed arch repeating pattern --%3E%3Cpath d='M0,40 L0,20 Q25,0 50,20 L50,40' fill='none' stroke='%234A4A58' stroke-width='1'/%3E%3Cpath d='M50,40 L50,20 Q75,0 100,20 L100,40' fill='none' stroke='%234A4A58' stroke-width='1'/%3E%3Cpath d='M100,40 L100,20 Q125,0 150,20 L150,40' fill='none' stroke='%234A4A58' stroke-width='1'/%3E%3Cpath d='M150,40 L150,20 Q175,0 200,20 L200,40' fill='none' stroke='%234A4A58' stroke-width='1'/%3E%3Cpath d='M200,40 L200,20 Q225,0 250,20 L250,40' fill='none' stroke='%234A4A58' stroke-width='1'/%3E%3Cpath d='M250,40 L250,20 Q275,0 300,20 L300,40' fill='none' stroke='%234A4A58' stroke-width='1'/%3E%3Cpath d='M300,40 L300,20 Q325,0 350,20 L350,40' fill='none' stroke='%234A4A58' stroke-width='1'/%3E%3Cpath d='M350,40 L350,20 Q375,0 400,20 L400,40' fill='none' stroke='%234A4A58' stroke-width='1'/%3E%3Cpath d='M400,40 L400,20 Q425,0 450,20 L450,40' fill='none' stroke='%234A4A58' stroke-width='1'/%3E%3Cpath d='M450,40 L450,20 Q475,0 500,20 L500,40' fill='none' stroke='%234A4A58' stroke-width='1'/%3E%3Cpath d='M500,40 L500,20 Q525,0 550,20 L550,40' fill='none' stroke='%234A4A58' stroke-width='1'/%3E%3Cpath d='M550,40 L550,20 Q575,0 600,20 L600,40' fill='none' stroke='%234A4A58' stroke-width='1'/%3E%3C!-- trefoil accents at arch intersections --%3E%3Ccircle cx='50' cy='22' r='3' fill='none' stroke='%23C5A033' stroke-width='0.8'/%3E%3Ccircle cx='150' cy='22' r='3' fill='none' stroke='%23C5A033' stroke-width='0.8'/%3E%3Ccircle cx='250' cy='22' r='3' fill='none' stroke='%23C5A033' stroke-width='0.8'/%3E%3Ccircle cx='350' cy='22' r='3' fill='none' stroke='%23C5A033' stroke-width='0.8'/%3E%3Ccircle cx='450' cy='22' r='3' fill='none' stroke='%23C5A033' stroke-width='0.8'/%3E%3Ccircle cx='550' cy='22' r='3' fill='none' stroke='%23C5A033' stroke-width='0.8'/%3E%3C/svg%3E");
  opacity: 0.8;
}

/* Simpler CSS-only trefoil divider */
.gothic-trefoil-divider {
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 6px;
  margin: 2rem auto;
  width: fit-content;
}

.gothic-trefoil-divider::before,
.gothic-trefoil-divider::after {
  content: '';
  width: 80px;
  height: 1px;
  background: linear-gradient(
    90deg,
    transparent,
    var(--gothic-gargoyle),
    transparent
  );
}

/* Use a trefoil character or SVG as the center element */
.gothic-trefoil-divider span {
  color: var(--gothic-gold);
  font-size: 1rem;
  line-height: 1;
}
```

### Gothic Text Glow Effect

```css
/* Illuminated text effect -- text that appears to glow
   as if lit by candlelight or stained glass light */
.gothic-glow-text {
  color: var(--gothic-gold);
  text-shadow:
    0 0 8px rgba(197, 160, 51, 0.4),
    0 0 20px rgba(197, 160, 51, 0.2),
    0 0 40px rgba(197, 160, 51, 0.1);
}

/* Ruby glow variant */
.gothic-glow-text--ruby {
  color: #c83040;
  text-shadow:
    0 0 8px rgba(139, 26, 43, 0.5),
    0 0 20px rgba(139, 26, 43, 0.3),
    0 0 40px rgba(139, 26, 43, 0.15);
}

/* Animated candlelight flicker */
@keyframes gothic-flicker {
  0%, 100% { text-shadow: 0 0 8px rgba(197, 160, 51, 0.4), 0 0 20px rgba(197, 160, 51, 0.2); }
  25% { text-shadow: 0 0 12px rgba(197, 160, 51, 0.5), 0 0 30px rgba(197, 160, 51, 0.25); }
  50% { text-shadow: 0 0 6px rgba(197, 160, 51, 0.35), 0 0 16px rgba(197, 160, 51, 0.15); }
  75% { text-shadow: 0 0 10px rgba(197, 160, 51, 0.45), 0 0 25px rgba(197, 160, 51, 0.22); }
}

.gothic-flicker {
  animation: gothic-flicker 3s ease-in-out infinite;
}
```

---

## Design Do's and Don'ts

### Do's

- **Do use deep, dark backgrounds** as the foundation -- near-black or very dark cool grays create the essential Gothic atmosphere
- **Do use gold and jewel tones sparingly** as accents against darkness; restraint creates impact
- **Do employ pointed arch shapes** in frames, clip-paths, and decorative elements to reinforce the Gothic vocabulary
- **Do pair blackletter display fonts with readable serif body fonts** -- legibility must never be sacrificed for style
- **Do create layered depth** with overlapping backgrounds, textures, borders, and content for richness
- **Do use symmetrical, centered layouts** for headers, hero sections, and navigation to echo cathedral facades
- **Do add subtle texture** (stone grain, noise overlays, parchment patterns) to flat backgrounds for tactile quality
- **Do use ornamental dividers and rules** between sections instead of plain horizontal lines
- **Do let content glow from darkness** -- use radial gradients, text shadows, and box shadows to simulate light emanating from within

### Don'ts

- **Don't use bright, saturated backgrounds** -- Gothic is built on darkness; bright backgrounds destroy the atmosphere entirely
- **Don't overuse blackletter fonts** -- reserve them for display headings and titles only; body text must be readable serif
- **Don't make the palette monotonously black** -- without jewel-toned accents and gold highlights, the design becomes flat and lifeless
- **Don't use rounded, bubbly shapes** -- Gothic is angular, pointed, and sharp; rounded corners and pill shapes contradict the aesthetic
- **Don't use sans-serif fonts** for primary typography -- sans-serif belongs to modernist and minimalist aesthetics, not Gothic
- **Don't ignore accessibility** -- dark interfaces need sufficient text contrast; ensure parchment/bone text on dark backgrounds meets WCAG AA (4.5:1) standards
- **Don't clutter with too many ornaments** -- Gothic ornamentation is structured and architectural, not chaotic; each decorative element should have purpose and placement
- **Don't use flat, matte design** -- Gothic demands texture, depth, shadow, and subtle gradients; purely flat UI loses the atmospheric quality

---

## Related Aesthetics

| Aesthetic | Relationship to Gothic |
|-----------|----------------------|
| **Industrial Gothic** | Fuses Gothic atmosphere with heavy machinery, decay, and mechanical dread; Gothic provides the darkness and drama, Industrial adds technological blight |
| **Whimsigothic** | Playful, nature-infused reinterpretation of Gothic; retains the dark palette and pointed forms but adds whimsy, plants, moons, and softer edges |
| **Dark Academia** | Shares Gothic's dark palette, classical typography, and architectural references; Dark Academia focuses on scholarly themes while Gothic emphasizes the architectural and spiritual |
| **Medievalcore** | Broader medieval aesthetic that includes Gothic elements alongside heraldry, armor, tapestries, and illuminated manuscripts |
| **Baroque** | Successor movement that amplified Gothic's ornamentation into extravagant excess; shares the love of drama, gold, and layered complexity |
| **Art Nouveau** | Inherited Gothic's organic tracery and stained glass traditions, transforming pointed arches into sinuous whiplash curves |
| **Cyberpunk** | Both use dark foundations with vivid accent lighting; Cyberpunk replaces stone and gold with neon and chrome |
| **Dark Mode Neon** | Shares the dark-background-with-vivid-accents approach but uses modern neon colors instead of Gothic jewel tones |

---

## Quick-Start HTML Template

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Gothic Design Template</title>
  <link href="https://fonts.googleapis.com/css2?family=UnifrakturMaguntia&family=Cinzel:wght@400;600;700;900&family=Cinzel+Decorative:wght@400;700;900&family=EB+Garamond:ital,wght@0,400;0,500;0,600;1,400&family=Cormorant:ital,wght@0,400;0,600;1,400&display=swap" rel="stylesheet">
  <style>
    /* ============================================
       GOTHIC DESIGN SYSTEM -- CSS Custom Properties
       ============================================ */
    :root {
      --gothic-void: #0C0C0F;
      --gothic-stone: #1A1A22;
      --gothic-cloister: #2A2A35;
      --gothic-midnight: #101828;
      --gothic-gargoyle: #4A4A58;
      --gothic-ash: #7A7A8A;
      --gothic-parchment: #D4CFC0;
      --gothic-bone: #E8E0D0;
      --gothic-ruby: #8B1A2B;
      --gothic-blood: #5A1018;
      --gothic-blue: #1A3A6B;
      --gothic-purple: #4A1A5E;
      --gothic-emerald: #1A5A3A;
      --gothic-gold: #C5A033;
      --gothic-amber: #D4A020;
    }

    /* ============================================
       RESET & BASE
       ============================================ */
    *, *::before, *::after {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    html {
      scroll-behavior: smooth;
    }

    body {
      background: var(--gothic-void);
      color: var(--gothic-parchment);
      font-family: 'EB Garamond', 'Cormorant', serif;
      font-size: 1.1rem;
      line-height: 1.8;
      letter-spacing: 0.02em;
      min-height: 100vh;
    }

    a {
      color: var(--gothic-gold);
      text-decoration: none;
      transition: color 0.3s ease;
    }

    a:hover {
      color: var(--gothic-amber);
    }

    img {
      max-width: 100%;
      display: block;
    }

    /* ============================================
       NAVIGATION
       ============================================ */
    .nav {
      background: var(--gothic-void);
      border-bottom: 1px solid var(--gothic-gargoyle);
      position: sticky;
      top: 0;
      z-index: 100;
    }

    .nav-inner {
      max-width: 1000px;
      margin: 0 auto;
      display: flex;
      align-items: center;
      justify-content: center;
      flex-wrap: wrap;
      padding: 0 1rem;
    }

    .nav-brand {
      font-family: 'UnifrakturMaguntia', cursive;
      font-size: 1.5rem;
      color: var(--gothic-gold);
      padding: 0.8rem 1.5rem;
      text-decoration: none;
    }

    .nav-divider {
      width: 1px;
      height: 24px;
      background: linear-gradient(to bottom, transparent, var(--gothic-gargoyle), transparent);
      margin: 0 0.5rem;
    }

    .nav-links {
      display: flex;
      list-style: none;
      gap: 0;
    }

    .nav-links a {
      display: block;
      font-family: 'Cinzel', serif;
      font-size: 0.7rem;
      font-weight: 600;
      letter-spacing: 0.18em;
      text-transform: uppercase;
      color: var(--gothic-ash);
      padding: 1.2rem 1rem;
      position: relative;
    }

    .nav-links a::after {
      content: '';
      position: absolute;
      bottom: 0;
      left: 50%;
      transform: translateX(-50%);
      width: 0;
      height: 2px;
      background: var(--gothic-gold);
      transition: width 0.3s ease;
    }

    .nav-links a:hover {
      color: var(--gothic-gold);
    }

    .nav-links a:hover::after {
      width: 70%;
    }

    /* ============================================
       HERO SECTION
       ============================================ */
    .hero {
      min-height: 100vh;
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      text-align: center;
      padding: 4rem 2rem;
      position: relative;
      overflow: hidden;
      background:
        radial-gradient(
          ellipse at 50% 40%,
          rgba(26, 58, 107, 0.08) 0%,
          transparent 50%
        ),
        radial-gradient(
          ellipse at 50% 60%,
          rgba(139, 26, 43, 0.05) 0%,
          transparent 50%
        ),
        var(--gothic-void);
    }

    /* Vignette */
    .hero::before {
      content: '';
      position: absolute;
      inset: 0;
      background: radial-gradient(
        ellipse at 50% 50%,
        transparent 40%,
        rgba(12, 12, 15, 0.7) 100%
      );
      pointer-events: none;
    }

    /* Stone noise texture */
    .hero::after {
      content: '';
      position: absolute;
      inset: 0;
      background-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='4' height='4'%3E%3Crect width='4' height='4' fill='%231A1A22'/%3E%3Crect width='1' height='1' x='2' y='0' fill='%23222230' opacity='0.2'/%3E%3Crect width='1' height='1' x='0' y='2' fill='%23222230' opacity='0.15'/%3E%3C/svg%3E");
      background-size: 4px 4px;
      opacity: 0.4;
      pointer-events: none;
    }

    .hero-content {
      position: relative;
      z-index: 1;
    }

    .hero h1 {
      font-family: 'UnifrakturMaguntia', cursive;
      font-size: clamp(3rem, 10vw, 7rem);
      color: var(--gothic-gold);
      line-height: 1.1;
      text-shadow:
        0 0 40px rgba(197, 160, 51, 0.2),
        0 4px 20px rgba(0, 0, 0, 0.6);
      margin-bottom: 0.5rem;
    }

    .hero .subtitle {
      font-family: 'Cinzel', serif;
      font-size: clamp(0.8rem, 2vw, 1.1rem);
      font-weight: 400;
      letter-spacing: 0.3em;
      text-transform: uppercase;
      color: var(--gothic-ash);
      margin-bottom: 2rem;
    }

    /* Pointed ornamental rule */
    .ornament-rule {
      width: 140px;
      height: 24px;
      margin: 0 auto 2.5rem;
      background: no-repeat center / contain;
      background-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 140 24'%3E%3Cline x1='0' y1='12' x2='55' y2='12' stroke='%234A4A58' stroke-width='1'/%3E%3Cline x1='85' y1='12' x2='140' y2='12' stroke='%234A4A58' stroke-width='1'/%3E%3Cpolygon points='70,2 78,12 70,22 62,12' fill='none' stroke='%23C5A033' stroke-width='1'/%3E%3Ccircle cx='70' cy='12' r='2' fill='%23C5A033'/%3E%3Ccircle cx='0' cy='12' r='1.5' fill='%234A4A58'/%3E%3Ccircle cx='140' cy='12' r='1.5' fill='%234A4A58'/%3E%3C/svg%3E");
      opacity: 0.8;
    }

    /* ============================================
       BUTTONS
       ============================================ */
    .btn {
      display: inline-block;
      font-family: 'Cinzel', serif;
      font-weight: 600;
      font-size: 0.8rem;
      letter-spacing: 0.15em;
      text-transform: uppercase;
      color: var(--gothic-gold);
      background: transparent;
      border: 1px solid var(--gothic-gold);
      padding: 0.9rem 2.5rem;
      cursor: pointer;
      position: relative;
      overflow: hidden;
      transition: all 0.4s ease;
      text-decoration: none;
    }

    .btn::before,
    .btn::after {
      content: '';
      position: absolute;
      width: 8px;
      height: 8px;
      border: 1px solid var(--gothic-gold);
      transition: all 0.3s ease;
    }

    .btn::before {
      top: 4px;
      left: 4px;
      border-right: none;
      border-bottom: none;
    }

    .btn::after {
      bottom: 4px;
      right: 4px;
      border-left: none;
      border-top: none;
    }

    .btn:hover {
      background: var(--gothic-gold);
      color: var(--gothic-void);
      box-shadow: 0 0 25px rgba(197, 160, 51, 0.25);
    }

    .btn:hover::before,
    .btn:hover::after {
      width: 12px;
      height: 12px;
    }

    .btn--ruby {
      color: var(--gothic-ruby);
      border-color: var(--gothic-ruby);
    }

    .btn--ruby:hover {
      background: var(--gothic-ruby);
      color: var(--gothic-bone);
      box-shadow: 0 0 25px rgba(139, 26, 43, 0.3);
    }

    .btn--ruby::before,
    .btn--ruby::after {
      border-color: var(--gothic-ruby);
    }

    /* ============================================
       SECTIONS
       ============================================ */
    .section {
      max-width: 900px;
      margin: 0 auto;
      padding: 5rem 2rem;
    }

    .section-title {
      font-family: 'Cinzel', serif;
      font-weight: 700;
      font-size: clamp(1.5rem, 3.5vw, 2.2rem);
      letter-spacing: 0.12em;
      text-transform: uppercase;
      color: var(--gothic-bone);
      text-align: center;
      margin-bottom: 0.5rem;
    }

    .section-subtitle {
      font-family: 'Cormorant', serif;
      font-style: italic;
      font-size: 1.2rem;
      color: var(--gothic-ash);
      text-align: center;
      margin-bottom: 3rem;
    }

    /* ============================================
       TRACERY DIVIDER
       ============================================ */
    .tracery-divider {
      height: 40px;
      margin: 0 auto;
      max-width: 600px;
      background: no-repeat center / 100% 100%;
      background-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 600 40'%3E%3Cpath d='M0,38 L0,20 Q25,2 50,20 Q75,2 100,20 Q125,2 150,20 Q175,2 200,20 Q225,2 250,20 Q275,2 300,20 Q325,2 350,20 Q375,2 400,20 Q425,2 450,20 Q475,2 500,20 Q525,2 550,20 Q575,2 600,20 L600,38' fill='none' stroke='%234A4A58' stroke-width='1'/%3E%3Cline x1='0' y1='38' x2='600' y2='38' stroke='%234A4A58' stroke-width='1'/%3E%3C/svg%3E");
      opacity: 0.6;
    }

    /* ============================================
       CARD GRID
       ============================================ */
    .card-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(260px, 1fr));
      gap: 1.5rem;
      margin-top: 2rem;
    }

    .card {
      background: var(--gothic-stone);
      border: 1px solid var(--gothic-gargoyle);
      padding: 2rem 1.5rem 2.5rem;
      text-align: center;
      position: relative;
      overflow: hidden;
      transition: border-color 0.4s ease, box-shadow 0.4s ease;
    }

    .card::before {
      content: '';
      position: absolute;
      top: 0;
      left: 0;
      right: 0;
      height: 5px;
      background: linear-gradient(90deg,
        transparent,
        var(--gothic-gold) 30%,
        var(--gothic-gold) 70%,
        transparent
      );
      clip-path: polygon(0 100%, 50% 0%, 100% 100%);
    }

    .card::after {
      content: '';
      position: absolute;
      inset: 0;
      background: radial-gradient(
        ellipse at 50% 0%,
        rgba(197, 160, 51, 0.05) 0%,
        transparent 60%
      );
      pointer-events: none;
    }

    .card:hover {
      border-color: var(--gothic-gold);
      box-shadow:
        0 0 20px rgba(197, 160, 51, 0.08),
        0 8px 30px rgba(0, 0, 0, 0.3);
    }

    .card-icon {
      font-size: 2rem;
      margin-bottom: 1rem;
      display: block;
    }

    .card h3 {
      font-family: 'Cinzel', serif;
      font-weight: 600;
      font-size: 1rem;
      letter-spacing: 0.1em;
      text-transform: uppercase;
      color: var(--gothic-gold);
      margin-bottom: 1rem;
    }

    .card p {
      color: var(--gothic-parchment);
      font-size: 1rem;
      line-height: 1.7;
    }

    /* ============================================
       STAINED GLASS FEATURE
       ============================================ */
    .stained-glass {
      display: grid;
      grid-template-columns: repeat(4, 1fr);
      gap: 3px;
      background: var(--gothic-void);
      padding: 3px;
      border: 2px solid var(--gothic-gargoyle);
      max-width: 700px;
      margin: 2rem auto;
    }

    .glass-pane {
      padding: 2rem 1rem;
      text-align: center;
      font-family: 'Cinzel', serif;
      font-size: 0.75rem;
      letter-spacing: 0.1em;
      text-transform: uppercase;
      line-height: 1.6;
    }

    .glass-pane--ruby {
      background: rgba(139, 26, 43, 0.2);
      color: #d8909a;
    }

    .glass-pane--blue {
      background: rgba(26, 58, 107, 0.25);
      color: #90b0d8;
    }

    .glass-pane--emerald {
      background: rgba(26, 90, 58, 0.2);
      color: #80c0a0;
    }

    .glass-pane--amber {
      background: rgba(212, 160, 32, 0.15);
      color: #d8c880;
    }

    .glass-pane--purple {
      background: rgba(74, 26, 94, 0.2);
      color: #b890c8;
    }

    .glass-pane--center {
      grid-column: span 2;
      background: radial-gradient(
        circle at 50% 50%,
        rgba(197, 160, 51, 0.12) 0%,
        rgba(139, 26, 43, 0.08) 50%,
        rgba(26, 58, 107, 0.1) 100%
      );
      color: var(--gothic-gold);
      font-size: 0.85rem;
    }

    /* ============================================
       QUOTE / PULL QUOTE
       ============================================ */
    .gothic-quote {
      max-width: 650px;
      margin: 3rem auto;
      padding: 2.5rem 3rem;
      text-align: center;
      position: relative;
      border-top: 1px solid var(--gothic-gargoyle);
      border-bottom: 1px solid var(--gothic-gargoyle);
    }

    .gothic-quote::before {
      content: '\201C';
      font-family: 'Cinzel Decorative', serif;
      font-size: 4rem;
      color: var(--gothic-gold);
      position: absolute;
      top: -0.2em;
      left: 50%;
      transform: translateX(-50%);
      background: var(--gothic-void);
      padding: 0 0.5rem;
      line-height: 1;
      opacity: 0.6;
    }

    .gothic-quote blockquote {
      font-family: 'Cormorant', serif;
      font-style: italic;
      font-size: 1.4rem;
      line-height: 1.7;
      color: var(--gothic-bone);
    }

    .gothic-quote cite {
      display: block;
      margin-top: 1rem;
      font-family: 'Cinzel', serif;
      font-style: normal;
      font-size: 0.75rem;
      letter-spacing: 0.15em;
      text-transform: uppercase;
      color: var(--gothic-ash);
    }

    /* ============================================
       ROSE WINDOW ORNAMENT
       ============================================ */
    .rose-window {
      width: 160px;
      height: 160px;
      border-radius: 50%;
      margin: 3rem auto;
      position: relative;
      background:
        radial-gradient(circle at 50% 50%,
          var(--gothic-gold) 0%,
          var(--gothic-gold) 5%,
          transparent 5.5%,
          transparent 14%,
          rgba(139, 26, 43, 0.25) 14%,
          rgba(139, 26, 43, 0.25) 22%,
          transparent 22.5%,
          transparent 30%,
          rgba(26, 58, 107, 0.2) 30%,
          rgba(26, 58, 107, 0.2) 40%,
          transparent 40.5%,
          transparent 52%,
          rgba(74, 26, 94, 0.15) 52%,
          rgba(74, 26, 94, 0.15) 62%,
          transparent 62.5%,
          transparent 76%,
          var(--gothic-gargoyle) 76%,
          var(--gothic-gargoyle) 78%,
          transparent 78.5%
        );
      border: 2px solid var(--gothic-gargoyle);
      box-shadow:
        0 0 30px rgba(197, 160, 51, 0.12),
        inset 0 0 15px rgba(0, 0, 0, 0.3);
    }

    .rose-window::before {
      content: '';
      position: absolute;
      inset: 0;
      border-radius: 50%;
      background: repeating-conic-gradient(
        from 0deg,
        transparent 0deg 14deg,
        rgba(74, 74, 88, 0.25) 14deg 16deg
      );
    }

    .rose-window::after {
      content: '';
      position: absolute;
      top: 50%;
      left: 50%;
      transform: translate(-50%, -50%);
      width: 12px;
      height: 12px;
      background: var(--gothic-gold);
      border-radius: 50%;
      box-shadow: 0 0 10px rgba(197, 160, 51, 0.5);
    }

    /* ============================================
       FOOTER
       ============================================ */
    .footer {
      border-top: 1px solid var(--gothic-gargoyle);
      padding: 3rem 2rem;
      text-align: center;
    }

    .footer p {
      font-family: 'Cinzel', serif;
      font-size: 0.75rem;
      letter-spacing: 0.15em;
      text-transform: uppercase;
      color: var(--gothic-ash);
    }

    .footer .footer-ornament {
      margin: 1rem auto 0;
      color: var(--gothic-gold);
      font-size: 1rem;
      opacity: 0.5;
    }

    /* ============================================
       RESPONSIVE
       ============================================ */
    @media (max-width: 768px) {
      .nav-inner {
        flex-direction: column;
        gap: 0;
      }

      .nav-divider {
        width: 40px;
        height: 1px;
        background: linear-gradient(to right, transparent, var(--gothic-gargoyle), transparent);
        margin: 0;
      }

      .nav-links {
        flex-wrap: wrap;
        justify-content: center;
      }

      .hero {
        min-height: 80vh;
      }

      .stained-glass {
        grid-template-columns: repeat(2, 1fr);
      }

      .glass-pane--center {
        grid-column: span 2;
      }

      .card-grid {
        grid-template-columns: 1fr;
      }

      .gothic-quote {
        padding: 2rem 1.5rem;
      }
    }
  </style>
</head>
<body>

  <!-- NAVIGATION -->
  <nav class="nav">
    <div class="nav-inner">
      <a href="#" class="nav-brand">Gothica</a>
      <div class="nav-divider"></div>
      <ul class="nav-links">
        <li><a href="#about">Origins</a></li>
        <li><a href="#features">Elements</a></li>
        <li><a href="#gallery">Gallery</a></li>
        <li><a href="#wisdom">Wisdom</a></li>
      </ul>
    </div>
  </nav>

  <!-- HERO -->
  <section class="hero">
    <div class="hero-content">
      <h1>Gothica</h1>
      <p class="subtitle">Where Stone Meets Light</p>
      <div class="ornament-rule"></div>
      <a href="#about" class="btn">Enter the Cathedral</a>
    </div>
  </section>

  <!-- ABOUT SECTION -->
  <div class="tracery-divider"></div>
  <section class="section" id="about">
    <h2 class="section-title">The Gothic Tradition</h2>
    <p class="section-subtitle">Soaring arches and luminous glass, born of 12th-century France</p>
    <p>
      The Gothic style emerged in the Ile-de-France region around 1140 and went on to define European
      architecture, sculpture, and decorative arts for nearly four centuries. Its defining innovations --
      the pointed arch, the ribbed vault, and the flying buttress -- allowed builders to raise walls to
      unprecedented heights and fill them with vast expanses of stained glass. The result was an
      architecture of light and vertical aspiration, designed to lift the spirit upward toward the divine.
    </p>
    <br>
    <p>
      In its transition to modern graphic and web design, the Gothic aesthetic preserves this essential
      duality of darkness and radiance. Deep, shadowed backgrounds serve as the stone walls, while
      jewel-toned accents and gold ornamentation become the stained glass through which light enters.
      Blackletter typography, pointed arch motifs, and ornate tracery patterns bring the vocabulary of
      the medieval cathedral into the digital space.
    </p>
  </section>

  <!-- FEATURES / CARDS -->
  <div class="tracery-divider"></div>
  <section class="section" id="features">
    <h2 class="section-title">Elements of the Style</h2>
    <p class="section-subtitle">The pillars upon which Gothic design is constructed</p>
    <div class="card-grid">
      <div class="card">
        <span class="card-icon">&#9768;</span>
        <h3>Pointed Arches</h3>
        <p>The signature Gothic form -- directing the eye upward and creating a sense of soaring vertical space in every composition.</p>
      </div>
      <div class="card">
        <span class="card-icon">&#10022;</span>
        <h3>Stained Glass</h3>
        <p>Jewel-toned color panels set against dark leading, transforming light into art and bringing radiance to shadowed spaces.</p>
      </div>
      <div class="card">
        <span class="card-icon">&#10053;</span>
        <h3>Ornate Tracery</h3>
        <p>Intricate geometric and curvilinear stone patterns -- trefoils, quatrefoils, and mouchettes -- adapted as borders and textures.</p>
      </div>
      <div class="card">
        <span class="card-icon">&#9883;</span>
        <h3>Rose Windows</h3>
        <p>Radially symmetric circular compositions that serve as focal points, combining geometric precision with transcendent beauty.</p>
      </div>
      <div class="card">
        <span class="card-icon">&#9041;</span>
        <h3>Ribbed Vaults</h3>
        <p>Intersecting arched ribs radiating from central points, creating ceiling-like frameworks that distribute visual weight elegantly.</p>
      </div>
      <div class="card">
        <span class="card-icon">&#9874;</span>
        <h3>Flying Buttresses</h3>
        <p>External supporting structures made visible and beautiful -- exposed frameworks that celebrate engineering as ornament.</p>
      </div>
    </div>
  </section>

  <!-- STAINED GLASS GALLERY -->
  <div class="tracery-divider"></div>
  <section class="section" id="gallery">
    <h2 class="section-title">The Glass Gallery</h2>
    <p class="section-subtitle">A stained glass composition in jewel tones</p>
    <div class="stained-glass">
      <div class="glass-pane glass-pane--ruby">Ruby<br>Passion</div>
      <div class="glass-pane glass-pane--blue">Azure<br>Devotion</div>
      <div class="glass-pane glass-pane--emerald">Emerald<br>Renewal</div>
      <div class="glass-pane glass-pane--purple">Amethyst<br>Mystery</div>
      <div class="glass-pane glass-pane--amber">Amber<br>Wisdom</div>
      <div class="glass-pane glass-pane--center">&#10022; Rose Window &#10022;<br>The Heart of Light</div>
      <div class="glass-pane glass-pane--blue">Sapphire<br>Truth</div>
    </div>
  </section>

  <!-- ROSE WINDOW ORNAMENT -->
  <div class="rose-window"></div>

  <!-- QUOTE -->
  <section class="section" id="wisdom">
    <h2 class="section-title">Wisdom in Stone</h2>
    <p class="section-subtitle">Words that echo through vaulted halls</p>
    <div class="gothic-quote">
      <blockquote>Architecture is frozen music, and Gothic architecture is a symphony of light, stone, and shadow reaching toward the infinite.</blockquote>
      <cite>Adapted from Johann Wolfgang von Goethe</cite>
    </div>

    <div style="text-align: center; margin-top: 3rem;">
      <a href="#" class="btn">Explore the Archives</a>
      &nbsp;&nbsp;
      <a href="#" class="btn btn--ruby">Read the Chronicle</a>
    </div>
  </section>

  <!-- FOOTER -->
  <div class="tracery-divider"></div>
  <footer class="footer">
    <p>Crafted in the Gothic Tradition</p>
    <div class="footer-ornament">&#10022;</div>
  </footer>

</body>
</html>
```
