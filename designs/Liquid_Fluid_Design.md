# Liquid / Fluid Design Reference

Liquid / Fluid Design is an organic, nature-inspired aesthetic built around blob shapes, flowing curves, amorphous forms, and soft undulating surfaces. It emerged as a counter-movement to the rigid geometry and sharp edges of Flat Design and Material Design, gaining significant momentum around 2017 when designers began anchoring landing pages with pseudo-organic SVG shapes. The aesthetic draws on the physics of liquids -- surface tension, viscosity, and flow -- to create interfaces that feel human, warm, and alive. Unlike the mechanical precision of grid-based layouts, Liquid Design embraces irregularity, asymmetry, and gentle motion, producing digital experiences that breathe and shift like living organisms. In web and UI design, this translates to gradient-filled blob backgrounds, soft rounded containers, morphing SVG animations, layered translucent shapes, and an overall sense of calm fluidity that invites exploration rather than commanding attention.

---

## Visual Characteristics

### Core Design Traits

- **Organic blob shapes** -- amorphous, pseudo-random vector forms with smooth curves and no sharp corners, used as backgrounds, masks, and decorative elements
- **Flowing gradient fills** -- soft, multi-stop gradients that blend harmoniously, often with pastel or muted tones transitioning gently across surfaces
- **Layered translucent forms** -- semi-transparent blobs and shapes stacked at varying opacities to create depth and atmospheric perspective
- **Soft shadows and diffused edges** -- large-radius, low-opacity box shadows that make elements appear to float gently rather than sit rigidly on a surface
- **Undulating borders** -- containers and sections with wavy, irregular edges instead of straight lines, created via SVG paths or complex border-radius values
- **Morphing animations** -- subtle, slow shape transformations where blobs continuously shift their contours, suggesting liquid in gentle motion
- **Rounded corners everywhere** -- generous border-radius values on cards, buttons, inputs, and containers, reinforcing the soft organic feel
- **Asymmetric compositions** -- layouts that deliberately avoid perfect symmetry, allowing visual weight to flow naturally across the page
- **Nature-inspired imagery** -- references to water, clouds, lava lamps, soap bubbles, and biological forms like cells and amoebae
- **Generous whitespace** -- ample breathing room between elements, letting organic shapes and gradients take visual precedence

### Design Principles

- Embrace organic irregularity -- nothing in nature is perfectly geometric, and neither should liquid interfaces be
- Build warmth through soft gradients: gentle color transitions evoke calmness, trust, and approachability
- Use motion sparingly and slowly -- liquid animations should be meditative, never frantic or jarring
- Create depth through layered transparency rather than hard borders or dramatic shadows
- Let negative space breathe -- the emptiness between blobs is as important as the blobs themselves
- Every shape should feel like it could plausibly exist in nature: a droplet, a cloud, an amoeba
- Color transitions should be smooth and barely perceptible, like watercolor bleeding into wet paper
- Contrast comes from shape and color, not from hard edges -- softness is the defining characteristic
- Balance organic freedom with functional clarity -- decorative blobs must never obscure content or navigation

---

## Color Palette

### Soft Gradient Palette

| Color Name | Hex | Role / Usage |
|------------|-----|-------------|
| **Lavender Mist** | `#C3B1E1` | Primary accent, blob fills, hero gradients |
| **Rose Quartz** | `#F7CAC9` | Secondary accent, warm blob overlays |
| **Soft Coral** | `#FF8A80` | CTA highlights, active states, warm emphasis |
| **Peach Cream** | `#FFDAB9` | Warm gradient endpoint, card backgrounds |
| **Sky Wash** | `#A8D8EA` | Cool accent, secondary blob fills, link color |
| **Mint Foam** | `#B5EAD7` | Success states, fresh accent, cool blobs |
| **Lilac Dream** | `#DCD0FF` | Light decorative blobs, hover states |
| **Ocean Depth** | `#5B7FFF` | Primary interactive color, buttons, links |
| **Warm Violet** | `#9B6DFF` | Gradient midpoint, decorative emphasis |
| **Cloud White** | `#F8F6FF` | Primary background, lightest surface |
| **Soft Ivory** | `#FFF8F0` | Alternate background, warm variant |
| **Mist Gray** | `#E8E4EF` | Borders, dividers, subtle separation |
| **Deep Ink** | `#2D2B55` | Primary text, headings, high contrast |
| **Slate Muted** | `#6B6B8D` | Secondary text, captions, labels |

### CSS Custom Properties

```css
:root {
  /* Primary accents */
  --liquid-lavender: #c3b1e1;
  --liquid-rose: #f7cac9;
  --liquid-coral: #ff8a80;
  --liquid-peach: #ffdab9;

  /* Cool accents */
  --liquid-sky: #a8d8ea;
  --liquid-mint: #b5ead7;
  --liquid-lilac: #dcd0ff;

  /* Interactive colors */
  --liquid-ocean: #5b7fff;
  --liquid-violet: #9b6dff;

  /* Backgrounds */
  --liquid-bg-cloud: #f8f6ff;
  --liquid-bg-ivory: #fff8f0;
  --liquid-bg-mist: #e8e4ef;

  /* Text */
  --liquid-text-primary: #2d2b55;
  --liquid-text-secondary: #6b6b8d;

  /* Gradients */
  --liquid-gradient-warm: linear-gradient(135deg, #f7cac9 0%, #c3b1e1 50%, #a8d8ea 100%);
  --liquid-gradient-cool: linear-gradient(135deg, #a8d8ea 0%, #dcd0ff 50%, #c3b1e1 100%);
  --liquid-gradient-sunset: linear-gradient(135deg, #ffdab9 0%, #ff8a80 30%, #c3b1e1 70%, #a8d8ea 100%);
  --liquid-gradient-ocean: linear-gradient(135deg, #5b7fff 0%, #9b6dff 50%, #c3b1e1 100%);

  /* Shadows */
  --liquid-shadow-soft: 0 8px 32px rgba(45, 43, 85, 0.08);
  --liquid-shadow-elevated: 0 16px 48px rgba(45, 43, 85, 0.12);
  --liquid-shadow-blob: 0 20px 60px rgba(195, 177, 225, 0.3);
}
```

---

## Typography

### Typeface Characteristics

Liquid / Fluid Design typography is:

- **Soft and rounded** -- letterforms with rounded terminals and gentle curves that complement the organic shapes
- **Medium weight preferred** -- neither too thin (fragile) nor too bold (aggressive); a balanced, approachable weight
- **Generous letter-spacing** -- slightly open tracking that gives text room to breathe within flowing layouts
- **Mixed case for warmth** -- sentence case or title case rather than all-caps, which feels too rigid for this aesthetic
- **Clean sans-serifs** -- geometric or humanist sans-serif faces that avoid sharp angles and harsh terminals
- **Rounded display faces for headlines** -- fonts with visibly rounded strokes and soft geometry for maximum organic feel

### Recommended Web Fonts (Google Fonts)

| Font | Style | Best For |
|------|-------|----------|
| **Nunito** | Rounded geometric sans | Headlines, body text, versatile organic feel |
| **Comfortaa** | Rounded geometric | Headlines, logos, display text |
| **Quicksand** | Rounded geometric sans | Body text, subheadings, friendly tone |
| **Poppins** | Geometric sans | Headlines, body text, modern clean |
| **DM Sans** | Geometric humanist | Body text, UI elements, readability |
| **Outfit** | Modern geometric | Subheadings, body text, contemporary |
| **Varela Round** | Rounded grotesque | Headlines, navigation, soft branding |
| **Lexend** | Optimized reading | Long-form body text, accessibility focus |
| **Baloo 2** | Rounded heavy display | Large display text, playful headers |
| **Rubik** | Rounded corners neo-grotesque | Headlines, body text, balanced warmth |

### Font Pairing Suggestions

| Heading Font | Body Font | Character |
|-------------|-----------|-----------|
| **Comfortaa** (700) | **Quicksand** (400) | Maximum organic softness, playful warmth |
| **Nunito** (800) | **DM Sans** (400) | Balanced rounded heads, clean readable body |
| **Poppins** (600) | **Outfit** (400) | Modern and geometric, professional fluidity |
| **Varela Round** (400) | **Lexend** (400) | Soft branding headers, optimized body reading |
| **Baloo 2** (700) | **Nunito** (400) | Playful display impact, versatile body text |

### Typography CSS Example

```css
/* Import fonts */
@import url('https://fonts.googleapis.com/css2?family=Comfortaa:wght@400;600;700&family=Quicksand:wght@400;500;600&display=swap');

/* Headings */
h1, h2, h3, h4, h5, h6 {
  font-family: 'Comfortaa', cursive;
  font-weight: 700;
  color: var(--liquid-text-primary);
  letter-spacing: 0.01em;
  line-height: 1.25;
}

/* Display / Hero text with gradient fill */
.liquid-display {
  font-family: 'Comfortaa', cursive;
  font-size: clamp(2.5rem, 6vw, 5rem);
  font-weight: 700;
  letter-spacing: -0.01em;
  background: var(--liquid-gradient-ocean);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  background-clip: text;
  line-height: 1.15;
}

/* Soft subtitle */
.liquid-subtitle {
  font-family: 'Quicksand', sans-serif;
  font-size: 1.25rem;
  font-weight: 500;
  color: var(--liquid-text-secondary);
  letter-spacing: 0.02em;
  line-height: 1.6;
}

/* Body text */
body {
  font-family: 'Quicksand', sans-serif;
  font-weight: 400;
  font-size: 1rem;
  line-height: 1.75;
  color: var(--liquid-text-primary);
}

/* Labels and captions */
.liquid-label {
  font-family: 'Quicksand', sans-serif;
  font-size: 0.8rem;
  font-weight: 600;
  letter-spacing: 0.08em;
  text-transform: uppercase;
  color: var(--liquid-text-secondary);
}
```

---

## Layout Principles

### Grid and Structure

- **Soft-edged full-width sections** -- sections span the viewport but use wavy SVG dividers or blob overlaps instead of hard horizontal lines
- **Medium-width content containers** -- body content at 1000-1200px max-width, centered with generous padding
- **Asymmetric blob placement** -- large decorative blobs positioned off-center, partially overflowing section boundaries to break rigidity
- **Overlapping layers** -- translucent blob shapes that cross section boundaries, creating visual continuity between areas
- **Fluid column layouts** -- CSS grid or flexbox with soft gaps (24-48px), columns that feel loosely arranged rather than rigidly snapped
- **Generous vertical rhythm** -- large padding between sections (100-160px), giving each area breathing room
- **Floating elements** -- cards and content blocks that appear to hover via soft shadows, disconnected from any visible grid

### Section Organization

- **Navigation**: Clean, minimal bar with rounded pill-shaped links or a floating rounded navbar with subtle backdrop blur
- **Hero**: Large gradient background with layered decorative blobs, centered headline with gradient text, soft rounded CTA button
- **Features**: Cards with large border-radius, soft shadows, optional blob-shaped icon backgrounds
- **Content rows**: Alternating text-and-visual pairs with blob-shaped image masks or frames
- **Testimonials**: Rounded cards with soft gradients, avatar images in circular frames
- **CTA section**: Gradient blob background with centered text and prominent rounded button
- **Footer**: Wavy top edge via SVG, soft muted background, rounded link groups

### Responsive Approach

- Maintain blob decorations at all breakpoints but scale them proportionally and reduce quantity on mobile
- Use `clamp()` extensively for typography, padding, and blob sizes to ensure smooth scaling
- Stack cards and content blocks vertically on mobile; maintain rounded corners and soft shadows
- Simplify SVG blob animations on mobile for performance -- reduce morph keyframes or use static shapes
- Keep generous whitespace even on small screens; resist the temptation to pack elements tightly

---

## CSS / Design Techniques

### Liquid Card Component

```css
.liquid-card {
  background: rgba(255, 255, 255, 0.8);
  backdrop-filter: blur(10px);
  -webkit-backdrop-filter: blur(10px);
  border: 1px solid rgba(195, 177, 225, 0.2);
  border-radius: 24px;
  padding: 36px;
  position: relative;
  transition: transform 0.4s ease, box-shadow 0.4s ease;
  box-shadow: var(--liquid-shadow-soft);
  overflow: hidden;
}

.liquid-card:hover {
  transform: translateY(-4px);
  box-shadow: var(--liquid-shadow-elevated);
}

/* Decorative blob accent in corner */
.liquid-card::before {
  content: '';
  position: absolute;
  top: -30px;
  right: -30px;
  width: 120px;
  height: 120px;
  border-radius: 60% 40% 50% 50% / 50% 60% 40% 50%;
  background: var(--liquid-gradient-warm);
  opacity: 0.15;
  z-index: 0;
  transition: opacity 0.4s ease;
}

.liquid-card:hover::before {
  opacity: 0.25;
}

/* Card grid */
.liquid-card-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
  gap: 32px;
}
```

### Liquid Button

```css
.liquid-button {
  display: inline-flex;
  align-items: center;
  justify-content: center;
  background: var(--liquid-gradient-ocean);
  color: #ffffff;
  border: none;
  border-radius: 50px;
  padding: 16px 40px;
  font-family: 'Quicksand', sans-serif;
  font-size: 0.95rem;
  font-weight: 600;
  letter-spacing: 0.02em;
  cursor: pointer;
  transition: transform 0.3s ease, box-shadow 0.3s ease;
  text-decoration: none;
  box-shadow: 0 4px 20px rgba(91, 127, 255, 0.3);
}

.liquid-button:hover {
  transform: translateY(-2px) scale(1.02);
  box-shadow: 0 8px 30px rgba(91, 127, 255, 0.4);
}

.liquid-button:active {
  transform: translateY(0) scale(0.98);
}

/* Soft outlined variant */
.liquid-button--outline {
  background: transparent;
  color: var(--liquid-ocean);
  border: 2px solid var(--liquid-ocean);
  box-shadow: none;
}

.liquid-button--outline:hover {
  background: var(--liquid-ocean);
  color: #ffffff;
  box-shadow: 0 8px 30px rgba(91, 127, 255, 0.3);
}

/* Pastel variant */
.liquid-button--pastel {
  background: var(--liquid-gradient-warm);
  color: var(--liquid-text-primary);
  box-shadow: 0 4px 20px rgba(195, 177, 225, 0.3);
}

.liquid-button--pastel:hover {
  box-shadow: 0 8px 30px rgba(195, 177, 225, 0.4);
}
```

### Navigation Bar

```css
.liquid-nav {
  display: flex;
  align-items: center;
  justify-content: space-between;
  max-width: 1200px;
  margin: 0 auto;
  padding: 20px 40px;
  position: relative;
  z-index: 100;
}

.liquid-nav__logo {
  font-family: 'Comfortaa', cursive;
  font-size: 1.4rem;
  font-weight: 700;
  color: var(--liquid-text-primary);
  text-decoration: none;
  letter-spacing: 0.02em;
}

.liquid-nav__links {
  display: flex;
  align-items: center;
  gap: 8px;
  list-style: none;
  margin: 0;
  padding: 0;
  background: rgba(255, 255, 255, 0.6);
  backdrop-filter: blur(12px);
  -webkit-backdrop-filter: blur(12px);
  border-radius: 50px;
  padding: 6px 8px;
  border: 1px solid rgba(195, 177, 225, 0.2);
}

.liquid-nav__links a {
  font-family: 'Quicksand', sans-serif;
  font-weight: 500;
  font-size: 0.9rem;
  color: var(--liquid-text-secondary);
  text-decoration: none;
  padding: 8px 20px;
  border-radius: 50px;
  transition: color 0.25s ease, background 0.25s ease;
}

.liquid-nav__links a:hover,
.liquid-nav__links a.active {
  color: var(--liquid-text-primary);
  background: rgba(195, 177, 225, 0.2);
}
```

### Hero Section with Blob Background

```css
.liquid-hero {
  position: relative;
  min-height: 100vh;
  display: flex;
  align-items: center;
  justify-content: center;
  text-align: center;
  padding: 100px 40px;
  background: var(--liquid-bg-cloud);
  overflow: hidden;
}

/* Large background decorative blob - top right */
.liquid-hero__blob-1 {
  position: absolute;
  top: -15%;
  right: -10%;
  width: 60vw;
  height: 60vw;
  max-width: 700px;
  max-height: 700px;
  border-radius: 60% 40% 55% 45% / 50% 60% 40% 50%;
  background: var(--liquid-gradient-warm);
  opacity: 0.4;
  animation: blob-morph-1 12s ease-in-out infinite alternate;
  z-index: 1;
}

/* Medium background blob - bottom left */
.liquid-hero__blob-2 {
  position: absolute;
  bottom: -10%;
  left: -8%;
  width: 45vw;
  height: 45vw;
  max-width: 500px;
  max-height: 500px;
  border-radius: 45% 55% 40% 60% / 55% 40% 60% 45%;
  background: var(--liquid-gradient-cool);
  opacity: 0.3;
  animation: blob-morph-2 15s ease-in-out infinite alternate;
  z-index: 1;
}

/* Small accent blob */
.liquid-hero__blob-3 {
  position: absolute;
  top: 20%;
  left: 12%;
  width: 18vw;
  height: 18vw;
  max-width: 200px;
  max-height: 200px;
  border-radius: 50% 60% 45% 55% / 60% 45% 55% 50%;
  background: var(--liquid-gradient-sunset);
  opacity: 0.25;
  animation: blob-morph-3 10s ease-in-out infinite alternate;
  z-index: 1;
}

.liquid-hero__content {
  position: relative;
  z-index: 10;
  max-width: 700px;
}

.liquid-hero__content h1 {
  font-size: clamp(2.5rem, 6vw, 5rem);
  margin-bottom: 1.5rem;
  background: var(--liquid-gradient-ocean);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  background-clip: text;
}

.liquid-hero__content p {
  font-size: 1.15rem;
  color: var(--liquid-text-secondary);
  margin-bottom: 2.5rem;
  line-height: 1.7;
}

@keyframes blob-morph-1 {
  0%   { border-radius: 60% 40% 55% 45% / 50% 60% 40% 50%; }
  50%  { border-radius: 45% 55% 40% 60% / 60% 40% 55% 45%; }
  100% { border-radius: 55% 45% 60% 40% / 45% 55% 50% 50%; }
}

@keyframes blob-morph-2 {
  0%   { border-radius: 45% 55% 40% 60% / 55% 40% 60% 45%; }
  50%  { border-radius: 55% 45% 60% 40% / 40% 60% 45% 55%; }
  100% { border-radius: 40% 60% 50% 50% / 60% 45% 55% 40%; }
}

@keyframes blob-morph-3 {
  0%   { border-radius: 50% 60% 45% 55% / 60% 45% 55% 50%; }
  50%  { border-radius: 60% 40% 55% 45% / 45% 55% 50% 60%; }
  100% { border-radius: 45% 55% 50% 50% / 55% 50% 45% 55%; }
}

@media (max-width: 768px) {
  .liquid-hero { min-height: auto; padding: 80px 20px; }
  .liquid-hero__blob-1 { width: 80vw; height: 80vw; opacity: 0.25; }
  .liquid-hero__blob-2 { width: 60vw; height: 60vw; opacity: 0.2; }
  .liquid-hero__blob-3 { display: none; }
}
```

### CSS Blob Shape via Border-Radius (Eight-Value Syntax)

The eight-value `border-radius` syntax is the foundational technique for creating organic blob shapes in pure CSS. By independently controlling the horizontal and vertical radii of each corner, you can produce an enormous variety of amorphous forms from a single `<div>`.

```css
/* Static blob shape */
.blob {
  width: 300px;
  height: 300px;
  border-radius: 60% 40% 55% 45% / 50% 60% 40% 50%;
  background: var(--liquid-gradient-warm);
}

/*
  The eight-value syntax works as:
  border-radius: TL-h TR-h BR-h BL-h / TL-v TR-v BR-v BL-v;

  Where:
  TL = top-left, TR = top-right, BR = bottom-right, BL = bottom-left
  h = horizontal radius, v = vertical radius

  Using percentage values between 30% and 70% produces natural organic shapes.
  Values closer to 50% are rounder; values farther apart are more irregular.
*/

/* Animated morphing blob */
.blob--animated {
  width: 300px;
  height: 300px;
  background: var(--liquid-gradient-warm);
  animation: blob-pulse 8s ease-in-out infinite alternate;
}

@keyframes blob-pulse {
  0%   { border-radius: 60% 40% 55% 45% / 50% 60% 40% 50%; }
  25%  { border-radius: 45% 55% 40% 60% / 60% 40% 55% 45%; }
  50%  { border-radius: 55% 45% 60% 40% / 45% 55% 50% 50%; }
  75%  { border-radius: 40% 60% 50% 50% / 55% 45% 40% 60%; }
  100% { border-radius: 50% 50% 45% 55% / 40% 60% 55% 45%; }
}

/* Multiple blob sizes for layered compositions */
.blob--large  { width: 500px; height: 500px; }
.blob--medium { width: 300px; height: 300px; }
.blob--small  { width: 150px; height: 150px; }
.blob--tiny   { width: 80px;  height: 80px;  }
```

### SVG Blob with Morphing Animation

For more complex shapes including concave curves (which CSS `border-radius` cannot produce), inline SVG with animated paths provides full control. SMIL `<animate>` elements allow path-to-path morphing natively in the browser.

```html
<!-- Inline SVG blob with SMIL morph animation -->
<svg viewBox="0 0 200 200" xmlns="http://www.w3.org/2000/svg" width="400" height="400">
  <defs>
    <linearGradient id="blob-grad" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" style="stop-color:#c3b1e1" />
      <stop offset="50%" style="stop-color:#f7cac9" />
      <stop offset="100%" style="stop-color:#a8d8ea" />
    </linearGradient>
  </defs>
  <path fill="url(#blob-grad)">
    <animate
      attributeName="d"
      dur="10s"
      repeatCount="indefinite"
      values="
        M45.2,-58.3C57.3,-51.8,64.8,-36.3,68.9,-20.1C73,-3.9,73.6,13,67.4,27.1C61.2,41.2,48.1,52.5,33.6,59.3C19.1,66.1,3.2,68.4,-13.3,66.2C-29.7,64,-46.7,57.3,-57.1,45.1C-67.5,32.9,-71.3,15.1,-70.3,-2.4C-69.4,-19.9,-63.7,-37.1,-52.2,-43.7C-40.7,-50.3,-23.4,-46.3,-4.5,-40.3C14.4,-34.3,33.1,-64.8,45.2,-58.3Z;
        M39.5,-52.1C50.5,-43.8,58.1,-30.5,62.5,-15.8C66.9,-1.1,68.1,15,62.1,28.1C56.2,41.2,43.1,51.3,28.5,57.6C13.8,63.9,-2.5,66.4,-18.1,62.8C-33.7,59.2,-48.6,49.5,-57.9,35.8C-67.2,22.1,-70.8,4.4,-67.8,-11.5C-64.8,-27.4,-55.2,-41.5,-42.7,-49.4C-30.2,-57.3,-14.8,-59,-0.2,-58.8C14.4,-58.5,28.5,-60.4,39.5,-52.1Z;
        M45.2,-58.3C57.3,-51.8,64.8,-36.3,68.9,-20.1C73,-3.9,73.6,13,67.4,27.1C61.2,41.2,48.1,52.5,33.6,59.3C19.1,66.1,3.2,68.4,-13.3,66.2C-29.7,64,-46.7,57.3,-57.1,45.1C-67.5,32.9,-71.3,15.1,-70.3,-2.4C-69.4,-19.9,-63.7,-37.1,-52.2,-43.7C-40.7,-50.3,-23.4,-46.3,-4.5,-40.3C14.4,-34.3,33.1,-64.8,45.2,-58.3Z
      "
    />
  </path>
</svg>
```

```css
/* Positioning SVG blobs as background decorations */
.svg-blob-container {
  position: absolute;
  pointer-events: none;
  z-index: 1;
}

.svg-blob-container--top-right {
  top: -10%;
  right: -5%;
  width: 50vw;
  max-width: 600px;
  opacity: 0.35;
}

.svg-blob-container--bottom-left {
  bottom: -8%;
  left: -5%;
  width: 40vw;
  max-width: 450px;
  opacity: 0.25;
}
```

### SVG Gooey (Metaball) Filter Effect

The gooey effect makes nearby elements appear to merge like liquid blobs combining. It works by applying an SVG filter that blurs the elements and then increases alpha channel contrast, causing overlapping blurred regions to fuse together visually.

```html
<!-- SVG filter definition (place once in the page) -->
<svg style="position: absolute; width: 0; height: 0;">
  <defs>
    <filter id="gooey">
      <feGaussianBlur in="SourceGraphic" stdDeviation="10" result="blur" />
      <feColorMatrix
        in="blur"
        type="matrix"
        values="1 0 0 0 0
                0 1 0 0 0
                0 0 1 0 0
                0 0 0 20 -10"
        result="gooey"
      />
      <feComposite in="SourceGraphic" in2="gooey" operator="atop" />
    </filter>
  </defs>
</svg>
```

```css
/* Apply gooey filter to a container */
.gooey-group {
  filter: url(#gooey);
}

/* Child elements that will merge when overlapping */
.gooey-group .goo-dot {
  width: 80px;
  height: 80px;
  border-radius: 50%;
  background: var(--liquid-lavender);
  position: absolute;
  transition: transform 0.6s ease;
}

/* On hover, dots move together and merge */
.gooey-group:hover .goo-dot:nth-child(1) { transform: translateX(30px); }
.gooey-group:hover .goo-dot:nth-child(2) { transform: translateX(-30px); }

/*
  How it works:
  1. feGaussianBlur blurs all children, creating soft overlapping regions
  2. feColorMatrix increases alpha contrast: where blur overlap is high,
     alpha becomes fully opaque; where it's low, alpha becomes transparent
  3. This creates the visual illusion of liquid blobs merging together
  4. feComposite layers the sharp original graphics back on top

  Adjust stdDeviation to control the "gooeyness" -- higher values
  create thicker, more viscous-looking connections between shapes.
*/
```

### Wavy Section Divider

```css
/* Wavy section divider using inline SVG background */
.liquid-wave-divider {
  position: relative;
  width: 100%;
  height: 80px;
  overflow: hidden;
}

.liquid-wave-divider svg {
  position: absolute;
  bottom: 0;
  left: 0;
  width: 100%;
  height: 100%;
}

/*
  Usage in HTML:
  <div class="liquid-wave-divider">
    <svg viewBox="0 0 1200 80" preserveAspectRatio="none">
      <path
        d="M0,40 C200,80 400,0 600,40 C800,80 1000,0 1200,40 L1200,80 L0,80 Z"
        fill="#f8f6ff"
      />
    </svg>
  </div>

  Adjust the control points of the cubic Bezier curves (C commands)
  to vary the wave amplitude and frequency.
*/

/* Alternative: pure CSS wavy border using clip-path */
.liquid-wavy-section {
  clip-path: polygon(
    0% 5%,
    5% 2%,
    10% 5%,
    15% 3%,
    20% 6%,
    25% 2%,
    30% 5%,
    35% 3%,
    40% 6%,
    45% 2%,
    50% 5%,
    55% 3%,
    60% 6%,
    65% 2%,
    70% 5%,
    75% 3%,
    80% 6%,
    85% 2%,
    90% 5%,
    95% 3%,
    100% 5%,
    100% 100%,
    0% 100%
  );
  padding-top: 60px;
}
```

### Blob-Shaped Image Mask

```css
/* Apply organic blob mask to images */
.liquid-image-blob {
  width: 400px;
  height: 400px;
  object-fit: cover;
  border-radius: 60% 40% 55% 45% / 50% 60% 40% 50%;
  animation: image-blob-morph 12s ease-in-out infinite alternate;
}

@keyframes image-blob-morph {
  0%   { border-radius: 60% 40% 55% 45% / 50% 60% 40% 50%; }
  33%  { border-radius: 45% 55% 40% 60% / 60% 40% 55% 45%; }
  66%  { border-radius: 55% 45% 60% 40% / 45% 55% 50% 50%; }
  100% { border-radius: 40% 60% 50% 50% / 55% 45% 40% 60%; }
}

/* SVG clipPath alternative for more complex shapes */
/*
  <svg width="0" height="0">
    <clipPath id="blob-clip" clipPathUnits="objectBoundingBox">
      <path d="M0.5,0.05 C0.75,0,1,0.2,0.95,0.5
               C1,0.8,0.75,1,0.5,0.95
               C0.25,1,0,0.8,0.05,0.5
               C0,0.2,0.25,0,0.5,0.05Z" />
    </clipPath>
  </svg>
*/
.liquid-image-clip {
  clip-path: url(#blob-clip);
  width: 400px;
  height: 400px;
  object-fit: cover;
}
```

### Glassmorphism Blob Card

Liquid design pairs naturally with glassmorphism -- frosted glass effects layered over gradient blobs create depth and atmospheric softness.

```css
.liquid-glass-card {
  background: rgba(255, 255, 255, 0.25);
  backdrop-filter: blur(16px) saturate(180%);
  -webkit-backdrop-filter: blur(16px) saturate(180%);
  border: 1px solid rgba(255, 255, 255, 0.3);
  border-radius: 24px;
  padding: 40px;
  position: relative;
  box-shadow:
    0 8px 32px rgba(45, 43, 85, 0.06),
    inset 0 1px 0 rgba(255, 255, 255, 0.4);
}

/* Background gradient layer that the glass sits over */
.liquid-glass-wrapper {
  position: relative;
  padding: 60px;
  border-radius: 32px;
  background: var(--liquid-gradient-warm);
  overflow: hidden;
}

/* Moving blob behind the glass */
.liquid-glass-wrapper::before {
  content: '';
  position: absolute;
  top: -20%;
  left: -10%;
  width: 60%;
  height: 60%;
  border-radius: 50% 60% 45% 55% / 60% 45% 55% 50%;
  background: var(--liquid-gradient-ocean);
  opacity: 0.4;
  animation: blob-morph-1 12s ease-in-out infinite alternate;
}

.liquid-glass-wrapper::after {
  content: '';
  position: absolute;
  bottom: -15%;
  right: -10%;
  width: 50%;
  height: 50%;
  border-radius: 45% 55% 60% 40% / 55% 40% 45% 60%;
  background: var(--liquid-gradient-sunset);
  opacity: 0.35;
  animation: blob-morph-2 15s ease-in-out infinite alternate;
}
```

---

## Design Do's and Don'ts

### Do

- Use the eight-value `border-radius` syntax to create varied organic shapes from simple `<div>` elements
- Apply soft, multi-stop gradients with harmonious color transitions (analogous or triadic palettes)
- Animate blob shapes slowly and smoothly -- aim for 8-15 second animation cycles for a meditative feel
- Layer multiple translucent blobs at different sizes and opacities to create atmospheric depth
- Use generous whitespace and padding to let organic shapes breathe
- Pair blob shapes with rounded UI components (pill buttons, rounded cards, circular avatars)
- Use SVG for complex blob shapes that require concave curves or precise path control
- Apply the gooey SVG filter effect for interactive elements that merge on proximity
- Keep body text in clean, readable sans-serif typefaces with comfortable line-heights
- Use wavy SVG dividers between sections instead of hard horizontal lines

### Don't

- Use sharp corners, hard edges, or angular geometric shapes -- they contradict the organic aesthetic
- Apply harsh, high-contrast colors or neon palettes -- Liquid Design favors softness and subtlety
- Make blob animations fast or erratic -- quick, jerky motion destroys the calm fluid feeling
- Overload the page with too many animated blobs -- performance suffers and the design becomes chaotic
- Use all-uppercase, wide-tracked typography -- that mechanical treatment clashes with organic forms
- Mix liquid blob shapes with rigid grid patterns or hard-line geometric decorations
- Ignore performance on mobile -- animated SVG blobs and backdrop-filter can be expensive
- Make decorative blobs so prominent that they obscure content or impair readability
- Use pure black (`#000`) backgrounds or text -- opt for deep purples, navy, or very dark grays for warmth
- Forget about accessibility -- ensure sufficient contrast between text and gradient/blob backgrounds

---

## Related Aesthetics

| Aesthetic | Relationship to Liquid / Fluid Design |
|-----------|--------------------------------------|
| **Glassmorphism** | Natural companion; frosted glass cards layered over gradient blobs combine both aesthetics seamlessly |
| **Neumorphism** | Shares the soft, rounded approach but uses inner/outer shadows on flat surfaces rather than organic blob shapes |
| **Organic Design** | Broader design philosophy that Liquid Design draws from; Organic Design encompasses natural forms, sustainability themes, and biomorphic shapes beyond just blobs |
| **Aurora / Gradient Design** | Shares the soft gradient palette and flowing color transitions; Aurora focuses on color blending while Liquid adds shape deformation |
| **Y2K Futurism** | Both use blob shapes, but Y2K treats them with chrome, gloss, and maximalist exuberance rather than Liquid's calm restraint |
| **Vaporwave** | Both embrace soft gradients and flowing forms, but Vaporwave adds irony, retro references, and glitch effects |
| **Material Design** | The geometric opposite -- Material uses rigid cards, sharp shadows, and grid discipline that Liquid Design deliberately rejects |
| **Flat Design** | Another contrast point; Flat Design's hard edges, solid colors, and geometric precision are what Liquid Design evolved away from |
| **Biomorphic Architecture** | Shares the same intellectual roots -- organic forms inspired by living organisms, applied to physical rather than digital spaces |

---

## Quick-Start: Minimal Liquid / Fluid Design Page Template

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Liquid Design Page</title>
  <link href="https://fonts.googleapis.com/css2?family=Comfortaa:wght@400;600;700&family=Quicksand:wght@400;500;600&display=swap" rel="stylesheet">
  <style>
    :root {
      --liquid-lavender: #c3b1e1;
      --liquid-rose: #f7cac9;
      --liquid-coral: #ff8a80;
      --liquid-peach: #ffdab9;
      --liquid-sky: #a8d8ea;
      --liquid-mint: #b5ead7;
      --liquid-lilac: #dcd0ff;
      --liquid-ocean: #5b7fff;
      --liquid-violet: #9b6dff;
      --liquid-bg-cloud: #f8f6ff;
      --liquid-bg-ivory: #fff8f0;
      --liquid-bg-mist: #e8e4ef;
      --liquid-text-primary: #2d2b55;
      --liquid-text-secondary: #6b6b8d;
    }

    * { margin: 0; padding: 0; box-sizing: border-box; }

    body {
      background: var(--liquid-bg-cloud);
      color: var(--liquid-text-primary);
      font-family: 'Quicksand', sans-serif;
      font-size: 1rem;
      line-height: 1.75;
    }

    h1, h2, h3 {
      font-family: 'Comfortaa', cursive;
      font-weight: 700;
      letter-spacing: 0.01em;
      line-height: 1.25;
    }

    /* Navigation */
    nav {
      display: flex;
      align-items: center;
      justify-content: space-between;
      max-width: 1200px;
      margin: 0 auto;
      padding: 24px 40px;
      position: relative;
      z-index: 100;
    }

    nav a.logo {
      font-family: 'Comfortaa', cursive;
      font-size: 1.4rem;
      font-weight: 700;
      color: var(--liquid-text-primary);
      text-decoration: none;
    }

    nav ul {
      display: flex;
      align-items: center;
      gap: 6px;
      list-style: none;
      background: rgba(255, 255, 255, 0.6);
      backdrop-filter: blur(12px);
      -webkit-backdrop-filter: blur(12px);
      border-radius: 50px;
      padding: 6px 8px;
      border: 1px solid rgba(195, 177, 225, 0.2);
    }

    nav ul a {
      font-family: 'Quicksand', sans-serif;
      font-weight: 500;
      font-size: 0.9rem;
      color: var(--liquid-text-secondary);
      text-decoration: none;
      padding: 8px 20px;
      border-radius: 50px;
      transition: color 0.25s ease, background 0.25s ease;
    }

    nav ul a:hover {
      color: var(--liquid-text-primary);
      background: rgba(195, 177, 225, 0.2);
    }

    /* Hero */
    .hero {
      position: relative;
      display: flex;
      align-items: center;
      justify-content: center;
      text-align: center;
      min-height: 90vh;
      padding: 100px 40px;
      overflow: hidden;
    }

    /* Decorative blobs */
    .blob {
      position: absolute;
      pointer-events: none;
      z-index: 1;
    }

    .blob-1 {
      top: -12%;
      right: -8%;
      width: 55vw;
      height: 55vw;
      max-width: 650px;
      max-height: 650px;
      border-radius: 60% 40% 55% 45% / 50% 60% 40% 50%;
      background: linear-gradient(135deg, #f7cac9 0%, #c3b1e1 50%, #a8d8ea 100%);
      opacity: 0.4;
      animation: morph-a 12s ease-in-out infinite alternate;
    }

    .blob-2 {
      bottom: -8%;
      left: -6%;
      width: 42vw;
      height: 42vw;
      max-width: 480px;
      max-height: 480px;
      border-radius: 45% 55% 40% 60% / 55% 40% 60% 45%;
      background: linear-gradient(135deg, #a8d8ea 0%, #dcd0ff 50%, #c3b1e1 100%);
      opacity: 0.3;
      animation: morph-b 15s ease-in-out infinite alternate;
    }

    .blob-3 {
      top: 25%;
      left: 10%;
      width: 16vw;
      height: 16vw;
      max-width: 180px;
      max-height: 180px;
      border-radius: 50% 60% 45% 55% / 60% 45% 55% 50%;
      background: linear-gradient(135deg, #ffdab9 0%, #ff8a80 50%, #c3b1e1 100%);
      opacity: 0.25;
      animation: morph-c 10s ease-in-out infinite alternate;
    }

    @keyframes morph-a {
      0%   { border-radius: 60% 40% 55% 45% / 50% 60% 40% 50%; transform: rotate(0deg); }
      50%  { border-radius: 45% 55% 40% 60% / 60% 40% 55% 45%; }
      100% { border-radius: 55% 45% 60% 40% / 45% 55% 50% 50%; transform: rotate(3deg); }
    }

    @keyframes morph-b {
      0%   { border-radius: 45% 55% 40% 60% / 55% 40% 60% 45%; transform: rotate(0deg); }
      50%  { border-radius: 55% 45% 60% 40% / 40% 60% 45% 55%; }
      100% { border-radius: 40% 60% 50% 50% / 60% 45% 55% 40%; transform: rotate(-3deg); }
    }

    @keyframes morph-c {
      0%   { border-radius: 50% 60% 45% 55% / 60% 45% 55% 50%; transform: scale(1); }
      50%  { border-radius: 60% 40% 55% 45% / 45% 55% 50% 60%; transform: scale(1.05); }
      100% { border-radius: 45% 55% 50% 50% / 55% 50% 45% 55%; transform: scale(1); }
    }

    .hero-content {
      position: relative;
      z-index: 10;
      max-width: 680px;
    }

    .hero h1 {
      font-size: clamp(2.5rem, 6vw, 4.5rem);
      margin-bottom: 1.5rem;
      background: linear-gradient(135deg, #5b7fff 0%, #9b6dff 50%, #c3b1e1 100%);
      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent;
      background-clip: text;
    }

    .hero p {
      font-size: 1.15rem;
      color: var(--liquid-text-secondary);
      margin-bottom: 2.5rem;
      line-height: 1.7;
    }

    .btn {
      display: inline-block;
      background: linear-gradient(135deg, #5b7fff 0%, #9b6dff 100%);
      color: #ffffff;
      border: none;
      border-radius: 50px;
      padding: 16px 44px;
      font-family: 'Quicksand', sans-serif;
      font-size: 0.95rem;
      font-weight: 600;
      text-decoration: none;
      cursor: pointer;
      transition: transform 0.3s ease, box-shadow 0.3s ease;
      box-shadow: 0 4px 20px rgba(91, 127, 255, 0.3);
    }

    .btn:hover {
      transform: translateY(-2px) scale(1.02);
      box-shadow: 0 8px 30px rgba(91, 127, 255, 0.4);
    }

    .btn--outline {
      background: transparent;
      color: var(--liquid-ocean);
      border: 2px solid var(--liquid-ocean);
      box-shadow: none;
      margin-left: 12px;
    }

    .btn--outline:hover {
      background: var(--liquid-ocean);
      color: #ffffff;
      box-shadow: 0 8px 30px rgba(91, 127, 255, 0.3);
    }

    /* Wave divider */
    .wave-divider {
      width: 100%;
      line-height: 0;
      overflow: hidden;
    }

    .wave-divider svg {
      display: block;
      width: 100%;
      height: 80px;
    }

    /* Features */
    .features {
      padding: 80px 0 100px;
      background: var(--liquid-bg-ivory);
    }

    .features h2 {
      text-align: center;
      font-size: clamp(1.8rem, 3.5vw, 2.4rem);
      color: var(--liquid-text-primary);
      margin-bottom: 16px;
    }

    .features .subtitle {
      text-align: center;
      color: var(--liquid-text-secondary);
      font-size: 1.05rem;
      margin-bottom: 56px;
    }

    .features-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
      gap: 32px;
      max-width: 1100px;
      margin: 0 auto;
      padding: 0 40px;
    }

    .feature {
      background: rgba(255, 255, 255, 0.8);
      backdrop-filter: blur(8px);
      -webkit-backdrop-filter: blur(8px);
      border: 1px solid rgba(195, 177, 225, 0.15);
      border-radius: 24px;
      padding: 36px;
      position: relative;
      overflow: hidden;
      transition: transform 0.4s ease, box-shadow 0.4s ease;
      box-shadow: 0 8px 32px rgba(45, 43, 85, 0.06);
    }

    .feature:hover {
      transform: translateY(-4px);
      box-shadow: 0 16px 48px rgba(45, 43, 85, 0.1);
    }

    /* Decorative blob in card corner */
    .feature::before {
      content: '';
      position: absolute;
      top: -25px;
      right: -25px;
      width: 100px;
      height: 100px;
      border-radius: 55% 45% 60% 40% / 50% 60% 40% 50%;
      opacity: 0.12;
      z-index: 0;
      transition: opacity 0.4s;
    }

    .feature:nth-child(1)::before { background: linear-gradient(135deg, #c3b1e1, #a8d8ea); }
    .feature:nth-child(2)::before { background: linear-gradient(135deg, #f7cac9, #ffdab9); }
    .feature:nth-child(3)::before { background: linear-gradient(135deg, #b5ead7, #a8d8ea); }

    .feature:hover::before { opacity: 0.22; }

    .feature-icon {
      width: 56px;
      height: 56px;
      border-radius: 50% 60% 45% 55% / 60% 45% 55% 50%;
      display: flex;
      align-items: center;
      justify-content: center;
      font-size: 1.5rem;
      margin-bottom: 20px;
      position: relative;
      z-index: 1;
    }

    .feature:nth-child(1) .feature-icon { background: rgba(195, 177, 225, 0.25); }
    .feature:nth-child(2) .feature-icon { background: rgba(247, 202, 201, 0.3); }
    .feature:nth-child(3) .feature-icon { background: rgba(181, 234, 215, 0.3); }

    .feature h3 {
      font-size: 1.15rem;
      margin-bottom: 0.75rem;
      position: relative;
      z-index: 1;
    }

    .feature p {
      color: var(--liquid-text-secondary);
      font-size: 0.95rem;
      position: relative;
      z-index: 1;
    }

    /* Showcase / content section */
    .showcase {
      padding: 100px 40px;
      position: relative;
      overflow: hidden;
    }

    .showcase-inner {
      max-width: 1100px;
      margin: 0 auto;
      display: flex;
      align-items: center;
      gap: 60px;
    }

    .showcase-text { flex: 1; }

    .showcase-text h2 {
      font-size: clamp(1.8rem, 3.5vw, 2.4rem);
      margin-bottom: 1rem;
    }

    .showcase-text p {
      color: var(--liquid-text-secondary);
      font-size: 1.05rem;
      margin-bottom: 2rem;
      line-height: 1.7;
    }

    .showcase-visual {
      flex: 1;
      display: flex;
      align-items: center;
      justify-content: center;
      position: relative;
    }

    .showcase-blob {
      width: 100%;
      max-width: 400px;
      aspect-ratio: 1;
      border-radius: 60% 40% 55% 45% / 50% 60% 40% 50%;
      background: linear-gradient(135deg, #c3b1e1 0%, #f7cac9 40%, #a8d8ea 100%);
      animation: morph-a 12s ease-in-out infinite alternate;
      display: flex;
      align-items: center;
      justify-content: center;
      font-size: 4rem;
    }

    /* CTA */
    .cta {
      text-align: center;
      padding: 100px 40px;
      position: relative;
      overflow: hidden;
    }

    .cta-bg {
      position: absolute;
      inset: 0;
      background: linear-gradient(135deg, #f7cac9 0%, #c3b1e1 30%, #a8d8ea 60%, #b5ead7 100%);
      opacity: 0.15;
      z-index: 0;
    }

    .cta-content {
      position: relative;
      z-index: 1;
    }

    .cta h2 {
      font-size: clamp(1.8rem, 4vw, 2.6rem);
      margin-bottom: 1rem;
      background: linear-gradient(135deg, #5b7fff 0%, #9b6dff 100%);
      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent;
      background-clip: text;
    }

    .cta p {
      color: var(--liquid-text-secondary);
      margin-bottom: 2rem;
      font-size: 1.05rem;
    }

    /* Footer */
    footer {
      background: var(--liquid-bg-ivory);
      text-align: center;
      padding: 40px;
      color: var(--liquid-text-secondary);
      font-size: 0.85rem;
    }

    footer a {
      color: var(--liquid-ocean);
      text-decoration: none;
    }

    footer a:hover { text-decoration: underline; }

    /* Responsive */
    @media (max-width: 768px) {
      .hero { min-height: auto; padding: 80px 24px; }
      .blob-1 { width: 80vw; height: 80vw; opacity: 0.25; }
      .blob-2 { width: 65vw; height: 65vw; opacity: 0.2; }
      .blob-3 { display: none; }
      nav { padding: 16px 20px; }
      nav ul { gap: 2px; padding: 4px 6px; }
      nav ul a { padding: 6px 14px; font-size: 0.8rem; }
      .showcase-inner { flex-direction: column; gap: 40px; }
      .showcase-blob { max-width: 280px; }
    }
  </style>
</head>
<body>
  <!-- SVG filter for gooey effects (hidden) -->
  <svg style="position: absolute; width: 0; height: 0;">
    <defs>
      <filter id="goo">
        <feGaussianBlur in="SourceGraphic" stdDeviation="10" result="blur" />
        <feColorMatrix in="blur" type="matrix"
          values="1 0 0 0 0  0 1 0 0 0  0 0 1 0 0  0 0 0 20 -10" result="goo" />
        <feComposite in="SourceGraphic" in2="goo" operator="atop" />
      </filter>
    </defs>
  </svg>

  <nav>
    <a href="#" class="logo">amoeba</a>
    <ul>
      <li><a href="#">Flow</a></li>
      <li><a href="#">Forms</a></li>
      <li><a href="#">Create</a></li>
      <li><a href="#">About</a></li>
    </ul>
  </nav>

  <section class="hero">
    <div class="blob blob-1"></div>
    <div class="blob blob-2"></div>
    <div class="blob blob-3"></div>
    <div class="hero-content">
      <h1>Design that flows</h1>
      <p>Organic shapes, soft gradients, and gentle motion create interfaces that feel alive. Let your design breathe with fluid, natural forms.</p>
      <a href="#" class="btn">Get started</a>
      <a href="#" class="btn btn--outline">Learn more</a>
    </div>
  </section>

  <div class="wave-divider">
    <svg viewBox="0 0 1200 80" preserveAspectRatio="none" xmlns="http://www.w3.org/2000/svg">
      <path d="M0,40 C150,80 350,0 500,35 C650,70 850,10 1000,40 C1100,55 1150,30 1200,40 L1200,80 L0,80 Z" fill="#fff8f0"/>
    </svg>
  </div>

  <section class="features">
    <h2>Fluid by nature</h2>
    <p class="subtitle">Every element adapts, morphs, and flows with organic precision.</p>
    <div class="features-grid">
      <div class="feature">
        <div class="feature-icon">&#x2B24;</div>
        <h3>Organic shapes</h3>
        <p>Amorphous blob forms replace rigid geometry, bringing warmth and humanity to every surface and container.</p>
      </div>
      <div class="feature">
        <div class="feature-icon">&#x25CE;</div>
        <h3>Soft gradients</h3>
        <p>Harmonious color transitions flow like watercolor on wet paper, creating depth without harsh boundaries.</p>
      </div>
      <div class="feature">
        <div class="feature-icon">&#x223F;</div>
        <h3>Gentle motion</h3>
        <p>Slow, meditative animations that morph and undulate, making the interface feel calm and alive.</p>
      </div>
    </div>
  </section>

  <div class="wave-divider" style="transform: scaleY(-1);">
    <svg viewBox="0 0 1200 80" preserveAspectRatio="none" xmlns="http://www.w3.org/2000/svg">
      <path d="M0,40 C150,80 350,0 500,35 C650,70 850,10 1000,40 C1100,55 1150,30 1200,40 L1200,80 L0,80 Z" fill="#fff8f0"/>
    </svg>
  </div>

  <section class="showcase">
    <div class="showcase-inner">
      <div class="showcase-text">
        <h2>Shapes that breathe</h2>
        <p>Every blob is unique, every curve is intentional. Liquid design transforms static layouts into living, breathing experiences that connect with users on an emotional level.</p>
        <a href="#" class="btn">Explore</a>
      </div>
      <div class="showcase-visual">
        <div class="showcase-blob">&#x1F4A7;</div>
      </div>
    </div>
  </section>

  <section class="cta">
    <div class="cta-bg"></div>
    <div class="cta-content">
      <h2>Start creating fluid experiences</h2>
      <p>Let rigid layouts dissolve. Embrace the organic flow of liquid design and build interfaces that feel truly alive.</p>
      <a href="#" class="btn">Begin your flow</a>
    </div>
  </section>

  <footer>
    <p>amoeba &mdash; fluid design system &middot; crafted with organic precision</p>
  </footer>
</body>
</html>
```
