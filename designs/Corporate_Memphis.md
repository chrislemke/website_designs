# Corporate Memphis Design Reference

Corporate Memphis (also known as **Alegria**) is a flat, geometric illustration and design style that became the dominant visual language of major technology companies from 2017 through the early 2020s. Originated by design agency Buck for Facebook's "Alegria" design system, it is characterized by **flat vector illustrations** of disproportionate human figures with elongated, rubbery limbs, non-representational skin tones, and high-contrast solid color palettes. The style prioritizes scalability, mass-reproducibility, and a sense of cheerful universality across digital interfaces.

---

## Visual Characteristics

### Core Design Traits

- **Flat vector geometry** -- all elements are constructed from simple geometric shapes (circles, rectangles, organic curves) with no gradients, dynamic shading, or textures
- **Disproportionate human figures** -- small heads paired with massive torsos and elongated, boneless "bendy" limbs that lack skeletal structure
- **Non-representational skin tones** -- figures rendered in blue, purple, green, yellow, or pink rather than realistic human colors, intended to convey inclusivity through abstraction
- **Simplified facial features** -- ranging from minimal dot-eyes and simple mouths to completely blank faces
- **Action poses** -- figures are typically depicted dancing, jumping, collaborating, or gesturing enthusiastically
- **Flat, solid color fills** -- no blending, no texture, no depth simulation; strictly 2D appearance
- **Geometric backgrounds** -- abstract shapes, floating circles, rectangles, and organic blobs as decorative elements
- **Scalable, modular compositions** -- designed as interchangeable illustration systems that can be reused across hundreds of pages and contexts
- **Warm, optimistic tone** -- visual language designed to project friendliness, approachability, and positivity

### Design Principles

- Maintain a strictly flat appearance: no shadows, no gradients, no 3D effects
- Use a limited, high-contrast color palette for visual consistency across an entire product ecosystem
- Keep illustrations simple enough for mass production and easy animation
- Favor SVG/vector format for infinite scalability and small file sizes
- Abstract human representation to avoid specificity while suggesting diversity
- Compositions should feel open, airy, and uncluttered
- Illustrations serve a decorative/emotional role rather than conveying complex information
- All elements should be constructable from basic geometric primitives
- Embrace whimsy and exaggeration over realism

---

## Color Palette

### Primary Scheme

Corporate Memphis relies on a **limited palette of high-contrast solid primary colors or soft pastels**. The palette avoids dynamic shading or gradients entirely, maintaining a flat, sleek appearance.

| Role | Colors | Hex (suggested) |
|------|--------|-----------------|
| **Primary Blue** | Bright medium blue, sky blue | `#4A90D9`, `#5B9BD5` |
| **Primary Purple** | Vivid violet, soft lavender | `#7B61FF`, `#C8B4FF` |
| **Primary Pink / Coral** | Warm pink, salmon | `#F48196`, `#FF6B8A` |
| **Primary Green / Teal** | Caribbean green, teal | `#14C88C`, `#2ECDA7` |
| **Primary Yellow** | Warm amber, golden yellow | `#FAD141`, `#FBD15A` |
| **Accent Orange** | Warm tangerine | `#FF8C42`, `#FFA552` |
| **Skin Tone: Blue** | Soft blue, powder blue | `#86CCCA`, `#78C8C8` |
| **Skin Tone: Purple** | Muted lavender | `#C9AECF`, `#B4A0D0` |
| **Skin Tone: Green** | Soft sage, mint | `#7DD1A0`, `#82D993` |
| **Skin Tone: Pink** | Warm blush | `#F0A0B0`, `#FAD6DA` |
| **Background (Light)** | Near-white, soft cream | `#FAFBFC`, `#F5F6FA` |
| **Background (Dark)** | Deep navy, charcoal | `#1A1A2E`, `#141414` |
| **Text (Dark)** | Near-black | `#1D1D1F`, `#2C2C2E` |
| **Text (Light)** | Soft off-white | `#F1F1F1`, `#EDEFEC` |

### Suggested CSS Custom Properties

```css
:root {
  /* Primary palette */
  --cm-blue: #4a90d9;
  --cm-purple: #7b61ff;
  --cm-pink: #f48196;
  --cm-green: #14c88c;
  --cm-yellow: #fad141;
  --cm-orange: #ff8c42;
  --cm-teal: #78c8c8;

  /* Soft / pastel variants */
  --cm-blue-soft: #b4dcdc;
  --cm-purple-soft: #c8b4ff;
  --cm-pink-soft: #fad6da;
  --cm-green-soft: #a8e6cf;
  --cm-yellow-soft: #fef3c7;

  /* Non-representational skin tones */
  --cm-skin-blue: #86ccca;
  --cm-skin-purple: #c9aecf;
  --cm-skin-green: #7dd1a0;
  --cm-skin-pink: #f0a0b0;
  --cm-skin-yellow: #f5d76e;

  /* Backgrounds */
  --cm-bg-light: #fafbfc;
  --cm-bg-cream: #f5f6fa;
  --cm-bg-dark: #1a1a2e;

  /* Text */
  --cm-text-dark: #1d1d1f;
  --cm-text-medium: #6e6e73;
  --cm-text-light: #f1f1f1;

  /* Decorative blobs */
  --cm-blob-1: #c8b4f0;
  --cm-blob-2: #b4dcdc;
  --cm-blob-3: #fad6da;
}
```

### Color Guidelines

- **Strictly no gradients** -- every fill is a solid, flat color
- Use **3-5 colors maximum** per composition to maintain cohesion
- Non-representational skin tones (blue, purple, green) are a defining characteristic; never use realistic flesh tones
- Background colors should be either very light (near-white) or bold and saturated
- Decorative geometric shapes (floating circles, rectangles, blobs) use the accent/pastel palette
- Color contrast between figure and background must be high for readability at small sizes
- The palette should feel **warm, optimistic, and energetic** without being garish

---

## Typography

### Typeface Characteristics

Corporate Memphis typography should be:

- **Clean geometric sans-serif** -- matching the flat, constructed illustration style
- **Rounded or softened terminals preferred** -- reinforcing the friendly, approachable tone
- **Medium to bold weights for headings** -- confident but not aggressive
- **Regular weight for body text** -- clean legibility at scale
- **No serifs, no decorative scripts** -- these conflict with the geometric flatness
- **Generous letter-spacing and line-height** -- open, airy feel matching the illustrations

### Recommended Web Fonts (Google Fonts)

| Font | Style | Usage |
|------|-------|-------|
| **Poppins** | Geometric sans, rounded corners | Headlines, body text (the quintessential Corporate Memphis font) |
| **Nunito** | Rounded sans-serif, soft terminals | Headlines, body text, UI labels |
| **Nunito Sans** | Clean companion to Nunito | Body text, smaller copy |
| **DM Sans** | Clean geometric sans | Body text, UI elements |
| **Inter** | Neutral geometric sans | Body text, data-heavy layouts |
| **Quicksand** | Rounded geometric sans | Display headings, feature titles |
| **Rubik** | Slightly rounded geometric | Headlines, buttons, all-purpose |
| **Manrope** | Modern geometric grotesk | Headlines, body text |
| **Plus Jakarta Sans** | Contemporary geometric sans | Headlines, body (modern Corporate Memphis) |

### Typography CSS Example

```css
/* Import fonts */
@import url('https://fonts.googleapis.com/css2?family=Poppins:wght@400;500;600;700&family=Nunito+Sans:wght@400;600&display=swap');

/* Headlines */
h1, h2, h3 {
  font-family: 'Poppins', 'Nunito', sans-serif;
  font-weight: 600;
  color: var(--cm-text-dark);
  line-height: 1.2;
  letter-spacing: -0.01em;
}

/* Display / Hero text */
.cm-display {
  font-family: 'Poppins', sans-serif;
  font-size: clamp(2.5rem, 5vw, 4.5rem);
  font-weight: 700;
  letter-spacing: -0.02em;
  line-height: 1.1;
}

/* Body text */
body {
  font-family: 'Nunito Sans', 'Poppins', sans-serif;
  font-weight: 400;
  font-size: 1rem;
  line-height: 1.7;
  color: var(--cm-text-dark);
}

/* UI labels and buttons */
.cm-label {
  font-family: 'Poppins', sans-serif;
  font-weight: 600;
  font-size: 0.9rem;
  letter-spacing: 0.02em;
  text-transform: none; /* avoid uppercase -- too corporate/rigid */
}

/* Subtext / captions */
.cm-caption {
  font-family: 'Nunito Sans', sans-serif;
  font-weight: 400;
  font-size: 0.85rem;
  color: var(--cm-text-medium);
  line-height: 1.5;
}
```

---

## Layout Principles

### Grid and Structure

- **Centered, spacious layouts** -- generous whitespace is essential; illustrations and content need breathing room
- **Max-width containers** (1000-1200px) prevent sprawl and keep focus on content
- **Large hero sections** -- oversized illustrations paired with short, punchy copy
- **Card-based content blocks** -- flat cards with minimal or no borders, organized in grids
- **Alternating content/illustration rows** -- zigzag layout where text and illustration swap sides
- **Generous padding** (40-80px between sections) reinforces the open, airy feel
- **Simple CSS Grid or Flexbox** -- no complex responsive gymnastics; layouts are intentionally straightforward
- **Flat, borderless cards** -- no drop shadows; separation achieved through background color contrast or subtle spacing

### Section Organization

- **Hero**: Large illustration (40-60% of viewport) + bold headline + short tagline + CTA button
- **Features**: 3-4 column grid of icon/illustration + title + short description
- **Alternating rows**: Text block on one side, illustration on the other, swapping per section
- **Social proof / testimonials**: Simple cards or inline quotes with minimal decoration
- **CTA / footer**: Bold background color + centered text + prominent button
- Use **solid color blocks** to separate sections (e.g., white section, then blue section, then white again)
- No divider lines -- sections are separated purely by background color changes and vertical spacing

### Responsive Approach

- Stack columns vertically on mobile
- Illustrations scale down but maintain their prominence
- Maintain generous spacing even at smaller breakpoints
- Typography scales fluidly with `clamp()` or viewport units

---

## CSS/Design Techniques

### Flat Card Component

```css
.cm-card {
  background: #ffffff;
  border-radius: 16px;
  padding: 32px;
  /* No box-shadow -- this is flat design */
  /* Separation comes from background contrast */
}

/* On a colored background, cards stand out via color alone */
.cm-section--blue {
  background: var(--cm-blue);
}

.cm-section--blue .cm-card {
  background: #ffffff;
  color: var(--cm-text-dark);
}
```

### Flat Button

```css
.cm-button {
  display: inline-flex;
  align-items: center;
  justify-content: center;
  background: var(--cm-blue);
  color: #ffffff;
  border: none;
  border-radius: 50px; /* fully rounded pill shape */
  padding: 14px 36px;
  font-family: 'Poppins', sans-serif;
  font-weight: 600;
  font-size: 1rem;
  cursor: pointer;
  transition: background 0.2s ease, transform 0.15s ease;
  /* No box-shadow -- strictly flat */
}

.cm-button:hover {
  background: var(--cm-purple);
  transform: translateY(-1px);
}

.cm-button:active {
  transform: translateY(0);
}

/* Secondary / outline variant */
.cm-button--outline {
  background: transparent;
  color: var(--cm-blue);
  border: 2px solid var(--cm-blue);
}

.cm-button--outline:hover {
  background: var(--cm-blue);
  color: #ffffff;
}
```

### Hero Section

```css
.cm-hero {
  display: flex;
  align-items: center;
  justify-content: space-between;
  max-width: 1200px;
  margin: 0 auto;
  padding: 80px 40px;
  gap: 60px;
}

.cm-hero__content {
  flex: 1;
  max-width: 500px;
}

.cm-hero__illustration {
  flex: 1;
  display: flex;
  justify-content: center;
  align-items: center;
}

.cm-hero__illustration svg,
.cm-hero__illustration img {
  width: 100%;
  max-width: 550px;
  height: auto;
}

.cm-hero h1 {
  font-size: clamp(2.5rem, 5vw, 4rem);
  font-weight: 700;
  margin-bottom: 1rem;
  line-height: 1.15;
}

.cm-hero p {
  font-size: 1.15rem;
  color: var(--cm-text-medium);
  margin-bottom: 2rem;
  line-height: 1.7;
}

@media (max-width: 768px) {
  .cm-hero {
    flex-direction: column-reverse;
    text-align: center;
    padding: 40px 20px;
  }
}
```

### Feature Grid

```css
.cm-features {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
  gap: 40px;
  max-width: 1200px;
  margin: 0 auto;
  padding: 80px 40px;
}

.cm-feature {
  text-align: center;
  padding: 24px;
}

.cm-feature__icon {
  width: 80px;
  height: 80px;
  margin: 0 auto 20px;
}

.cm-feature h3 {
  font-size: 1.25rem;
  margin-bottom: 0.75rem;
}

.cm-feature p {
  font-size: 0.95rem;
  color: var(--cm-text-medium);
  line-height: 1.6;
}
```

### Alternating Content Rows

```css
.cm-row {
  display: flex;
  align-items: center;
  gap: 60px;
  max-width: 1200px;
  margin: 0 auto;
  padding: 80px 40px;
}

.cm-row:nth-child(even) {
  flex-direction: row-reverse;
}

.cm-row__text {
  flex: 1;
}

.cm-row__image {
  flex: 1;
}

.cm-row__image img,
.cm-row__image svg {
  width: 100%;
  max-width: 500px;
  height: auto;
}

@media (max-width: 768px) {
  .cm-row,
  .cm-row:nth-child(even) {
    flex-direction: column;
    gap: 30px;
    padding: 40px 20px;
  }
}
```

### Section Color Blocks

```css
.cm-section {
  padding: 80px 0;
}

.cm-section--white {
  background: var(--cm-bg-light);
}

.cm-section--blue {
  background: var(--cm-blue);
  color: #ffffff;
}

.cm-section--purple {
  background: var(--cm-purple);
  color: #ffffff;
}

.cm-section--cream {
  background: var(--cm-bg-cream);
}

.cm-section--dark {
  background: var(--cm-bg-dark);
  color: var(--cm-text-light);
}
```

### Decorative Floating Shapes (SVG Blobs)

A hallmark of Corporate Memphis is decorative geometric shapes floating in the background.

```css
.cm-blobs {
  position: relative;
  overflow: hidden;
}

.cm-blob {
  position: absolute;
  border-radius: 50%;
  opacity: 0.15;
  z-index: 0;
}

.cm-blob--1 {
  width: 300px;
  height: 300px;
  background: var(--cm-purple-soft);
  top: -100px;
  right: -80px;
}

.cm-blob--2 {
  width: 200px;
  height: 200px;
  background: var(--cm-pink-soft);
  bottom: -60px;
  left: -40px;
}

.cm-blob--3 {
  width: 150px;
  height: 150px;
  background: var(--cm-green-soft);
  top: 40%;
  left: 10%;
}
```

### Inline SVG Illustration Style (CSS for SVG figures)

```css
/* Style guide for inline SVG illustrations */
.cm-illustration svg {
  /* Flat fills, no strokes */
  fill-rule: evenodd;
}

.cm-illustration .figure-body {
  fill: var(--cm-skin-blue);
}

.cm-illustration .figure-hair {
  fill: var(--cm-purple);
}

.cm-illustration .figure-clothing {
  fill: var(--cm-pink);
}

.cm-illustration .background-shape {
  fill: var(--cm-yellow-soft);
  opacity: 0.4;
}

/* Simple hover animation for interactive illustrations */
.cm-illustration:hover svg {
  transform: scale(1.02);
  transition: transform 0.3s ease;
}
```

### Navigation Bar

```css
.cm-nav {
  display: flex;
  align-items: center;
  justify-content: space-between;
  max-width: 1200px;
  margin: 0 auto;
  padding: 20px 40px;
  /* No borders, no shadows -- flat */
}

.cm-nav__logo {
  font-family: 'Poppins', sans-serif;
  font-weight: 700;
  font-size: 1.4rem;
  color: var(--cm-text-dark);
  text-decoration: none;
}

.cm-nav__links {
  display: flex;
  gap: 32px;
  list-style: none;
}

.cm-nav__links a {
  font-family: 'Poppins', sans-serif;
  font-weight: 500;
  font-size: 0.95rem;
  color: var(--cm-text-medium);
  text-decoration: none;
  transition: color 0.2s ease;
}

.cm-nav__links a:hover {
  color: var(--cm-blue);
}
```

---

## Illustration Construction Guide

### Building Corporate Memphis Figures

Corporate Memphis illustrations are constructed from basic geometric primitives:

| Body Part | Shape | Proportion |
|-----------|-------|------------|
| **Head** | Small circle or oval | Disproportionately small relative to body |
| **Torso** | Large rounded rectangle or trapezoid | Oversized, dominant element |
| **Arms** | Long, curved paths (no joints) | Extremely elongated, rubbery, boneless |
| **Legs** | Long, tapered paths | Elongated, bendy, often in dynamic poses |
| **Hands** | Simple circles or mitten shapes | Minimal detail |
| **Feet** | Rounded rectangles | Simple, block-like |
| **Hair** | Solid colored shape overlaid on head | Abstract, single-color block |
| **Face** | Minimal: dot eyes, simple curve mouth | Often no face at all |

### Key Construction Rules

- **No outlines or strokes** -- all elements are solid filled shapes
- **No realistic proportions** -- exaggeration is the point
- **No anatomical joints** -- limbs bend smoothly like rubber hoses
- **Non-representational colors** -- skin in blue, purple, green, never realistic
- **No fine detail** -- clothing is solid blocks of color, no patterns or textures
- **Dynamic, active poses** -- figures should feel alive and in motion
- **Geometric simplification** -- reduce everything to its most basic geometric form

---

## Key Companies and Products Using This Style

| Company / Product | Notes |
|-------------------|-------|
| **Facebook / Meta** | Originated the Alegria system (2017) with agency Buck |
| **Google** | Adopted similar flat illustration systems across products |
| **Slack** | Flat, colorful character illustrations throughout the app |
| **Airbnb** | Flat illustrations with non-representational figures |
| **Lyft** | Geometric flat illustrations for rider/driver experience |
| **Duolingo** | Flat character system (Duo and friends) |
| **Headspace** | Simplified flat meditation illustrations |
| **Discord** | Flat character illustrations (Wumpus and human figures) |
| **YouTube** | Flat explainer and error page illustrations |

### Open Illustration Libraries in This Style

- **unDraw** (undraw.co) -- open-source flat SVG illustrations
- **Humaaans** (humaaans.com) -- mix-and-match flat human illustrations by Pablo Stanley
- **Open Peeps** -- hand-drawn-style flat character library
- **Blush** (blush.design) -- customizable flat illustration collections

---

## Related Aesthetics

| Aesthetic | Relationship to Corporate Memphis |
|-----------|----------------------------------|
| **Flat Design** | Parent category; Corporate Memphis is a specialized subset of flat design focused on illustration systems |
| **Memphis Design** | 1980s Italian design movement (Memphis Group); namesake reference for bright colors, geometric shapes, and playful patterns |
| **Claymorphism** | 3D successor trend; gives flat elements a puffy, clay-like depth that Corporate Memphis explicitly avoids |
| **Glassmorphism** | Contemporary alternative; uses transparency, blur, and glass effects vs. Corporate Memphis's opaque flatness |
| **Minimalism** | Shares the reductive philosophy but Corporate Memphis adds warmth through color and illustration |
| **Neubrutalism** | Reactionary counter-movement; embraces raw, unpolished, high-contrast aesthetics as an antidote to Corporate Memphis's polish |
| **Material Design** | Google's design system; shares flat principles but adds elevation/shadow layers that Corporate Memphis rejects |

---

## Quick-Start: Minimal Corporate Memphis Page Template

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Corporate Memphis Page</title>
  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;500;600;700&family=Nunito+Sans:wght@400;600&display=swap" rel="stylesheet">
  <style>
    :root {
      --cm-blue: #4a90d9;
      --cm-purple: #7b61ff;
      --cm-pink: #f48196;
      --cm-green: #14c88c;
      --cm-yellow: #fad141;
      --cm-bg: #fafbfc;
      --cm-text: #1d1d1f;
      --cm-text-muted: #6e6e73;
    }

    * { margin: 0; padding: 0; box-sizing: border-box; }

    body {
      background: var(--cm-bg);
      color: var(--cm-text);
      font-family: 'Nunito Sans', 'Poppins', sans-serif;
      font-weight: 400;
      line-height: 1.7;
    }

    h1, h2, h3 {
      font-family: 'Poppins', sans-serif;
      font-weight: 600;
      line-height: 1.2;
    }

    /* Navigation */
    nav {
      display: flex;
      align-items: center;
      justify-content: space-between;
      max-width: 1200px;
      margin: 0 auto;
      padding: 20px 40px;
    }

    nav a.logo {
      font-family: 'Poppins', sans-serif;
      font-weight: 700;
      font-size: 1.3rem;
      color: var(--cm-text);
      text-decoration: none;
    }

    nav ul {
      display: flex;
      gap: 28px;
      list-style: none;
    }

    nav ul a {
      color: var(--cm-text-muted);
      text-decoration: none;
      font-weight: 500;
      font-size: 0.95rem;
      transition: color 0.2s;
    }

    nav ul a:hover { color: var(--cm-blue); }

    /* Hero */
    .hero {
      display: flex;
      align-items: center;
      justify-content: space-between;
      max-width: 1200px;
      margin: 0 auto;
      padding: 80px 40px;
      gap: 60px;
    }

    .hero-content { flex: 1; max-width: 520px; }

    .hero h1 {
      font-size: clamp(2.5rem, 5vw, 4rem);
      margin-bottom: 1rem;
    }

    .hero p {
      font-size: 1.15rem;
      color: var(--cm-text-muted);
      margin-bottom: 2rem;
    }

    .hero-illustration {
      flex: 1;
      display: flex;
      justify-content: center;
    }

    /* Flat button */
    .btn {
      display: inline-block;
      background: var(--cm-blue);
      color: #fff;
      border: none;
      border-radius: 50px;
      padding: 14px 36px;
      font-family: 'Poppins', sans-serif;
      font-weight: 600;
      font-size: 1rem;
      cursor: pointer;
      text-decoration: none;
      transition: background 0.2s, transform 0.15s;
    }

    .btn:hover {
      background: var(--cm-purple);
      transform: translateY(-1px);
    }

    /* Feature section */
    .features {
      background: #ffffff;
      padding: 80px 0;
    }

    .features-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
      gap: 40px;
      max-width: 1200px;
      margin: 0 auto;
      padding: 0 40px;
    }

    .feature {
      text-align: center;
      padding: 24px;
    }

    .feature-icon {
      width: 72px;
      height: 72px;
      border-radius: 50%;
      margin: 0 auto 20px;
      display: flex;
      align-items: center;
      justify-content: center;
      font-size: 2rem;
    }

    .feature h3 { margin-bottom: 0.5rem; }
    .feature p { color: var(--cm-text-muted); font-size: 0.95rem; }

    /* CTA section */
    .cta {
      background: var(--cm-blue);
      color: #ffffff;
      text-align: center;
      padding: 80px 40px;
    }

    .cta h2 {
      font-size: 2.5rem;
      margin-bottom: 1rem;
    }

    .cta p {
      font-size: 1.1rem;
      opacity: 0.9;
      margin-bottom: 2rem;
    }

    .cta .btn {
      background: #ffffff;
      color: var(--cm-blue);
    }

    .cta .btn:hover {
      background: var(--cm-yellow);
      color: var(--cm-text);
    }

    @media (max-width: 768px) {
      .hero {
        flex-direction: column-reverse;
        text-align: center;
        padding: 40px 20px;
      }
      nav { padding: 16px 20px; }
      nav ul { gap: 16px; }
    }
  </style>
</head>
<body>
  <nav>
    <a href="#" class="logo">Acme Co</a>
    <ul>
      <li><a href="#">Product</a></li>
      <li><a href="#">Features</a></li>
      <li><a href="#">Pricing</a></li>
      <li><a href="#">About</a></li>
    </ul>
  </nav>

  <section class="hero">
    <div class="hero-content">
      <h1>Build something people love</h1>
      <p>Our platform helps teams collaborate, ship faster, and delight their users with less effort and more joy.</p>
      <a href="#" class="btn">Get Started Free</a>
    </div>
    <div class="hero-illustration">
      <!-- Replace with Corporate Memphis SVG illustration -->
      <svg width="400" height="320" viewBox="0 0 400 320" fill="none" xmlns="http://www.w3.org/2000/svg">
        <!-- Background blob -->
        <ellipse cx="200" cy="170" rx="180" ry="140" fill="#C8B4FF" opacity="0.2"/>
        <!-- Figure body -->
        <rect x="160" y="100" width="80" height="100" rx="20" fill="#86CCCA"/>
        <!-- Head -->
        <circle cx="200" cy="80" r="28" fill="#86CCCA"/>
        <!-- Hair -->
        <path d="M175 68 Q200 40 225 68" fill="#7B61FF"/>
        <!-- Left arm -->
        <path d="M160 120 Q100 90 80 140" stroke="#86CCCA" stroke-width="16" stroke-linecap="round" fill="none"/>
        <!-- Right arm -->
        <path d="M240 120 Q300 90 320 140" stroke="#86CCCA" stroke-width="16" stroke-linecap="round" fill="none"/>
        <!-- Left leg -->
        <path d="M180 200 Q170 260 150 290" stroke="#86CCCA" stroke-width="16" stroke-linecap="round" fill="none"/>
        <!-- Right leg -->
        <path d="M220 200 Q230 260 250 290" stroke="#86CCCA" stroke-width="16" stroke-linecap="round" fill="none"/>
        <!-- Clothing -->
        <rect x="165" y="130" width="70" height="50" rx="10" fill="#F48196"/>
        <!-- Simple face -->
        <circle cx="190" cy="78" r="3" fill="#1D1D1F"/>
        <circle cx="210" cy="78" r="3" fill="#1D1D1F"/>
        <path d="M192 88 Q200 94 208 88" stroke="#1D1D1F" stroke-width="2" fill="none" stroke-linecap="round"/>
        <!-- Decorative shapes -->
        <circle cx="60" cy="60" r="20" fill="#FAD141" opacity="0.5"/>
        <rect x="310" y="200" width="30" height="30" rx="6" fill="#14C88C" opacity="0.4" transform="rotate(15 325 215)"/>
        <circle cx="340" cy="80" r="12" fill="#F48196" opacity="0.4"/>
      </svg>
    </div>
  </section>

  <section class="features">
    <div class="features-grid">
      <div class="feature">
        <div class="feature-icon" style="background: #C8B4FF30;">
          <svg width="36" height="36" viewBox="0 0 36 36"><circle cx="18" cy="18" r="14" fill="#7B61FF"/><rect x="12" y="14" width="12" height="8" rx="2" fill="#fff"/></svg>
        </div>
        <h3>Easy Collaboration</h3>
        <p>Work together in real time with your entire team, no matter where they are.</p>
      </div>
      <div class="feature">
        <div class="feature-icon" style="background: #F4819630;">
          <svg width="36" height="36" viewBox="0 0 36 36"><circle cx="18" cy="18" r="14" fill="#F48196"/><polygon points="18,10 22,22 14,22" fill="#fff"/></svg>
        </div>
        <h3>Ship Faster</h3>
        <p>Streamlined workflows and smart automation help you launch in record time.</p>
      </div>
      <div class="feature">
        <div class="feature-icon" style="background: #14C88C30;">
          <svg width="36" height="36" viewBox="0 0 36 36"><circle cx="18" cy="18" r="14" fill="#14C88C"/><path d="M12 18 L16 22 L24 14" stroke="#fff" stroke-width="2.5" fill="none" stroke-linecap="round"/></svg>
        </div>
        <h3>Reliable & Secure</h3>
        <p>Enterprise-grade security and 99.9% uptime so you can focus on building.</p>
      </div>
    </div>
  </section>

  <section class="cta">
    <h2>Ready to get started?</h2>
    <p>Join thousands of teams already using our platform.</p>
    <a href="#" class="btn">Start Free Trial</a>
  </section>
</body>
</html>
```
