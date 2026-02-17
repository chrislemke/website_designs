# Hygge

A Danish and Norwegian lifestyle aesthetic centered on coziness, comfort, and well-being. Pronounced "hoo-gah," Hygge represents the art of creating warmth and contentment through simple pleasures -- soft lighting, warm drinks, natural materials, and intimate gatherings. In design, Hygge translates to spaces and interfaces that feel like a sanctuary: warm, inviting, unhurried, and gently embracing. The visual language draws heavily from Scandinavian design principles but softens the clinical minimalism with tactile warmth, candlelit tones, and an emphasis on natural imperfection. Hygge is a feeling, not a trend -- it prioritizes emotional experience over material consumption.

---

## Color Palette

- **Primary palette:** Warm creams, soft beiges, muted browns, and gentle off-whites -- the colors of wool blankets, wooden surfaces, and candlelight
- **Accent tones:** Rust, burnt amber, forest green, and muted orange -- the deeper hues of autumn leaves, fireside embers, and spiced drinks
- **Cool complements:** Soft sage, pale blue-gray, and dusty stone -- subtle cool tones that prevent the palette from becoming overly sweet
- **Overall feel:** Low saturation, high warmth; colors should feel like they have been softened by firelight or filtered through a linen curtain
- **Contrast strategy:** Minimal contrast; tonal layering of warm neutrals creates depth without harsh edges. Dark accents (deep brown, charcoal) are used sparingly for text and grounding elements

### Suggested CSS Color Tokens

| Role            | Description              | Suggested Value         |
|-----------------|--------------------------|-------------------------|
| Background      | Warm ivory               | `#FAF7F2` / `#F7F2E7`  |
| Surface         | Soft linen               | `#F0EAE0` / `#EDE6DA`  |
| Surface Alt     | Pale oat                 | `#E6D5C1` / `#D9CBAE`  |
| Primary         | Warm amber               | `#C76A3D` / `#D69434`  |
| Secondary       | Deep walnut              | `#7D5B3A` / `#5B3A29`  |
| Accent 1        | Rust / burnt sienna      | `#A65E2E` / `#B5673A`  |
| Accent 2        | Muted forest green       | `#6B7F5E` / `#7A8E6D`  |
| Accent 3        | Dusty sage               | `#B7C9B2` / `#A8B9A2`  |
| Accent 4        | Soft peach               | `#ECA78D` / `#E8C4A8`  |
| Accent 5        | Warm gray-blue           | `#A4A9AD` / `#8E9499`  |
| Text            | Dark espresso            | `#2C2420` / `#3A3330`  |
| Text light      | Warm medium gray         | `#7A6E65` / `#8F8279`  |
| Border          | Faded taupe              | `#D4C8BB` / `#C9BDB0`  |

### Extended Palette (Hygge Combinations)

| Combo Name          | Color A     | Color B     | Usage                                   |
|---------------------|-------------|-------------|-----------------------------------------|
| Candlelight         | `#FAF7F2`   | `#D69434`   | Hero sections, warm glow overlays       |
| Fireside            | `#7D5B3A`   | `#C76A3D`   | CTAs, active states, navigation         |
| Winter Morning      | `#F7F2E7`   | `#B7C9B2`   | Content cards, soft backgrounds         |
| Woolen Comfort      | `#E6D5C1`   | `#5B3A29`   | Text on light surfaces, subtle depth    |
| Autumn Walk         | `#A65E2E`   | `#6B7F5E`   | Accent pairings, badges, highlights     |
| Linen & Stone       | `#F0EAE0`   | `#A4A9AD`   | Muted sections, footer areas            |

---

## Typography

- **Lettering style:** Clean, warm, and quietly elegant -- Scandinavian simplicity with humanist softness; avoid anything cold, technical, or overly decorative
- **Suggested font families:**
  - Display/headings: Warm sans-serifs with humanist proportions or refined serifs with gentle character (e.g., **Albert Sans**, **DM Serif Display**, **Merriweather**, **Libre Baskerville**)
  - Body: Clean, readable sans-serifs with warm geometry (e.g., **Instrument Sans**, **Work Sans**, **Nunito Sans**, **Inter**)
  - Accent/decorative: For quotes, callouts, or intimate text moments (e.g., **Lora**, **Cormorant Garamond**, **EB Garamond** in italic)
- **Weight usage:** Regular to medium for body text; semi-bold for headings -- avoid extra-bold weights that feel aggressive; light weights for large display text to maintain quietness
- **Sizing:** Comfortable and generous; large headings with ample line height (1.5-1.7 for body, 1.2-1.3 for headings); generosity of spacing reflects the unhurried Hygge ethos
- **Letter spacing:** Slightly open for headings (0.01-0.03em); normal for body; wide tracking on small caps or labels (0.08-0.12em)

### Google Fonts Import

```css
@import url('https://fonts.googleapis.com/css2?family=Albert+Sans:wght@300;400;500;600&family=DM+Serif+Display&family=Instrument+Sans:wght@400;500;600&family=Lora:ital,wght@0,400;0,500;1,400;1,500&display=swap');
```

---

## Visual Characteristics

### Shapes and Forms

- **Soft, rounded rectangles** with generous border-radius -- nothing sharp or angular; every container should feel like a cushion or a smooth stone
- **Organic but restrained** -- subtle curves and natural forms, not the exaggerated blobs of more playful aesthetics; think hand-thrown pottery, not cartoon shapes
- **Gentle asymmetry** -- slight imperfections and organic irregularity that feel handmade and human, not machine-precise
- **Layered depth** -- elements stacked softly like blankets, with subtle shadows suggesting physical overlap rather than flat layers
- **Generous whitespace** -- or rather, "warm space" -- ample breathing room between elements that creates the feeling of an unhurried, uncluttered room

### Patterns and Textures

- **Linen and fabric textures** -- subtle woven patterns or noise overlays that suggest natural textiles
- **Wood grain** -- fine horizontal or diagonal grain patterns at very low opacity for warmth
- **Knit patterns** -- subtle cable-knit or herringbone patterns used sparingly as background textures
- **Candlelight glow** -- soft radial gradients in warm amber that suggest the diffuse light of candles
- **Grain and noise** -- a light film-grain or paper-noise overlay that adds analog warmth
- **Natural photography** -- close-up shots of wool, wood, ceramic, steam from beverages, flickering flames

### Key Decorative Motifs

- Candles and warm light sources (translate to soft glow effects and warm gradient overlays)
- Steaming mugs and beverages (translate to organic, curving steam-like SVG decorations)
- Knitted textures and woven fabrics (translate to subtle CSS pattern backgrounds)
- Fireplaces and hearths (translate to warm-toned hero sections with radial amber gradients)
- Hyggekrog -- cozy nooks (translate to inset content areas with extra padding and warm backgrounds)
- String lights (translate to small, scattered warm dots or subtle sparkle effects)
- Natural botanicals -- dried flowers, eucalyptus (translate to muted green accent elements)

---

## Layout Principles

- **Sanctuary-like enclosure:** Content should feel embraced and protected, like being wrapped in a blanket; generous padding and soft containers create this sense of warmth
- **Unhurried pacing:** Ample vertical spacing between sections; the scroll should feel like a slow, meditative walk, not a rush through information
- **Centered and intimate:** Narrow max-widths (700-800px for text content) create an intimate reading experience rather than a wide, impersonal spread
- **Layered warmth:** Background surfaces stack in soft, warm tones -- ivory behind linen behind oat -- creating tonal depth without hard section breaks
- **Grouped conviviality:** Content arranged in small, cozy groups rather than long isolated lists; card clusters of 2-3 items feel more intimate than grids of 12
- **Anchored with stillness:** Key elements (hero, featured content) should feel still and grounded; avoid busy animations or constant motion
- **Natural flow:** Vertical rhythm follows a natural breathing pattern -- content, pause, content, pause -- rather than relentless density

---

## CSS / Web Design Techniques

### Soft Containers and Rounded Forms

```css
/* Hygge containers are soft and cushion-like */
.card { border-radius: 16px; }
.button { border-radius: 12px; }
.container { border-radius: 20px; }
.image { border-radius: 12px; }
.tag { border-radius: 8px; }
.input { border-radius: 10px; }
```

### Candlelight Glow Effect

```css
.candleglow {
  position: relative;
  overflow: hidden;
}

.candleglow::before {
  content: '';
  position: absolute;
  top: -50%;
  left: 50%;
  transform: translateX(-50%);
  width: 120%;
  height: 100%;
  background: radial-gradient(
    ellipse at center top,
    rgba(214, 148, 52, 0.08) 0%,
    rgba(214, 148, 52, 0.03) 40%,
    transparent 70%
  );
  pointer-events: none;
}
```

### Linen Texture Overlay

```css
.linen-texture {
  position: relative;
}

.linen-texture::after {
  content: '';
  position: absolute;
  inset: 0;
  opacity: 0.03;
  background-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='4' height='4'%3E%3Crect width='1' height='1' x='0' y='0' fill='%237A6E65'/%3E%3Crect width='1' height='1' x='2' y='2' fill='%237A6E65'/%3E%3C/svg%3E");
  background-size: 4px 4px;
  pointer-events: none;
}
```

### Warm Shadows

```css
/* Warm-tinted shadows instead of cold gray */
.card-warm {
  box-shadow:
    0 1px 2px rgba(125, 91, 58, 0.04),
    0 4px 16px rgba(125, 91, 58, 0.06),
    0 12px 40px rgba(125, 91, 58, 0.04);
}

/* Subtle inner glow for cozy nooks */
.hyggekrog {
  box-shadow:
    inset 0 2px 20px rgba(214, 148, 52, 0.05),
    0 4px 16px rgba(125, 91, 58, 0.06);
}

/* Gentle hover warmth */
.card:hover {
  box-shadow:
    0 2px 4px rgba(125, 91, 58, 0.06),
    0 8px 24px rgba(125, 91, 58, 0.08),
    0 16px 48px rgba(125, 91, 58, 0.05);
  transform: translateY(-2px);
  transition: all 0.4s ease;
}
```

### String Light Dots

```css
.string-lights {
  background-image: radial-gradient(
    circle 3px at center,
    rgba(214, 148, 52, 0.25) 0%,
    rgba(214, 148, 52, 0.08) 50%,
    transparent 100%
  );
  background-size: 40px 40px;
  background-position: 0 0;
}
```

### Warm Gradient Backgrounds

```css
/* Fireplace warmth gradient */
.gradient-fireside {
  background: linear-gradient(
    180deg,
    #FAF7F2 0%,
    #F0EAE0 40%,
    #E6D5C1 100%
  );
}

/* Gentle amber wash for hero sections */
.gradient-candlelit {
  background: linear-gradient(
    160deg,
    #FAF7F2 0%,
    #F7F2E7 30%,
    rgba(214, 148, 52, 0.06) 100%
  );
}

/* Autumn walk -- green to warm tones */
.gradient-autumn {
  background: linear-gradient(
    135deg,
    rgba(183, 201, 178, 0.15) 0%,
    #FAF7F2 40%,
    rgba(199, 106, 61, 0.06) 100%
  );
}
```

### Soft Section Dividers

```css
/* Gentle fade divider instead of hard lines */
.section-divider {
  height: 1px;
  border: none;
  background: linear-gradient(
    90deg,
    transparent 0%,
    #D4C8BB 20%,
    #D4C8BB 80%,
    transparent 100%
  );
  margin: 4rem auto;
  max-width: 60%;
}

/* Dotted cozy divider */
.section-divider-dots {
  border: none;
  height: auto;
  text-align: center;
  margin: 3rem auto;
}

.section-divider-dots::before {
  content: '\2022 \00a0\00a0 \2022 \00a0\00a0 \2022';
  color: #D4C8BB;
  font-size: 1rem;
  letter-spacing: 0.3em;
}
```

### Cozy Input Fields

```css
.input-hygge {
  background: #F0EAE0;
  border: 1.5px solid #D4C8BB;
  border-radius: 10px;
  padding: 14px 18px;
  font-family: 'Instrument Sans', sans-serif;
  font-size: 1rem;
  color: #2C2420;
  transition: all 0.3s ease;
}

.input-hygge:focus {
  outline: none;
  border-color: #C76A3D;
  background: #FAF7F2;
  box-shadow: 0 0 0 4px rgba(199, 106, 61, 0.08);
}

.input-hygge::placeholder {
  color: #A89B8E;
}
```

### Buttons

```css
/* Primary -- warm and inviting */
.btn-hygge {
  background: #7D5B3A;
  color: #FAF7F2;
  border: none;
  border-radius: 12px;
  padding: 14px 28px;
  font-family: 'Albert Sans', sans-serif;
  font-weight: 500;
  font-size: 0.95rem;
  letter-spacing: 0.02em;
  cursor: pointer;
  transition: all 0.3s ease;
}

.btn-hygge:hover {
  background: #5B3A29;
  box-shadow: 0 4px 16px rgba(91, 58, 41, 0.15);
  transform: translateY(-1px);
}

/* Secondary -- subtle and soft */
.btn-hygge-secondary {
  background: transparent;
  color: #7D5B3A;
  border: 1.5px solid #D4C8BB;
  border-radius: 12px;
  padding: 13px 27px;
  font-family: 'Albert Sans', sans-serif;
  font-weight: 500;
  font-size: 0.95rem;
  cursor: pointer;
  transition: all 0.3s ease;
}

.btn-hygge-secondary:hover {
  background: #F0EAE0;
  border-color: #7D5B3A;
}
```

### Film Grain Noise Overlay

```css
/* Adds analog warmth to the entire page */
.grain-overlay::before {
  content: '';
  position: fixed;
  inset: 0;
  opacity: 0.02;
  background-image: url("data:image/svg+xml,%3Csvg viewBox='0 0 256 256' xmlns='http://www.w3.org/2000/svg'%3E%3Cfilter id='noise'%3E%3CfeTurbulence type='fractalNoise' baseFrequency='0.9' numOctaves='4' stitchTiles='stitch'/%3E%3C/filter%3E%3Crect width='100%25' height='100%25' filter='url(%23noise)'/%3E%3C/svg%3E");
  background-size: 256px 256px;
  pointer-events: none;
  z-index: 9999;
}
```

### Full Page Scaffold

```css
:root {
  --hygge-bg: #FAF7F2;
  --hygge-surface: #F0EAE0;
  --hygge-surface-alt: #E6D5C1;
  --hygge-primary: #C76A3D;
  --hygge-secondary: #7D5B3A;
  --hygge-accent-rust: #A65E2E;
  --hygge-accent-green: #6B7F5E;
  --hygge-accent-sage: #B7C9B2;
  --hygge-accent-peach: #ECA78D;
  --hygge-accent-gray: #A4A9AD;
  --hygge-text: #2C2420;
  --hygge-text-light: #7A6E65;
  --hygge-border: #D4C8BB;
  --hygge-glow: rgba(214, 148, 52, 0.08);
  --hygge-radius-sm: 8px;
  --hygge-radius-md: 12px;
  --hygge-radius-lg: 16px;
  --hygge-radius-xl: 20px;
}

* {
  box-sizing: border-box;
}

body {
  font-family: 'Instrument Sans', 'Work Sans', sans-serif;
  background-color: var(--hygge-bg);
  color: var(--hygge-text);
  line-height: 1.65;
  margin: 0;
  -webkit-font-smoothing: antialiased;
}

h1, h2, h3 {
  font-family: 'Albert Sans', 'DM Serif Display', serif;
  font-weight: 500;
  line-height: 1.25;
  color: var(--hygge-text);
}

h1 { font-size: 2.5rem; letter-spacing: -0.01em; }
h2 { font-size: 1.75rem; letter-spacing: 0.01em; }
h3 { font-size: 1.25rem; letter-spacing: 0.01em; }

p {
  max-width: 42em;
  margin-bottom: 1.5em;
}

a {
  color: var(--hygge-secondary);
  text-decoration: underline;
  text-decoration-color: var(--hygge-border);
  text-underline-offset: 3px;
  transition: color 0.2s ease, text-decoration-color 0.2s ease;
}

a:hover {
  color: var(--hygge-primary);
  text-decoration-color: var(--hygge-primary);
}

.container {
  max-width: 780px;
  margin: 0 auto;
  padding: 0 2rem;
}

section {
  padding: 4rem 0;
}

/* Cozy nook -- inset content area */
.hyggekrog {
  background: var(--hygge-surface);
  border-radius: var(--hygge-radius-xl);
  padding: 2.5rem;
  box-shadow: inset 0 2px 20px var(--hygge-glow);
}
```

---

## Design Influences

- **Scandinavian Design** -- clean functionality, natural materials, democratic beauty, and honest simplicity as the structural foundation
- **Wabi-Sabi (via Japandi)** -- appreciation for imperfection, natural aging, and the beauty of well-used objects
- **Arts and Crafts Movement** -- emphasis on handmade quality, natural materials, and the integration of beauty into everyday life
- **Nordic Naturalism** -- the deep Scandinavian connection to nature, seasons, and outdoor landscapes brought indoors
- **Slow Living** -- the broader cultural movement toward mindfulness, intentionality, and prioritizing experience over consumption

---

## Related Aesthetics

- Autumn
- Comfy/Cozy
- Cottagecore
- Japandi
- Minimalism
- Northerness
- Scandi Girl Winter
- Scandinavian Design
- Winter
- Danish Pastel (the brighter, younger counterpart)
- Grandmillennial (shared warmth and textile focus)
- Coastal Style (shared calm, natural palette)

---

## Key Design Values

- **Warmth** -- every visual decision should add warmth; cold, clinical, or sterile elements break the spell entirely
- **Simplicity with soul** -- minimalist in quantity but rich in texture and feeling; not empty, but curated
- **Tactile quality** -- elements should feel like you could reach out and touch them; natural materials, soft textures, gentle shadows
- **Intimacy** -- design for a small gathering, not a stadium; narrow widths, close groupings, personal scale
- **Stillness** -- resist the urge to animate, flash, or demand attention; Hygge design is quiet and patient
- **Sanctuary** -- the user should feel protected and embraced; the interface is a refuge from the noise outside
