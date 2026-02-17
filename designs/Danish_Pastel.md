# Danish Pastel

A Gen Z interior-turned-graphic-design aesthetic characterized by brightly-colored pastels set against clean white backgrounds, asymmetrical decorations, bold color combinations, and eye-catching patterns. Rooted in Scandinavian design sensibility but rejecting 2010s minimalism in favor of joyful maximalism. Often described as "Scandinavian meets 70s psychedelics" or "grown-up Barbie." The style draws inspiration from modern art that emphasizes shapes in flat colors, particularly the work of Matisse and Picasso.

---

## Color Palette

- **Primary palette:** Soft sage green, dusty rose/pink, pale sky blue, muted lavender, soft butter yellow
- **Background tones:** Clean white or warm off-white -- the hallmark "naturally lit white room" backdrop
- **Overall feel:** Neon pastels -- brighter and more saturated than typical Scandi pastels, but still soft and approachable
- **Contrast strategy:** Pastel elements pop against dominant white space; bold pastel-on-pastel combinations (e.g., pink + lavender, yellow + blue) create playful tension without visual harshness

### Suggested CSS Color Tokens

| Role            | Description          | Suggested Value         |
|-----------------|----------------------|-------------------------|
| Background      | Clean white          | `#FFFFFF` / `#FBF9F7`  |
| Surface         | Warm off-white       | `#F5F0EB` / `#FAF7F4`  |
| Primary         | Dusty rose           | `#EBCAD5` / `#F2D1DC`  |
| Secondary       | Pale sky blue        | `#CEE5ED` / `#B8DAE9`  |
| Accent 1        | Soft sage green      | `#ADD0B3` / `#B8D9BE`  |
| Accent 2        | Muted lavender       | `#807DBB` / `#A7A4D0`  |
| Accent 3        | Soft butter yellow   | `#FBF38A` / `#F9EFA0`  |
| Accent 4        | Peach / coral pink   | `#F9DED7` / `#F5C4B8`  |
| Accent 5        | Mauve                | `#E2BEF1` / `#D4A8E8`  |
| Text            | Soft charcoal        | `#3A3A3A` / `#4A4A4A`  |
| Text light      | Medium gray          | `#7A7A7A` / `#9A9A9A`  |

### Extended Palette (Danish Pastel Combinations)

| Combo Name         | Color A     | Color B     | Usage                              |
|--------------------|-------------|-------------|------------------------------------|
| Pink + Lavender    | `#EBCAD5`   | `#807DBB`   | Checkerboard, hero sections        |
| Yellow + Blue      | `#FBF38A`   | `#CEE5ED`   | Accent pairings, cards             |
| Sage + Rose        | `#ADD0B3`   | `#EBCAD5`   | Backgrounds, gradient washes       |
| Peach + Mauve      | `#F9DED7`   | `#E2BEF1`   | Soft gradient overlays             |
| Lavender + Yellow  | `#A7A4D0`   | `#FBF38A`   | Bold accent moments                |

---

## Typography

- **Lettering style:** Rounded, friendly, and organic -- softness is key; avoid rigid, angular, or corporate typefaces
- **Suggested font families:**
  - Display/headings: Rounded sans-serifs with generous curves (e.g., **Quicksand**, **Comfortaa**, **Nunito**, **Fredoka One**)
  - Body: Clean, geometric sans-serifs with soft character (e.g., **Poppins**, **DM Sans**, **Nunito Sans**, **Work Sans**)
  - Accent/decorative: For playful callouts or quotes, retro-inspired or hand-drawn faces (e.g., **Shrikhand**, **Baloo 2**, **Pacifico**)
- **Weight usage:** Bold to extra-bold for headings; regular or medium for body; light weights for large display text to maintain airiness
- **Sizing:** Generous scale; large headings with comfortable line height (1.4-1.6 for body, 1.1-1.2 for headings)
- **Letter spacing:** Slightly open for headings; normal for body text

### Google Fonts Import

```css
@import url('https://fonts.googleapis.com/css2?family=Quicksand:wght@400;500;600;700&family=Nunito:wght@300;400;600;700&family=Comfortaa:wght@400;500;700&family=Poppins:wght@300;400;500;600&display=swap');
```

---

## Visual Characteristics

### Shapes and Forms

- **Organic, curvy shapes** dominate -- blob mirrors, wavy lines, and irregular rounded forms
- **Generous border-radius** on all elements; nothing should feel sharp or angular
- **Asymmetry** is preferred over rigid symmetry; balance is achieved through color weight rather than alignment
- **Matisse-inspired cutout shapes** -- flat-color organic forms that feel art-directed and joyful
- **Sculptural quality** -- elements should feel three-dimensional and tactile, like the novelty candles and ceramic dishes central to the aesthetic

### Patterns and Textures

- **Checkerboard / wavy checkerboard** -- the signature pattern; standard or distorted with wavy, psychedelic 70s-inspired warping
- **Hearts** -- Powerpuff Girls-inspired, sweet and romantic
- **Wavy lines and squiggly borders** -- used as dividers, decorative accents, and frame elements
- **Floral motifs** -- simple, flat-color flowers in pastel tones
- **Argyle** -- classic diamond pattern rendered in pastel combinations
- **Stars and sparkles** -- small decorative accents scattered as visual seasoning
- **Subtle gradients** -- pastel-to-pastel washes that feel like watercolor

### Key Decorative Motifs

- Curvy blob-shaped mirrors (translate to irregular containers or image frames)
- Novelty candle forms (translate to sculptural, organic UI elements)
- Pastel posters and gallery arrangements (translate to card grids with varied content)
- Faux leaf garlands and flowers (translate to organic decorative SVG elements)
- Pastel plastic milk-crate bins (translate to grid containers with visible structure)

---

## Layout Principles

- **Maximalist but curated:** Many visual elements, but each placed with intention; the space should feel full and joyful, not chaotic
- **White space as canvas:** White backgrounds are essential -- they let the pastel elements breathe and create the "naturally lit white room" feeling
- **Collections and groupings:** Photography and content should be arranged as pleasing color-palette collections rather than isolated items
- **Asymmetric balance:** Avoid rigid grid symmetry; balance through color weight, visual density, and organic placement
- **Layered composition:** Elements can overlap and stack to create depth, as in a curated shelf display
- **Mixed scales:** Use the same colors and patterns at different sizes to build cohesion across the layout
- **Soft containment:** Sections and cards should feel like gentle containers, not hard boxes

---

## CSS / Web Design Techniques

### Border Radius and Soft Shapes

```css
/* Everything is soft and rounded */
.card { border-radius: 24px; }
.button { border-radius: 999px; } /* pill shape */
.container { border-radius: 20px; }
.image { border-radius: 16px; }
.tag { border-radius: 12px; }
```

### Checkerboard Pattern (Standard)

```css
.checkerboard {
  background-image:
    linear-gradient(45deg, #EBCAD5 25%, transparent 25%),
    linear-gradient(-45deg, #EBCAD5 25%, transparent 25%),
    linear-gradient(45deg, transparent 75%, #EBCAD5 75%),
    linear-gradient(-45deg, transparent 75%, #EBCAD5 75%);
  background-size: 40px 40px;
  background-position: 0 0, 0 20px, 20px -20px, -20px 0;
  background-color: #FBF9F7;
}
```

### Wavy Checkerboard Pattern (SVG Filter)

```css
.wavy-checkerboard {
  background-image:
    linear-gradient(45deg, #A7A4D0 25%, transparent 25%),
    linear-gradient(-45deg, #A7A4D0 25%, transparent 25%),
    linear-gradient(45deg, transparent 75%, #A7A4D0 75%),
    linear-gradient(-45deg, transparent 75%, #A7A4D0 75%);
  background-size: 30px 30px;
  background-position: 0 0, 0 15px, 15px -15px, -15px 0;
  background-color: #F2D1DC;
  filter: url(#wavy-distort); /* Apply SVG turbulence filter for warping */
}

/* Pair with inline SVG filter: */
/*
<svg width="0" height="0">
  <filter id="wavy-distort">
    <feTurbulence type="turbulence" baseFrequency="0.015" numOctaves="3" result="turbulence"/>
    <feDisplacementMap in="SourceGraphic" in2="turbulence" scale="15" xChannelSelector="R" yChannelSelector="G"/>
  </filter>
</svg>
*/
```

### Blob / Organic Shapes

```css
.blob {
  border-radius: 60% 40% 55% 45% / 50% 65% 35% 55%;
  /* Irregular border-radius creates curvy mirror-like shapes */
}

.blob-alt {
  border-radius: 42% 58% 70% 30% / 45% 45% 55% 55%;
}

/* Animated blob that subtly morphs */
@keyframes blob-morph {
  0%, 100% { border-radius: 60% 40% 55% 45% / 50% 65% 35% 55%; }
  25%      { border-radius: 45% 55% 40% 60% / 60% 40% 55% 45%; }
  50%      { border-radius: 55% 45% 60% 40% / 45% 55% 45% 55%; }
  75%      { border-radius: 40% 60% 45% 55% / 55% 45% 60% 40%; }
}

.blob-animated {
  animation: blob-morph 8s ease-in-out infinite;
}
```

### Wavy Section Dividers

```css
.wavy-divider {
  position: relative;
  overflow: hidden;
}

.wavy-divider::after {
  content: '';
  position: absolute;
  bottom: -2px;
  left: 0;
  width: 100%;
  height: 60px;
  background: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 1200 120'%3E%3Cpath d='M0,60 C200,120 400,0 600,60 C800,120 1000,0 1200,60 L1200,120 L0,120 Z' fill='%23FFFFFF'/%3E%3C/svg%3E") no-repeat;
  background-size: cover;
}
```

### Soft Shadows and Glows

```css
/* Pastel-tinted shadows instead of gray */
.card-pink {
  box-shadow: 0 8px 30px rgba(235, 202, 213, 0.35);
}

.card-blue {
  box-shadow: 0 8px 30px rgba(206, 229, 237, 0.4);
}

.card-lavender {
  box-shadow: 0 8px 30px rgba(128, 125, 187, 0.2);
}

/* Gentle hover lift */
.card:hover {
  transform: translateY(-4px);
  box-shadow: 0 12px 40px rgba(235, 202, 213, 0.45);
  transition: all 0.3s ease;
}
```

### Pastel Gradients

```css
/* Sage to rose gradient */
.gradient-sage-rose {
  background: linear-gradient(135deg, #ADD0B3 0%, #EBCAD5 100%);
}

/* Blue to lavender to peach */
.gradient-sky-sunset {
  background: linear-gradient(135deg, #CEE5ED 0%, #A7A4D0 50%, #F9DED7 100%);
}

/* Subtle background wash */
.gradient-subtle {
  background: linear-gradient(180deg, #FBF9F7 0%, #F2D1DC08 50%, #FBF9F7 100%);
}
```

### Heart Pattern (CSS)

```css
.hearts-pattern {
  background-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='40' height='40' viewBox='0 0 40 40'%3E%3Cpath d='M20,35 L3,18 C-2,12 3,4 10,4 C14,4 18,7 20,11 C22,7 26,4 30,4 C37,4 42,12 37,18 Z' fill='%23EBCAD5' opacity='0.3'/%3E%3C/svg%3E");
  background-size: 60px 60px;
}
```

### Squiggly Line Border

```css
.squiggly-border {
  border-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='200' height='10' viewBox='0 0 200 10'%3E%3Cpath d='M0,5 Q10,0 20,5 Q30,10 40,5 Q50,0 60,5 Q70,10 80,5 Q90,0 100,5 Q110,10 120,5 Q130,0 140,5 Q150,10 160,5 Q170,0 180,5 Q190,10 200,5' stroke='%23807DBB' fill='none' stroke-width='2'/%3E%3C/svg%3E") 0 0 10 0 / 0 0 10px 0 repeat;
}
```

### Star / Sparkle Decorations

```css
.sparkle::before,
.sparkle::after {
  content: '\2726'; /* four-pointed star */
  position: absolute;
  color: #FBF38A;
  font-size: 1.2rem;
  opacity: 0.7;
}

.sparkle::before { top: -8px; right: -8px; }
.sparkle::after { bottom: -8px; left: -8px; font-size: 0.8rem; }
```

### Full Page Scaffold

```css
:root {
  --dp-white: #FFFFFF;
  --dp-off-white: #FBF9F7;
  --dp-rose: #EBCAD5;
  --dp-blue: #CEE5ED;
  --dp-sage: #ADD0B3;
  --dp-lavender: #807DBB;
  --dp-yellow: #FBF38A;
  --dp-peach: #F9DED7;
  --dp-mauve: #E2BEF1;
  --dp-text: #3A3A3A;
  --dp-text-light: #7A7A7A;
  --dp-radius-sm: 12px;
  --dp-radius-md: 20px;
  --dp-radius-lg: 24px;
  --dp-radius-pill: 999px;
}

body {
  font-family: 'Poppins', 'Nunito Sans', sans-serif;
  background-color: var(--dp-off-white);
  color: var(--dp-text);
  line-height: 1.6;
}

h1, h2, h3 {
  font-family: 'Quicksand', 'Comfortaa', sans-serif;
  font-weight: 700;
  line-height: 1.2;
}
```

---

## Design Influences

- **Scandinavian Design** -- the structural foundation: clean lines, functional forms, white-dominant spaces, and natural light
- **Matisse and Picasso** -- flat-color modern art with bold shapes; organic cutouts and simplified forms
- **1970s Psychedelia** -- wavy distortions, warped checkerboards, flowing organic patterns
- **IKEA and JYSK** -- accessible Scandinavian design retail; practical items elevated through color and shape
- **Gen Z Maximalism** -- the cultural rejection of millennial minimalism; more is more, done with intention and joy

---

## Related Aesthetics

- Avant Basic
- Cottagecore
- Dopamine (Dopamine Dressing)
- Plant Mom
- Scandinavian Design
- Kidcore
- Gen Z Maximalism
- Indie Kid
- Psychedelia

---

## Key Design Values

- **Joyfulness** -- every element should feel cheerful, approachable, and uplifting
- **Playful maximalism** -- embrace visual abundance with curation and intention, not chaos
- **Asymmetric beauty** -- imperfection and organic irregularity are preferred over rigid order
- **Bold combinations** -- pair pastels fearlessly; pink next to lavender, yellow next to blue
- **Sculptural sensibility** -- elements should feel tactile and dimensional, like handmade ceramics or novelty candles
- **Curated collection** -- the overall composition should feel like a carefully arranged shelf of beautiful objects
