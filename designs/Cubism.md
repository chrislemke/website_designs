# Cubism Design Reference

Cubism is one of the most revolutionary art movements in history, pioneered by Pablo Picasso and Georges Braque in Paris between 1907 and 1914. It shattered the centuries-old convention of single-point perspective by depicting subjects from multiple simultaneous viewpoints, fragmenting forms into geometric planes and reassembling them in flattened, abstract compositions. The movement progressed through two major phases -- Analytical Cubism (1909-1912), characterized by monochromatic palettes and dense geometric deconstruction, and Synthetic Cubism (1912-1914), which introduced bolder colors, collage elements, and larger decorative shapes. In web and UI design, Cubism translates to fragmented and overlapping layouts, angular geometric containers, multi-perspective compositions where content panels collide and interpenetrate, collage-like arrangements mixing disparate media, and the deliberate rejection of orderly single-axis grids in favor of dynamic, faceted spatial relationships.

---

## Visual Characteristics

### Core Design Traits

- **Fragmented forms** -- objects and layouts are broken into geometric shards, planes, and facets rather than presented as whole, continuous shapes
- **Multiple simultaneous perspectives** -- different viewpoints of the same subject are shown at once, translated in web design as overlapping panels that reveal different content angles simultaneously
- **Geometric deconstruction** -- circles, triangles, rectangles, and irregular polygons replace organic forms; every element is reduced to its geometric essence
- **Faceted planes and surfaces** -- flat, angular planes overlap and intersect to create a sense of shallow depth without traditional perspective or shadow
- **Collage and mixed media** -- Synthetic Cubism introduced papier colle (pasted paper); in web design this manifests as mixed content types, textures, and layered media elements within a single composition
- **Flattened picture plane** -- depth is suggested through overlapping planes rather than vanishing points, creating a compressed spatial field
- **Angular intersections and edges** -- hard, sharp edges where planes meet replace smooth transitions and rounded corners
- **Muted earth tones with selective bold accents** -- the Analytical phase favors ochres, browns, grays, and blacks, while Synthetic Cubism introduces strategic bursts of color
- **Visible construction lines** -- structural grid lines, edges, and borders are left visible as design elements rather than hidden
- **Typographic fragmentation** -- text can be broken, rotated, or distributed across multiple planes as a compositional element

### Design Principles

- Reject single-point perspective; present multiple viewpoints simultaneously within the same composition
- Deconstruct every element into its geometric components before reassembling the layout
- Flatten spatial depth into overlapping planes rather than creating illusionistic three-dimensional space
- Embrace collage thinking; combine disparate elements, textures, and media within a unified composition
- Structural lines and edges are features, not flaws; let the skeleton of the design remain visible
- Color serves form; restrict the palette to emphasize geometric structure, using bold accents sparingly for focal emphasis
- Every plane and fragment should contribute to the overall compositional rhythm and balance

---

## Color Palette

The Cubist palette draws from two phases: the restrained monochromes of Analytical Cubism (browns, grays, ochres, blacks) and the bolder, more decorative hues of Synthetic Cubism (terracotta, muted blue, olive, dusty rose). The palette remains grounded in earth tones with selective chromatic accents.

| Color Name | Hex | Role / Usage |
|------------|-----|-------------|
| **Raw Umber** | `#6B5B4E` | Primary earth tone, card backgrounds, grounding surfaces |
| **Ochre Gold** | `#C8A94E` | Key accent, heading highlights, active states |
| **Burnt Sienna** | `#A0522D` | Warm accent, borders, decorative bands |
| **Charcoal** | `#2D2D2D` | Primary text, structural outlines, dark panels |
| **Warm Gray** | `#9C9486` | Secondary text, muted planes, subtle backgrounds |
| **Parchment** | `#F0E8D8` | Primary light background, content surfaces |
| **Stone White** | `#EDE6D6` | Alternate light background, card surfaces |
| **Deep Black** | `#1A1612` | High-contrast edges, bold outlines, anchoring elements |
| **Olive Drab** | `#6B7B4E` | Synthetic Cubism accent, secondary color blocks |
| **Dusty Blue** | `#5B7A8A` | Cool accent, link color, contrasting panels |
| **Terracotta** | `#B85C3A` | Warm feature accent, call-to-action elements |
| **Dusty Rose** | `#A0707A` | Synthetic Cubism accent, decorative fragments |
| **Slate** | `#4A5568` | Navigation backgrounds, dark overlapping planes |
| **Cream** | `#F5F0E1` | Light fill panels, text backgrounds |
| **Muted Violet** | `#7A6B8A` | Sparse tertiary accent, decorative collage elements |

### CSS Custom Properties

```css
:root {
  /* Earth tones -- Analytical Cubism */
  --cubism-umber: #6b5b4e;
  --cubism-ochre: #c8a94e;
  --cubism-sienna: #a0522d;
  --cubism-warm-gray: #9c9486;
  --cubism-charcoal: #2d2d2d;
  --cubism-black: #1a1612;

  /* Chromatic accents -- Synthetic Cubism */
  --cubism-olive: #6b7b4e;
  --cubism-blue: #5b7a8a;
  --cubism-terracotta: #b85c3a;
  --cubism-rose: #a0707a;
  --cubism-violet: #7a6b8a;

  /* Light surfaces */
  --cubism-parchment: #f0e8d8;
  --cubism-stone: #ede6d6;
  --cubism-cream: #f5f0e1;

  /* Dark surfaces */
  --cubism-slate: #4a5568;

  /* Functional tokens */
  --cubism-bg-primary: var(--cubism-parchment);
  --cubism-bg-secondary: var(--cubism-stone);
  --cubism-bg-dark: var(--cubism-charcoal);
  --cubism-text-primary: var(--cubism-charcoal);
  --cubism-text-light: var(--cubism-cream);
  --cubism-text-muted: var(--cubism-warm-gray);
  --cubism-accent: var(--cubism-ochre);
  --cubism-accent-warm: var(--cubism-terracotta);
  --cubism-border: var(--cubism-black);
  --cubism-border-light: var(--cubism-warm-gray);
}
```

---

## Typography

### Recommended Google Fonts

| Font | Style | Usage |
|------|-------|-------|
| **Josefin Sans** | Geometric, angular, vintage modernist | Headlines, display text |
| **Bebas Neue** | Bold condensed uppercase | Hero titles, banners, large statements |
| **Oswald** | Condensed, strong vertical rhythm | Section headings, navigation |
| **Archivo Black** | Bold geometric grotesque | Display headings, feature titles |
| **Barlow Condensed** | Clean condensed geometric | Subheadings, labels, captions |
| **Source Sans 3** | Neutral geometric sans | Body text, paragraphs |
| **IBM Plex Sans** | Constructed, precise geometric | Body text, UI elements |
| **Playfair Display** | Sharp transitional serif with angular features | Accent headings, pull quotes |
| **Cormorant Garamond** | High-contrast angular serif | Decorative body text, editorial use |

### Font Pairing Suggestions

| Heading Font | Body Font | Character |
|-------------|-----------|-----------|
| **Bebas Neue** | **Source Sans 3** | Bold architectural display with clean readable body; maximum Cubist impact |
| **Josefin Sans** | **IBM Plex Sans** | Angular vintage geometry paired with precise constructed body text |
| **Archivo Black** | **Barlow Condensed** | Heavy geometric display with condensed supporting text for dense layouts |
| **Playfair Display** | **Source Sans 3** | Sharp serif headlines add Synthetic Cubism elegance against neutral body |
| **Oswald** | **Cormorant Garamond** | Condensed modern headings contrasted with angular serif body for editorial feel |

### CSS Example

```css
@import url('https://fonts.googleapis.com/css2?family=Bebas+Neue&family=Josefin+Sans:wght@400;700&family=Source+Sans+3:wght@400;600&family=Barlow+Condensed:wght@400;600&family=Playfair+Display:wght@700&display=swap');

/* Headlines -- angular, constructed, uppercase */
h1, h2, h3 {
  font-family: 'Josefin Sans', 'Bebas Neue', sans-serif;
  text-transform: uppercase;
  letter-spacing: 0.1em;
  color: var(--cubism-charcoal);
  font-weight: 700;
  line-height: 1.1;
}

/* Display / Hero text */
.cubism-display {
  font-family: 'Bebas Neue', sans-serif;
  font-size: clamp(3rem, 8vw, 8rem);
  letter-spacing: 0.12em;
  line-height: 0.95;
  color: var(--cubism-black);
}

/* Body text */
body {
  font-family: 'Source Sans 3', 'IBM Plex Sans', sans-serif;
  font-weight: 400;
  letter-spacing: 0.02em;
  line-height: 1.7;
  color: var(--cubism-text-primary);
}

/* Subheadings / Labels */
.cubism-label {
  font-family: 'Barlow Condensed', sans-serif;
  text-transform: uppercase;
  letter-spacing: 0.08em;
  font-size: 0.85rem;
  color: var(--cubism-text-muted);
}

/* Accent serif for editorial moments */
.cubism-serif-accent {
  font-family: 'Playfair Display', serif;
  font-weight: 700;
  font-style: italic;
  letter-spacing: 0.02em;
}
```

---

## Layout Principles

- **Fragmented grid** -- avoid perfectly regular grids; break the layout into asymmetric, overlapping planes that suggest multiple perspectives
- **Overlapping panels** -- content containers should overlap and intersect, creating a collage-like spatial arrangement with shallow depth
- **Angular and rotated elements** -- tilt cards, sections, and decorative elements at slight angles (2-5 degrees) to break rigid alignment
- **Multi-axis composition** -- arrange content along diagonal and intersecting axes rather than a single vertical flow
- **Visible structural lines** -- expose grid lines, borders, and edges as compositional elements rather than hiding them
- **Collage layering** -- stack different content types (text, images, geometric shapes, textures) in overlapping arrangements
- **Shallow depth through overlap** -- create the illusion of compressed space by layering translucent and opaque planes
- **Asymmetric balance** -- achieve visual equilibrium through the weight of fragments rather than through mirror symmetry
- **Faceted section transitions** -- use angular clip-paths and diagonal dividers between sections instead of straight horizontal lines
- **Dense but rhythmic composition** -- fill space with geometric fragments but maintain a visual rhythm through repeated angles and proportional relationships

---

## CSS / Design Techniques

### Card Component

```css
.cubism-card {
  background: var(--cubism-stone);
  border: 2px solid var(--cubism-black);
  padding: 2rem;
  position: relative;
  clip-path: polygon(
    0% 4%, 4% 0%, 96% 0%, 100% 4%,
    100% 96%, 96% 100%, 4% 100%, 0% 96%
  );
  transform: rotate(-1deg);
  transition: transform 0.3s ease, box-shadow 0.3s ease;
}

.cubism-card:hover {
  transform: rotate(0deg) translateY(-4px);
}

/* Ochre accent stripe at top */
.cubism-card::before {
  content: '';
  position: absolute;
  top: 0;
  left: 8%;
  right: 8%;
  height: 4px;
  background: var(--cubism-ochre);
}

/* Geometric corner fragment */
.cubism-card::after {
  content: '';
  position: absolute;
  bottom: 0;
  right: 0;
  width: 40px;
  height: 40px;
  background: linear-gradient(
    315deg,
    var(--cubism-umber) 50%,
    transparent 50%
  );
  opacity: 0.6;
}

.cubism-card h3 {
  font-family: 'Josefin Sans', sans-serif;
  text-transform: uppercase;
  letter-spacing: 0.08em;
  margin-bottom: 0.75rem;
  color: var(--cubism-charcoal);
}

.cubism-card p {
  font-size: 0.95rem;
  color: var(--cubism-text-muted);
  line-height: 1.6;
}

/* Card grid with offset rhythm */
.cubism-card-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
  gap: 2rem;
  max-width: 1200px;
  margin: 0 auto;
}

.cubism-card-grid .cubism-card:nth-child(even) {
  transform: rotate(1deg);
  margin-top: 1.5rem;
}

.cubism-card-grid .cubism-card:nth-child(even):hover {
  transform: rotate(0deg) translateY(-4px);
}
```

### Button Component

```css
.cubism-button {
  display: inline-block;
  background: var(--cubism-charcoal);
  color: var(--cubism-cream);
  border: 2px solid var(--cubism-black);
  border-radius: 0;
  padding: 14px 36px;
  font-family: 'Josefin Sans', sans-serif;
  font-size: 0.95rem;
  font-weight: 700;
  letter-spacing: 0.12em;
  text-transform: uppercase;
  text-decoration: none;
  cursor: pointer;
  position: relative;
  clip-path: polygon(
    0% 6%, 6% 0%, 100% 0%, 100% 100%, 94% 100%, 0% 100%
  );
  transition: background 0.2s ease, transform 0.2s ease;
}

.cubism-button:hover {
  background: var(--cubism-terracotta);
  transform: translateY(-2px);
}

/* Hard geometric shadow */
.cubism-button::after {
  content: '';
  position: absolute;
  top: 4px;
  left: 4px;
  right: -4px;
  bottom: -4px;
  background: var(--cubism-ochre);
  z-index: -1;
  clip-path: polygon(
    0% 6%, 6% 0%, 100% 0%, 100% 100%, 94% 100%, 0% 100%
  );
  transition: transform 0.2s ease;
}

.cubism-button:hover::after {
  transform: translate(2px, 2px);
}

/* Accent variant */
.cubism-button--accent {
  background: var(--cubism-ochre);
  color: var(--cubism-black);
  border-color: var(--cubism-black);
}

.cubism-button--accent:hover {
  background: var(--cubism-sienna);
  color: var(--cubism-cream);
}

/* Outline variant */
.cubism-button--outline {
  background: transparent;
  color: var(--cubism-charcoal);
  border: 2px solid var(--cubism-charcoal);
}

.cubism-button--outline:hover {
  background: var(--cubism-charcoal);
  color: var(--cubism-cream);
}
```

### Navigation Bar

```css
.cubism-nav {
  display: flex;
  align-items: center;
  justify-content: space-between;
  background: var(--cubism-charcoal);
  padding: 0 40px;
  position: relative;
  overflow: hidden;
}

/* Fragmented geometric accent bar */
.cubism-nav::before {
  content: '';
  position: absolute;
  bottom: 0;
  left: 0;
  width: 100%;
  height: 4px;
  background: linear-gradient(
    90deg,
    var(--cubism-ochre) 0%, var(--cubism-ochre) 25%,
    var(--cubism-terracotta) 25%, var(--cubism-terracotta) 45%,
    var(--cubism-olive) 45%, var(--cubism-olive) 60%,
    var(--cubism-blue) 60%, var(--cubism-blue) 75%,
    var(--cubism-umber) 75%, var(--cubism-umber) 100%
  );
}

/* Angled background fragment */
.cubism-nav::after {
  content: '';
  position: absolute;
  top: 0;
  right: -20px;
  width: 200px;
  height: 100%;
  background: var(--cubism-slate);
  transform: skewX(-12deg);
  opacity: 0.3;
}

.cubism-nav__logo {
  font-family: 'Bebas Neue', sans-serif;
  font-size: 1.8rem;
  color: var(--cubism-ochre);
  text-decoration: none;
  letter-spacing: 0.1em;
  padding: 18px 0;
  position: relative;
  z-index: 1;
}

.cubism-nav__links {
  display: flex;
  gap: 28px;
  list-style: none;
  margin: 0;
  padding: 0;
  position: relative;
  z-index: 1;
}

.cubism-nav__links a {
  font-family: 'Josefin Sans', sans-serif;
  font-size: 0.9rem;
  font-weight: 700;
  color: var(--cubism-cream);
  text-decoration: none;
  letter-spacing: 0.08em;
  text-transform: uppercase;
  padding: 18px 0;
  position: relative;
  transition: color 0.2s ease;
}

.cubism-nav__links a:hover {
  color: var(--cubism-ochre);
}

.cubism-nav__links a::after {
  content: '';
  position: absolute;
  bottom: 12px;
  left: 0;
  width: 0;
  height: 2px;
  background: var(--cubism-ochre);
  transition: width 0.3s ease;
}

.cubism-nav__links a:hover::after {
  width: 100%;
}
```

### Hero Section

```css
.cubism-hero {
  background: var(--cubism-bg-dark);
  color: var(--cubism-text-light);
  padding: 100px 40px 120px;
  position: relative;
  overflow: hidden;
}

/* Overlapping geometric planes */
.cubism-hero::before {
  content: '';
  position: absolute;
  top: -50px;
  right: -80px;
  width: 500px;
  height: 600px;
  background: var(--cubism-umber);
  transform: rotate(15deg);
  opacity: 0.15;
}

.cubism-hero::after {
  content: '';
  position: absolute;
  bottom: -100px;
  left: 10%;
  width: 400px;
  height: 500px;
  background: var(--cubism-ochre);
  transform: rotate(-20deg);
  opacity: 0.08;
  clip-path: polygon(20% 0%, 100% 0%, 80% 100%, 0% 100%);
}

.cubism-hero__content {
  max-width: 1200px;
  margin: 0 auto;
  position: relative;
  z-index: 1;
}

.cubism-hero__content h1 {
  font-family: 'Bebas Neue', sans-serif;
  font-size: clamp(3.5rem, 10vw, 8rem);
  letter-spacing: 0.12em;
  line-height: 0.9;
  color: var(--cubism-cream);
  margin-bottom: 1.5rem;
}

.cubism-hero__content h1 .accent {
  color: var(--cubism-ochre);
}

.cubism-hero__content p {
  font-size: 1.15rem;
  color: var(--cubism-warm-gray);
  max-width: 550px;
  line-height: 1.7;
  margin-bottom: 2.5rem;
}

/* Fragmented decorative element beside hero text */
.cubism-hero__fragment {
  position: absolute;
  top: 15%;
  right: 5%;
  width: 300px;
  height: 350px;
  z-index: 0;
}

.cubism-hero__fragment div {
  position: absolute;
  border: 2px solid rgba(200, 169, 78, 0.3);
}

.cubism-hero__fragment div:nth-child(1) {
  width: 120px; height: 160px;
  top: 0; left: 40px;
  background: rgba(107, 91, 78, 0.2);
  transform: rotate(8deg);
}

.cubism-hero__fragment div:nth-child(2) {
  width: 140px; height: 100px;
  top: 60px; left: 100px;
  background: rgba(200, 169, 78, 0.1);
  transform: rotate(-5deg);
}

.cubism-hero__fragment div:nth-child(3) {
  width: 100px; height: 180px;
  top: 80px; left: 0;
  background: rgba(91, 122, 138, 0.15);
  transform: rotate(12deg);
}

@media (max-width: 768px) {
  .cubism-hero {
    padding: 60px 24px 80px;
  }
  .cubism-hero__fragment {
    display: none;
  }
}
```

### Fragmented Panel / Multi-Perspective Block

```css
/* A composition of overlapping planes suggesting multiple viewpoints */
.cubism-fragmented-panel {
  position: relative;
  min-height: 400px;
  max-width: 900px;
  margin: 4rem auto;
}

.cubism-fragmented-panel__plane {
  position: absolute;
  padding: 2rem;
  border: 2px solid var(--cubism-border);
}

.cubism-fragmented-panel__plane--a {
  top: 0;
  left: 0;
  width: 55%;
  height: 65%;
  background: var(--cubism-parchment);
  transform: rotate(-2deg);
  z-index: 3;
}

.cubism-fragmented-panel__plane--b {
  top: 15%;
  right: 0;
  width: 50%;
  height: 55%;
  background: var(--cubism-stone);
  transform: rotate(3deg);
  z-index: 2;
  clip-path: polygon(8% 0%, 100% 0%, 100% 100%, 0% 92%);
}

.cubism-fragmented-panel__plane--c {
  bottom: 0;
  left: 10%;
  width: 45%;
  height: 40%;
  background: var(--cubism-charcoal);
  color: var(--cubism-cream);
  transform: rotate(1deg);
  z-index: 4;
}

/* Intersection line accent */
.cubism-fragmented-panel::after {
  content: '';
  position: absolute;
  top: 20%;
  left: 30%;
  width: 50%;
  height: 2px;
  background: var(--cubism-ochre);
  transform: rotate(-8deg);
  z-index: 5;
}
```

### Angular Section Divider

```css
/* Faceted diagonal divider between sections */
.cubism-divider {
  width: 100%;
  height: 80px;
  position: relative;
  overflow: hidden;
}

.cubism-divider::before {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  background: linear-gradient(
    to bottom right,
    var(--cubism-parchment) 48%,
    var(--cubism-charcoal) 48%,
    var(--cubism-charcoal) 50%,
    var(--cubism-stone) 50%
  );
}

/* Accent fragment within divider */
.cubism-divider::after {
  content: '';
  position: absolute;
  top: 10px;
  left: 40%;
  width: 120px;
  height: 60px;
  background: var(--cubism-ochre);
  opacity: 0.5;
  transform: skewX(-20deg);
}

/* Zig-zag variant */
.cubism-divider--zigzag {
  height: 30px;
  background: var(--cubism-ochre);
  clip-path: polygon(
    0% 0%, 5% 100%, 10% 0%, 15% 100%, 20% 0%,
    25% 100%, 30% 0%, 35% 100%, 40% 0%, 45% 100%,
    50% 0%, 55% 100%, 60% 0%, 65% 100%, 70% 0%,
    75% 100%, 80% 0%, 85% 100%, 90% 0%, 95% 100%, 100% 0%
  );
}
```

### Collage Overlay Section

```css
/* A section with layered, collage-like overlapping elements */
.cubism-collage {
  position: relative;
  padding: 6rem 2rem;
  background: var(--cubism-parchment);
  overflow: hidden;
}

/* Background geometric texture */
.cubism-collage::before {
  content: '';
  position: absolute;
  inset: 0;
  background:
    linear-gradient(35deg, rgba(107,91,78,0.04) 25%, transparent 25%),
    linear-gradient(145deg, rgba(107,91,78,0.04) 25%, transparent 25%),
    linear-gradient(215deg, rgba(107,91,78,0.04) 25%, transparent 25%),
    linear-gradient(325deg, rgba(107,91,78,0.04) 25%, transparent 25%);
  background-size: 80px 80px;
  pointer-events: none;
}

.cubism-collage__item {
  position: relative;
  display: inline-block;
  border: 2px solid var(--cubism-border);
  padding: 1.5rem;
  background: var(--cubism-cream);
  margin: 1rem;
  transition: transform 0.3s ease;
}

.cubism-collage__item:nth-child(odd) {
  transform: rotate(-2deg);
}

.cubism-collage__item:nth-child(even) {
  transform: rotate(2deg);
}

.cubism-collage__item:hover {
  transform: rotate(0deg) scale(1.03);
  z-index: 10;
}

/* Paper-torn edge effect for collage fragments */
.cubism-collage__item--torn {
  clip-path: polygon(
    2% 0%, 98% 3%, 100% 5%, 97% 97%,
    95% 100%, 3% 98%, 0% 95%, 1% 2%
  );
}
```

### Faceted Background Pattern

```css
/* Geometric triangular mosaic background */
.cubism-faceted-bg {
  position: relative;
  background-color: var(--cubism-parchment);
}

.cubism-faceted-bg::after {
  content: '';
  position: absolute;
  inset: 0;
  background:
    linear-gradient(60deg, var(--cubism-warm-gray) 25%, transparent 25.5%),
    linear-gradient(-60deg, var(--cubism-warm-gray) 25%, transparent 25.5%),
    linear-gradient(60deg, transparent 74.5%, var(--cubism-warm-gray) 75%),
    linear-gradient(-60deg, transparent 74.5%, var(--cubism-warm-gray) 75%);
  background-size: 50px 86px;
  background-position: 0 0, 0 0, 25px 43px, 25px 43px;
  opacity: 0.08;
  pointer-events: none;
}

/* Cubist cross-hatch overlay for texture */
.cubism-crosshatch {
  position: relative;
}

.cubism-crosshatch::after {
  content: '';
  position: absolute;
  inset: 0;
  background:
    repeating-linear-gradient(
      45deg,
      transparent,
      transparent 8px,
      rgba(42, 42, 42, 0.03) 8px,
      rgba(42, 42, 42, 0.03) 9px
    ),
    repeating-linear-gradient(
      -45deg,
      transparent,
      transparent 8px,
      rgba(42, 42, 42, 0.03) 8px,
      rgba(42, 42, 42, 0.03) 9px
    );
  pointer-events: none;
}
```

---

## Design Do's and Don'ts

### Do

- Fragment layouts into overlapping geometric planes with angular edges
- Use muted earth tones (ochre, umber, sienna, warm gray) as the dominant palette
- Show multiple perspectives simultaneously through layered and overlapping content panels
- Leave structural borders, edges, and grid lines visible as compositional elements
- Apply slight rotations (1-5 degrees) to cards and panels for dynamic tension
- Mix content types in collage-like arrangements inspired by Synthetic Cubism's papier colle
- Use bold, condensed, geometric sans-serif typefaces for headlines
- Create section dividers with angular clip-paths and diagonal transitions
- Use selective bold color accents (terracotta, ochre) sparingly against the earth-tone base
- Embrace asymmetry and off-center compositions for visual energy

### Don't

- Use single-point perspective, realistic depth, or drop shadows that suggest three-dimensional space
- Rely on perfectly regular, symmetrical grid layouts -- Cubism is about fractured geometry
- Apply rounded corners, soft gradients, or organic curves as primary elements
- Use a bright, saturated, high-chroma color palette -- the Cubist palette is restrained and earthy
- Leave all elements axis-aligned and orderly; static layouts contradict the Cubist ethos
- Use photographic imagery without geometric fragmentation or collage treatment
- Apply smooth transitions between sections; breaks should be angular and faceted
- Make every element the same size and weight; Cubism requires compositional hierarchy through scale contrast
- Hide structural lines and construction geometry; exposed edges are a feature
- Treat whitespace as emptiness; negative space in Cubism is shaped by the angular fragments around it

---

## Related Aesthetics

| Aesthetic | Relationship to Cubism |
|-----------|------------------------|
| **Czech Cubism** | Direct descendant; extended Cubist fragmentation into architecture, furniture, and decorative arts with crystalline, prismatic forms |
| **Constructivism** | Post-Cubist evolution; inherited geometric abstraction and collage but redirected it toward social and political function |
| **Art Deco** | Influenced successor; absorbed Cubist geometric vocabulary and stylized it into decorative elegance |
| **Futurism** | Contemporary sibling; shared fragmented forms but emphasized speed, motion, and temporal dynamism |
| **De Stijl** | Parallel reductionist movement; both embraced geometric abstraction but De Stijl restricted to orthogonal forms and primary colors |
| **Bauhaus** | Descendant school; integrated Cubist spatial concepts into functional design and architecture curriculum |
| **Suprematism** | Russian parallel; pursued pure geometric abstraction to its most radical conclusion |
| **Dadaism** | Contemporary reaction; shared Cubist collage techniques but used them for anarchic, anti-art purposes |
| **Surrealism** | Successor movement; inherited spatial fragmentation but redirected it toward dreamlike and unconscious imagery |
| **Pop Art** | Later descendant; Lichtenstein explicitly combined Pop imagery with Cubist fragmentation and faceted planes |

---

## Quick-Start HTML Template

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Cubism Design</title>
  <link href="https://fonts.googleapis.com/css2?family=Bebas+Neue&family=Josefin+Sans:wght@400;700&family=Source+Sans+3:wght@400;600&family=Barlow+Condensed:wght@400;600&display=swap" rel="stylesheet">
  <style>
    :root {
      --cubism-umber: #6b5b4e;
      --cubism-ochre: #c8a94e;
      --cubism-sienna: #a0522d;
      --cubism-warm-gray: #9c9486;
      --cubism-charcoal: #2d2d2d;
      --cubism-black: #1a1612;
      --cubism-olive: #6b7b4e;
      --cubism-blue: #5b7a8a;
      --cubism-terracotta: #b85c3a;
      --cubism-rose: #a0707a;
      --cubism-violet: #7a6b8a;
      --cubism-parchment: #f0e8d8;
      --cubism-stone: #ede6d6;
      --cubism-cream: #f5f0e1;
      --cubism-slate: #4a5568;
    }

    * { margin: 0; padding: 0; box-sizing: border-box; }

    body {
      background: var(--cubism-parchment);
      color: var(--cubism-charcoal);
      font-family: 'Source Sans 3', sans-serif;
      font-weight: 400;
      letter-spacing: 0.02em;
      line-height: 1.7;
    }

    h1, h2, h3 {
      font-family: 'Josefin Sans', sans-serif;
      text-transform: uppercase;
      letter-spacing: 0.1em;
      font-weight: 700;
      line-height: 1.1;
    }

    /* ---- NAVIGATION ---- */
    nav {
      display: flex;
      align-items: center;
      justify-content: space-between;
      background: var(--cubism-charcoal);
      padding: 0 40px;
      position: relative;
      overflow: hidden;
    }

    nav::before {
      content: '';
      position: absolute;
      bottom: 0;
      left: 0;
      width: 100%;
      height: 4px;
      background: linear-gradient(
        90deg,
        var(--cubism-ochre) 0%, var(--cubism-ochre) 25%,
        var(--cubism-terracotta) 25%, var(--cubism-terracotta) 45%,
        var(--cubism-olive) 45%, var(--cubism-olive) 60%,
        var(--cubism-blue) 60%, var(--cubism-blue) 75%,
        var(--cubism-umber) 75%, var(--cubism-umber) 100%
      );
    }

    nav::after {
      content: '';
      position: absolute;
      top: 0;
      right: -20px;
      width: 180px;
      height: 100%;
      background: var(--cubism-slate);
      transform: skewX(-12deg);
      opacity: 0.3;
    }

    .nav-logo {
      font-family: 'Bebas Neue', sans-serif;
      font-size: 1.8rem;
      color: var(--cubism-ochre);
      text-decoration: none;
      letter-spacing: 0.1em;
      padding: 18px 0;
      position: relative;
      z-index: 1;
    }

    .nav-links {
      display: flex;
      gap: 28px;
      list-style: none;
      position: relative;
      z-index: 1;
    }

    .nav-links a {
      font-family: 'Josefin Sans', sans-serif;
      font-size: 0.85rem;
      font-weight: 700;
      color: var(--cubism-cream);
      text-decoration: none;
      letter-spacing: 0.08em;
      text-transform: uppercase;
      padding: 18px 0;
      transition: color 0.2s ease;
    }

    .nav-links a:hover { color: var(--cubism-ochre); }

    /* ---- HERO ---- */
    .hero {
      background: var(--cubism-charcoal);
      color: var(--cubism-cream);
      padding: 80px 40px 100px;
      position: relative;
      overflow: hidden;
    }

    .hero::before {
      content: '';
      position: absolute;
      top: -40px;
      right: -60px;
      width: 450px;
      height: 550px;
      background: var(--cubism-umber);
      transform: rotate(15deg);
      opacity: 0.12;
    }

    .hero::after {
      content: '';
      position: absolute;
      bottom: -80px;
      left: 8%;
      width: 350px;
      height: 400px;
      background: var(--cubism-ochre);
      transform: rotate(-18deg);
      opacity: 0.07;
      clip-path: polygon(20% 0%, 100% 0%, 80% 100%, 0% 100%);
    }

    .hero-inner {
      max-width: 1100px;
      margin: 0 auto;
      position: relative;
      z-index: 1;
      display: grid;
      grid-template-columns: 1fr 300px;
      gap: 2rem;
      align-items: center;
    }

    .hero h1 {
      font-family: 'Bebas Neue', sans-serif;
      font-size: clamp(3rem, 8vw, 6.5rem);
      letter-spacing: 0.1em;
      line-height: 0.95;
      color: var(--cubism-cream);
    }

    .hero h1 .accent { color: var(--cubism-ochre); }

    .hero p {
      font-size: 1.1rem;
      color: var(--cubism-warm-gray);
      max-width: 500px;
      margin: 1.5rem 0 2rem;
      line-height: 1.7;
    }

    .hero-btn {
      display: inline-block;
      background: var(--cubism-ochre);
      color: var(--cubism-black);
      border: 2px solid var(--cubism-black);
      padding: 14px 36px;
      font-family: 'Josefin Sans', sans-serif;
      font-size: 0.9rem;
      font-weight: 700;
      letter-spacing: 0.12em;
      text-transform: uppercase;
      text-decoration: none;
      clip-path: polygon(0% 6%, 6% 0%, 100% 0%, 100% 100%, 94% 100%, 0% 100%);
      transition: background 0.2s ease;
    }

    .hero-btn:hover {
      background: var(--cubism-terracotta);
      color: var(--cubism-cream);
    }

    /* Decorative fragmented planes beside hero */
    .hero-fragments {
      position: relative;
      height: 300px;
    }

    .hero-fragments div {
      position: absolute;
      border: 2px solid rgba(200,169,78,0.3);
    }

    .frag-1 {
      width: 110px; height: 150px;
      top: 0; left: 30px;
      background: rgba(107,91,78,0.2);
      transform: rotate(8deg);
    }

    .frag-2 {
      width: 130px; height: 90px;
      top: 50px; left: 100px;
      background: rgba(200,169,78,0.12);
      transform: rotate(-5deg);
    }

    .frag-3 {
      width: 90px; height: 170px;
      top: 70px; left: 0;
      background: rgba(91,122,138,0.15);
      transform: rotate(12deg);
    }

    .frag-4 {
      width: 80px; height: 80px;
      top: 160px; left: 120px;
      background: rgba(160,112,122,0.15);
      transform: rotate(-3deg);
    }

    /* ---- ANGULAR DIVIDER ---- */
    .divider {
      width: 100%;
      height: 70px;
      position: relative;
      overflow: hidden;
    }

    .divider::before {
      content: '';
      position: absolute;
      inset: 0;
      background: linear-gradient(
        to bottom right,
        var(--cubism-charcoal) 48%,
        var(--cubism-black) 48%,
        var(--cubism-black) 50%,
        var(--cubism-parchment) 50%
      );
    }

    .divider::after {
      content: '';
      position: absolute;
      top: 8px;
      left: 38%;
      width: 100px;
      height: 50px;
      background: var(--cubism-ochre);
      opacity: 0.4;
      transform: skewX(-20deg);
    }

    /* ---- ABOUT SECTION ---- */
    .about {
      max-width: 1100px;
      margin: 0 auto;
      padding: 5rem 2rem;
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 3rem;
      align-items: start;
    }

    .about h2 {
      font-size: 2.2rem;
      margin-bottom: 1rem;
      position: relative;
      display: inline-block;
    }

    .about h2::after {
      content: '';
      position: absolute;
      bottom: -6px;
      left: 0;
      width: 50px;
      height: 4px;
      background: var(--cubism-ochre);
      transform: skewX(-15deg);
    }

    .about p {
      color: var(--cubism-charcoal);
      line-height: 1.8;
    }

    /* Collage panel on right of about */
    .about-collage {
      position: relative;
      min-height: 300px;
    }

    .about-collage .plane {
      position: absolute;
      border: 2px solid var(--cubism-charcoal);
      padding: 1.5rem;
    }

    .plane-a {
      top: 0; left: 0;
      width: 70%;
      background: var(--cubism-stone);
      transform: rotate(-2deg);
      z-index: 2;
    }

    .plane-b {
      top: 40px; left: 30%;
      width: 65%;
      background: var(--cubism-cream);
      transform: rotate(3deg);
      z-index: 1;
      clip-path: polygon(6% 0%, 100% 0%, 100% 100%, 0% 92%);
    }

    .plane-c {
      top: 140px; left: 5%;
      width: 55%;
      background: var(--cubism-charcoal);
      color: var(--cubism-cream);
      transform: rotate(1deg);
      z-index: 3;
    }

    .plane-label {
      font-family: 'Barlow Condensed', sans-serif;
      font-size: 0.75rem;
      text-transform: uppercase;
      letter-spacing: 0.1em;
      color: var(--cubism-warm-gray);
      margin-bottom: 0.5rem;
    }

    .plane-c .plane-label { color: var(--cubism-ochre); }

    /* ---- ZIGZAG BAND ---- */
    .zigzag {
      width: 100%;
      height: 24px;
      background: var(--cubism-ochre);
      clip-path: polygon(
        0% 0%, 4% 100%, 8% 0%, 12% 100%, 16% 0%,
        20% 100%, 24% 0%, 28% 100%, 32% 0%, 36% 100%,
        40% 0%, 44% 100%, 48% 0%, 52% 100%, 56% 0%,
        60% 100%, 64% 0%, 68% 100%, 72% 0%, 76% 100%,
        80% 0%, 84% 100%, 88% 0%, 92% 100%, 96% 0%, 100% 100%
      );
    }

    /* ---- CARDS SECTION ---- */
    .cards-section {
      background: var(--cubism-stone);
      padding: 5rem 2rem;
      position: relative;
    }

    /* Faceted background texture */
    .cards-section::before {
      content: '';
      position: absolute;
      inset: 0;
      background:
        linear-gradient(60deg, var(--cubism-warm-gray) 25%, transparent 25.5%),
        linear-gradient(-60deg, var(--cubism-warm-gray) 25%, transparent 25.5%),
        linear-gradient(60deg, transparent 74.5%, var(--cubism-warm-gray) 75%),
        linear-gradient(-60deg, transparent 74.5%, var(--cubism-warm-gray) 75%);
      background-size: 50px 86px;
      background-position: 0 0, 0 0, 25px 43px, 25px 43px;
      opacity: 0.06;
      pointer-events: none;
    }

    .cards-section h2 {
      text-align: center;
      font-size: 2rem;
      margin-bottom: 3rem;
      position: relative;
    }

    .card-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
      gap: 2rem;
      max-width: 1100px;
      margin: 0 auto;
      position: relative;
      z-index: 1;
    }

    .card {
      background: var(--cubism-parchment);
      border: 2px solid var(--cubism-black);
      padding: 2rem;
      position: relative;
      clip-path: polygon(
        0% 4%, 4% 0%, 96% 0%, 100% 4%,
        100% 96%, 96% 100%, 4% 100%, 0% 96%
      );
      transform: rotate(-1deg);
      transition: transform 0.3s ease;
    }

    .card:nth-child(even) {
      transform: rotate(1deg);
      margin-top: 1.5rem;
    }

    .card:hover {
      transform: rotate(0deg) translateY(-4px);
    }

    .card::before {
      content: '';
      position: absolute;
      top: 0;
      left: 8%;
      right: 8%;
      height: 4px;
      background: var(--cubism-ochre);
    }

    .card::after {
      content: '';
      position: absolute;
      bottom: 0;
      right: 0;
      width: 36px;
      height: 36px;
      background: linear-gradient(315deg, var(--cubism-umber) 50%, transparent 50%);
      opacity: 0.5;
    }

    .card h3 {
      font-size: 1.1rem;
      margin-bottom: 0.75rem;
    }

    .card p {
      font-size: 0.9rem;
      color: var(--cubism-warm-gray);
      line-height: 1.6;
    }

    .card-number {
      font-family: 'Bebas Neue', sans-serif;
      font-size: 3rem;
      color: var(--cubism-stone);
      line-height: 1;
      margin-bottom: 0.5rem;
    }

    /* ---- MANIFESTO / STATEMENT SECTION ---- */
    .statement {
      background: var(--cubism-charcoal);
      color: var(--cubism-cream);
      padding: 5rem 2rem;
      text-align: center;
      position: relative;
      clip-path: polygon(0 5%, 100% 0, 100% 95%, 0 100%);
    }

    .statement h2 {
      font-family: 'Bebas Neue', sans-serif;
      font-size: clamp(2rem, 5vw, 3.5rem);
      letter-spacing: 0.12em;
      margin-bottom: 1.5rem;
      color: var(--cubism-ochre);
    }

    .statement p {
      max-width: 600px;
      margin: 0 auto;
      font-size: 1.1rem;
      color: var(--cubism-warm-gray);
      line-height: 1.8;
    }

    /* ---- FOOTER ---- */
    footer {
      background: var(--cubism-black);
      color: var(--cubism-warm-gray);
      padding: 3rem 2rem 2rem;
      text-align: center;
      position: relative;
    }

    footer::before {
      content: '';
      position: absolute;
      top: 0;
      left: 0;
      width: 100%;
      height: 4px;
      background: linear-gradient(
        90deg,
        var(--cubism-terracotta) 0%, var(--cubism-terracotta) 30%,
        var(--cubism-ochre) 30%, var(--cubism-ochre) 55%,
        var(--cubism-olive) 55%, var(--cubism-olive) 70%,
        var(--cubism-blue) 70%, var(--cubism-blue) 100%
      );
    }

    .footer-logo {
      font-family: 'Bebas Neue', sans-serif;
      font-size: 1.4rem;
      color: var(--cubism-ochre);
      letter-spacing: 0.1em;
      margin-bottom: 1rem;
    }

    footer p {
      font-size: 0.85rem;
      color: var(--cubism-warm-gray);
    }

    /* ---- RESPONSIVE ---- */
    @media (max-width: 768px) {
      .hero-inner {
        grid-template-columns: 1fr;
      }
      .hero-fragments {
        display: none;
      }
      .about {
        grid-template-columns: 1fr;
      }
      .about-collage {
        min-height: 250px;
      }
      nav { padding: 0 20px; }
      .nav-links { gap: 16px; }
      .nav-links a { font-size: 0.75rem; }
    }
  </style>
</head>
<body>

  <!-- Navigation -->
  <nav>
    <a href="#" class="nav-logo">Cubisme</a>
    <ul class="nav-links">
      <li><a href="#">Perspectives</a></li>
      <li><a href="#">Fragments</a></li>
      <li><a href="#">Collage</a></li>
      <li><a href="#">Gallery</a></li>
    </ul>
  </nav>

  <!-- Hero -->
  <div class="hero">
    <div class="hero-inner">
      <div>
        <h1>Multiple<br><span class="accent">Perspectives</span></h1>
        <p>Fragmented forms, geometric planes, and the rejection of single-point perspective. A design language born from the most revolutionary art movement of the twentieth century.</p>
        <a href="#" class="hero-btn">Explore Fragments</a>
      </div>
      <div class="hero-fragments">
        <div class="frag-1"></div>
        <div class="frag-2"></div>
        <div class="frag-3"></div>
        <div class="frag-4"></div>
      </div>
    </div>
  </div>

  <!-- Divider -->
  <div class="divider"></div>

  <!-- About -->
  <section class="about">
    <div>
      <h2>Deconstructed Vision</h2>
      <p>Cubism dismantled the conventions of representation that had governed Western art since the Renaissance. Objects are analyzed, broken apart, and reassembled as faceted geometric planes -- viewed from all angles at once rather than from a single fixed point.</p>
      <p style="margin-top:1rem;">This approach transforms web design into a dynamic field of overlapping perspectives, where content panels intersect like the fragmented still lifes of Braque and Picasso.</p>
    </div>
    <div class="about-collage">
      <div class="plane plane-a">
        <span class="plane-label">Analytical Phase</span>
        <p style="font-size:0.9rem;">Monochromatic deconstruction of form into dense geometric facets.</p>
      </div>
      <div class="plane plane-b">
        <span class="plane-label">Synthetic Phase</span>
        <p style="font-size:0.9rem;">Bolder colors and collage elements reassemble fragmented forms.</p>
      </div>
      <div class="plane plane-c">
        <span class="plane-label">Digital Translation</span>
        <p style="font-size:0.9rem;">Overlapping layouts, angular containers, and multi-axis compositions.</p>
      </div>
    </div>
  </section>

  <!-- Zigzag -->
  <div class="zigzag"></div>

  <!-- Cards -->
  <section class="cards-section">
    <h2>Geometric Principles</h2>
    <div class="card-grid">
      <div class="card">
        <div class="card-number">01</div>
        <h3>Fragmentation</h3>
        <p>Break every element into its geometric components. Nothing remains whole; everything is faceted, analyzed, and reconstructed.</p>
      </div>
      <div class="card">
        <div class="card-number">02</div>
        <h3>Simultaneity</h3>
        <p>Present multiple viewpoints at once. Overlapping panels reveal different aspects of content simultaneously.</p>
      </div>
      <div class="card">
        <div class="card-number">03</div>
        <h3>Flat Depth</h3>
        <p>Suggest spatial relationships through overlapping planes rather than vanishing points or realistic shadows.</p>
      </div>
    </div>
  </section>

  <!-- Statement -->
  <div class="statement">
    <h2>The Object Has No Fixed Form</h2>
    <p>In Cubism, reality is not a single snapshot from a single position. It is the sum of all possible views, compressed into a unified composition of interlocking planes and angles.</p>
  </div>

  <!-- Footer -->
  <footer>
    <div class="footer-logo">Cubisme</div>
    <p>A design reference for the Cubist aesthetic. Fragmented forms, multiple perspectives, geometric truth.</p>
  </footer>

</body>
</html>
```
