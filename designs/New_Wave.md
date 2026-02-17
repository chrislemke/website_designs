# New Wave Design Reference

New Wave is the visual aesthetic that emerged from the late-1970s music movement of the same name, a pop-oriented evolution of Punk. It is characterized by **geometric precision, bright fluorescent colors, skewed typography, industrial textures (halftones, xerox grain), and a "retro-futuristic" collision of 1950s Atomic Age optimism with 1980s irony**. Where punk was raw and aggressive, New Wave replaced that aggression with a philosophy of **"synthetic modernity"** -- a celebration of the artificial, the plastic, and the deliberately constructed. Visually, New Wave was pioneered through record sleeve design and concert posters by figures like Barney Bubbles, Malcolm Garrett, and Peter Saville, who deconstructed the rigid rules of Modernist graphic design. The aesthetic defined the early MTV era: angular, colorful, campy, and self-consciously artificial.

---

## Visual Characteristics

### Core Motifs and Patterns

- **Dysfunctional grids** -- the defining technique: take the clean, rigid grid systems of Swiss International Typographic Style and deliberately break them with skewed angles, misalignment, overlapping elements, and compositions that defy rational logic
- **Geometric shapes** -- triangles, circles, squares, and grids floating in space or arranged in erratic patterns that mirror the "herky-jerky" rhythms of the music
- **Halftone dot patterns** -- coarse halftone screens from photocopied and printed media, used as texture and pattern elements
- **Xerox grain and photocopy artifacts** -- high-contrast textures from low-fidelity reproduction tools; toner bleed, registration errors, and crushed midtones
- **Chartpak / adhesive film textures** -- moire patterns, stipple fields, and optical-illusion surfaces derived from paste-up graphic design materials
- **Angular and diagonal compositions** -- nothing sits perfectly horizontal or vertical; elements tilt, skew, and collide at sharp angles
- **Layered, deconstructed typography** -- text treated as graphic element: overlapping, rotated, scaled, and fragmented across the composition
- **Retro-futuristic imagery** -- 1950s atomic-age motifs (rockets, atoms, ray guns, suburban kitsch) recontextualized through 1980s cynicism and irony
- **Synthetic and plastic textures** -- glossy, manufactured surfaces that celebrate artificiality over organic warmth
- **High-contrast processing** -- stark tonal ranges pushed to extremes; deep blacks against fluorescent highlights
- **Neon glow effects** -- fluorescent color halos and lighting that evoke nightclub and MTV-era video aesthetics
- **Fragmented and deconstructed layouts** -- compositions that feel deliberately "broken" or reassembled, as if modernist design rules were put through a shredder and taped back together wrong

### Design Principles

- **Deconstruct the grid** -- start with a modernist grid, then deliberately violate it; the tension between order and disorder is the entire point
- **Celebrate artificiality** -- nothing should look natural, organic, or handmade; embrace plastic, synthetic, and manufactured qualities
- **Angular energy** -- compositions should feel jittery, nervous, and angular; no soft curves or relaxed organic flow
- **High contrast, high saturation** -- colors are fluorescent and aggressive; tonal range is pushed to stark extremes
- **Ironic retro-futurism** -- reference the past (especially 1950s Atomic Age) but subvert it with modern cynicism and knowing humor
- **Typography as architecture** -- text is not just read, it is seen; treat letterforms as structural and decorative elements
- **Mix high and low culture** -- synthesize Bauhaus, Constructivism, and Pop Art influences into a deliberately commercial, accessible package
- **Campy pop sensibility** -- the tone is quirky, witty, and self-aware; never take yourself too seriously
- **Modernity over tradition** -- prefer synthesizers over guitars, neon over natural light, plastic over wood
- **The visible process** -- let production artifacts (halftone dots, registration marks, crop marks) remain visible as part of the design language

---

## Color Palette

### Primary Scheme

New Wave favors a specific palette of **"tertiary" tones (purples, oranges, greens) alongside aggressive hot pink and electric yellow**. Pink was used as a deliberate reassignment of the color, stripping it of traditional gendered associations and applying it as a signifier of modern artificiality. The palette sits against either stark white or deep black backgrounds, often with neon glow effects.

| Role | Color | Hex (suggested) |
|------|-------|-----------------|
| **Hot Pink / Magenta** | Neon pink, electric magenta -- the signature New Wave color | `#FF1493`, `#F72585` |
| **Electric Yellow** | Bright fluorescent yellow, lemon | `#FFE600`, `#F5E616` |
| **Cyan / Electric Blue** | Bright cyan, new wave blue | `#00E5FF`, `#00BCD4` |
| **Tertiary Purple** | Vivid violet, electric purple | `#9B30FF`, `#7B2FBE` |
| **Tertiary Orange** | Neon tangerine, fluorescent orange | `#FF6D00`, `#FF8C00` |
| **Tertiary Green** | Electric green, synthetic lime | `#39FF14`, `#76FF03` |
| **Black** | Deep black for backgrounds, outlines, and contrast | `#0A0A0A`, `#111111` |
| **White** | Stark white for clean modernist backgrounds | `#FFFFFF`, `#F5F5F5` |
| **Cool Gray** | Metallic, synthetic gray for secondary surfaces | `#B0BEC5`, `#78909C` |
| **Charcoal** | Dark surface alternative to pure black | `#1A1A2E`, `#16213E` |
| **Neon Pink Glow** | Lighter pink for glow effects and halos | `#FF69B4`, `#FBB4D4` |
| **Halftone Gray** | Mid-gray for halftone dot patterns and textures | `#9E9E9E`, `#BDBDBD` |

### Suggested CSS Custom Properties

```css
:root {
  /* Core New Wave palette */
  --nw-pink: #ff1493;
  --nw-yellow: #ffe600;
  --nw-cyan: #00e5ff;
  --nw-purple: #9b30ff;
  --nw-orange: #ff6d00;
  --nw-green: #39ff14;

  /* Neutrals */
  --nw-black: #0a0a0a;
  --nw-white: #ffffff;
  --nw-cool-gray: #b0bec5;
  --nw-charcoal: #1a1a2e;
  --nw-halftone-gray: #9e9e9e;

  /* Glow variants */
  --nw-pink-glow: #ff69b4;
  --nw-cyan-glow: #80deea;
  --nw-yellow-glow: #fff59d;

  /* Functional mappings */
  --nw-bg-light: var(--nw-white);
  --nw-bg-dark: var(--nw-black);
  --nw-bg-charcoal: var(--nw-charcoal);
  --nw-text-primary: var(--nw-black);
  --nw-text-inverse: var(--nw-white);
  --nw-accent: var(--nw-pink);
  --nw-accent-secondary: var(--nw-cyan);
  --nw-border: var(--nw-black);
  --nw-border-width: 2px;
}
```

### Color Guidelines

- **Tertiary tones dominate** -- unlike primary-color movements (De Stijl, Bauhaus), New Wave leans toward purples, oranges, and greens alongside pink and yellow
- **Hot pink is the signature color** -- use it liberally as the primary accent; it signals modern artificiality and gender-role subversion
- **Fluorescent intensity** -- colors should look like they are lit from within; if a color could exist on a neon sign, it belongs here
- **High contrast pairings** -- hot pink on black, cyan on charcoal, electric yellow on deep purple; never pair similar tones softly
- **Black backgrounds for drama** -- dark backgrounds make fluorescent colors pop and evoke the nightclub/MTV aesthetic
- **White backgrounds for modernist tension** -- clean white creates the Swiss-style grid that the aesthetic then proceeds to break
- **No earth tones, no pastels, no muted warmth** -- everything is synthetic, electric, and manufactured
- **Neon glow effects** -- use `text-shadow` or `box-shadow` with color-matched glows to create the fluorescent tube lighting feel

---

## Typography

### Typeface Characteristics

New Wave typography is defined by the deconstruction of Modernist type conventions:

- **Mixed typeface compositions** -- clean sans-serifs combined with decorative scripts, stenciled lettering, or geometric display faces within a single composition
- **Skewed and rotated text** -- letterforms tilted at sharp angles, sometimes each word or line at a different rotation
- **Geometric sans-serifs as base** -- the underlying modernist foundation uses clean, precise geometric type (Futura, Avant Garde)
- **Contrast with decorative faces** -- the geometric base is disrupted by inserting ornamental, script, or experimental display type
- **Extreme scale variation** -- dramatic size differences between elements; a single word might be 10x larger than the surrounding text
- **Text as graphic element** -- words and letters used architecturally: stacked vertically, arranged in circles, fragmented across the page
- **Visible baseline disruption** -- text deliberately pushed off its baseline, creating visual "jitter" that mirrors the music's rhythm
- **Condensed and extended mixing** -- ultra-condensed type next to wide, expanded letterforms within the same layout
- **All-caps geometric headers** -- clean, precise, authoritative headings in the modernist tradition, before subverting them elsewhere

### Recommended Web Fonts (Google Fonts)

| Font | Style | Usage |
|------|-------|-------|
| **Orbitron** | Geometric, futuristic, angular | Display headings, retro-futuristic hero text, technological feel |
| **Audiowide** | Wide, electronic, display | Section headers, bold statements, synthetic personality |
| **Rajdhani** | Semi-condensed geometric | Subheadings, UI elements, angular modernist feel |
| **Syncopate** | Wide-set, geometric, stark | Display text, spaced-out modern headings |
| **Space Grotesk** | Modern geometric grotesk | Body text, clean modernist base to subvert |
| **Inter** | Clean geometric sans | Body text, the "Swiss" foundation that gets broken |
| **Gruppo** | Thin geometric display | Elegant display text, modernist thin-line aesthetic |
| **Michroma** | Wide, geometric, industrial | Bold headings, technological / futuristic treatments |
| **Faster One** | Speed-styled, angular display | Aggressive accent text, dynamic energy |
| **Staatliches** | Condensed, industrial block | All-caps headings, poster-style treatments |
| **Monoton** | Inline display, retro | Decorative headings, neon-sign lettering effect |

### Typography CSS Example

```css
/* Import New Wave-appropriate Google Fonts */
@import url('https://fonts.googleapis.com/css2?family=Orbitron:wght@400;500;700;900&family=Space+Grotesk:wght@300;400;500;700&family=Rajdhani:wght@300;400;500;600;700&family=Syncopate:wght@400;700&family=Monoton&display=swap');

/* Hero / Display -- angular futuristic */
h1, .nw-display {
  font-family: 'Orbitron', 'Syncopate', sans-serif;
  font-weight: 900;
  font-size: clamp(2.5rem, 7vw, 5.5rem);
  line-height: 1.0;
  letter-spacing: 0.04em;
  text-transform: uppercase;
  color: var(--nw-accent);
}

/* Section headings -- condensed modernist */
h2 {
  font-family: 'Rajdhani', 'Space Grotesk', sans-serif;
  font-weight: 700;
  font-size: clamp(1.5rem, 4vw, 2.8rem);
  letter-spacing: 0.06em;
  text-transform: uppercase;
  line-height: 1.15;
  color: var(--nw-text-primary);
}

/* Subheadings -- geometric with angular personality */
h3 {
  font-family: 'Space Grotesk', 'Rajdhani', sans-serif;
  font-weight: 500;
  font-size: 1.3rem;
  letter-spacing: 0.03em;
  text-transform: uppercase;
  color: var(--nw-accent-secondary);
}

/* Body text -- clean geometric base */
body {
  font-family: 'Space Grotesk', 'Inter', sans-serif;
  font-weight: 300;
  font-size: 1rem;
  line-height: 1.7;
  color: var(--nw-text-primary);
}

/* Neon glow text treatment */
.nw-glow {
  color: var(--nw-pink);
  text-shadow:
    0 0 7px var(--nw-pink-glow),
    0 0 20px rgba(255, 20, 147, 0.4),
    0 0 40px rgba(255, 20, 147, 0.2);
}

/* Skewed text -- the dysfunctional grid in action */
.nw-skew {
  display: inline-block;
  transform: skewX(-8deg);
}

.nw-rotated {
  display: inline-block;
  transform: rotate(-5deg);
  transform-origin: bottom left;
}

/* Inline display face -- for decorative accent words */
.nw-display-accent {
  font-family: 'Monoton', 'Orbitron', sans-serif;
  font-weight: 400;
  letter-spacing: 0.08em;
  color: var(--nw-cyan);
}
```

---

## Layout Principles

### Grid and Structure

- **Start with a grid, then break it** -- the composition should feel like a Swiss modernist layout that has been deliberately disrupted; the underlying order should be visible beneath the chaos
- **Skewed and rotated element placement** -- panels, text blocks, and images tilt at 3-12 degree angles, creating angular tension
- **Diagonal compositions** -- content flows along diagonal axes rather than purely horizontal/vertical; use CSS `transform: skew()` and `rotate()`
- **Layered, overlapping elements** -- shapes, text blocks, and images overlap in collage-like arrangements, but with more precision than punk collage
- **Strong horizontal and vertical lines** -- visible rules, borders, and dividers that reference the modernist grid before being violated by skewed content
- **Asymmetric balance** -- visual weight is distributed unevenly but deliberately; compositions feel dynamic rather than chaotic
- **Full-bleed color blocks** -- large areas of solid fluorescent color as section backgrounds
- **Negative space as tension** -- areas of stark white or black emptiness create dramatic contrast against dense, colorful zones
- **Angular section dividers** -- diagonal lines, chevrons, or triangular cuts between sections rather than horizontal rules
- **Mixed column widths** -- grid columns that vary in proportion, referencing constructivist layouts

### Section Organization

- **Hero**: Oversized geometric display text in a fluorescent accent color, set against black or white. Text may be skewed or rotated. Geometric shapes (triangles, circles, grid lines) float as decorative elements. Halftone texture overlay at low opacity.
- **Content blocks**: Rectangular panels with strong borders, tilted at slight angles. Different background colors (black, pink, cyan) create rhythmic alternation.
- **Feature sections**: Angular layouts with diagonal dividers. Content arranged along diagonal axes with geometric shape accents.
- **Dividers**: Diagonal lines, chevron patterns, or triangular clip-paths rather than straight horizontal rules. Also: thin horizontal rules referencing the modernist grid.
- **Backgrounds**: Halftone dot patterns, moire textures, or gradient overlays at low opacity. Solid neon color blocks for emphasis.
- **CTA sections**: Stark black backgrounds with fluorescent text (pink, cyan, or yellow) and neon glow effects. Angular, geometric button styles.

### Responsive Approach

- Maintain angular, skewed elements on mobile but reduce rotation angles for readability
- Typography scales with `clamp()` -- headings remain bold and geometric at all sizes
- Simplify overlapping layers on small screens while keeping the fluorescent color palette
- Preserve halftone and texture overlays but reduce opacity on mobile for performance
- Geometric decorative shapes scale proportionally; do not remove them

---

## CSS/Design Techniques

### Halftone Dot Texture Overlay

```css
/* Coarse halftone dot pattern -- the signature New Wave print texture */
.nw-halftone-bg {
  position: relative;
  background-color: var(--nw-bg-light);
}

.nw-halftone-bg::after {
  content: '';
  position: absolute;
  inset: 0;
  background-image: radial-gradient(circle, var(--nw-black) 1px, transparent 1px);
  background-size: 6px 6px;
  opacity: 0.06;
  pointer-events: none;
  mix-blend-mode: multiply;
}
```

### Moire / Chartpak Texture

```css
/* Moire interference pattern -- adhesive film texture from paste-up design */
.nw-moire-bg {
  position: relative;
  overflow: hidden;
}

.nw-moire-bg::before {
  content: '';
  position: absolute;
  inset: -20%;
  background-image:
    repeating-linear-gradient(
      0deg,
      transparent,
      transparent 2px,
      rgba(0, 0, 0, 0.03) 2px,
      rgba(0, 0, 0, 0.03) 4px
    ),
    repeating-linear-gradient(
      60deg,
      transparent,
      transparent 2px,
      rgba(0, 0, 0, 0.03) 2px,
      rgba(0, 0, 0, 0.03) 4px
    );
  pointer-events: none;
}
```

### Diagonal Section Divider

```css
/* Angular chevron divider between sections */
.nw-diagonal-divider {
  width: 100%;
  height: 60px;
  background: linear-gradient(
    to bottom right,
    var(--nw-pink) 49.5%,
    transparent 50%
  );
  position: relative;
}

/* Alternative: sharp diagonal cut */
.nw-angle-cut {
  clip-path: polygon(0 0, 100% 0, 100% 30%, 0 100%);
  height: 80px;
  background: var(--nw-black);
}

/* Triangle divider */
.nw-triangle-divider {
  width: 100%;
  height: 50px;
  background: url("data:image/svg+xml,%3Csvg width='100' height='50' xmlns='http://www.w3.org/2000/svg'%3E%3Cpolygon points='50,0 100,50 0,50' fill='%23ff1493'/%3E%3C/svg%3E") repeat-x;
  background-size: 100px 50px;
}
```

### Neon Glow Box / Panel

```css
/* Panel with fluorescent neon border glow */
.nw-glow-panel {
  background: var(--nw-bg-dark);
  border: 2px solid var(--nw-pink);
  padding: 2rem;
  position: relative;
  box-shadow:
    0 0 8px rgba(255, 20, 147, 0.4),
    0 0 20px rgba(255, 20, 147, 0.2),
    inset 0 0 8px rgba(255, 20, 147, 0.1);
}

/* Cyan variant */
.nw-glow-panel--cyan {
  border-color: var(--nw-cyan);
  box-shadow:
    0 0 8px rgba(0, 229, 255, 0.4),
    0 0 20px rgba(0, 229, 255, 0.2),
    inset 0 0 8px rgba(0, 229, 255, 0.1);
}

/* Yellow variant */
.nw-glow-panel--yellow {
  border-color: var(--nw-yellow);
  box-shadow:
    0 0 8px rgba(255, 230, 0, 0.4),
    0 0 20px rgba(255, 230, 0, 0.2),
    inset 0 0 8px rgba(255, 230, 0, 0.1);
}
```

### Dysfunctional Grid Layout

```css
/* The core New Wave layout technique: a grid that deliberately breaks itself */
.nw-grid {
  display: grid;
  grid-template-columns: repeat(12, 1fr);
  gap: 2px;
  position: relative;
}

/* Grid items tilt at varying angles */
.nw-grid-item {
  padding: 1.5rem;
  border: var(--nw-border-width) solid var(--nw-border);
  position: relative;
}

.nw-grid-item:nth-child(1) {
  grid-column: 1 / 8;
  transform: rotate(-2deg);
  background: var(--nw-pink);
  color: var(--nw-white);
}

.nw-grid-item:nth-child(2) {
  grid-column: 7 / 13;
  transform: rotate(3deg);
  background: var(--nw-black);
  color: var(--nw-cyan);
  margin-top: -1rem;
}

.nw-grid-item:nth-child(3) {
  grid-column: 2 / 10;
  transform: skewX(-4deg);
  background: var(--nw-yellow);
  color: var(--nw-black);
}

/* Visible grid lines (the modernist structure being broken) */
.nw-grid::before {
  content: '';
  position: absolute;
  inset: 0;
  background-image:
    linear-gradient(rgba(0, 0, 0, 0.05) 1px, transparent 1px),
    linear-gradient(90deg, rgba(0, 0, 0, 0.05) 1px, transparent 1px);
  background-size: calc(100% / 12) 40px;
  pointer-events: none;
  z-index: 0;
}
```

### Geometric Shape Decorations

```css
/* Floating triangle */
.nw-triangle {
  width: 0;
  height: 0;
  border-left: 35px solid transparent;
  border-right: 35px solid transparent;
  border-bottom: 60px solid var(--nw-pink);
  position: absolute;
  transform: rotate(15deg);
}

/* Circle accent */
.nw-circle {
  width: 80px;
  height: 80px;
  border-radius: 50%;
  border: 3px solid var(--nw-cyan);
  background: transparent;
  position: absolute;
}

/* Filled circle */
.nw-circle--filled {
  background: var(--nw-yellow);
  border: none;
}

/* Small grid of dots -- constructivist reference */
.nw-dot-grid {
  width: 120px;
  height: 120px;
  background-image: radial-gradient(circle 3px, var(--nw-pink) 100%, transparent 100%);
  background-size: 15px 15px;
  position: absolute;
  opacity: 0.6;
}

/* Diagonal line accent */
.nw-diagonal-line {
  width: 150px;
  height: 2px;
  background: var(--nw-cyan);
  position: absolute;
  transform: rotate(-35deg);
}

/* Plus / cross mark */
.nw-cross {
  width: 40px;
  height: 40px;
  position: absolute;
}
.nw-cross::before,
.nw-cross::after {
  content: '';
  position: absolute;
  background: var(--nw-yellow);
}
.nw-cross::before {
  width: 100%;
  height: 3px;
  top: 50%;
  transform: translateY(-50%);
}
.nw-cross::after {
  width: 3px;
  height: 100%;
  left: 50%;
  transform: translateX(-50%);
}
```

### New Wave Button

```css
.nw-button {
  display: inline-block;
  padding: 12px 32px;
  font-family: 'Orbitron', 'Rajdhani', sans-serif;
  font-weight: 700;
  font-size: 0.9rem;
  text-transform: uppercase;
  letter-spacing: 0.1em;
  color: var(--nw-white);
  background: var(--nw-pink);
  border: 2px solid var(--nw-pink);
  text-decoration: none;
  cursor: pointer;
  position: relative;
  transform: skewX(-6deg);
  transition: all 0.2s ease;
}

.nw-button:hover {
  background: transparent;
  color: var(--nw-pink);
  box-shadow: 0 0 12px rgba(255, 20, 147, 0.5);
}

/* Dark background variant */
.nw-button--outline {
  background: transparent;
  color: var(--nw-cyan);
  border-color: var(--nw-cyan);
}

.nw-button--outline:hover {
  background: var(--nw-cyan);
  color: var(--nw-black);
  box-shadow: 0 0 12px rgba(0, 229, 255, 0.5);
}
```

### New Wave Card

```css
.nw-card {
  background: var(--nw-bg-dark);
  border: 2px solid var(--nw-cool-gray);
  padding: 2rem;
  position: relative;
  transform: rotate(calc(var(--tilt, 0) * 1deg));
  transition: transform 0.2s ease, box-shadow 0.2s ease;
}

.nw-card:hover {
  border-color: var(--nw-pink);
  box-shadow: 0 0 15px rgba(255, 20, 147, 0.3);
  transform: rotate(0deg);
}

/* Accent corner -- geometric triangle */
.nw-card::before {
  content: '';
  position: absolute;
  top: 0;
  right: 0;
  width: 0;
  height: 0;
  border-top: 30px solid var(--nw-pink);
  border-left: 30px solid transparent;
}

.nw-card h3 {
  color: var(--nw-cyan);
  margin-bottom: 0.75rem;
}

.nw-card p {
  color: var(--nw-cool-gray);
  font-weight: 300;
}
```

### Hero Section

```css
.nw-hero {
  position: relative;
  min-height: 90vh;
  display: flex;
  align-items: center;
  padding: 80px 40px;
  overflow: hidden;
  background: var(--nw-bg-dark);
  color: var(--nw-white);
}

.nw-hero__content {
  max-width: 700px;
  position: relative;
  z-index: 2;
}

.nw-hero h1 {
  font-family: 'Orbitron', sans-serif;
  font-size: clamp(3rem, 8vw, 6rem);
  font-weight: 900;
  line-height: 1.0;
  text-transform: uppercase;
  letter-spacing: 0.04em;
  margin-bottom: 1.5rem;
  color: var(--nw-pink);
  text-shadow:
    0 0 10px rgba(255, 20, 147, 0.5),
    0 0 30px rgba(255, 20, 147, 0.2);
}

.nw-hero h1 .accent-word {
  color: var(--nw-cyan);
  display: inline-block;
  transform: skewX(-8deg);
  text-shadow:
    0 0 10px rgba(0, 229, 255, 0.5),
    0 0 30px rgba(0, 229, 255, 0.2);
}

.nw-hero p {
  font-family: 'Space Grotesk', sans-serif;
  font-weight: 300;
  font-size: 1.15rem;
  line-height: 1.7;
  color: var(--nw-cool-gray);
  max-width: 500px;
  margin-bottom: 2.5rem;
}

/* Background grid lines -- the modernist structure */
.nw-hero__grid {
  position: absolute;
  inset: 0;
  background-image:
    linear-gradient(rgba(255, 255, 255, 0.03) 1px, transparent 1px),
    linear-gradient(90deg, rgba(255, 255, 255, 0.03) 1px, transparent 1px);
  background-size: 80px 80px;
  z-index: 0;
  pointer-events: none;
}

/* Decorative geometric shapes container */
.nw-hero__shapes {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  z-index: 1;
  pointer-events: none;
}
```

### Navigation Bar

```css
.nw-nav {
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 16px 40px;
  background: var(--nw-black);
  border-bottom: 2px solid var(--nw-pink);
}

.nw-nav__logo {
  font-family: 'Orbitron', sans-serif;
  font-weight: 700;
  font-size: 1.3rem;
  color: var(--nw-pink);
  text-decoration: none;
  text-transform: uppercase;
  letter-spacing: 0.08em;
}

.nw-nav__links {
  display: flex;
  gap: 28px;
  list-style: none;
}

.nw-nav__links a {
  font-family: 'Rajdhani', 'Space Grotesk', sans-serif;
  font-weight: 500;
  font-size: 0.9rem;
  color: var(--nw-cool-gray);
  text-decoration: none;
  text-transform: uppercase;
  letter-spacing: 0.06em;
  padding: 4px 0;
  border-bottom: 2px solid transparent;
  transition: color 0.2s ease, border-color 0.2s ease;
}

.nw-nav__links a:hover {
  color: var(--nw-cyan);
  border-bottom-color: var(--nw-cyan);
}
```

### Section Color Blocks

```css
.nw-section {
  padding: 80px 40px;
  position: relative;
  overflow: hidden;
}

.nw-section--dark {
  background: var(--nw-bg-dark);
  color: var(--nw-white);
}

.nw-section--light {
  background: var(--nw-bg-light);
  color: var(--nw-text-primary);
}

.nw-section--charcoal {
  background: var(--nw-charcoal);
  color: var(--nw-white);
}

.nw-section--pink {
  background: var(--nw-pink);
  color: var(--nw-white);
}

.nw-section--cyan {
  background: var(--nw-cyan);
  color: var(--nw-black);
}

.nw-section--yellow {
  background: var(--nw-yellow);
  color: var(--nw-black);
}
```

### Scanline / CRT Overlay

```css
/* CRT scanline effect -- evokes early MTV and video monitors */
.nw-scanlines::after {
  content: '';
  position: absolute;
  inset: 0;
  background: repeating-linear-gradient(
    0deg,
    transparent,
    transparent 2px,
    rgba(0, 0, 0, 0.05) 2px,
    rgba(0, 0, 0, 0.05) 4px
  );
  pointer-events: none;
  z-index: 10;
}
```

### Xerox / High-Contrast Image Treatment

```css
/* High-contrast processed image -- photocopy aesthetic */
.nw-xerox-img {
  filter: contrast(1.8) grayscale(0.8) brightness(1.1);
  mix-blend-mode: multiply;
}

/* Neon tinted image -- pink or cyan wash */
.nw-tint-pink {
  filter: grayscale(1) contrast(1.4) brightness(1.2);
  mix-blend-mode: multiply;
  position: relative;
}

.nw-tint-pink::after {
  content: '';
  position: absolute;
  inset: 0;
  background: rgba(255, 20, 147, 0.25);
  mix-blend-mode: color;
  pointer-events: none;
}
```

### Angular Stripe Pattern

```css
/* Diagonal stripe background -- angular energy */
.nw-stripe-bg {
  background: repeating-linear-gradient(
    -45deg,
    var(--nw-black),
    var(--nw-black) 10px,
    var(--nw-charcoal) 10px,
    var(--nw-charcoal) 20px
  );
}

/* Thinner, more refined stripes */
.nw-stripe-fine {
  background: repeating-linear-gradient(
    -45deg,
    transparent,
    transparent 4px,
    rgba(255, 20, 147, 0.08) 4px,
    rgba(255, 20, 147, 0.08) 8px
  );
}
```

---

## Signature Patterns Reference

### The Dysfunctional Grid

The defining visual technique of New Wave graphic design. Start with the clean, mathematical grid of Swiss International Typographic Style (the standard of 1960s-70s corporate design), then deliberately misalign, skew, overlap, and fragment elements within it. The underlying grid structure should remain visible as a ghost -- through faint guide lines, consistent column widths, or aligned baselines -- while the content violates every rule the grid establishes. This creates a tension between order and disorder that is the visual equivalent of the music's "nervous" energy.

### Halftone and Print Artifacts

Coarse halftone dot patterns, moire interference patterns, registration marks, and crop marks from the print production process. New Wave designers used photocopiers, Chartpak adhesive films, and other analog production tools, and they let the artifacts of these tools become part of the design language. Translate to web using CSS `radial-gradient` dot patterns, SVG noise filters, and subtle repeating-line overlays.

### Retro-Futurist Motifs

Imagery borrowed from 1950s American atomic-age culture -- space rockets, atom symbols, ray guns, suburban ranch houses, vintage televisions -- but rendered in fluorescent colors and placed in angular, ironic compositions. The optimism of the Eisenhower era is subverted by 1980s cynicism. These motifs work as decorative accents, icon systems, or background illustrations.

### Geometric Floating Elements

Abstract geometric shapes -- triangles, circles, squares, lines -- scattered across compositions in arrangements that reference Constructivism and Bauhaus but with the precision deliberately disrupted. Shapes float in space, overlap text, and break out of containers. They are the visual equivalent of the music's staccato, angular rhythms.

---

## Related Aesthetics

| Aesthetic | Relationship to New Wave |
|-----------|-------------------------|
| **Memphis Design** | Contemporary sibling; shares the fluorescent colors and geometric shapes but Memphis is maximalist and pattern-dense where New Wave is more angular and grid-deconstructing |
| **Post-Punk** | Darker, more experimental evolution; retains the angular energy but replaces New Wave's campy pop sensibility with cold seriousness |
| **Italo Disco** | European parallel; shares the synthetic, electronic, and fluorescent visual language but with a more glamorous, nightlife-oriented sensibility |
| **New Romantic** | Glamorous offshoot; takes New Wave's synthetic modernity into high-fashion, androgynous territory with lush production |
| **Bauhaus / Swiss Style** | The modernist foundation that New Wave deliberately deconstructs; the clean grids and geometric type that New Wave takes and breaks |
| **Constructivism** | Historical ancestor; New Wave borrows the diagonal compositions, geometric shapes, and political-poster energy but strips away the political sincerity |
| **Pop Art** | Shared embrace of popular culture, commercial imagery, and the blurring of high and low art boundaries |
| **Synthwave** | Later nostalgic reinterpretation; takes New Wave's neon palette and retro-futurism into a more overtly 1980s-nostalgic direction |
| **Electroclash** | Early 2000s revival movement that directly recycled New Wave's visual and musical aesthetics with a self-aware, ironic twist |
| **Laser Grid** | Shares the neon-on-dark palette and retro-futurist sensibility, focused specifically on the grid/wireframe visual language |
| **Early Cyber** | Successor aesthetic that takes the angular, technological energy into the early internet age |
| **Minimal Wave** | Stripped-down subgenre; the lo-fi, ultra-minimal end of the New Wave spectrum with colder, more austere visuals |

---

## Quick-Start: Minimal New Wave Page Template

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>New Wave Page</title>
  <link href="https://fonts.googleapis.com/css2?family=Orbitron:wght@400;700;900&family=Space+Grotesk:wght@300;400;500;700&family=Rajdhani:wght@400;500;600;700&display=swap" rel="stylesheet">
  <style>
    :root {
      --nw-pink: #ff1493;
      --nw-yellow: #ffe600;
      --nw-cyan: #00e5ff;
      --nw-purple: #9b30ff;
      --nw-orange: #ff6d00;
      --nw-green: #39ff14;
      --nw-black: #0a0a0a;
      --nw-white: #ffffff;
      --nw-cool-gray: #b0bec5;
      --nw-charcoal: #1a1a2e;
    }

    * { margin: 0; padding: 0; box-sizing: border-box; }

    body {
      background: var(--nw-black);
      color: var(--nw-white);
      font-family: 'Space Grotesk', sans-serif;
      font-weight: 300;
      line-height: 1.7;
    }

    h1, h2, h3 {
      font-family: 'Orbitron', sans-serif;
      font-weight: 700;
      text-transform: uppercase;
      letter-spacing: 0.04em;
      line-height: 1.1;
    }

    /* Navigation */
    nav {
      display: flex;
      align-items: center;
      justify-content: space-between;
      padding: 16px 40px;
      border-bottom: 2px solid var(--nw-pink);
    }

    nav .logo {
      font-family: 'Orbitron', sans-serif;
      font-weight: 700;
      font-size: 1.3rem;
      color: var(--nw-pink);
      text-decoration: none;
      text-transform: uppercase;
      letter-spacing: 0.08em;
    }

    nav ul {
      display: flex;
      gap: 28px;
      list-style: none;
    }

    nav ul a {
      color: var(--nw-cool-gray);
      text-decoration: none;
      font-family: 'Rajdhani', sans-serif;
      font-weight: 500;
      font-size: 0.9rem;
      text-transform: uppercase;
      letter-spacing: 0.06em;
      border-bottom: 2px solid transparent;
      padding-bottom: 2px;
      transition: color 0.2s, border-color 0.2s;
    }

    nav ul a:hover {
      color: var(--nw-cyan);
      border-bottom-color: var(--nw-cyan);
    }

    /* Hero */
    .hero {
      position: relative;
      min-height: 85vh;
      display: flex;
      align-items: center;
      padding: 80px 40px;
      overflow: hidden;
    }

    /* Background grid lines */
    .hero::before {
      content: '';
      position: absolute;
      inset: 0;
      background-image:
        linear-gradient(rgba(255, 255, 255, 0.03) 1px, transparent 1px),
        linear-gradient(90deg, rgba(255, 255, 255, 0.03) 1px, transparent 1px);
      background-size: 80px 80px;
      pointer-events: none;
    }

    .hero-content {
      max-width: 700px;
      position: relative;
      z-index: 2;
    }

    .hero h1 {
      font-size: clamp(3rem, 8vw, 6rem);
      font-weight: 900;
      margin-bottom: 1.5rem;
      color: var(--nw-pink);
      text-shadow: 0 0 10px rgba(255, 20, 147, 0.5), 0 0 30px rgba(255, 20, 147, 0.2);
    }

    .hero h1 .word-accent {
      color: var(--nw-cyan);
      display: inline-block;
      transform: skewX(-8deg);
      text-shadow: 0 0 10px rgba(0, 229, 255, 0.5), 0 0 30px rgba(0, 229, 255, 0.2);
    }

    .hero p {
      font-size: 1.15rem;
      color: var(--nw-cool-gray);
      max-width: 500px;
      margin-bottom: 2.5rem;
    }

    .btn {
      display: inline-block;
      padding: 12px 32px;
      font-family: 'Orbitron', sans-serif;
      font-weight: 700;
      font-size: 0.9rem;
      text-transform: uppercase;
      letter-spacing: 0.1em;
      color: var(--nw-white);
      background: var(--nw-pink);
      border: 2px solid var(--nw-pink);
      text-decoration: none;
      cursor: pointer;
      transform: skewX(-6deg);
      transition: all 0.2s;
    }

    .btn:hover {
      background: transparent;
      color: var(--nw-pink);
      box-shadow: 0 0 12px rgba(255, 20, 147, 0.5);
    }

    .btn--outline {
      background: transparent;
      color: var(--nw-cyan);
      border-color: var(--nw-cyan);
    }

    .btn--outline:hover {
      background: var(--nw-cyan);
      color: var(--nw-black);
    }

    /* Floating geometric shapes */
    .shape {
      position: absolute;
      z-index: 1;
      pointer-events: none;
    }

    .shape--triangle-pink {
      width: 0; height: 0;
      border-left: 40px solid transparent;
      border-right: 40px solid transparent;
      border-bottom: 70px solid var(--nw-pink);
      top: 15%;
      right: 15%;
      transform: rotate(20deg);
      opacity: 0.7;
    }

    .shape--circle-cyan {
      width: 120px; height: 120px;
      border: 3px solid var(--nw-cyan);
      border-radius: 50%;
      bottom: 25%;
      right: 10%;
      opacity: 0.5;
    }

    .shape--dot-grid {
      width: 100px; height: 100px;
      background-image: radial-gradient(circle 2px, var(--nw-yellow) 100%, transparent 100%);
      background-size: 12px 12px;
      top: 60%;
      right: 30%;
      opacity: 0.3;
      transform: rotate(-10deg);
    }

    .shape--line-diagonal {
      width: 160px;
      height: 2px;
      background: var(--nw-purple);
      top: 40%;
      right: 20%;
      transform: rotate(-35deg);
      opacity: 0.5;
    }

    .shape--cross-yellow {
      width: 40px; height: 40px;
      top: 30%;
      right: 40%;
    }
    .shape--cross-yellow::before,
    .shape--cross-yellow::after {
      content: '';
      position: absolute;
      background: var(--nw-yellow);
    }
    .shape--cross-yellow::before {
      width: 100%; height: 3px;
      top: 50%; transform: translateY(-50%);
    }
    .shape--cross-yellow::after {
      width: 3px; height: 100%;
      left: 50%; transform: translateX(-50%);
    }

    /* Features section */
    .features {
      padding: 80px 40px;
      background: var(--nw-charcoal);
      position: relative;
    }

    .features h2 {
      font-size: 2rem;
      text-align: center;
      margin-bottom: 3rem;
      color: var(--nw-cyan);
      letter-spacing: 0.06em;
    }

    .features-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
      gap: 24px;
      max-width: 1100px;
      margin: 0 auto;
    }

    .feature-card {
      background: var(--nw-black);
      border: 2px solid var(--nw-cool-gray);
      padding: 2rem;
      position: relative;
      transition: border-color 0.2s, box-shadow 0.2s;
    }

    .feature-card:hover {
      border-color: var(--nw-pink);
      box-shadow: 0 0 12px rgba(255, 20, 147, 0.3);
    }

    .feature-card::before {
      content: '';
      position: absolute;
      top: 0;
      right: 0;
      width: 0;
      height: 0;
      border-top: 25px solid var(--nw-pink);
      border-left: 25px solid transparent;
    }

    .feature-card:nth-child(2)::before { border-top-color: var(--nw-cyan); }
    .feature-card:nth-child(3)::before { border-top-color: var(--nw-yellow); }

    .feature-card h3 {
      font-family: 'Rajdhani', sans-serif;
      font-size: 1.2rem;
      color: var(--nw-cyan);
      margin-bottom: 0.75rem;
      letter-spacing: 0.05em;
    }

    .feature-card p {
      color: var(--nw-cool-gray);
      font-size: 0.95rem;
      line-height: 1.6;
    }

    /* Angular divider */
    .angle-divider {
      height: 60px;
      background: linear-gradient(to bottom right, var(--nw-charcoal) 49.5%, var(--nw-black) 50%);
    }

    /* CTA section */
    .cta {
      background: var(--nw-black);
      text-align: center;
      padding: 80px 40px;
      position: relative;
    }

    /* Scanline overlay */
    .cta::after {
      content: '';
      position: absolute;
      inset: 0;
      background: repeating-linear-gradient(
        0deg,
        transparent,
        transparent 2px,
        rgba(0, 0, 0, 0.06) 2px,
        rgba(0, 0, 0, 0.06) 4px
      );
      pointer-events: none;
    }

    .cta h2 {
      font-size: clamp(1.8rem, 5vw, 3rem);
      color: var(--nw-pink);
      text-shadow: 0 0 10px rgba(255, 20, 147, 0.4);
      margin-bottom: 1rem;
    }

    .cta p {
      color: var(--nw-cool-gray);
      font-size: 1.1rem;
      margin-bottom: 2rem;
    }

    @media (max-width: 768px) {
      .hero { min-height: auto; padding: 60px 20px; }
      .hero h1 { font-size: 2.5rem; }
      nav { padding: 14px 20px; }
      nav ul { gap: 16px; }
      .shape { opacity: 0.3; }
      .features, .cta { padding: 60px 20px; }
    }
  </style>
</head>
<body>
  <nav>
    <a href="#" class="logo">New Wave</a>
    <ul>
      <li><a href="#">About</a></li>
      <li><a href="#">Work</a></li>
      <li><a href="#">Contact</a></li>
    </ul>
  </nav>

  <section class="hero">
    <div class="hero-content">
      <h1>
        Synthetic<br>
        <span class="word-accent">Modernity.</span>
      </h1>
      <p>Design that deconstructs the grid, celebrates the artificial, and turns the rules of modernism inside out.</p>
      <a href="#" class="btn">Explore Now</a>
    </div>
    <!-- Geometric decorative shapes -->
    <div class="shape shape--triangle-pink"></div>
    <div class="shape shape--circle-cyan"></div>
    <div class="shape shape--dot-grid"></div>
    <div class="shape shape--line-diagonal"></div>
    <div class="shape shape--cross-yellow"></div>
  </section>

  <section class="features">
    <h2>What Defines It</h2>
    <div class="features-grid">
      <div class="feature-card">
        <h3>Dysfunctional Grid</h3>
        <p>Start with Swiss modernist precision, then deliberately break every rule. Skew, rotate, and overlap until order becomes angular tension.</p>
      </div>
      <div class="feature-card">
        <h3>Fluorescent Palette</h3>
        <p>Hot pink, electric cyan, and neon yellow on dark backgrounds. Colors that look lit from within, like signs in a late-night club.</p>
      </div>
      <div class="feature-card">
        <h3>Plastic Futurism</h3>
        <p>1950s atomic-age optimism collides with 1980s irony. Everything is synthetic, angular, and deliberately artificial.</p>
      </div>
    </div>
  </section>

  <div class="angle-divider"></div>

  <section class="cta">
    <h2>Ready to Break the Grid?</h2>
    <p>New Wave proves that dysfunction is a design choice. Embrace the angular.</p>
    <a href="#" class="btn">Get Started</a>
  </section>
</body>
</html>
```
