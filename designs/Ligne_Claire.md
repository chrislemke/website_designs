# Ligne Claire Reference

Ligne Claire (French for "clear line") is an illustration and visual design aesthetic pioneered by Belgian cartoonist Herge, creator of The Adventures of Tintin. It is defined by uniform-weight outlines, flat unmodulated color, minimal shading, and a balance of cartoonish simplicity in foreground elements against realistically detailed backgrounds. The style prioritizes clarity, readability, and structured visual storytelling above all else. Herge's guiding maxim was: "the line must prevail over the tint, clarity over virtuosity."

---

## Visual Characteristics

### Core Design Traits

- **Uniform-weight outlines** -- every element is defined by clear, distinct black lines of consistent thickness; no variation in stroke weight for emphasis or depth
- **Flat, unmodulated color** -- solid color fills without gradients, blending, or color modulation; each area is a single uniform hue
- **No hatching or cross-hatching** -- shading is eliminated entirely; depth and form are communicated through line and color alone, never through tonal rendering
- **Illuminated shadows** -- cast shadows, when present, are rendered in lighter or colored tones rather than dark values, preserving the overall brightness and clarity
- **Downplayed contrast** -- value contrasts are kept moderate; the style avoids dramatic chiaroscuro or stark light-dark opposition
- **Realistic proportions with stylized rendering** -- objects and environments maintain believable proportions and perspectives despite the simplified drawing technique
- **Cartoonish foregrounds against detailed backgrounds** -- simplified, expressive characters are placed in front of meticulously rendered architectural and environmental settings
- **Clean separation of elements** -- every object, character, and environmental element is distinctly separated by its outline, preventing visual ambiguity
- **Minimal decorative embellishment** -- ornamentation is stripped away; every visual element serves the narrative or spatial clarity
- **Panel-based structure** -- strict grid-based panel arrangements create order, rhythm, and a deliberate reading flow

### Design Principles

- Clarity and readability take absolute priority over artistic expressiveness
- The outline defines everything -- without the clear line, the image loses its identity
- Color serves the drawing, never the reverse; tint supports linework rather than overshadowing it
- Flat color fields enhance legibility by eliminating tonal noise
- Compositional depth is achieved through layered planes (foreground, midground, background) defined by line, not by atmospheric perspective or shading
- Apparent simplicity is deceptive -- achieving clean, precise linework and carefully chosen flat color requires significant craftsmanship
- Every shade is chosen for readability and narrative function, not for decorative effect
- Visual hierarchy is established through line weight consistency, color contrast, and spatial positioning

---

## Color Palette

### Ligne Claire Primary Palette

The canonical Ligne Claire palette draws from Herge's Tintin albums: strong, saturated primaries and secondaries applied flat, with warm cream or off-white backgrounds. Every color is chosen to be instantly readable and narratively functional.

| Color Name | Hex | Role / Usage |
|------------|-----|-------------|
| **Tintin Blue** | `#3B7DD8` | Primary blue, skies, clothing (Tintin's iconic sweater), water |
| **Signal Red** | `#D42B2B` | Accent red, danger signals, key objects, Haddock's sweater |
| **Sunshine Yellow** | `#F5C842` | Warm highlights, Tintin's hair, desert scenes, optimism |
| **Herge Green** | `#4AA84E` | Vegetation, landscapes, secondary clothing elements |
| **Warm Orange** | `#E87D2F` | Earthy warmth, adventure settings, brick, terracotta |
| **Deep Brown** | `#6B3A2A` | Woodwork, earth tones, furniture, leather |
| **Cream White** | `#FAF5E8` | Primary page background, open sky, negative space |
| **Ink Black** | `#1A1A1A` | All outlines, text, defining lines (never pure #000) |
| **Sky Cerulean** | `#7AB8E0` | Open skies, horizon backgrounds, calm water |
| **Soft Sand** | `#E8D5A3` | Desert settings, aged paper, warm neutrals |
| **Muted Mauve** | `#9C7BAD` | Twilight scenes, shadow tinting, indoor atmospherics |
| **Slate Grey** | `#7A8B96` | Machinery, urban surfaces, overcast skies |

### Extended Tint Scale

Each base color extends into lighter tints for backgrounds and panels, maintaining the flat-fill principle:

| Level | Purpose | Example (Tintin Blue) |
|-------|---------|----------------------|
| 100 | Tinted panel backgrounds | `#E0EBF7` |
| 200 | Section backgrounds, sky washes | `#B8D4EE` |
| 300 | Secondary fills, water highlights | `#8FBDE5` |
| 400 | Mid-tone fills | `#5F9DDC` |
| **500** | **Base color** | **`#3B7DD8`** |
| 600 | Shaded variant | `#2F64AD` |
| 700 | Dark accent | `#234B82` |
| 800 | Deep contrast | `#183257` |

### CSS Custom Properties

```css
:root {
  /* Primary palette */
  --lc-blue: #3b7dd8;
  --lc-red: #d42b2b;
  --lc-yellow: #f5c842;
  --lc-green: #4aa84e;
  --lc-orange: #e87d2f;
  --lc-brown: #6b3a2a;

  /* Neutrals */
  --lc-cream: #faf5e8;
  --lc-ink: #1a1a1a;
  --lc-sand: #e8d5a3;
  --lc-slate: #7a8b96;

  /* Atmospheric */
  --lc-cerulean: #7ab8e0;
  --lc-mauve: #9c7bad;

  /* Tinted backgrounds */
  --lc-blue-tint: #e0ebf7;
  --lc-red-tint: #f8e0e0;
  --lc-yellow-tint: #fdf3d6;
  --lc-green-tint: #dff0df;

  /* Page surfaces */
  --lc-bg-page: #faf5e8;
  --lc-bg-panel: #ffffff;
  --lc-bg-muted: #f2ece0;

  /* Text */
  --lc-text-primary: #1a1a1a;
  --lc-text-secondary: #5a5245;
  --lc-text-caption: #7a8b96;

  /* Outline -- the defining element */
  --lc-outline: #1a1a1a;
  --lc-outline-width: 2px;
}
```

### Color Usage Guidelines

- **Use flat, solid fills exclusively** -- no gradients, no texture overlays, no color modulation within a single area
- **Strong primaries for key elements** -- blue, red, and yellow carry the visual narrative; use them for focal points
- **Cream or warm off-white backgrounds** -- never use stark white (#fff) as the page background; the warm cream (#FAF5E8) evokes the printed album feel
- **Illuminated shadows** -- when indicating shadow, use a lighter tint of the base color or a warm muted tone, never a dark grey or black fill
- **Limit the active palette** -- any single panel or section should use 3-4 colors maximum from the palette; the rest is line and background
- **Black is reserved for outlines** -- the ink color is used exclusively for defining lines; large black fills should be avoided
- **Color contrast is moderate** -- neighboring areas should differ in hue but maintain similar value range, avoiding harsh juxtapositions

---

## Typography

### Typeface Characteristics

Ligne Claire typography mirrors the aesthetic's core principle: clear, legible, unpretentious. Text in the original comics used hand-lettered capitals; for web applications, this translates to:

- **Clean sans-serif faces** -- geometric or humanist sans-serifs that echo the precision and clarity of the linework
- **Medium weight preferred** -- neither too light nor too heavy; matching the uniform stroke weight of the illustrations
- **Rounded or softened terminals** -- typefaces with slightly rounded endings harmonize with the organic-yet-precise quality of the linework
- **Uppercase for display / headings** -- referencing the all-caps lettering tradition of Franco-Belgian comics
- **Comfortable, generous spacing** -- open tracking and line-height for readability, matching the style's anti-clutter philosophy
- **No decorative, serif, or script faces** -- these conflict with the fundamental clarity principle

### Recommended Web Fonts (Google Fonts)

| Font | Style | Best For |
|------|-------|----------|
| **Nunito** | Rounded geometric sans-serif | Body text -- rounded terminals echo the smooth, clear linework |
| **Quicksand** | Rounded geometric, friendly | Headlines and display -- soft geometry matches the style's warmth |
| **Comfortaa** | Rounded geometric, modern | Display titles -- distinctive rounded character evokes comic lettering |
| **Baloo 2** | Rounded, slightly playful | Headers -- bridges comic lettering and web typography |
| **Fredoka** | Bold rounded, comic-inspired | Display headlines -- direct reference to comic book aesthetics |
| **Varela Round** | Simple rounded sans | Body text -- clean, unassuming, highly legible |
| **Nunito Sans** | Rounded humanist sans | Body text, UI elements -- slightly more neutral than Nunito |
| **Lexend** | Optimized readability, clean | Long-form body text -- maximizes readability, the core Ligne Claire value |
| **Outfit** | Modern geometric sans | Navigation, labels -- clean and contemporary feel |
| **Bangers** | Comic book display font | Large hero text only -- authentic comic lettering for impact |

### Font Pairing Suggestions

| Heading Font | Body Font | Character |
|-------------|-----------|-----------|
| **Fredoka** (600) | **Nunito** (400) | Comic-inspired, warm, approachable -- closest to authentic Ligne Claire |
| **Quicksand** (600) | **Lexend** (400) | Modern clarity, geometric precision, highly readable |
| **Comfortaa** (700) | **Varela Round** (400) | Distinctly rounded, playful yet refined |
| **Bangers** (400) | **Nunito Sans** (400) | Bold comic impact for headers, clean reading for body |
| **Outfit** (600) | **Nunito** (400) | Contemporary, clean, versatile for professional contexts |

### Typography CSS Example

```css
/* Import fonts */
@import url('https://fonts.googleapis.com/css2?family=Fredoka:wght@400;500;600;700&family=Nunito:wght@400;500;600;700&display=swap');

/* Headings -- comic-inspired clarity */
h1, h2, h3, h4, h5, h6 {
  font-family: 'Fredoka', 'Quicksand', sans-serif;
  font-weight: 600;
  color: var(--lc-text-primary);
  line-height: 1.2;
  letter-spacing: 0.01em;
  text-transform: uppercase;
}

/* Display / Hero text */
.lc-display {
  font-family: 'Fredoka', sans-serif;
  font-size: clamp(2.5rem, 5vw, 4.5rem);
  font-weight: 700;
  letter-spacing: 0.02em;
  line-height: 1.1;
  text-transform: uppercase;
}

/* Body text */
body {
  font-family: 'Nunito', 'Varela Round', sans-serif;
  font-weight: 400;
  font-size: 1rem;
  line-height: 1.75;
  color: var(--lc-text-primary);
}

/* Caption / secondary text */
.lc-caption {
  font-family: 'Nunito', sans-serif;
  font-weight: 400;
  font-size: 0.85rem;
  color: var(--lc-text-caption);
  line-height: 1.5;
  letter-spacing: 0.02em;
  text-transform: uppercase;
}

/* Comic speech-bubble style callout text */
.lc-callout {
  font-family: 'Fredoka', sans-serif;
  font-weight: 500;
  font-size: 1.1rem;
  line-height: 1.5;
  text-align: center;
  text-transform: uppercase;
  letter-spacing: 0.03em;
}
```

---

## Layout Principles

### Grid and Structure

- **Panel-based layout** -- content is organized in clearly delineated rectangular panels separated by visible borders or gutters, referencing the comic-strip grid
- **Strict grid adherence** -- panels and sections align to a regular, predictable grid; the structure itself communicates stability and order
- **Prominent black outlines on containers** -- every card, panel, and section boundary is defined by a clear, uniform-weight border (2-3px solid black), the web equivalent of the clear line
- **Warm off-white page background** -- the page surface uses cream/off-white (#FAF5E8) to evoke the feel of a printed comic album
- **Generous gutters between panels** -- spacing between content blocks is deliberate and consistent, typically 16-24px, mimicking comic-panel gutters
- **Balanced symmetry** -- elements are arranged with deliberate symmetry and balance; asymmetry is used sparingly and intentionally
- **Layered depth through composition** -- foreground, midground, and background elements are separated through positioning and color, not through shadows or blur
- **Maximum width constraint** -- content is contained within a comfortable reading width (1000-1200px) centered on the page
- **Flat, border-defined hierarchy** -- visual hierarchy comes from outline weight, color fills, and spatial positioning, never from shadows or elevation

### Section Organization

- **Navigation**: Top bar with clear outline border on the bottom; logo and links in uniform weight, uppercase text; cream background
- **Hero**: Large illustrated panel occupying full width; bold headline in comic lettering style; flat-colored illustration or character in the foreground against a detailed background
- **Content panels**: 2-3 column grid of outlined cards, each with a flat-colored header area, clear title, and body text
- **Feature strip**: Horizontal row of icon + label pairs, each in its own bordered cell, resembling a comic strip row
- **Illustrated callout**: Full-width panel with a speech-bubble or caption-box overlay containing key messaging
- **Detail sections**: Alternating text/image panels arranged in a comic-page layout, with clear gutter separation
- **Footer**: Bordered panel at the bottom with muted background; organized links in columns; clear outline on top edge

### Responsive Approach

- Panels stack vertically on mobile, maintaining their outlines and internal padding
- Grid transitions from multi-column to single-column below 768px
- Outline widths remain consistent across breakpoints -- the clear line does not thin on small screens
- Typography scales using `clamp()` but maintains uppercase heading treatment at all sizes
- Gutters between panels reduce proportionally but never collapse entirely
- Touch targets maintain minimum 44px sizing within bordered interactive elements

---

## CSS / Design Techniques

### The Clear-Line Panel Component

```css
.lc-panel {
  background: var(--lc-bg-panel);
  border: var(--lc-outline-width) solid var(--lc-outline);
  border-radius: 4px;
  padding: 28px;
  /* No box-shadow -- outlines define everything in Ligne Claire */
  position: relative;
}

/* Panel with colored header band */
.lc-panel--headed {
  padding-top: 0;
}

.lc-panel--headed .lc-panel__header {
  background: var(--lc-blue);
  color: #ffffff;
  margin: -1px -1px 24px -1px;
  padding: 16px 28px;
  border-radius: 3px 3px 0 0;
  border-bottom: var(--lc-outline-width) solid var(--lc-outline);
  font-family: 'Fredoka', sans-serif;
  font-weight: 600;
  text-transform: uppercase;
  letter-spacing: 0.02em;
}

/* Panel grid */
.lc-panel-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
  gap: 20px;
}
```

### Comic-Strip Row Layout

```css
.lc-strip {
  display: flex;
  gap: 0;
  border: var(--lc-outline-width) solid var(--lc-outline);
  border-radius: 4px;
  overflow: hidden;
}

.lc-strip__cell {
  flex: 1;
  padding: 24px;
  text-align: center;
  border-right: var(--lc-outline-width) solid var(--lc-outline);
}

.lc-strip__cell:last-child {
  border-right: none;
}

.lc-strip__cell h3 {
  font-family: 'Fredoka', sans-serif;
  font-size: 1rem;
  text-transform: uppercase;
  margin-top: 12px;
}

@media (max-width: 768px) {
  .lc-strip {
    flex-direction: column;
  }

  .lc-strip__cell {
    border-right: none;
    border-bottom: var(--lc-outline-width) solid var(--lc-outline);
  }

  .lc-strip__cell:last-child {
    border-bottom: none;
  }
}
```

### Clear-Line Button

```css
.lc-button {
  display: inline-flex;
  align-items: center;
  justify-content: center;
  background: var(--lc-blue);
  color: #ffffff;
  border: var(--lc-outline-width) solid var(--lc-outline);
  border-radius: 4px;
  padding: 12px 32px;
  font-family: 'Fredoka', sans-serif;
  font-weight: 600;
  font-size: 0.95rem;
  text-transform: uppercase;
  letter-spacing: 0.04em;
  cursor: pointer;
  transition: background 0.15s ease;
  text-decoration: none;
  /* No box-shadow -- the outline IS the definition */
}

.lc-button:hover {
  background: var(--lc-cerulean);
}

.lc-button:active {
  background: #2f64ad;
}

/* Red variant */
.lc-button--red {
  background: var(--lc-red);
}

.lc-button--red:hover {
  background: #b02323;
}

/* Yellow variant */
.lc-button--yellow {
  background: var(--lc-yellow);
  color: var(--lc-text-primary);
}

.lc-button--yellow:hover {
  background: #e0b53a;
}

/* Ghost / outline variant */
.lc-button--ghost {
  background: transparent;
  color: var(--lc-text-primary);
}

.lc-button--ghost:hover {
  background: var(--lc-cream);
}
```

### Navigation Bar

```css
.lc-nav {
  display: flex;
  align-items: center;
  justify-content: space-between;
  max-width: 1200px;
  margin: 0 auto;
  padding: 16px 40px;
  border-bottom: var(--lc-outline-width) solid var(--lc-outline);
  background: var(--lc-bg-page);
}

.lc-nav__logo {
  font-family: 'Fredoka', sans-serif;
  font-weight: 700;
  font-size: 1.5rem;
  color: var(--lc-text-primary);
  text-decoration: none;
  text-transform: uppercase;
  letter-spacing: 0.03em;
}

.lc-nav__links {
  display: flex;
  gap: 28px;
  list-style: none;
  margin: 0;
  padding: 0;
}

.lc-nav__links a {
  font-family: 'Nunito', sans-serif;
  font-weight: 600;
  font-size: 0.9rem;
  color: var(--lc-text-secondary);
  text-decoration: none;
  text-transform: uppercase;
  letter-spacing: 0.04em;
  padding: 4px 0;
  border-bottom: 2px solid transparent;
  transition: color 0.15s ease, border-color 0.15s ease;
}

.lc-nav__links a:hover {
  color: var(--lc-blue);
  border-bottom-color: var(--lc-blue);
}

.lc-nav__links a.active {
  color: var(--lc-blue);
  border-bottom-color: var(--lc-blue);
}
```

### Hero Section

```css
.lc-hero {
  display: flex;
  align-items: center;
  justify-content: space-between;
  max-width: 1200px;
  margin: 0 auto;
  padding: 60px 40px;
  gap: 48px;
}

.lc-hero__content {
  flex: 1;
  max-width: 500px;
}

.lc-hero__content h1 {
  font-size: clamp(2.2rem, 5vw, 3.8rem);
  font-weight: 700;
  margin-bottom: 1rem;
  line-height: 1.1;
  text-transform: uppercase;
}

.lc-hero__content p {
  font-size: 1.1rem;
  color: var(--lc-text-secondary);
  margin-bottom: 2rem;
  line-height: 1.75;
}

.lc-hero__visual {
  flex: 1;
  display: flex;
  justify-content: center;
  align-items: center;
}

/* The hero illustration panel -- bordered like a comic panel */
.lc-hero__illustration {
  border: var(--lc-outline-width) solid var(--lc-outline);
  border-radius: 4px;
  overflow: hidden;
  background: var(--lc-cerulean);
  width: 100%;
  max-width: 480px;
  aspect-ratio: 4 / 3;
}

.lc-hero__illustration img,
.lc-hero__illustration svg {
  width: 100%;
  height: 100%;
  object-fit: cover;
}

@media (max-width: 768px) {
  .lc-hero {
    flex-direction: column-reverse;
    text-align: center;
    padding: 40px 20px;
    gap: 32px;
  }
}
```

### Speech Bubble / Callout Component

```css
.lc-speech-bubble {
  position: relative;
  background: var(--lc-bg-panel);
  border: var(--lc-outline-width) solid var(--lc-outline);
  border-radius: 20px;
  padding: 24px 32px;
  font-family: 'Fredoka', sans-serif;
  font-weight: 500;
  font-size: 1.05rem;
  text-align: center;
  text-transform: uppercase;
  letter-spacing: 0.02em;
  line-height: 1.5;
  max-width: 400px;
}

/* Tail pointing down */
.lc-speech-bubble::after {
  content: '';
  position: absolute;
  bottom: -16px;
  left: 50%;
  transform: translateX(-50%);
  width: 0;
  height: 0;
  border-left: 12px solid transparent;
  border-right: 12px solid transparent;
  border-top: 16px solid var(--lc-bg-panel);
}

.lc-speech-bubble::before {
  content: '';
  position: absolute;
  bottom: -19px;
  left: 50%;
  transform: translateX(-50%);
  width: 0;
  height: 0;
  border-left: 14px solid transparent;
  border-right: 14px solid transparent;
  border-top: 18px solid var(--lc-outline);
}
```

### Highlighted Element (Ligne Claire style)

```css
/* Clear-line highlight: thick uniform outline in accent color */
.lc-highlight {
  outline: 3px solid var(--lc-red);
  outline-offset: 4px;
  border-radius: 2px;
  transition: outline-color 0.2s ease;
}

/* Flat color badge */
.lc-badge {
  display: inline-flex;
  align-items: center;
  padding: 4px 12px;
  background: var(--lc-yellow);
  color: var(--lc-text-primary);
  border: var(--lc-outline-width) solid var(--lc-outline);
  border-radius: 3px;
  font-family: 'Fredoka', sans-serif;
  font-weight: 600;
  font-size: 0.75rem;
  text-transform: uppercase;
  letter-spacing: 0.05em;
}
```

### Section Color Blocks

```css
.lc-section {
  padding: 80px 0;
}

.lc-section--cream {
  background: var(--lc-bg-page);
}

.lc-section--white {
  background: var(--lc-bg-panel);
}

.lc-section--muted {
  background: var(--lc-bg-muted);
}

.lc-section--blue {
  background: var(--lc-blue);
  color: #ffffff;
}

.lc-section--red {
  background: var(--lc-red);
  color: #ffffff;
}

.lc-section--yellow {
  background: var(--lc-yellow);
  color: var(--lc-text-primary);
}

/* Bordered section separator -- the clear line as a structural device */
.lc-section + .lc-section {
  border-top: var(--lc-outline-width) solid var(--lc-outline);
}

/* Text color overrides on colored sections */
.lc-section--blue h1,
.lc-section--blue h2,
.lc-section--blue h3,
.lc-section--red h1,
.lc-section--red h2,
.lc-section--red h3 {
  color: #ffffff;
}

.lc-section--blue p,
.lc-section--red p {
  color: rgba(255, 255, 255, 0.9);
}
```

### Form Elements

```css
.lc-input {
  width: 100%;
  padding: 12px 16px;
  border: var(--lc-outline-width) solid var(--lc-outline);
  border-radius: 4px;
  font-family: 'Nunito', sans-serif;
  font-size: 0.95rem;
  color: var(--lc-text-primary);
  background: var(--lc-bg-panel);
  transition: border-color 0.15s ease;
  outline: none;
  /* No box-shadow -- clear line only */
}

.lc-input:focus {
  border-color: var(--lc-blue);
}

.lc-input::placeholder {
  color: var(--lc-text-caption);
}

/* Select dropdown */
.lc-select {
  appearance: none;
  width: 100%;
  padding: 12px 40px 12px 16px;
  border: var(--lc-outline-width) solid var(--lc-outline);
  border-radius: 4px;
  font-family: 'Nunito', sans-serif;
  font-size: 0.95rem;
  color: var(--lc-text-primary);
  background: var(--lc-bg-panel) url("data:image/svg+xml,%3Csvg width='12' height='8' viewBox='0 0 12 8' fill='none' xmlns='http://www.w3.org/2000/svg'%3E%3Cpath d='M1 1.5L6 6.5L11 1.5' stroke='%231a1a1a' stroke-width='2' stroke-linecap='round' stroke-linejoin='round'/%3E%3C/svg%3E") no-repeat right 14px center;
  cursor: pointer;
  outline: none;
}

.lc-select:focus {
  border-color: var(--lc-blue);
}
```

### Ligne Claire Icon Style (SVG)

```css
/* Icons should use uniform stroke weight, no fills -- pure outline */
.lc-icon {
  stroke: var(--lc-outline);
  stroke-width: 2px;
  fill: none;
  stroke-linecap: round;
  stroke-linejoin: round;
  width: 24px;
  height: 24px;
}

/* Icon with flat-color fill behind outline */
.lc-icon--filled {
  fill: var(--lc-blue);
  stroke: var(--lc-outline);
  stroke-width: 2px;
}

/* Icon in a bordered circle container */
.lc-icon-circle {
  display: inline-flex;
  align-items: center;
  justify-content: center;
  width: 52px;
  height: 52px;
  border-radius: 50%;
  border: var(--lc-outline-width) solid var(--lc-outline);
  background: var(--lc-yellow-tint);
}
```

---

## Design Do's and Don'ts

### Do

- Define every element with a clear, uniform-weight black outline -- this is the fundamental rule
- Use flat, solid color fills without any gradients, textures, or modulation
- Choose warm off-white or cream backgrounds to evoke the printed album aesthetic
- Organize content in panel-based grid layouts with visible borders and consistent gutters
- Use uppercase, rounded sans-serif typography for headings
- Maintain moderate contrast -- avoid stark black-on-white; prefer warm neutrals
- Keep color palettes limited per section (3-4 active colors plus neutrals)
- Light shadows when needed (use lighter tints, never dark values)
- Use clear visual separation between all elements through outlines and spacing
- Reference comic-strip conventions: speech bubbles, caption boxes, panel sequences

### Don't

- Use drop shadows, box shadows, or any depth simulation effects
- Apply gradients, blend modes, or color transitions within a single element
- Use varying line weights for emphasis -- the line must be uniform
- Use dark, heavy shadows or chiaroscuro effects
- Employ hatching, cross-hatching, or stippling for shading
- Use photographic textures, wood grains, or material simulations
- Choose decorative, serif, or script typefaces for body text
- Create stark, high-contrast compositions -- the style favors moderate, readable values
- Leave elements undefined -- everything must have its clear outline border
- Use pure black (#000000) for large fills -- reserve near-black (#1A1A1A) for outlines only

---

## Related Aesthetics

| Aesthetic | Relationship to Ligne Claire |
|-----------|------------------------------|
| **Adventurecore** | Shares the sense of exploration and travel narrative; Tintin's globe-trotting adventures are a foundational reference for Adventurecore |
| **Fleischer Style** | Contemporary early-animation aesthetic with similar clear outlines and flat color, though with more rubbery, exaggerated proportions |
| **Vintage Hero** | Overlapping visual vocabulary of clear outlines, primary colors, and narrative-driven illustration from the golden age of comics |
| **Flat Design** | Modern digital descendant; shares the flat color, no-shadow, no-gradient principles but strips away the defining outline and illustrative warmth |
| **Atoomstijl (Atomic Style)** | Direct stylistic offspring; applied Ligne Claire principles to posters, LP covers, and graphic design with mid-century modernist influence |
| **Franco-Belgian Comics** | The broader tradition from which Ligne Claire emerged; includes related but distinct styles from Moebius, Franquin, and others |
| **Pop Art** | Shares bold outlines, flat color, and comic-book visual language, though Pop Art embraces irony and appropriation that Ligne Claire avoids |
| **Ukiyo-e / Shin-hanga** | Japanese woodblock prints contributed compositional principles and flat-color-within-outline techniques that influenced Herge |
| **Corporate Memphis** | Modern flat illustration style that echoes the flat-fill, outline-defined approach but with a distinctly corporate, disproportionate human figure vocabulary |

---

## Quick-Start: Minimal Ligne Claire Page Template

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Ligne Claire Page</title>
  <link href="https://fonts.googleapis.com/css2?family=Fredoka:wght@400;500;600;700&family=Nunito:wght@400;500;600;700&display=swap" rel="stylesheet">
  <style>
    :root {
      --lc-blue: #3b7dd8;
      --lc-red: #d42b2b;
      --lc-yellow: #f5c842;
      --lc-green: #4aa84e;
      --lc-orange: #e87d2f;
      --lc-cream: #faf5e8;
      --lc-ink: #1a1a1a;
      --lc-cerulean: #7ab8e0;
      --lc-sand: #e8d5a3;
      --lc-slate: #7a8b96;
      --lc-outline: #1a1a1a;
      --lc-outline-width: 2px;
    }

    * { margin: 0; padding: 0; box-sizing: border-box; }

    body {
      background: var(--lc-cream);
      color: var(--lc-ink);
      font-family: 'Nunito', sans-serif;
      font-weight: 400;
      line-height: 1.75;
    }

    h1, h2, h3 {
      font-family: 'Fredoka', sans-serif;
      font-weight: 600;
      line-height: 1.2;
      text-transform: uppercase;
      letter-spacing: 0.01em;
    }

    /* Navigation */
    nav {
      display: flex;
      align-items: center;
      justify-content: space-between;
      max-width: 1200px;
      margin: 0 auto;
      padding: 16px 40px;
      border-bottom: var(--lc-outline-width) solid var(--lc-outline);
    }

    nav a.logo {
      font-family: 'Fredoka', sans-serif;
      font-weight: 700;
      font-size: 1.5rem;
      color: var(--lc-ink);
      text-decoration: none;
      text-transform: uppercase;
    }

    nav ul {
      display: flex;
      gap: 24px;
      list-style: none;
    }

    nav ul a {
      color: #5a5245;
      text-decoration: none;
      font-weight: 600;
      font-size: 0.9rem;
      text-transform: uppercase;
      letter-spacing: 0.03em;
      transition: color 0.15s;
    }

    nav ul a:hover { color: var(--lc-blue); }

    /* Hero */
    .hero {
      display: flex;
      align-items: center;
      justify-content: space-between;
      max-width: 1200px;
      margin: 0 auto;
      padding: 60px 40px;
      gap: 48px;
    }

    .hero-content { flex: 1; max-width: 480px; }

    .hero h1 {
      font-size: clamp(2.2rem, 5vw, 3.6rem);
      margin-bottom: 1rem;
    }

    .hero p {
      font-size: 1.05rem;
      color: #5a5245;
      margin-bottom: 2rem;
    }

    .hero-visual {
      flex: 1;
      display: flex;
      justify-content: center;
    }

    /* Clear-line button */
    .btn {
      display: inline-block;
      background: var(--lc-blue);
      color: #fff;
      border: var(--lc-outline-width) solid var(--lc-outline);
      border-radius: 4px;
      padding: 12px 32px;
      font-family: 'Fredoka', sans-serif;
      font-weight: 600;
      font-size: 0.95rem;
      text-transform: uppercase;
      letter-spacing: 0.03em;
      cursor: pointer;
      text-decoration: none;
      transition: background 0.15s;
    }

    .btn:hover { background: var(--lc-cerulean); }

    /* Feature strip */
    .features {
      border-top: var(--lc-outline-width) solid var(--lc-outline);
      border-bottom: var(--lc-outline-width) solid var(--lc-outline);
      padding: 0;
    }

    .features h2 {
      text-align: center;
      font-size: 1.8rem;
      padding: 48px 40px 0;
    }

    .features-strip {
      display: flex;
      max-width: 1200px;
      margin: 40px auto;
      border: var(--lc-outline-width) solid var(--lc-outline);
      border-radius: 4px;
      overflow: hidden;
      margin-left: 40px;
      margin-right: 40px;
    }

    .feature-cell {
      flex: 1;
      padding: 28px 20px;
      text-align: center;
      border-right: var(--lc-outline-width) solid var(--lc-outline);
    }

    .feature-cell:last-child { border-right: none; }

    .feature-icon {
      width: 52px;
      height: 52px;
      border-radius: 50%;
      border: var(--lc-outline-width) solid var(--lc-outline);
      margin: 0 auto 16px;
      display: flex;
      align-items: center;
      justify-content: center;
    }

    .feature-cell h3 {
      font-size: 0.95rem;
      margin-bottom: 8px;
    }

    .feature-cell p {
      font-size: 0.9rem;
      color: #5a5245;
    }

    /* CTA section */
    .cta {
      background: var(--lc-blue);
      color: #ffffff;
      text-align: center;
      padding: 60px 40px;
      border-top: var(--lc-outline-width) solid var(--lc-outline);
      border-bottom: var(--lc-outline-width) solid var(--lc-outline);
    }

    .cta h2 {
      font-size: 2rem;
      margin-bottom: 0.75rem;
      color: #ffffff;
    }

    .cta p {
      font-size: 1.05rem;
      opacity: 0.92;
      margin-bottom: 1.5rem;
    }

    .cta .btn {
      background: var(--lc-yellow);
      color: var(--lc-ink);
    }

    .cta .btn:hover {
      background: #e0b53a;
    }

    /* Footer */
    footer {
      background: var(--lc-ink);
      color: var(--lc-sand);
      text-align: center;
      padding: 32px 40px;
      font-size: 0.85rem;
      letter-spacing: 0.02em;
    }

    @media (max-width: 768px) {
      .hero {
        flex-direction: column-reverse;
        text-align: center;
        padding: 40px 20px;
      }
      nav { padding: 12px 20px; }
      nav ul { gap: 16px; }
      .features-strip {
        flex-direction: column;
        margin-left: 20px;
        margin-right: 20px;
      }
      .feature-cell {
        border-right: none;
        border-bottom: var(--lc-outline-width) solid var(--lc-outline);
      }
      .feature-cell:last-child { border-bottom: none; }
    }
  </style>
</head>
<body>
  <nav>
    <a href="#" class="logo">ClearLine</a>
    <ul>
      <li><a href="#">Explore</a></li>
      <li><a href="#">Features</a></li>
      <li><a href="#">Gallery</a></li>
      <li><a href="#">About</a></li>
    </ul>
  </nav>

  <section class="hero">
    <div class="hero-content">
      <h1>Adventures in clarity</h1>
      <p>Clean lines, bold colors, and stories that speak for themselves. A design philosophy where every element earns its place.</p>
      <a href="#" class="btn">Begin the journey</a>
    </div>
    <div class="hero-visual">
      <svg width="420" height="320" viewBox="0 0 420 320" fill="none" xmlns="http://www.w3.org/2000/svg">
        <!-- Sky background -->
        <rect width="420" height="320" rx="4" fill="#7AB8E0" stroke="#1a1a1a" stroke-width="2"/>
        <!-- Clouds -->
        <ellipse cx="100" cy="60" rx="40" ry="18" fill="#FAF5E8" stroke="#1a1a1a" stroke-width="2"/>
        <ellipse cx="80" cy="56" rx="24" ry="14" fill="#FAF5E8" stroke="#1a1a1a" stroke-width="2"/>
        <ellipse cx="310" cy="80" rx="32" ry="14" fill="#FAF5E8" stroke="#1a1a1a" stroke-width="2"/>
        <!-- Building -->
        <rect x="50" y="120" width="100" height="180" fill="#E8D5A3" stroke="#1a1a1a" stroke-width="2"/>
        <rect x="65" y="140" width="24" height="32" rx="2" fill="#3B7DD8" stroke="#1a1a1a" stroke-width="2"/>
        <rect x="110" y="140" width="24" height="32" rx="2" fill="#3B7DD8" stroke="#1a1a1a" stroke-width="2"/>
        <rect x="65" y="200" width="24" height="32" rx="2" fill="#3B7DD8" stroke="#1a1a1a" stroke-width="2"/>
        <rect x="110" y="200" width="24" height="32" rx="2" fill="#3B7DD8" stroke="#1a1a1a" stroke-width="2"/>
        <rect x="82" y="260" width="36" height="40" rx="2" fill="#6B3A2A" stroke="#1a1a1a" stroke-width="2"/>
        <!-- Second building -->
        <rect x="170" y="90" width="80" height="210" fill="#D42B2B" stroke="#1a1a1a" stroke-width="2"/>
        <rect x="185" y="110" width="20" height="28" rx="2" fill="#F5C842" stroke="#1a1a1a" stroke-width="2"/>
        <rect x="215" y="110" width="20" height="28" rx="2" fill="#F5C842" stroke="#1a1a1a" stroke-width="2"/>
        <rect x="185" y="160" width="20" height="28" rx="2" fill="#F5C842" stroke="#1a1a1a" stroke-width="2"/>
        <rect x="215" y="160" width="20" height="28" rx="2" fill="#F5C842" stroke="#1a1a1a" stroke-width="2"/>
        <rect x="185" y="210" width="20" height="28" rx="2" fill="#F5C842" stroke="#1a1a1a" stroke-width="2"/>
        <rect x="215" y="210" width="20" height="28" rx="2" fill="#F5C842" stroke="#1a1a1a" stroke-width="2"/>
        <!-- Third building -->
        <rect x="270" y="150" width="90" height="150" fill="#4AA84E" stroke="#1a1a1a" stroke-width="2"/>
        <rect x="285" y="170" width="22" height="28" rx="2" fill="#FAF5E8" stroke="#1a1a1a" stroke-width="2"/>
        <rect x="323" y="170" width="22" height="28" rx="2" fill="#FAF5E8" stroke="#1a1a1a" stroke-width="2"/>
        <rect x="285" y="220" width="22" height="28" rx="2" fill="#FAF5E8" stroke="#1a1a1a" stroke-width="2"/>
        <rect x="323" y="220" width="22" height="28" rx="2" fill="#FAF5E8" stroke="#1a1a1a" stroke-width="2"/>
        <!-- Ground -->
        <rect x="0" y="298" width="420" height="22" fill="#E8D5A3" stroke="#1a1a1a" stroke-width="2"/>
        <!-- Sun -->
        <circle cx="370" cy="40" r="22" fill="#F5C842" stroke="#1a1a1a" stroke-width="2"/>
      </svg>
    </div>
  </section>

  <section class="features">
    <h2>The clear line approach</h2>
    <div class="features-strip">
      <div class="feature-cell">
        <div class="feature-icon" style="background: #e0ebf7;">
          <svg width="24" height="24" viewBox="0 0 24 24" fill="none"><path d="M12 2L2 7l10 5 10-5-10-5z" fill="#3B7DD8" stroke="#1a1a1a" stroke-width="2"/><path d="M2 17l10 5 10-5" stroke="#1a1a1a" stroke-width="2" fill="none"/><path d="M2 12l10 5 10-5" stroke="#1a1a1a" stroke-width="2" fill="none"/></svg>
        </div>
        <h3>Uniform lines</h3>
        <p>Every outline drawn at consistent weight, creating visual harmony across the entire composition.</p>
      </div>
      <div class="feature-cell">
        <div class="feature-icon" style="background: #f8e0e0;">
          <svg width="24" height="24" viewBox="0 0 24 24" fill="none"><rect x="3" y="3" width="18" height="18" rx="3" fill="#D42B2B" stroke="#1a1a1a" stroke-width="2"/><rect x="7" y="7" width="10" height="10" rx="1" fill="#FAF5E8" stroke="#1a1a1a" stroke-width="2"/></svg>
        </div>
        <h3>Flat color</h3>
        <p>Solid, unmodulated fills that enhance clarity and let the linework define every form.</p>
      </div>
      <div class="feature-cell">
        <div class="feature-icon" style="background: #fdf3d6;">
          <svg width="24" height="24" viewBox="0 0 24 24" fill="none"><circle cx="12" cy="12" r="9" fill="#F5C842" stroke="#1a1a1a" stroke-width="2"/><circle cx="12" cy="12" r="4" fill="#FAF5E8" stroke="#1a1a1a" stroke-width="2"/></svg>
        </div>
        <h3>Total clarity</h3>
        <p>Readability above all. Every element is instantly understood, crossing language barriers.</p>
      </div>
    </div>
  </section>

  <section class="cta">
    <h2>Draw your own clear line</h2>
    <p>Join a tradition of clarity and precision that spans nearly a century of visual storytelling.</p>
    <a href="#" class="btn">Start creating</a>
  </section>

  <footer>
    <p>Designed in the Ligne Claire tradition. Clear lines, bold colors, honest craft.</p>
  </footer>
</body>
</html>
```
