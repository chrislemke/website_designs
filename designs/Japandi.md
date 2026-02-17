# Japandi

A design aesthetic born from the union of Japanese minimalism and Scandinavian functionalism. Japandi marries the Nordic concept of "hygge" (cozy contentment) with the Japanese philosophy of "wabi-sabi" (finding beauty in imperfection). The result is a visual language of serene restraint -- warm but uncluttered, minimal but never sterile. Spaces feel intentional and hand-touched: natural materials are left unprocessed, forms are simple but artisanal, and color is drawn from stone, sand, clay, and forest. Japandi rejects ornamentation for its own sake; every element must serve a purpose or embody craftsmanship. It is quieter than Scandinavian design alone and warmer than Japanese minimalism alone -- a middle path that values sustainability, longevity, and meditative calm.

---

## Color Palette

- **Primary palette:** Soft whites, warm beiges, muted taupes, and earthy grays -- the colors of raw linen, unglazed ceramics, light wood, and river stone
- **Warm earth tones:** Sandy beige, oat, warm clay, terracotta, and walnut brown -- grounding colors drawn from natural, unfinished materials
- **Cool neutrals:** Pale gray, charcoal, slate, and gentle blue-gray -- borrowed from Scandinavian restraint, providing balance and quiet contrast
- **Natural accent tones:** Sage green, moss, muted olive, and dusty forest green -- organic greens that suggest bamboo, tea leaves, and indoor plants
- **Overall feel:** Desaturated, tonal, and layered; colors should feel like they exist in soft natural light filtered through rice paper or linen curtains. The 60-30-10 rule applies: 60% dominant neutral, 30% secondary warm or cool neutral, 10% muted accent
- **Contrast strategy:** Deliberate but restrained; dark elements (charcoal, espresso brown) are used for grounding text and structure. Avoid pure black (#000) and pure white (#FFF) -- they are too harsh for this palette. All contrast should feel organic, like dark wood against pale stone

### Suggested CSS Color Tokens

| Role            | Description              | Suggested Value         |
|-----------------|--------------------------|-------------------------|
| Background      | Warm parchment           | `#F4F0E8` / `#FAF6F0`  |
| Surface         | Pale oat                 | `#EDE6DA` / `#E8E0D2`  |
| Surface Alt     | Soft clay                | `#D5CABA` / `#CEC4A7`  |
| Primary         | Warm taupe               | `#9E8B7D` / `#8F837A`  |
| Secondary       | Dark walnut              | `#5B3A29` / `#523A21`  |
| Accent 1        | Sage green               | `#707E57` / `#6B7F5E`  |
| Accent 2        | Muted terracotta         | `#C19E85` / `#CC9A7A`  |
| Accent 3        | Dusty moss               | `#6B6445` / `#7A7652`  |
| Accent 4        | Soft sand                | `#DED5B9` / `#D5B88D`  |
| Accent 5        | Cool stone gray          | `#A4A09A` / `#8E9499`  |
| Text            | Deep charcoal            | `#2C2825` / `#33302D`  |
| Text light      | Warm medium gray         | `#7A7168` / `#8A8078`  |
| Border          | Faded taupe              | `#D4CBBF` / `#C9BFB3`  |

### Extended Palette (Japandi Combinations)

| Combo Name          | Color A     | Color B     | Usage                                   |
|---------------------|-------------|-------------|-----------------------------------------|
| Zen Garden          | `#F4F0E8`   | `#707E57`   | Hero sections, nature-inspired overlays |
| Wabi-Sabi           | `#9E8B7D`   | `#523A21`   | Text on neutral surfaces, grounding     |
| Paper & Ink         | `#FAF6F0`   | `#2C2825`   | High-contrast content, editorial layout |
| Bamboo Grove        | `#EDE6DA`   | `#6B6445`   | Accent pairings, tags, subtle badges    |
| Clay & Stone        | `#C19E85`   | `#A4A09A`   | Warm-cool interplay, card accents       |
| Morning Mist        | `#F4F0E8`   | `#D5CABA`   | Layered backgrounds, tonal depth        |
| Tea Ceremony        | `#DED5B9`   | `#5B3A29`   | CTA elements, active states             |
| Forest Floor        | `#707E57`   | `#6B6445`   | Monochromatic green sections, footers   |

---

## Typography

- **Lettering style:** Clean, minimal, and quietly refined -- the intersection of Scandinavian geometric clarity and Japanese understated elegance. Fonts should feel timeless, not trendy; precise, not cold; humanist, not mechanical
- **Suggested font families:**
  - Display/headings: Geometric or humanist sans-serifs with refined proportions, or clean serifs with Japanese-influenced simplicity (e.g., **Zen Kaku Gothic New**, **Noto Serif Display**, **DM Sans**, **Cormorant Garamond**)
  - Body: Open, readable sans-serifs with warm neutrality and generous x-height (e.g., **Noto Sans JP**, **Work Sans**, **Inter**, **M PLUS 1**)
  - Accent/decorative: For quotes, callouts, or contemplative moments -- refined serifs or light-weight display faces (e.g., **Cormorant**, **EB Garamond**, **Zen Old Mincho** in italic or light weight)
- **Weight usage:** Light to regular for body; medium for headings. Avoid bold or extra-bold weights -- they break the tranquil restraint. Light weights at large sizes convey quiet confidence
- **Sizing:** Generous heading sizes with restrained body text. Line height of 1.6-1.8 for body (spacious, breathing), 1.2-1.3 for headings. The open spacing reflects the Japanese concept of "ma" (negative space as meaningful)
- **Letter spacing:** Slightly open for headings (0.01-0.04em); normal for body text; wide tracking on uppercase labels or small caps (0.1-0.15em) for a deliberate, spaced-out Japanese aesthetic

### Google Fonts Import

```css
@import url('https://fonts.googleapis.com/css2?family=Cormorant+Garamond:ital,wght@0,300;0,400;0,500;1,300;1,400&family=DM+Sans:wght@300;400;500&family=Inter:wght@300;400;500&family=Noto+Serif+Display:wght@300;400;500&family=Work+Sans:wght@300;400;500&display=swap');
```

---

## Visual Characteristics

### Shapes and Forms

- **Clean, straight lines with subtle softening** -- border-radius is minimal (4-8px) rather than the generous rounding of Hygge or Frutiger Aero. Japandi prefers quiet geometry with just enough softness to avoid feeling industrial
- **Deliberate asymmetry** -- inspired by wabi-sabi, layouts and compositions should include subtle, intentional imbalance. A grid offset, an image that bleeds slightly, a heading that does not perfectly center
- **Low-profile forms** -- elements sit quietly, with minimal elevation. Shadows are barely perceptible, suggesting weight rather than floating. Think of objects resting on a wooden surface, not hovering above it
- **Generous negative space ("ma")** -- the Japanese concept of meaningful emptiness is central. Space is not wasted but intentional -- it gives remaining elements room to breathe and significance to exist
- **Horizontal emphasis** -- reflecting the low furniture and grounded proportions of Japanese interiors. Wide, landscape-oriented containers and images feel more Japandi than tall, vertical ones

### Patterns and Textures

- **Wood grain** -- light-toned ash, birch, or hinoki cypress grain at low opacity; warm and organic without overwhelming
- **Ceramic and clay textures** -- the matte, imperfect surface of handmade pottery; subtle noise overlays that suggest unglazed stoneware
- **Washi (Japanese paper)** -- a soft, fibrous paper texture at very low opacity as a background element; organic and handmade
- **Linen weave** -- fine cross-hatch patterns suggesting natural cloth, used sparingly as section backgrounds
- **Sumi ink wash** -- soft, watercolor-like gradients in gray or black at extremely low opacity for atmospheric depth
- **Natural photography** -- raw wood, bamboo, ceramic vessels, stone, dried botanicals, muted indoor plants. Always desaturated and softly lit

### Key Decorative Motifs

- Enso circles (the Zen brushstroke circle -- translate to subtle circular SVG borders or decorative ring elements, intentionally imperfect)
- Indoor plants and dried botanicals (translate to muted green accent elements and organic SVG illustrations)
- Ceramic vessels and handmade pottery (translate to rounded, matte-finished container styles with subtle texture)
- Bamboo and wood (translate to fine-grain CSS pattern backgrounds and warm surface colors)
- Shoji screen grids (translate to thin-bordered grid layouts and translucent overlay panels)
- Ikebana-style asymmetric arrangements (translate to off-center hero images, asymmetric grid placements)
- Tatami mat geometry (translate to modular, proportional grid systems)

---

## Layout Principles

- **"Ma" (negative space as content):** Whitespace is not empty -- it is an active design element. Generous margins, padding, and section spacing create a meditative rhythm. Content should feel like objects carefully placed in a room, not crammed into a shelf
- **Grounded, horizontal composition:** Elements should feel anchored and low. Avoid tall, dramatic hero sections. Prefer wide, calm layouts with landscape-oriented imagery and short section heights that scroll smoothly
- **Restrained grid systems:** Simple, modular grids inspired by tatami proportions. Two- or three-column layouts with clear structure, generous gaps. Avoid complex multi-column magazine layouts -- simplicity is essential
- **Asymmetric balance:** Content need not be perfectly centered or mirrored. A text block offset to the left with an image breathing to the right feels more Japandi than rigid symmetry. The balance is visual, not mathematical
- **Single-focus sections:** Each section should present one idea, one message, one visual. Avoid combining multiple unrelated elements in a single view. The scroll reveals ideas one at a time, like turning pages in a book
- **Functional flow:** Every layout choice should serve navigation and comprehension. Decoration that interferes with function violates both Japanese and Scandinavian principles
- **Narrow to moderate content widths:** 700-900px for text-heavy content; up to 1200px for grid layouts. Never stretch to full viewport width -- contained layouts feel more intentional

---

## CSS / Web Design Techniques

### Minimal Rounded Containers

```css
/* Japandi containers: subtle softening, not pillowy */
.card { border-radius: 6px; }
.button { border-radius: 4px; }
.container { border-radius: 8px; }
.image { border-radius: 4px; }
.tag { border-radius: 3px; }
.input { border-radius: 4px; }
```

### Washi Paper Texture Overlay

```css
.washi-texture {
  position: relative;
}

.washi-texture::after {
  content: '';
  position: absolute;
  inset: 0;
  opacity: 0.025;
  background-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='6' height='6'%3E%3Crect width='1' height='1' x='1' y='0' fill='%237A7168' opacity='0.5'/%3E%3Crect width='1' height='1' x='4' y='3' fill='%237A7168' opacity='0.3'/%3E%3Crect width='1' height='1' x='0' y='5' fill='%237A7168' opacity='0.4'/%3E%3C/svg%3E");
  background-size: 6px 6px;
  pointer-events: none;
}
```

### Barely-There Shadows

```css
/* Shadows should suggest weight, not elevation */
.card-japandi {
  box-shadow:
    0 1px 2px rgba(44, 40, 37, 0.04),
    0 2px 8px rgba(44, 40, 37, 0.03);
}

/* Hover: a slight deepening, not a dramatic lift */
.card-japandi:hover {
  box-shadow:
    0 1px 3px rgba(44, 40, 37, 0.06),
    0 4px 12px rgba(44, 40, 37, 0.04);
  transform: translateY(-1px);
  transition: all 0.3s ease;
}
```

### Sumi Ink Wash Gradient

```css
/* Atmospheric depth inspired by Japanese ink painting */
.sumi-wash {
  background: linear-gradient(
    180deg,
    rgba(44, 40, 37, 0.01) 0%,
    rgba(44, 40, 37, 0.03) 50%,
    rgba(44, 40, 37, 0.01) 100%
  );
}

/* Soft fog effect for section transitions */
.mist-gradient {
  background: linear-gradient(
    180deg,
    #F4F0E8 0%,
    #EDE6DA 40%,
    #D5CABA 100%
  );
}
```

### Shoji Screen Dividers

```css
/* Translucent panel borders inspired by shoji screens */
.shoji-panel {
  border: 1px solid rgba(44, 40, 37, 0.08);
  background: rgba(250, 246, 240, 0.6);
  backdrop-filter: blur(4px);
  border-radius: 4px;
  padding: 2rem;
}

/* Thin, quiet section dividers */
.section-divider {
  height: 1px;
  border: none;
  background: linear-gradient(
    90deg,
    transparent 0%,
    #D4CBBF 30%,
    #D4CBBF 70%,
    transparent 100%
  );
  margin: 5rem auto;
  max-width: 40%;
}

/* Enso-inspired circular divider */
.section-divider-enso {
  border: none;
  height: auto;
  text-align: center;
  margin: 4rem auto;
}

.section-divider-enso::before {
  content: '';
  display: inline-block;
  width: 28px;
  height: 28px;
  border: 1.5px solid #9E8B7D;
  border-radius: 50%;
  opacity: 0.4;
  border-top-color: transparent; /* Imperfect circle -- wabi-sabi */
  transform: rotate(-30deg);
}
```

### Tatami Grid Layout

```css
/* Modular grid inspired by tatami mat proportions (1:2 ratio) */
.tatami-grid {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 1.5rem;
}

.tatami-grid .item-wide {
  grid-column: span 2;
}

/* Asymmetric two-column layout */
.japandi-split {
  display: grid;
  grid-template-columns: 2fr 3fr;
  gap: 3rem;
  align-items: start;
}

@media (max-width: 768px) {
  .tatami-grid {
    grid-template-columns: 1fr;
  }

  .japandi-split {
    grid-template-columns: 1fr;
    gap: 2rem;
  }
}
```

### Warm Neutral Gradient Backgrounds

```css
/* Stone garden -- warm neutral layering */
.gradient-stone {
  background: linear-gradient(
    180deg,
    #F4F0E8 0%,
    #EDE6DA 50%,
    #D5CABA 100%
  );
}

/* Morning light -- subtle warm wash */
.gradient-morning {
  background: linear-gradient(
    160deg,
    #FAF6F0 0%,
    #F4F0E8 40%,
    rgba(193, 158, 133, 0.08) 100%
  );
}

/* Forest breath -- green undertone */
.gradient-forest {
  background: linear-gradient(
    170deg,
    #F4F0E8 0%,
    rgba(112, 126, 87, 0.06) 50%,
    #EDE6DA 100%
  );
}
```

### Buttons

```css
/* Primary -- understated and functional */
.btn-japandi {
  background: #2C2825;
  color: #F4F0E8;
  border: none;
  border-radius: 4px;
  padding: 12px 28px;
  font-family: 'DM Sans', 'Work Sans', sans-serif;
  font-weight: 400;
  font-size: 0.9rem;
  letter-spacing: 0.06em;
  text-transform: uppercase;
  cursor: pointer;
  transition: all 0.25s ease;
}

.btn-japandi:hover {
  background: #5B3A29;
  box-shadow: 0 2px 8px rgba(44, 40, 37, 0.12);
}

/* Secondary -- minimal outline */
.btn-japandi-secondary {
  background: transparent;
  color: #2C2825;
  border: 1px solid #D4CBBF;
  border-radius: 4px;
  padding: 11px 27px;
  font-family: 'DM Sans', 'Work Sans', sans-serif;
  font-weight: 400;
  font-size: 0.9rem;
  letter-spacing: 0.06em;
  text-transform: uppercase;
  cursor: pointer;
  transition: all 0.25s ease;
}

.btn-japandi-secondary:hover {
  border-color: #9E8B7D;
  background: rgba(237, 230, 218, 0.5);
}
```

### Input Fields

```css
.input-japandi {
  background: #FAF6F0;
  border: 1px solid #D4CBBF;
  border-radius: 4px;
  padding: 12px 16px;
  font-family: 'Work Sans', 'Inter', sans-serif;
  font-size: 0.95rem;
  color: #2C2825;
  transition: all 0.25s ease;
}

.input-japandi:focus {
  outline: none;
  border-color: #9E8B7D;
  background: #FFFFFF;
  box-shadow: 0 0 0 3px rgba(158, 139, 125, 0.08);
}

.input-japandi::placeholder {
  color: #A4A09A;
  letter-spacing: 0.02em;
}
```

### Enso Circle Decorative Element

```css
/* Zen brushstroke circle -- pure CSS */
.enso {
  width: 120px;
  height: 120px;
  border: 2px solid #9E8B7D;
  border-radius: 50%;
  border-top-width: 1px;
  border-right-width: 3px;
  border-bottom-width: 2px;
  border-left-width: 1px;
  opacity: 0.3;
  transform: rotate(15deg);
}

/* Smaller inline enso */
.enso-sm {
  width: 40px;
  height: 40px;
  border: 1.5px solid #9E8B7D;
  border-radius: 50%;
  border-top-color: transparent;
  opacity: 0.25;
  display: inline-block;
  transform: rotate(-20deg);
}
```

### Full Page Scaffold

```css
:root {
  --japandi-bg: #F4F0E8;
  --japandi-surface: #EDE6DA;
  --japandi-surface-alt: #D5CABA;
  --japandi-primary: #9E8B7D;
  --japandi-secondary: #5B3A29;
  --japandi-accent-sage: #707E57;
  --japandi-accent-terra: #C19E85;
  --japandi-accent-moss: #6B6445;
  --japandi-accent-sand: #DED5B9;
  --japandi-accent-stone: #A4A09A;
  --japandi-text: #2C2825;
  --japandi-text-light: #7A7168;
  --japandi-border: #D4CBBF;
  --japandi-radius-sm: 3px;
  --japandi-radius-md: 4px;
  --japandi-radius-lg: 6px;
  --japandi-radius-xl: 8px;
}

* {
  box-sizing: border-box;
}

body {
  font-family: 'Work Sans', 'Inter', sans-serif;
  background-color: var(--japandi-bg);
  color: var(--japandi-text);
  line-height: 1.7;
  margin: 0;
  -webkit-font-smoothing: antialiased;
}

h1, h2, h3 {
  font-family: 'Noto Serif Display', 'Cormorant Garamond', serif;
  font-weight: 400;
  line-height: 1.25;
  color: var(--japandi-text);
}

h1 { font-size: 2.75rem; letter-spacing: -0.01em; font-weight: 300; }
h2 { font-size: 1.75rem; letter-spacing: 0.01em; }
h3 { font-size: 1.2rem; letter-spacing: 0.02em; }

p {
  max-width: 40em;
  margin-bottom: 1.6em;
}

a {
  color: var(--japandi-secondary);
  text-decoration: underline;
  text-decoration-color: var(--japandi-border);
  text-underline-offset: 3px;
  transition: color 0.2s ease, text-decoration-color 0.2s ease;
}

a:hover {
  color: var(--japandi-accent-moss);
  text-decoration-color: var(--japandi-accent-moss);
}

.container {
  max-width: 860px;
  margin: 0 auto;
  padding: 0 2rem;
}

section {
  padding: 5rem 0;
}

/* Tokonoma -- a featured display alcove */
.tokonoma {
  background: var(--japandi-surface);
  border-radius: var(--japandi-radius-xl);
  border: 1px solid var(--japandi-border);
  padding: 3rem;
}

/* Wide label style */
.label-japandi {
  font-family: 'DM Sans', sans-serif;
  font-size: 0.7rem;
  font-weight: 500;
  letter-spacing: 0.14em;
  text-transform: uppercase;
  color: var(--japandi-text-light);
}
```

---

## Design Influences

- **Wabi-Sabi** -- the Japanese philosophy of finding beauty in imperfection, transience, and incompleteness; the foundation of Japandi's embrace of handmade irregularity and natural aging
- **Scandinavian Design** -- functional minimalism, democratic simplicity, and the belief that beautiful design should be accessible and purposeful
- **Mingei (Japanese Folk Art)** -- the beauty of ordinary, utilitarian objects made by anonymous craftspeople; function and craft as art
- **Bauhaus** -- the shared emphasis on form following function, and the integration of craft and design, filtered through a warmer, more organic lens
- **Zen Buddhism** -- meditative emptiness, deliberate simplicity, and the intentional use of space as a spiritual practice
- **Slow Living Movement** -- mindful consumption, sustainability, and the prioritization of longevity over disposability

---

## Related Aesthetics

- Hygge
- Minimalism
- Scandinavian Design
- Wabi-Sabi
- Modernism
- Rustic
- Maillard Style
- Technozen
- Earth Tones
- Craftcore
- Coastal Style (shared calm, natural palette)
- Danish Pastel (the brighter Scandinavian counterpart)
- Grandmillennial (shared appreciation for craft and heritage)

---

## Key Design Values

- **Intentionality** -- every element earns its place; nothing is decorative without function, nothing is functional without care. If it does not serve the user or embody craft, remove it
- **Imperfect beauty** -- resist the urge to polish everything to machine perfection. Slight irregularities, handmade textures, and organic asymmetry convey authenticity and humanity
- **Meaningful emptiness** -- negative space ("ma") is not wasted space. It is the pause between notes that gives music meaning. Let elements breathe, let sections rest, let the eye find calm
- **Material honesty** -- textures, colors, and forms should reference natural materials without artifice. Wood looks like wood, stone like stone. No glossy fakes, no excessive gradients
- **Sustainability in design** -- choose lasting over trendy. Japandi design should age gracefully; avoid techniques or color trends that will feel dated in a year
- **Quiet confidence** -- this aesthetic does not shout. It invites. It whispers. Typography is light, animations are slow or absent, and the loudest statement is the quality of the craft
