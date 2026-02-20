# Deconstructivism Design Reference

## Overview

Deconstructivism is a radical design philosophy rooted in Jacques Derrida's literary theory of deconstruction and the formal experiments of Russian Constructivism, challenging the assumption that structures -- whether architectural, typographic, or digital -- must express harmony, stability, or coherent order. Emerging as a recognizable movement through the landmark 1988 "Deconstructivist Architecture" exhibition at MoMA (curated by Philip Johnson and Mark Wigley), it crystallized around the work of Frank Gehry, Daniel Libeskind, Zaha Hadid, Rem Koolhaas, Peter Eisenman, Coop Himmelb(l)au, and Bernard Tschumi -- architects who fragmented, distorted, and collided conventional forms to expose the instability hidden within every "stable" structure. In graphic design, practitioners like David Carson (Ray Gun magazine), the Cranbrook Academy school, and the Emigre foundry translated these ideas into shattered grids, illegible-by-choice typography, overlapping layers, and the deliberate disruption of visual hierarchy. On the web, Deconstructivism manifests as broken grid layouts, extreme angular transforms, overlapping and colliding elements, clashing typographic scales, z-index warfare, clip-path fragmentation, and interfaces that subvert conventional UX patterns -- not for chaos alone, but to reveal that the "natural" order of a webpage is itself an arbitrary construct. The aesthetic demands active engagement from the viewer: nothing is passively consumable, every element questions its own placement, and the tension between structure and collapse is the design itself.

---

## Visual Characteristics

### Core Design Traits

- **Fragmented composition**: Elements appear broken apart, sliced, or shattered -- cards split at angles, sections overlap unevenly, and layout blocks collide as though the page has been subjected to tectonic force
- **Extreme angular geometry**: Diagonal lines, acute angles, and non-rectilinear shapes dominate; nothing sits comfortably at 90 degrees, with skewed transforms applied to containers, text blocks, and dividers
- **Deliberate instability**: Layouts feel precarious and off-balance, with asymmetric weight distribution, elements that appear to slide or topple, and visual tension that resists resolution into comfortable equilibrium
- **Overlapping and layered elements**: Content blocks, images, and typography occupy the same spatial plane, overlapping via z-index stacking, negative margins, and absolute positioning to create depth through collision
- **Distorted and deconstructed typography**: Letterforms are stretched, rotated, fragmented, given extreme tracking, or set at conflicting scales -- type is treated as a visual object to be manipulated, not merely a vessel for content
- **Non-Euclidean spatial relationships**: Elements ignore the conventional Cartesian grid; shapes curve, fold, and intersect in ways that suggest warped or folded space rather than flat screen coordinates
- **Material contrast and collision**: Disparate visual textures -- raw concrete grays, polished metallics, translucent overlays, sharp wireframes -- collide within the same composition without blending or harmonizing
- **Exposed structural logic**: Grids, alignment guides, construction lines, and wireframe scaffolding are made visible as part of the design rather than hidden beneath a polished surface
- **Void and negative space as active elements**: Large, irregular voids are cut into the layout, functioning not as rest areas but as deliberate ruptures that fragment the reading experience
- **Kinetic tension without motion**: Static layouts suggest movement, explosion, or collapse through directional lines, implied vectors, and the placement of elements along diagonal axes

### Design Principles

- **Structure exists to be questioned**: Every grid, alignment rule, and convention is a starting point to be subverted; the design should make the viewer aware of the systems it dismantles
- **Tension over resolution**: Compositions should sustain visual conflict rather than resolving into comfortable balance; opposing forces (scale, direction, weight) remain in permanent dialectic
- **Form follows fracture**: Rather than expressing unified purpose, the design reveals the fractures, contradictions, and multiplicity of meaning within any structure
- **The viewer must work**: Deconstructivist design demands active interpretation; legibility and navigability are deliberately complicated to transform passive consumption into engaged reading
- **Collision is composition**: Overlapping, intersecting, and conflicting elements are not errors but the primary compositional strategy; meaning emerges from the friction between parts
- **No element is neutral**: Every design choice -- margin, angle, typeface, color -- carries ideological weight; the design should expose rather than naturalize these choices
- **Incompleteness as intent**: The design should appear unfinished, in-process, or mid-collapse; polish and perfection are antithetical to the deconstructivist stance

---

## Color Palette

Deconstructivism draws from the raw materiality of architectural concrete, steel, and titanium, punctuated by aggressive signal colors that slash across the neutral foundation. Palettes are deliberately dissonant -- industrial grays meet high-voltage accents, and harmonious relationships are avoided in favor of jarring juxtaposition.

| Swatch | Hex | Role / Usage |
|--------|-----|-------------|
| ![#1A1A1A](https://via.placeholder.com/20/1A1A1A/1A1A1A) | `#1A1A1A` | Primary dark ground, deep structural surfaces |
| ![#2C2C2C](https://via.placeholder.com/20/2C2C2C/2C2C2C) | `#2C2C2C` | Secondary dark surface, layered panels |
| ![#4A4A4A](https://via.placeholder.com/20/4A4A4A/4A4A4A) | `#4A4A4A` | Concrete mid-gray, muted structural elements |
| ![#7B7B7B](https://via.placeholder.com/20/7B7B7B/7B7B7B) | `#7B7B7B` | Exposed aggregate gray, secondary text |
| ![#A8A8A8](https://via.placeholder.com/20/A8A8A8/A8A8A8) | `#A8A8A8` | Light concrete, wireframe lines, ghost elements |
| ![#E0E0E0](https://via.placeholder.com/20/E0E0E0/E0E0E0) | `#E0E0E0` | Light surface, negative space fills |
| ![#F5F5F0](https://via.placeholder.com/20/F5F5F0/F5F5F0) | `#F5F5F0` | Off-white ground, paper-like backgrounds |
| ![#FFFFFF](https://via.placeholder.com/20/FFFFFF/FFFFFF) | `#FFFFFF` | Pure white, high-contrast text on dark |
| ![#FF2D2D](https://via.placeholder.com/20/FF2D2D/FF2D2D) | `#FF2D2D` | Primary accent slash, danger, structural fracture lines |
| ![#FF6B00](https://via.placeholder.com/20/FF6B00/FF6B00) | `#FF6B00` | Warning signal, aggressive highlight |
| ![#FFD600](https://via.placeholder.com/20/FFD600/FFD600) | `#FFD600` | Caution accent, construction-zone reference |
| ![#0066FF](https://via.placeholder.com/20/0066FF/0066FF) | `#0066FF` | Blueprint blue, technical overlay, interactive elements |
| ![#00E5A0](https://via.placeholder.com/20/00E5A0/00E5A0) | `#00E5A0` | Digital accent, secondary interactive state |
| ![#C8B8DB](https://via.placeholder.com/20/C8B8DB/C8B8DB) | `#C8B8DB` | Titanium reflection, muted ethereal accent |
| ![#D4D4D4](https://via.placeholder.com/20/D4D4D4/D4D4D4) | `#D4D4D4` | Steel surface, brushed metal reference, borders |

### CSS Custom Properties

```css
:root {
  /* --- Structural Grays (Concrete & Steel) --- */
  --decon-black: #1a1a1a;
  --decon-dark: #2c2c2c;
  --decon-concrete: #4a4a4a;
  --decon-aggregate: #7b7b7b;
  --decon-light-concrete: #a8a8a8;
  --decon-surface: #e0e0e0;
  --decon-ground: #f5f5f0;
  --decon-white: #ffffff;
  --decon-steel: #d4d4d4;

  /* --- Signal Accents --- */
  --decon-red: #ff2d2d;
  --decon-orange: #ff6b00;
  --decon-yellow: #ffd600;
  --decon-blue: #0066ff;
  --decon-green: #00e5a0;
  --decon-titanium: #c8b8db;

  /* --- Functional Tokens --- */
  --decon-bg: var(--decon-ground);
  --decon-text: var(--decon-black);
  --decon-text-muted: var(--decon-aggregate);
  --decon-border: var(--decon-concrete);
  --decon-accent: var(--decon-red);
  --decon-interactive: var(--decon-blue);
  --decon-highlight: var(--decon-yellow);
  --decon-panel-dark: var(--decon-dark);
  --decon-panel-light: var(--decon-surface);
}
```

---

## Typography

Deconstructivist typography treats letterforms as architectural material to be fragmented, collided, and distorted. Typefaces are chosen for their ability to sustain extreme manipulation -- condensed or extended widths, heavy weights that hold up under rotation and clipping, and monospaced faces that expose the mechanical grid of text. Pairings are deliberately dissonant: a hyper-geometric display face clashes with a raw monospace body, or an ultra-condensed headline collides with a wide, generous serif.

### Recommended Google Fonts

| Font | Weight(s) | Usage | Link |
|------|-----------|-------|------|
| Bebas Neue | 400 | Display headlines, oversized titling, angular compositions | [fonts.google.com/specimen/Bebas+Neue](https://fonts.google.com/specimen/Bebas+Neue) |
| Oswald | 300, 400, 700 | Condensed headlines, navigation labels, structural text | [fonts.google.com/specimen/Oswald](https://fonts.google.com/specimen/Oswald) |
| Archivo Black | 400 | Impact headlines, all-caps slab display | [fonts.google.com/specimen/Archivo+Black](https://fonts.google.com/specimen/Archivo+Black) |
| Space Grotesk | 300, 400, 700 | Geometric body text, UI elements, captions | [fonts.google.com/specimen/Space+Grotesk](https://fonts.google.com/specimen/Space+Grotesk) |
| Space Mono | 400, 700 | Code, metadata, exposed structural text, monospaced body | [fonts.google.com/specimen/Space+Mono](https://fonts.google.com/specimen/Space+Mono) |
| Syne | 400, 500, 700, 800 | Expressive display, distorted headlines, art-direction type | [fonts.google.com/specimen/Syne](https://fonts.google.com/specimen/Syne) |
| Inter | 400, 700, 900 | Clean body text fallback, UI labels, form elements | [fonts.google.com/specimen/Inter](https://fonts.google.com/specimen/Inter) |
| Chakra Petch | 300, 400, 700 | Technical display, angular aesthetic, futurist accent | [fonts.google.com/specimen/Chakra+Petch](https://fonts.google.com/specimen/Chakra+Petch) |

### Font Pairing Suggestions

| Heading | Body | Vibe |
|---------|------|------|
| Bebas Neue | Space Mono | Towering condensed verticals meet raw mechanical grid -- the architect's blueprint |
| Syne (800) | Space Grotesk | Expressive, slightly warped display headlines against clean geometric body -- controlled chaos |
| Archivo Black | Inter | Heavyweight slab impact over neutral Swiss body -- the collision of brute force and rationalism |
| Oswald (700) | Space Mono | Narrow condensed headings with monospaced precision -- structural compression and exposed scaffolding |
| Chakra Petch | Space Grotesk | Angular futurist display paired with geometric clarity -- Hadid's curves meet Eisenman's grids |

### CSS Example

```css
@import url('https://fonts.googleapis.com/css2?family=Bebas+Neue&family=Syne:wght@400;700;800&family=Space+Mono:wght@400;700&family=Space+Grotesk:wght@300;400;700&display=swap');

/* === Deconstructivist Base Typography === */
body {
  font-family: 'Space Grotesk', 'Segoe UI', system-ui, sans-serif;
  font-size: 16px;
  line-height: 1.6;
  color: var(--decon-text);
  background-color: var(--decon-bg);
  letter-spacing: 0.01em;
}

h1, h2, h3, h4, h5, h6 {
  font-family: 'Bebas Neue', 'Impact', 'Arial Narrow', sans-serif;
  text-transform: uppercase;
  letter-spacing: 0.04em;
  line-height: 0.92;
  margin: 0 0 0.5em 0;
}

h1 {
  font-size: clamp(4rem, 10vw, 10rem);
  letter-spacing: -0.02em;
}

h2 {
  font-size: clamp(2.5rem, 6vw, 5rem);
}

h3 {
  font-family: 'Syne', 'Arial Black', sans-serif;
  font-weight: 800;
  font-size: clamp(1.5rem, 3vw, 2.5rem);
  text-transform: none;
  letter-spacing: -0.01em;
}

/* Deconstructed link style -- slash accent on hover */
a {
  color: var(--decon-interactive);
  text-decoration: none;
  border-bottom: 2px solid transparent;
  transition: border-color 0.15s ease;
}

a:hover {
  border-bottom-color: var(--decon-accent);
  color: var(--decon-accent);
}

/* Monospaced metadata / structural text */
.mono {
  font-family: 'Space Mono', 'Courier New', monospace;
  font-size: 0.8rem;
  letter-spacing: 0.08em;
  text-transform: uppercase;
  color: var(--decon-text-muted);
}

/* Fragmented text -- letters spaced and rotated */
.decon-shatter-text {
  font-family: 'Bebas Neue', sans-serif;
  font-size: clamp(3rem, 8vw, 8rem);
  text-transform: uppercase;
  display: flex;
  flex-wrap: wrap;
}

.decon-shatter-text span {
  display: inline-block;
  transform: rotate(calc(var(--r, 0) * 1deg)) translateY(calc(var(--y, 0) * 1px));
  transition: transform 0.2s ease;
}

blockquote {
  border-left: 4px solid var(--decon-accent);
  padding: 1rem 1.5rem;
  margin: 2rem 0;
  background-color: var(--decon-panel-light);
  transform: rotate(-0.5deg);
  font-style: italic;
}

code, pre {
  font-family: 'Space Mono', 'Courier New', monospace;
  background-color: var(--decon-dark);
  color: var(--decon-white);
  border: 1px solid var(--decon-concrete);
}

code { padding: 0.2em 0.4em; font-size: 0.875em; }
pre { padding: 1.5rem; overflow-x: auto; white-space: pre; }
```

---

## Layout Principles

- **Broken grid as default**: Abandon the uniform 12-column grid; use CSS Grid with irregularly sized tracks, overlapping grid areas, and items that deliberately span or break out of their containers
- **Diagonal axis composition**: Orient the primary compositional flow along a diagonal rather than horizontal/vertical; use `transform: rotate()` on section-level containers to tilt entire layout regions
- **Z-index layering as spatial depth**: Build compositions through aggressive stacking -- background planes, mid-ground content, and foreground accent elements occupy distinct z-index layers, with overlaps creating the illusion of architectural depth
- **Negative margin collisions**: Use negative margins to force elements into each other's space, creating intentional overlaps between sections, cards, text blocks, and images
- **Asymmetric weight distribution**: Place the heaviest visual elements (large type, dark panels, dense content) off-center, forcing the layout into a state of deliberate imbalance
- **Viewport-breaking elements**: Allow elements to extend beyond the viewport edge using `overflow: visible` or negative positioning, suggesting that the design continues beyond the visible frame
- **Section ruptures over smooth transitions**: Instead of gradual transitions between page sections, use sharp angular dividers, clip-path cuts, or abrupt material changes to create visible fracture lines
- **Whitespace as void**: Large empty areas are not neutral rest zones but active negative space -- angular voids cut into the layout that fragment the reading path and force the eye to jump
- **Multiple reading directions**: Unlike conventional top-to-bottom flow, Deconstructivist layouts may present content along competing axes, requiring the viewer to choose and navigate between simultaneous reading paths
- **Responsive fragmentation**: At smaller viewports, do not simply stack elements vertically; instead, maintain angular relationships and overlapping behaviors, scaling the degree of fragmentation proportionally

---

## CSS / Design Techniques

### Fractured Card

A content card that appears sliced and displaced, with angular clip-paths and offset layers that suggest structural failure.

```css
.decon-card {
  position: relative;
  background-color: var(--decon-white);
  border: 2px solid var(--decon-border);
  padding: 2rem;
  transform: rotate(-1.5deg);
  clip-path: polygon(0 0, 100% 2%, 98% 100%, 3% 97%);
  transition: transform 0.3s ease, box-shadow 0.3s ease;
}

.decon-card::before {
  content: '';
  position: absolute;
  top: -4px;
  left: -4px;
  right: -4px;
  bottom: -4px;
  background-color: var(--decon-accent);
  z-index: -1;
  clip-path: polygon(2% 1%, 100% 0, 97% 100%, 0 98%);
}

.decon-card:hover {
  transform: rotate(0deg) scale(1.02);
  box-shadow: -6px 6px 0 var(--decon-black);
}

.decon-card h3 {
  font-family: 'Syne', sans-serif;
  font-weight: 800;
  font-size: 1.5rem;
  margin-bottom: 0.75rem;
  border-bottom: 2px solid var(--decon-accent);
  padding-bottom: 0.5rem;
}

.decon-card p {
  font-size: 0.95rem;
  line-height: 1.6;
  color: var(--decon-concrete);
}

.decon-card .tag {
  display: inline-block;
  font-family: 'Space Mono', monospace;
  font-size: 0.65rem;
  text-transform: uppercase;
  letter-spacing: 0.12em;
  border: 1px solid var(--decon-border);
  padding: 0.2rem 0.6rem;
  margin-top: 1rem;
  margin-right: 0.25rem;
  transform: rotate(1deg);
}
```

### Angular Button

Buttons with aggressive clip-paths, slashed corners, and volatile hover states that feel like pressing a structural trigger.

```css
.decon-btn {
  display: inline-block;
  font-family: 'Bebas Neue', 'Impact', sans-serif;
  font-size: 1.1rem;
  letter-spacing: 0.12em;
  text-transform: uppercase;
  padding: 0.9rem 2.2rem;
  background-color: var(--decon-black);
  color: var(--decon-white);
  border: none;
  clip-path: polygon(8% 0, 100% 0, 92% 100%, 0 100%);
  cursor: pointer;
  text-decoration: none;
  position: relative;
  transition: background-color 0.2s ease, transform 0.2s ease;
}

.decon-btn:hover {
  background-color: var(--decon-accent);
  transform: skewX(-3deg);
}

.decon-btn:active {
  background-color: var(--decon-orange);
  transform: skewX(-3deg) scale(0.97);
}

/* Outline variant */
.decon-btn--outline {
  background-color: transparent;
  color: var(--decon-black);
  border: 2px solid var(--decon-black);
  clip-path: polygon(6% 0, 100% 0, 94% 100%, 0 100%);
}

.decon-btn--outline:hover {
  background-color: var(--decon-black);
  color: var(--decon-white);
}
```

### Deconstructed Navigation

A navigation bar where links are scattered at slight angles, resisting the horizontal alignment convention, with a fractured baseline and exposed structural markers.

```css
.decon-nav {
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 1rem 2rem;
  border-bottom: 3px solid var(--decon-black);
  position: relative;
  overflow: visible;
}

.decon-nav::after {
  content: '';
  position: absolute;
  bottom: -3px;
  left: 0;
  width: 100%;
  height: 3px;
  background: repeating-linear-gradient(
    90deg,
    var(--decon-accent) 0,
    var(--decon-accent) 30px,
    transparent 30px,
    transparent 60px
  );
}

.decon-nav .logo {
  font-family: 'Bebas Neue', sans-serif;
  font-size: 1.8rem;
  letter-spacing: 0.08em;
  color: var(--decon-black);
  text-decoration: none;
  transform: rotate(-2deg);
}

.decon-nav ul {
  list-style: none;
  display: flex;
  gap: 0;
  padding: 0;
  margin: 0;
}

.decon-nav li {
  transform: rotate(calc(var(--tilt, 0) * 1deg));
}

.decon-nav li:nth-child(odd) { --tilt: -1.5; }
.decon-nav li:nth-child(even) { --tilt: 1; }

.decon-nav a {
  display: block;
  padding: 0.5rem 1.2rem;
  font-family: 'Space Grotesk', sans-serif;
  font-size: 0.85rem;
  font-weight: 700;
  text-transform: uppercase;
  letter-spacing: 0.1em;
  color: var(--decon-black);
  text-decoration: none;
  border: none;
  position: relative;
}

.decon-nav a::after {
  content: '/';
  position: absolute;
  right: -2px;
  top: 50%;
  transform: translateY(-50%);
  color: var(--decon-accent);
  font-weight: 400;
}

.decon-nav li:last-child a::after { content: none; }

.decon-nav a:hover {
  background-color: var(--decon-black);
  color: var(--decon-white);
  transform: skewX(-5deg);
}
```

### Hero Section -- Shattered Title

A hero section where the title appears fractured across the viewport, with fragments at different angles and z-indices, and a diagonal slash dividing the section.

```css
.decon-hero {
  position: relative;
  min-height: 100vh;
  display: flex;
  flex-direction: column;
  justify-content: center;
  padding: 4rem;
  background-color: var(--decon-black);
  color: var(--decon-white);
  overflow: hidden;
}

/* Diagonal slash divider */
.decon-hero::before {
  content: '';
  position: absolute;
  top: -10%;
  right: 30%;
  width: 3px;
  height: 120%;
  background-color: var(--decon-accent);
  transform: rotate(15deg);
  z-index: 1;
}

/* Grid construction line overlay */
.decon-hero::after {
  content: '';
  position: absolute;
  inset: 0;
  background:
    repeating-linear-gradient(
      0deg,
      transparent,
      transparent 99px,
      rgba(255, 255, 255, 0.03) 99px,
      rgba(255, 255, 255, 0.03) 100px
    ),
    repeating-linear-gradient(
      90deg,
      transparent,
      transparent 99px,
      rgba(255, 255, 255, 0.03) 99px,
      rgba(255, 255, 255, 0.03) 100px
    );
  pointer-events: none;
  z-index: 0;
}

.decon-hero > * {
  position: relative;
  z-index: 2;
}

.decon-hero h1 {
  font-size: clamp(4rem, 12vw, 12rem);
  line-height: 0.85;
  transform: rotate(-2deg);
  margin-left: -0.05em;
}

.decon-hero h1 span {
  display: block;
}

.decon-hero h1 .fragment-shift {
  transform: translateX(8vw) rotate(1deg);
  color: var(--decon-accent);
}

.decon-hero .subtitle {
  font-family: 'Space Mono', monospace;
  font-size: clamp(0.85rem, 1.5vw, 1.1rem);
  max-width: 45ch;
  margin-top: 2rem;
  line-height: 1.7;
  transform: rotate(-0.5deg);
  color: var(--decon-light-concrete);
}

.decon-hero .hero-meta {
  font-family: 'Space Mono', monospace;
  font-size: 0.7rem;
  text-transform: uppercase;
  letter-spacing: 0.15em;
  color: var(--decon-aggregate);
  margin-top: 3rem;
}
```

### Shattered Grid Layout

A CSS Grid layout where items are deliberately misaligned, overlapping, and rotated to create a fractured spatial composition.

```css
.decon-shattered-grid {
  display: grid;
  grid-template-columns: repeat(12, 1fr);
  grid-template-rows: auto;
  gap: 0;
  padding: 4rem 2rem;
  position: relative;
}

.decon-shattered-grid .item-a {
  grid-column: 1 / 7;
  grid-row: 1 / 2;
  transform: rotate(-1.5deg);
  z-index: 2;
  background-color: var(--decon-white);
  border: 2px solid var(--decon-border);
  padding: 2rem;
  margin-right: -3rem; /* Overlap into adjacent space */
}

.decon-shattered-grid .item-b {
  grid-column: 5 / 13;
  grid-row: 1 / 2;
  transform: rotate(1deg) translateY(3rem);
  z-index: 1;
  background-color: var(--decon-dark);
  color: var(--decon-white);
  padding: 2rem;
  margin-left: -2rem; /* Collision with item-a */
}

.decon-shattered-grid .item-c {
  grid-column: 2 / 8;
  grid-row: 2 / 3;
  transform: rotate(0.5deg) translateY(-2rem);
  z-index: 3;
  background-color: var(--decon-accent);
  color: var(--decon-white);
  padding: 2rem;
  clip-path: polygon(0 4%, 100% 0, 97% 100%, 3% 96%);
}

.decon-shattered-grid .item-d {
  grid-column: 7 / 13;
  grid-row: 2 / 3;
  transform: rotate(-2deg) translateY(1rem);
  z-index: 2;
  background-color: var(--decon-surface);
  border: 2px solid var(--decon-border);
  padding: 2rem;
}

/* Structural annotation lines */
.decon-shattered-grid::before {
  content: '';
  position: absolute;
  top: 2rem;
  left: 50%;
  width: 2px;
  height: calc(100% - 4rem);
  background: var(--decon-light-concrete);
  transform: rotate(5deg);
  opacity: 0.4;
  z-index: 0;
}
```

### Angular Clip-Path Section Divider

A section transition that uses aggressive angular clip-paths to create a fractured boundary between content zones.

```css
.decon-divider-section {
  position: relative;
  padding: 6rem 2rem;
  background-color: var(--decon-dark);
  color: var(--decon-white);
  clip-path: polygon(
    0 6%,
    100% 0,
    100% 94%,
    0 100%
  );
  margin: -3rem 0;
  z-index: 2;
}

/* Double-slash accent marks */
.decon-divider-section::before {
  content: '//';
  position: absolute;
  top: 2rem;
  right: 3rem;
  font-family: 'Bebas Neue', sans-serif;
  font-size: 6rem;
  color: var(--decon-accent);
  opacity: 0.3;
  line-height: 1;
}

.decon-divider-section h2 {
  transform: rotate(-1deg);
  display: inline-block;
}
```

### Tilted Panel with Offset Border

A content panel that sits at an angle with a deliberately displaced border frame, creating the illusion of structural misalignment.

```css
.decon-tilted-panel {
  position: relative;
  padding: 3rem;
  margin: 4rem 2rem;
  background-color: var(--decon-white);
  transform: rotate(-1deg);
}

/* Displaced border frame */
.decon-tilted-panel::before {
  content: '';
  position: absolute;
  top: 8px;
  left: -8px;
  right: 8px;
  bottom: -8px;
  border: 2px solid var(--decon-black);
  transform: rotate(0.5deg);
  z-index: -1;
}

/* Accent corner mark */
.decon-tilted-panel::after {
  content: '';
  position: absolute;
  top: -6px;
  right: -6px;
  width: 24px;
  height: 24px;
  background-color: var(--decon-accent);
  clip-path: polygon(0 0, 100% 0, 100% 100%);
}

.decon-tilted-panel h3 {
  font-family: 'Syne', sans-serif;
  font-weight: 800;
  font-size: 1.8rem;
  margin-bottom: 1rem;
}

.decon-tilted-panel p {
  font-size: 0.95rem;
  line-height: 1.7;
  max-width: 60ch;
}
```

### Fractured Image Container

An image wrapper that fragments the photo using clip-paths and overlapping pseudo-elements, as though the frame has been shattered.

```css
.decon-image-frame {
  position: relative;
  display: inline-block;
  transform: rotate(-2deg);
}

.decon-image-frame img {
  display: block;
  width: 100%;
  clip-path: polygon(2% 0, 100% 3%, 97% 100%, 0 96%);
  filter: grayscale(40%) contrast(1.1);
}

/* Offset color shard */
.decon-image-frame::before {
  content: '';
  position: absolute;
  top: -10px;
  left: -10px;
  width: 40%;
  height: 40%;
  background-color: var(--decon-accent);
  clip-path: polygon(0 0, 100% 15%, 80% 100%, 10% 85%);
  z-index: -1;
  opacity: 0.7;
}

/* Structural line overlay */
.decon-image-frame::after {
  content: '';
  position: absolute;
  top: 50%;
  left: -5%;
  width: 110%;
  height: 2px;
  background-color: var(--decon-accent);
  transform: rotate(8deg);
  z-index: 2;
}
```

---

## Design Do's and Don'ts

### Do's

- **Embrace visual tension and imbalance** -- let elements collide, overlap, and compete for attention; the discomfort is the design working as intended
- **Use CSS transforms extensively** -- `rotate()`, `skewX()`, `translateX/Y()`, and `scale()` are your primary layout tools for breaking conventional alignment
- **Expose the structural grid** -- show construction lines, grid overlays, alignment markers, and wireframe scaffolding as visible design elements
- **Mix typography aggressively** -- combine condensed and extended faces, clash serif with monospace, set type at conflicting scales and angles within the same composition
- **Use clip-path for angular fragmentation** -- create non-rectangular containers, slashed section dividers, and shattered image frames using CSS `clip-path: polygon()`
- **Create intentional overlaps with z-index** -- layer content blocks, typographic elements, and accent shapes into spatial depth using absolute positioning and z-index stacking
- **Apply angular dividers between sections** -- replace horizontal lines with diagonal slashes, angled clip-path transitions, and rotated separator elements
- **Maintain a functional structure beneath the chaos** -- the DOM should be semantic and accessible even when the visual presentation is fragmented; use `aria-` attributes and logical heading hierarchy
- **Use monochrome foundations with aggressive accents** -- keep the base palette in concrete grays and let signal colors (red, orange, yellow) slice across the composition

### Don'ts

- **Don't confuse chaos with randomness** -- every angle, overlap, and collision should be a deliberate compositional choice; random noise is not deconstruction
- **Don't sacrifice all readability** -- body text should remain legible even within a fragmented layout; save extreme typographic distortion for display elements and headlines
- **Don't use rounded corners or soft shadows** -- border-radius and diffused box-shadows soften the architectural angularity that defines the aesthetic; keep edges sharp and shadows hard
- **Don't apply the aesthetic uniformly** -- monotonous repetition of the same angle or overlap across every element defeats the purpose; vary the degree and direction of fragmentation
- **Don't ignore accessibility** -- ensure keyboard navigation works, focus states are visible, color contrast meets WCAG standards for body text, and screen readers can parse the content in logical order
- **Don't overuse animation** -- the tension in Deconstructivism is primarily spatial and static; excessive motion design dilutes the architectural weight of the composition
- **Don't use stock photography without treatment** -- polished stock images contradict the raw aesthetic; if images are used, apply grayscale filters, clip-path fragmentation, or duotone treatments
- **Don't center everything symmetrically** -- centered, balanced compositions are the antithesis of the deconstructivist stance; off-center, diagonal, and edge-aligned placement is essential

---

## Related Aesthetics

| Aesthetic | Relationship |
|-----------|-------------|
| [Brutalist Web Design](Brutalist_Web_Design.md) | Shares the anti-polish, structural-honesty ethos, but Brutalism strips to raw defaults while Deconstructivism actively fragments and reconstructs form |
| [Constructivism](Constructivism.md) | The direct historical ancestor -- Deconstructivism takes Constructivist geometry and dynamism and subjects it to rupture and disassembly |
| [Dadaism](Dadaism.md) | Both reject rational order, but Dada works through absurdist collage and anti-art provocation while Deconstructivism operates through architectural rigor turned against itself |
| [New Wave](New_Wave.md) | New Wave (Weingart, Emigre era) is the typographic bridge between Swiss modernism and deconstruction; shares the layering and grid-breaking but retains more playfulness |
| [Cyberpunk](Cyberpunk.md) | Both use angular fragmentation and industrial materials, but Cyberpunk is narrative and world-building while Deconstructivism is philosophical and structural |
| [Futurism](Futurism.md) | Futurism's dynamic diagonals and kinetic typography anticipate Deconstructivism's angularity, but Futurism celebrates speed and progress while Deconstructivism interrogates stability |
| [Raw Industrial](Raw_Industrial.md) | Kindred material vocabulary -- exposed steel, concrete, visible structure -- but Raw Industrial is honest about material while Deconstructivism is deliberately destabilizing |
| [Neubrutalism](Neubrutalism.md) | A more approachable, UI-friendly cousin; Neubrutalism's thick borders and hard shadows are a domesticated echo of Deconstructivism's aggressive fragmentation |
| [Maximalism](Maximalism.md) | Both reject minimalist restraint and embrace visual density, but Maximalism accumulates and celebrates while Deconstructivism fractures and interrogates |

---

## Quick-Start HTML Template

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Deconstructivism -- Design Template</title>
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Bebas+Neue&family=Syne:wght@400;700;800&family=Space+Mono:wght@400;700&family=Space+Grotesk:wght@300;400;700&display=swap" rel="stylesheet">
  <style>
    /* ============================================
       DECONSTRUCTIVISM -- CSS CUSTOM PROPERTIES
       ============================================ */
    :root {
      --decon-black: #1a1a1a;
      --decon-dark: #2c2c2c;
      --decon-concrete: #4a4a4a;
      --decon-aggregate: #7b7b7b;
      --decon-light-concrete: #a8a8a8;
      --decon-surface: #e0e0e0;
      --decon-ground: #f5f5f0;
      --decon-white: #ffffff;
      --decon-steel: #d4d4d4;
      --decon-red: #ff2d2d;
      --decon-orange: #ff6b00;
      --decon-yellow: #ffd600;
      --decon-blue: #0066ff;
      --decon-green: #00e5a0;
      --decon-titanium: #c8b8db;
    }

    /* ============================================
       RESET & BASE
       ============================================ */
    *, *::before, *::after {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
    }

    body {
      font-family: 'Space Grotesk', 'Segoe UI', system-ui, sans-serif;
      font-size: 16px;
      line-height: 1.6;
      color: var(--decon-black);
      background-color: var(--decon-ground);
      overflow-x: hidden;
    }

    /* ============================================
       TYPOGRAPHY
       ============================================ */
    h1, h2, h4 {
      font-family: 'Bebas Neue', 'Impact', 'Arial Narrow', sans-serif;
      text-transform: uppercase;
      letter-spacing: 0.04em;
      line-height: 0.92;
    }

    h3 {
      font-family: 'Syne', 'Arial Black', sans-serif;
      font-weight: 800;
      line-height: 1.1;
    }

    a {
      color: var(--decon-blue);
      text-decoration: none;
      border-bottom: 2px solid transparent;
      transition: border-color 0.15s ease, color 0.15s ease;
    }

    a:hover {
      color: var(--decon-red);
      border-bottom-color: var(--decon-red);
    }

    .mono {
      font-family: 'Space Mono', 'Courier New', monospace;
      font-size: 0.75rem;
      letter-spacing: 0.1em;
      text-transform: uppercase;
      color: var(--decon-aggregate);
    }

    /* ============================================
       NAVIGATION
       ============================================ */
    .nav {
      display: flex;
      align-items: center;
      justify-content: space-between;
      padding: 1rem 2.5rem;
      border-bottom: 3px solid var(--decon-black);
      position: relative;
      z-index: 100;
      background-color: var(--decon-ground);
    }

    .nav::after {
      content: '';
      position: absolute;
      bottom: -3px;
      left: 0;
      width: 100%;
      height: 3px;
      background: repeating-linear-gradient(
        90deg,
        var(--decon-red) 0,
        var(--decon-red) 25px,
        transparent 25px,
        transparent 50px
      );
    }

    .nav .logo {
      font-family: 'Bebas Neue', sans-serif;
      font-size: 1.6rem;
      letter-spacing: 0.1em;
      color: var(--decon-black);
      text-decoration: none;
      border: none;
      transform: rotate(-2deg);
      display: inline-block;
    }

    .nav .logo:hover {
      color: var(--decon-red);
      border: none;
    }

    .nav ul {
      list-style: none;
      display: flex;
      gap: 0;
    }

    .nav li:nth-child(odd) { transform: rotate(-1.5deg); }
    .nav li:nth-child(even) { transform: rotate(1deg); }

    .nav a {
      display: block;
      padding: 0.4rem 1rem;
      font-family: 'Space Grotesk', sans-serif;
      font-size: 0.8rem;
      font-weight: 700;
      text-transform: uppercase;
      letter-spacing: 0.1em;
      color: var(--decon-black);
      border: none;
    }

    .nav a:hover {
      background-color: var(--decon-black);
      color: var(--decon-white);
      transform: skewX(-5deg);
    }

    /* ============================================
       HERO
       ============================================ */
    .hero {
      position: relative;
      min-height: 100vh;
      display: flex;
      flex-direction: column;
      justify-content: center;
      padding: 4rem;
      background-color: var(--decon-black);
      color: var(--decon-white);
      overflow: hidden;
    }

    /* Diagonal accent slash */
    .hero::before {
      content: '';
      position: absolute;
      top: -10%;
      right: 32%;
      width: 3px;
      height: 120%;
      background-color: var(--decon-red);
      transform: rotate(15deg);
      z-index: 1;
    }

    /* Grid construction lines overlay */
    .hero::after {
      content: '';
      position: absolute;
      inset: 0;
      background:
        repeating-linear-gradient(
          0deg,
          transparent,
          transparent 79px,
          rgba(255, 255, 255, 0.025) 79px,
          rgba(255, 255, 255, 0.025) 80px
        ),
        repeating-linear-gradient(
          90deg,
          transparent,
          transparent 79px,
          rgba(255, 255, 255, 0.025) 79px,
          rgba(255, 255, 255, 0.025) 80px
        );
      pointer-events: none;
      z-index: 0;
    }

    .hero > * {
      position: relative;
      z-index: 2;
    }

    .hero h1 {
      font-size: clamp(4rem, 11vw, 11rem);
      line-height: 0.85;
      transform: rotate(-2deg);
      margin-left: -0.05em;
    }

    .hero h1 .fragment {
      display: block;
    }

    .hero h1 .fragment-shift {
      display: block;
      transform: translateX(8vw) rotate(1deg);
      color: var(--decon-red);
    }

    .hero .subtitle {
      font-family: 'Space Mono', monospace;
      font-size: clamp(0.8rem, 1.3vw, 1rem);
      max-width: 48ch;
      margin-top: 2.5rem;
      line-height: 1.8;
      transform: rotate(-0.5deg);
      color: var(--decon-light-concrete);
    }

    .hero .hero-meta {
      font-family: 'Space Mono', monospace;
      font-size: 0.7rem;
      text-transform: uppercase;
      letter-spacing: 0.15em;
      color: var(--decon-aggregate);
      margin-top: 3rem;
    }

    .hero .btn-row {
      margin-top: 2.5rem;
      display: flex;
      flex-wrap: wrap;
      gap: 1rem;
    }

    /* ============================================
       BUTTONS
       ============================================ */
    .btn {
      display: inline-block;
      font-family: 'Bebas Neue', 'Impact', sans-serif;
      font-size: 1.1rem;
      letter-spacing: 0.12em;
      text-transform: uppercase;
      padding: 0.85rem 2rem;
      background-color: var(--decon-white);
      color: var(--decon-black);
      border: none;
      clip-path: polygon(6% 0, 100% 0, 94% 100%, 0 100%);
      cursor: pointer;
      text-decoration: none;
      transition: background-color 0.2s ease, transform 0.2s ease;
    }

    .btn:hover {
      background-color: var(--decon-red);
      color: var(--decon-white);
      transform: skewX(-3deg);
      border: none;
    }

    .btn--outline {
      background-color: transparent;
      color: var(--decon-white);
      border: 2px solid var(--decon-white);
      clip-path: none;
    }

    .btn--outline:hover {
      background-color: var(--decon-white);
      color: var(--decon-black);
    }

    /* ============================================
       SECTION BASE
       ============================================ */
    .section {
      padding: 5rem 2.5rem;
      position: relative;
    }

    .section h2 {
      font-size: clamp(2.5rem, 6vw, 5rem);
      margin-bottom: 1rem;
      transform: rotate(-1deg);
      display: inline-block;
    }

    .section .section-subtitle {
      font-family: 'Space Mono', monospace;
      font-size: 0.8rem;
      text-transform: uppercase;
      letter-spacing: 0.15em;
      color: var(--decon-aggregate);
      margin-bottom: 2rem;
      display: block;
    }

    .section p {
      max-width: 65ch;
      margin-bottom: 1rem;
      line-height: 1.7;
    }

    /* ============================================
       ANGULAR DIVIDER SECTION
       ============================================ */
    .divider-section {
      padding: 7rem 2.5rem;
      background-color: var(--decon-dark);
      color: var(--decon-white);
      clip-path: polygon(0 6%, 100% 0, 100% 94%, 0 100%);
      margin: -3rem 0;
      z-index: 2;
      position: relative;
    }

    .divider-section::before {
      content: '//';
      position: absolute;
      top: 3rem;
      right: 3rem;
      font-family: 'Bebas Neue', sans-serif;
      font-size: 5rem;
      color: var(--decon-red);
      opacity: 0.25;
      line-height: 1;
    }

    .divider-section h2 {
      color: var(--decon-white);
    }

    .divider-section p {
      color: var(--decon-light-concrete);
    }

    /* ============================================
       SHATTERED GRID
       ============================================ */
    .shattered-grid {
      display: grid;
      grid-template-columns: repeat(12, 1fr);
      gap: 0;
      padding: 4rem 2.5rem;
      position: relative;
    }

    .shattered-grid .grid-item {
      padding: 2rem;
      position: relative;
    }

    .shattered-grid .item-a {
      grid-column: 1 / 7;
      transform: rotate(-1.5deg);
      z-index: 3;
      background-color: var(--decon-white);
      border: 2px solid var(--decon-concrete);
      margin-right: -2rem;
    }

    .shattered-grid .item-b {
      grid-column: 5 / 13;
      transform: rotate(1deg) translateY(2rem);
      z-index: 2;
      background-color: var(--decon-dark);
      color: var(--decon-white);
      margin-left: -1rem;
    }

    .shattered-grid .item-c {
      grid-column: 2 / 8;
      transform: rotate(0.5deg) translateY(-1.5rem);
      z-index: 4;
      background-color: var(--decon-red);
      color: var(--decon-white);
      clip-path: polygon(0 3%, 100% 0, 97% 100%, 3% 97%);
    }

    .shattered-grid .item-d {
      grid-column: 7 / 13;
      transform: rotate(-1deg) translateY(1rem);
      z-index: 2;
      background-color: var(--decon-surface);
      border: 2px solid var(--decon-concrete);
    }

    .shattered-grid .grid-item h3 {
      font-size: 1.4rem;
      margin-bottom: 0.75rem;
    }

    .shattered-grid .grid-item p {
      font-size: 0.9rem;
      line-height: 1.6;
    }

    .shattered-grid .grid-item .tag {
      display: inline-block;
      font-family: 'Space Mono', monospace;
      font-size: 0.6rem;
      text-transform: uppercase;
      letter-spacing: 0.12em;
      border: 1px solid currentColor;
      padding: 0.15rem 0.5rem;
      margin-top: 0.75rem;
      margin-right: 0.25rem;
      opacity: 0.7;
    }

    /* Construction line */
    .shattered-grid::before {
      content: '';
      position: absolute;
      top: 1rem;
      left: 50%;
      width: 2px;
      height: calc(100% - 2rem);
      background: var(--decon-steel);
      transform: rotate(4deg);
      opacity: 0.3;
      z-index: 0;
    }

    /* ============================================
       TILTED PANEL
       ============================================ */
    .tilted-panel {
      position: relative;
      padding: 3rem;
      margin: 3rem auto;
      max-width: 700px;
      background-color: var(--decon-white);
      transform: rotate(-1deg);
    }

    .tilted-panel::before {
      content: '';
      position: absolute;
      top: 8px;
      left: -8px;
      right: 8px;
      bottom: -8px;
      border: 2px solid var(--decon-black);
      transform: rotate(0.5deg);
      z-index: -1;
    }

    .tilted-panel::after {
      content: '';
      position: absolute;
      top: -6px;
      right: -6px;
      width: 24px;
      height: 24px;
      background-color: var(--decon-red);
      clip-path: polygon(0 0, 100% 0, 100% 100%);
    }

    .tilted-panel h3 {
      font-size: 1.6rem;
      margin-bottom: 1rem;
    }

    /* ============================================
       FRACTURED CARDS
       ============================================ */
    .card-row {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
      gap: 2.5rem;
      padding: 2rem 0;
    }

    .frac-card {
      position: relative;
      background-color: var(--decon-white);
      border: 2px solid var(--decon-concrete);
      padding: 2rem;
      transform: rotate(calc(var(--rot, 0) * 1deg));
      clip-path: polygon(0 0, 100% 2%, 98% 100%, 2% 97%);
      transition: transform 0.25s ease, box-shadow 0.25s ease;
    }

    .frac-card:nth-child(1) { --rot: -1.5; }
    .frac-card:nth-child(2) { --rot: 0.8; }
    .frac-card:nth-child(3) { --rot: -0.5; }

    .frac-card::before {
      content: '';
      position: absolute;
      top: -4px;
      left: -4px;
      right: -4px;
      bottom: -4px;
      background-color: var(--decon-red);
      z-index: -1;
      clip-path: polygon(1% 1%, 100% 0, 98% 100%, 0 99%);
    }

    .frac-card:hover {
      transform: rotate(0deg) scale(1.02);
      box-shadow: -6px 6px 0 var(--decon-black);
    }

    .frac-card h3 {
      font-size: 1.3rem;
      margin-bottom: 0.75rem;
      border-bottom: 2px solid var(--decon-red);
      padding-bottom: 0.5rem;
    }

    .frac-card p {
      font-size: 0.9rem;
      line-height: 1.6;
      color: var(--decon-concrete);
      margin-bottom: 0;
    }

    .frac-card .card-number {
      font-family: 'Bebas Neue', sans-serif;
      font-size: 4rem;
      color: var(--decon-surface);
      position: absolute;
      top: -0.1em;
      right: 0.3em;
      line-height: 1;
      z-index: -1;
    }

    /* ============================================
       DATA TABLE
       ============================================ */
    .data-table {
      width: 100%;
      border-collapse: collapse;
      font-size: 0.85rem;
      margin-top: 2rem;
      transform: rotate(-0.3deg);
    }

    .data-table th,
    .data-table td {
      border: 2px solid var(--decon-black);
      padding: 0.7rem 1rem;
      text-align: left;
    }

    .data-table th {
      background-color: var(--decon-black);
      color: var(--decon-white);
      font-family: 'Space Mono', monospace;
      font-size: 0.7rem;
      text-transform: uppercase;
      letter-spacing: 0.12em;
    }

    .data-table tr:nth-child(even) td {
      background-color: var(--decon-surface);
    }

    .data-table tr:hover td {
      background-color: var(--decon-yellow);
      color: var(--decon-black);
    }

    /* ============================================
       FOOTER
       ============================================ */
    .footer {
      padding: 3rem 2.5rem;
      background-color: var(--decon-black);
      color: var(--decon-aggregate);
      position: relative;
    }

    .footer::before {
      content: '';
      position: absolute;
      top: 0;
      left: 0;
      width: 100%;
      height: 4px;
      background: linear-gradient(90deg, var(--decon-red) 0%, var(--decon-red) 33%, var(--decon-yellow) 33%, var(--decon-yellow) 66%, var(--decon-blue) 66%);
    }

    .footer .footer-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
      gap: 2rem;
    }

    .footer h4 {
      font-size: 1rem;
      letter-spacing: 0.1em;
      color: var(--decon-white);
      margin-bottom: 0.75rem;
    }

    .footer p, .footer a {
      font-size: 0.8rem;
      line-height: 1.7;
      color: var(--decon-aggregate);
    }

    .footer a {
      border-bottom: 1px solid var(--decon-concrete);
    }

    .footer a:hover {
      color: var(--decon-red);
      border-bottom-color: var(--decon-red);
    }

    .footer ul {
      list-style: none;
    }

    .footer li {
      padding: 0.2rem 0;
    }

    .footer .footer-bottom {
      margin-top: 2rem;
      padding-top: 1.5rem;
      border-top: 1px solid var(--decon-concrete);
      font-family: 'Space Mono', monospace;
      font-size: 0.7rem;
      letter-spacing: 0.08em;
      text-transform: uppercase;
      color: var(--decon-concrete);
    }

    /* ============================================
       RESPONSIVE
       ============================================ */
    @media (max-width: 768px) {
      .hero {
        min-height: 80vh;
        padding: 2.5rem;
      }

      .hero h1 {
        font-size: clamp(3rem, 14vw, 6rem);
      }

      .hero h1 .fragment-shift {
        transform: translateX(4vw) rotate(1deg);
      }

      .nav {
        flex-direction: column;
        gap: 0.75rem;
        padding: 1rem 1.5rem;
      }

      .nav ul {
        flex-wrap: wrap;
        justify-content: center;
      }

      .section {
        padding: 3rem 1.5rem;
      }

      .shattered-grid {
        display: flex;
        flex-direction: column;
        gap: 1rem;
        padding: 2rem 1.5rem;
      }

      .shattered-grid .grid-item {
        transform: rotate(calc(var(--rot, 0) * 0.5deg)) !important;
        margin: 0 !important;
        z-index: auto !important;
      }

      .shattered-grid .item-a { --rot: -1; }
      .shattered-grid .item-b { --rot: 0.8; }
      .shattered-grid .item-c { --rot: -0.5; }
      .shattered-grid .item-d { --rot: 0.6; }

      .divider-section {
        clip-path: polygon(0 3%, 100% 0, 100% 97%, 0 100%);
        padding: 5rem 1.5rem;
      }

      .tilted-panel {
        margin: 2rem 1rem;
        padding: 2rem;
      }
    }

    @media (max-width: 480px) {
      .hero h1 {
        font-size: clamp(2.5rem, 16vw, 4rem);
      }

      .nav a {
        font-size: 0.7rem;
        padding: 0.3rem 0.6rem;
      }

      .frac-card {
        transform: rotate(0deg);
        clip-path: none;
      }

      .frac-card::before {
        clip-path: none;
      }
    }
  </style>
</head>
<body>

  <!-- ======== NAVIGATION ======== -->
  <nav class="nav" role="navigation" aria-label="Main navigation">
    <a href="#" class="logo">DECON/STRUCT</a>
    <ul>
      <li><a href="#manifesto">Manifesto</a></li>
      <li><a href="#projects">Projects</a></li>
      <li><a href="#method">Method</a></li>
      <li><a href="#data">Data</a></li>
      <li><a href="#contact">Contact</a></li>
    </ul>
  </nav>

  <!-- ======== HERO ======== -->
  <section class="hero" id="manifesto">
    <span class="mono" style="margin-bottom: 0.5rem;">Est. 1988 / MoMA New York</span>
    <h1>
      <span class="fragment">Decon</span>
      <span class="fragment-shift">Structivism</span>
    </h1>
    <p class="subtitle">
      Structure exists to be questioned. Every grid is an ideology.
      Every alignment is a political act. We do not build to stand --
      we build to expose the instability that was always already there.
    </p>
    <span class="hero-meta">Gehry / Hadid / Libeskind / Eisenman / Koolhaas / Tschumi / Coop Himmelb(l)au</span>
    <div class="btn-row">
      <a href="#projects" class="btn">Explore Fragments</a>
      <a href="#method" class="btn btn--outline">Read Method</a>
    </div>
  </section>

  <!-- ======== SHATTERED GRID SECTION ======== -->
  <section class="section" id="projects">
    <h2>Projects</h2>
    <span class="section-subtitle">// Selected works in fragmented space</span>
    <p>
      Each project is a collision of intention and disruption. The grid is present
      but violated. Elements overlap, rotate, and refuse the comfort of alignment.
    </p>

    <div class="shattered-grid" style="margin-top: 2rem;">
      <div class="grid-item item-a">
        <h3>Bilbao Protocol</h3>
        <p>A titanium-clad interface system where every surface curves away from expectation. Navigation paths fold and refold, demanding the user construct their own spatial logic.</p>
        <span class="tag">Interface</span>
        <span class="tag">Non-linear</span>
      </div>
      <div class="grid-item item-b">
        <h3>Void Index</h3>
        <p>A data visualization that maps absence rather than presence. Empty cells, missing records, and null values become the primary visual elements, exposing the gaps that structured data conceals.</p>
        <span class="tag">Data</span>
        <span class="tag">Negative Space</span>
      </div>
      <div class="grid-item item-c">
        <h3>Fracture Line</h3>
        <p>A typographic experiment where letterforms are split along structural fault lines, each half displaced and rotated independently. Legibility survives through pattern recognition.</p>
        <span class="tag">Typography</span>
        <span class="tag">Fragmentation</span>
      </div>
      <div class="grid-item item-d">
        <h3>Angular Void</h3>
        <p>An architectural rendering engine that generates structures by subtracting volumes from solid blocks. Every form is defined by what has been removed, not what remains.</p>
        <span class="tag">Generative</span>
        <span class="tag">Subtraction</span>
      </div>
    </div>
  </section>

  <!-- ======== ANGULAR DIVIDER ======== -->
  <section class="divider-section" id="method">
    <h2>Method</h2>
    <span class="section-subtitle" style="color: var(--decon-aggregate);">// On the practice of structural interrogation</span>
    <p>
      Deconstruction is not destruction. It is the careful disassembly of assumptions --
      revealing how structures maintain the appearance of stability while concealing
      the contradictions that constitute them. In design, this means making the grid
      visible, breaking it deliberately, and letting the viewer see both the rule
      and its violation simultaneously.
    </p>
  </section>

  <!-- ======== FRACTURED CARDS ======== -->
  <section class="section">
    <h2>Principles</h2>
    <span class="section-subtitle">// Core axioms of deconstructivist practice</span>

    <div class="card-row">
      <div class="frac-card">
        <span class="card-number">01</span>
        <h3>Tension Over Resolution</h3>
        <p>Compositions sustain visual conflict rather than resolving into comfortable equilibrium. Opposing forces remain in permanent dialectic -- no element settles.</p>
      </div>
      <div class="frac-card">
        <span class="card-number">02</span>
        <h3>Form Follows Fracture</h3>
        <p>Rather than expressing unified purpose, the design reveals the contradictions and multiplicity of meaning within every structure it inhabits.</p>
      </div>
      <div class="frac-card">
        <span class="card-number">03</span>
        <h3>Collision Is Composition</h3>
        <p>Overlapping, intersecting, and conflicting elements are the primary compositional strategy. Meaning emerges from the friction between parts, not their harmony.</p>
      </div>
    </div>
  </section>

  <!-- ======== TILTED PANEL ======== -->
  <section class="section">
    <div class="tilted-panel">
      <h3>The Viewer Must Work</h3>
      <p>
        Deconstructivist design demands active interpretation. Legibility and
        navigability are deliberately complicated to transform passive consumption
        into engaged reading. Nothing is given freely -- every element of understanding
        must be constructed by the viewer from the fragments provided.
      </p>
    </div>
  </section>

  <!-- ======== DATA TABLE ======== -->
  <section class="section" id="data">
    <h2>Reference</h2>
    <span class="section-subtitle">// Key works and their architects</span>
    <p>The canon of deconstructivist architecture and the structures that defined the movement.</p>

    <table class="data-table">
      <thead>
        <tr>
          <th>Structure</th>
          <th>Architect</th>
          <th>Year</th>
          <th>Location</th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <td>Guggenheim Museum Bilbao</td>
          <td>Frank Gehry</td>
          <td>1997</td>
          <td>Bilbao, Spain</td>
        </tr>
        <tr>
          <td>Jewish Museum Berlin</td>
          <td>Daniel Libeskind</td>
          <td>2001</td>
          <td>Berlin, Germany</td>
        </tr>
        <tr>
          <td>Vitra Fire Station</td>
          <td>Zaha Hadid</td>
          <td>1993</td>
          <td>Weil am Rhein, Germany</td>
        </tr>
        <tr>
          <td>Seattle Central Library</td>
          <td>Rem Koolhaas / OMA</td>
          <td>2004</td>
          <td>Seattle, USA</td>
        </tr>
        <tr>
          <td>Parc de la Villette</td>
          <td>Bernard Tschumi</td>
          <td>1998</td>
          <td>Paris, France</td>
        </tr>
        <tr>
          <td>House VI</td>
          <td>Peter Eisenman</td>
          <td>1975</td>
          <td>Cornwall, USA</td>
        </tr>
        <tr>
          <td>UFA Cinema Center</td>
          <td>Coop Himmelb(l)au</td>
          <td>1998</td>
          <td>Dresden, Germany</td>
        </tr>
      </tbody>
    </table>
  </section>

  <!-- ======== CONTACT / CTA ======== -->
  <section class="section" id="contact" style="background-color: var(--decon-surface);">
    <h2>Contact</h2>
    <span class="section-subtitle">// Initiate structural dialogue</span>
    <p>
      Inquiries regarding collaboration, commissions, and structural interrogations.
    </p>
    <div style="margin-top: 1.5rem; display: flex; flex-wrap: wrap; gap: 1rem;">
      <a href="mailto:studio@example.com" class="btn" style="background-color: var(--decon-black); color: var(--decon-white); clip-path: polygon(6% 0, 100% 0, 94% 100%, 0 100%);">Send Inquiry</a>
    </div>
  </section>

  <!-- ======== FOOTER ======== -->
  <footer class="footer">
    <div class="footer-grid">
      <div>
        <h4>DECON/STRUCT</h4>
        <p>A design system built on the principle that every structure contains the seeds of its own undoing. Nothing is stable. Everything is material.</p>
      </div>
      <div>
        <h4>Navigation</h4>
        <ul>
          <li><a href="#manifesto">Manifesto</a></li>
          <li><a href="#projects">Projects</a></li>
          <li><a href="#method">Method</a></li>
          <li><a href="#data">Reference</a></li>
          <li><a href="#contact">Contact</a></li>
        </ul>
      </div>
      <div>
        <h4>Lineage</h4>
        <ul>
          <li><a href="#">Constructivism</a></li>
          <li><a href="#">Derrida / Deconstruction</a></li>
          <li><a href="#">MoMA 1988 Exhibition</a></li>
          <li><a href="#">David Carson / Ray Gun</a></li>
          <li><a href="#">Cranbrook Academy</a></li>
        </ul>
      </div>
    </div>
    <div class="footer-bottom">
      Structure is a hypothesis, not a conclusion. // Built with HTML + CSS. No frameworks. No stability.
    </div>
  </footer>

</body>
</html>
```
