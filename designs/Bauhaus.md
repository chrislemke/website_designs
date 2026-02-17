# Bauhaus

Form follows function: geometric primary-color shapes, grid systems, and sans-serif purity from 1920s Weimar. The Bauhaus school (1919-1933) fused fine art with industrial craft to create a unified design language built on geometric fundamentals -- circles, triangles, and squares -- combined with primary colors and stripped of ornament. Its legacy permeates modern graphic design, architecture, furniture, and digital interfaces, establishing the principle that beauty emerges from functional honesty and geometric clarity.

---

## Visual Characteristics

### Core Design Traits

- **Primary geometric shapes** -- circles, triangles, and squares are the foundational building blocks of every composition
- **Primary color palette** -- red, yellow, and blue dominate, paired with black and white; secondary colors appear rarely
- **Bold sans-serif typography** -- heavy, geometric letterforms that command attention; type as visual element
- **Strict grid alignment** -- every element snaps to an underlying modular grid; mathematical precision governs placement
- **Asymmetric balance** -- dynamic compositions that feel balanced through weight distribution rather than mirror symmetry
- **Thick black outlines and rules** -- heavy strokes define shapes and separate regions
- **Flat, unmodulated color** -- no gradients, no shading; each shape is a solid primary or neutral fill
- **Functional minimalism** -- no ornament, no decoration; every element exists because it serves a purpose
- **Diagonal and angular compositions** -- dynamic energy created through tilted elements and intersecting lines
- **Integration of type and image** -- text is treated as a graphic element equal in importance to shapes and color

### Design Principles

- Form follows function: the purpose of an element dictates its appearance
- Unite art and technology; design should be reproducible and industrially viable
- Reduce to fundamental elements: basic shapes, primary colors, universal forms
- Embrace the grid as the structural backbone of all composition
- Typography is architecture: letterforms are built from geometric parts
- Asymmetry creates dynamic visual tension superior to static symmetry
- Every design decision must be rationally justified
- Materials and methods should be honest; do not simulate what is not there

---

## Color Palette

### Bauhaus Core Palette

The Bauhaus color theory, largely shaped by Johannes Itten and Wassily Kandinsky, assigns primary colors to primary shapes: yellow to the triangle, red to the square, blue to the circle.

| Color Name | Hex | Role / Usage |
|------------|-----|-------------|
| **Bauhaus Red** | `#E3000B` | Primary accent, squares, call-to-action elements |
| **Bauhaus Yellow** | `#FFD700` | Secondary accent, triangular shapes, highlights |
| **Bauhaus Blue** | `#003DA5` | Tertiary accent, circular shapes, links |
| **Black** | `#000000` | Text, outlines, rules, structural elements |
| **White** | `#FFFFFF` | Backgrounds, negative space, text on dark |
| **Warm Gray** | `#D4D0C8` | Secondary backgrounds, neutral surfaces |
| **Dark Gray** | `#3C3C3C` | Secondary text, muted structural elements |
| **Deep Red** | `#B30009` | Hover/active state for red elements |
| **Deep Blue** | `#002D7A` | Hover/active state for blue elements |
| **Amber** | `#E6B800` | Hover/active state for yellow elements |

### CSS Custom Properties

```css
:root {
  /* Primary colors */
  --bau-red: #e3000b;
  --bau-yellow: #ffd700;
  --bau-blue: #003da5;

  /* Hover/active states */
  --bau-red-dark: #b30009;
  --bau-yellow-dark: #e6b800;
  --bau-blue-dark: #002d7a;

  /* Neutrals */
  --bau-black: #000000;
  --bau-white: #ffffff;
  --bau-warm-gray: #d4d0c8;
  --bau-dark-gray: #3c3c3c;

  /* Backgrounds */
  --bau-bg-primary: #ffffff;
  --bau-bg-secondary: #f5f3ef;
  --bau-bg-dark: #1a1a1a;

  /* Text */
  --bau-text-primary: #000000;
  --bau-text-secondary: #3c3c3c;
  --bau-text-inverse: #ffffff;
}
```

### Color Usage Guidelines

- **Use the three primary colors** as the dominant chromatic elements; avoid greens, purples, and oranges
- Black and white are structural; primary colors are expressive
- Each primary color should appear in roughly equal visual weight across a composition
- Yellow demands a dark background or thick black outline to maintain visibility
- Reserve large fields of color for hero sections and key interactive areas
- Never use gradients; all fills are solid and flat
- Gray tones serve as neutral connectors between the vibrant primaries

---

## Typography

### Typeface Characteristics

Bauhaus typography is:

- **Geometric sans-serif** -- built from circles, straight lines, and consistent stroke widths
- **Bold and heavy** -- headings use strong weights that assert graphic dominance
- **Lowercase-favoring** -- Herbert Bayer's Universal Typeface proposed eliminating uppercase entirely; lowercase is preferred for body text
- **Tight tracking for headings** -- letters sit close together, forming a unified visual block
- **Functional above decorative** -- type exists to communicate, not to ornament

### Recommended Web Fonts (Google Fonts)

| Font | Style | Best For |
|------|-------|----------|
| **Jost** | Geometric sans-serif (Futura-inspired) | Closest to the Bauhaus ideal; headings and display |
| **Poppins** | Pure geometric sans | Headings, UI elements, modern Bauhaus interpretation |
| **Raleway** | Elegant geometric sans | Display text, lighter-weight headings |
| **DM Sans** | Low-contrast geometric | Body text, UI labels |
| **Work Sans** | Geometric grotesque | Body text, editorial layouts |
| **Archivo** | Grotesque with geometric leanings | Headings and body, versatile |
| **Nunito Sans** | Rounded geometric | Softer interpretation of Bauhaus geometry |
| **Barlow** | Slightly condensed geometric | Navigation, labels, compact layouts |
| **Exo 2** | Geometric with contemporary feel | Techy Bauhaus-influenced headings |
| **Inter** | Humanist but geometric underpinnings | Screen-optimized body text |

### Font Pairing Suggestions

| Heading Font | Body Font | Character |
|-------------|-----------|-----------|
| **Jost** (700) | **Work Sans** (400) | Authentic Bauhaus spirit |
| **Poppins** (700) | **DM Sans** (400) | Clean geometric consistency |
| **Archivo** (700) | **Inter** (400) | Modern, highly legible |
| **Barlow** (700) | **Barlow** (400) | Monofamily, condensed efficiency |
| **Raleway** (600) | **Nunito Sans** (400) | Elegant with soft warmth |

### Typography CSS Example

```css
/* Import fonts */
@import url('https://fonts.googleapis.com/css2?family=Jost:wght@400;500;700;900&family=Work+Sans:wght@400;500&display=swap');

/* Headings */
h1, h2, h3, h4, h5, h6 {
  font-family: 'Jost', 'Futura', sans-serif;
  font-weight: 700;
  color: var(--bau-text-primary);
  line-height: 1.1;
  letter-spacing: -0.01em;
  text-transform: uppercase;
}

/* Display / Hero text */
.bau-display {
  font-family: 'Jost', sans-serif;
  font-size: clamp(3rem, 7vw, 6rem);
  font-weight: 900;
  letter-spacing: -0.03em;
  line-height: 0.95;
  text-transform: uppercase;
}

/* Body text */
body {
  font-family: 'Work Sans', sans-serif;
  font-weight: 400;
  font-size: 1rem;
  line-height: 1.7;
  color: var(--bau-text-secondary);
}

/* Labels */
.bau-label {
  font-family: 'Jost', sans-serif;
  font-weight: 500;
  font-size: 0.8rem;
  letter-spacing: 0.08em;
  text-transform: uppercase;
}

/* Caption */
.bau-caption {
  font-family: 'Work Sans', sans-serif;
  font-weight: 400;
  font-size: 0.85rem;
  color: var(--bau-dark-gray);
  line-height: 1.5;
}
```

---

## Layout Principles

### Grid and Structure

- **Modular grid system** -- strict 12-column or 6-column grid with consistent gutters; every element aligns to grid intersections
- **Asymmetric layouts** -- content is deliberately shifted off-center to create visual tension and dynamic movement
- **Thick black rules as dividers** -- 3-6px solid black lines separate sections and define spatial zones
- **Overlapping elements** -- shapes, type, and color blocks overlap to create depth and compositional energy
- **Max-width containers** -- content constrained to 1100-1200px for readability
- **Geometric section shapes** -- sections may have non-rectangular boundaries defined by diagonal lines or geometric cutouts

### Section Organization

- **Navigation**: Bold logo mark (geometric shape + text), horizontal links in uppercase, thick bottom border
- **Hero**: Massive geometric shape (circle, triangle, or square) paired with oversized type; a primary color background block
- **Features**: Grid of items, each anchored by a geometric icon (not decorative -- a circle, square, or triangle in primary color)
- **Content rows**: Text paired with geometric compositions or color blocks, alternating asymmetric alignment
- **Manifesto / Statement**: Large bold text on a primary color background; the design speaks its philosophy
- **Footer**: Black background, white text, geometric accents, grid-aligned link columns

### Responsive Approach

- Grid collapses from multi-column to single-column below 768px
- Geometric shapes scale proportionally using viewport units or `clamp()`
- Thick rules and borders maintain their visual weight at all sizes
- Typography scales dramatically; display text should still dominate on mobile
- Maintain asymmetric tension even in single-column layouts through offset alignment

---

## CSS / Design Techniques

### Bauhaus Card Component

```css
.bau-card {
  background: var(--bau-white);
  border: 3px solid var(--bau-black);
  padding: 32px;
  position: relative;
}

/* Geometric accent on card */
.bau-card::before {
  content: '';
  position: absolute;
  top: -3px;
  left: -3px;
  width: 40px;
  height: 40px;
  background: var(--bau-red);
}

.bau-card-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
  gap: 32px;
}
```

### Bauhaus Button

```css
.bau-button {
  display: inline-flex;
  align-items: center;
  justify-content: center;
  background: var(--bau-black);
  color: var(--bau-white);
  border: 3px solid var(--bau-black);
  border-radius: 0;
  padding: 14px 36px;
  font-family: 'Jost', sans-serif;
  font-weight: 700;
  font-size: 0.9rem;
  letter-spacing: 0.08em;
  text-transform: uppercase;
  cursor: pointer;
  transition: background 0.2s ease, color 0.2s ease;
  text-decoration: none;
}

.bau-button:hover {
  background: var(--bau-red);
  border-color: var(--bau-red);
}

/* Primary color variants */
.bau-button--red {
  background: var(--bau-red);
  border-color: var(--bau-red);
}

.bau-button--red:hover {
  background: var(--bau-red-dark);
  border-color: var(--bau-red-dark);
}

.bau-button--blue {
  background: var(--bau-blue);
  border-color: var(--bau-blue);
}

.bau-button--blue:hover {
  background: var(--bau-blue-dark);
  border-color: var(--bau-blue-dark);
}

/* Outline variant */
.bau-button--outline {
  background: transparent;
  color: var(--bau-black);
}

.bau-button--outline:hover {
  background: var(--bau-black);
  color: var(--bau-white);
}
```

### Navigation Bar

```css
.bau-nav {
  display: flex;
  align-items: center;
  justify-content: space-between;
  max-width: 1200px;
  margin: 0 auto;
  padding: 24px 40px;
  border-bottom: 4px solid var(--bau-black);
}

.bau-nav__logo {
  display: flex;
  align-items: center;
  gap: 12px;
  font-family: 'Jost', sans-serif;
  font-weight: 900;
  font-size: 1.5rem;
  color: var(--bau-black);
  text-decoration: none;
  text-transform: uppercase;
  letter-spacing: 0.04em;
}

.bau-nav__logo-shape {
  width: 32px;
  height: 32px;
  background: var(--bau-red);
  border-radius: 50%;
}

.bau-nav__links {
  display: flex;
  gap: 32px;
  list-style: none;
  margin: 0;
  padding: 0;
}

.bau-nav__links a {
  font-family: 'Jost', sans-serif;
  font-weight: 500;
  font-size: 0.85rem;
  color: var(--bau-black);
  text-decoration: none;
  text-transform: uppercase;
  letter-spacing: 0.06em;
  transition: color 0.2s ease;
}

.bau-nav__links a:hover {
  color: var(--bau-red);
}
```

### Hero Section

```css
.bau-hero {
  display: flex;
  align-items: center;
  justify-content: space-between;
  max-width: 1200px;
  margin: 0 auto;
  padding: 80px 40px;
  gap: 60px;
  position: relative;
}

.bau-hero__content {
  flex: 1;
  max-width: 560px;
}

.bau-hero__content h1 {
  font-size: clamp(3rem, 7vw, 5.5rem);
  font-weight: 900;
  text-transform: uppercase;
  line-height: 0.95;
  margin-bottom: 1.5rem;
}

.bau-hero__content p {
  font-size: 1.1rem;
  color: var(--bau-dark-gray);
  margin-bottom: 2rem;
  max-width: 420px;
  line-height: 1.7;
}

.bau-hero__visual {
  flex: 1;
  display: flex;
  justify-content: center;
  align-items: center;
}

@media (max-width: 768px) {
  .bau-hero {
    flex-direction: column;
    text-align: center;
    padding: 60px 24px;
    gap: 40px;
  }
}
```

### Feature Grid

```css
.bau-features {
  background: var(--bau-bg-secondary);
  padding: 80px 0;
  border-top: 4px solid var(--bau-black);
  border-bottom: 4px solid var(--bau-black);
}

.bau-features__header {
  max-width: 1200px;
  margin: 0 auto;
  padding: 0 40px 60px;
}

.bau-features__header h2 {
  font-size: 2.5rem;
  text-transform: uppercase;
}

.bau-features__grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
  gap: 32px;
  max-width: 1200px;
  margin: 0 auto;
  padding: 0 40px;
}

.bau-feature {
  border: 3px solid var(--bau-black);
  background: var(--bau-white);
  padding: 32px;
}

.bau-feature__shape {
  width: 48px;
  height: 48px;
  margin-bottom: 20px;
}

.bau-feature__shape--circle {
  background: var(--bau-blue);
  border-radius: 50%;
}

.bau-feature__shape--square {
  background: var(--bau-red);
}

.bau-feature__shape--triangle {
  width: 0;
  height: 0;
  border-left: 24px solid transparent;
  border-right: 24px solid transparent;
  border-bottom: 48px solid var(--bau-yellow);
  background: transparent;
}

.bau-feature h3 {
  font-size: 1.15rem;
  margin-bottom: 0.75rem;
  text-transform: uppercase;
}

.bau-feature p {
  font-size: 0.95rem;
  color: var(--bau-dark-gray);
  line-height: 1.6;
}
```

### Geometric Composition Block

```css
.bau-composition {
  position: relative;
  width: 400px;
  height: 400px;
}

.bau-composition__circle {
  position: absolute;
  width: 200px;
  height: 200px;
  background: var(--bau-blue);
  border-radius: 50%;
  top: 20px;
  right: 40px;
}

.bau-composition__square {
  position: absolute;
  width: 160px;
  height: 160px;
  background: var(--bau-red);
  bottom: 40px;
  left: 20px;
}

.bau-composition__triangle {
  position: absolute;
  width: 0;
  height: 0;
  border-left: 80px solid transparent;
  border-right: 80px solid transparent;
  border-bottom: 140px solid var(--bau-yellow);
  top: 140px;
  left: 120px;
}

.bau-composition__line {
  position: absolute;
  height: 4px;
  width: 300px;
  background: var(--bau-black);
  transform: rotate(-15deg);
  top: 200px;
  left: 50px;
}
```

---

## Design Do's and Don'ts

### Do

- Use only primary colors (red, yellow, blue) plus black and white
- Build compositions from circles, triangles, and squares
- Use bold, geometric sans-serif typography in uppercase for headings
- Employ thick black rules and borders to define spatial structure
- Create asymmetric layouts with dynamic visual tension
- Treat type as a graphic element equal to shapes and color
- Reference the Kandinsky shape-color theory (yellow triangle, red square, blue circle)
- Maintain strict grid alignment even in asymmetric compositions

### Don't

- Use gradients, shadows, or any depth simulation
- Apply decorative ornament, flourishes, or serif typefaces
- Use soft, pastel, or muted color palettes
- Create perfectly symmetrical layouts -- embrace dynamic asymmetry
- Use rounded corners (except for circles); geometry should be precise
- Add photographic imagery without geometric masking or treatment
- Mix too many secondary or tertiary colors
- Ignore the grid; randomness contradicts Bauhaus principles

---

## Related Aesthetics

| Aesthetic | Relationship to Bauhaus |
|-----------|------------------------|
| **Flat Design** | Digital descendent; applies Bauhaus flat-color, geometric, function-first principles to UI |
| **International Typographic Style** | Direct successor; Swiss designers formalized Bauhaus grid and typography principles into a systematic methodology |
| **De Stijl** | Contemporary sibling movement; shared the reductive geometric philosophy but restricted to strict horizontals and verticals |
| **Constructivism** | Parallel avant-garde movement; shared the integration of art and industry but with a revolutionary Soviet political dimension |
| **Minimalism** | Philosophical descendent; took the Bauhaus reductive impulse to its logical extreme |
| **Modernisme** | Architectural parallel; shared the belief in honest materials and functional form |
| **Memphis Design** | Postmodern reaction against Bauhaus; deliberately violated Bauhaus rules with pattern, decoration, and pastels |
| **Material Design** | Google's system borrows Bauhaus grid discipline and flat color while reintroducing shadow for hierarchy |
| **Neubrutalism** | Shares the raw honesty and bold graphic presence but rejects Bauhaus refinement for deliberate roughness |
| **Space Age** | Mid-century descendant; applied geometric and functional thinking to futuristic forms |

---

## Quick-Start: Minimal Bauhaus Page Template

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Bauhaus Page</title>
  <link href="https://fonts.googleapis.com/css2?family=Jost:wght@400;500;700;900&family=Work+Sans:wght@400;500&display=swap" rel="stylesheet">
  <style>
    :root {
      --bau-red: #e3000b;
      --bau-yellow: #ffd700;
      --bau-blue: #003da5;
      --bau-black: #000000;
      --bau-white: #ffffff;
      --bau-warm-gray: #d4d0c8;
      --bau-dark-gray: #3c3c3c;
      --bau-bg-secondary: #f5f3ef;
    }

    * { margin: 0; padding: 0; box-sizing: border-box; }

    body {
      background: var(--bau-white);
      color: var(--bau-black);
      font-family: 'Work Sans', sans-serif;
      font-weight: 400;
      line-height: 1.7;
    }

    h1, h2, h3 {
      font-family: 'Jost', sans-serif;
      font-weight: 700;
      text-transform: uppercase;
      line-height: 1.05;
    }

    /* Navigation */
    nav {
      display: flex;
      align-items: center;
      justify-content: space-between;
      max-width: 1200px;
      margin: 0 auto;
      padding: 24px 40px;
      border-bottom: 4px solid var(--bau-black);
    }

    nav .logo {
      display: flex;
      align-items: center;
      gap: 12px;
      font-family: 'Jost', sans-serif;
      font-weight: 900;
      font-size: 1.5rem;
      color: var(--bau-black);
      text-decoration: none;
      text-transform: uppercase;
    }

    nav .logo-circle {
      width: 28px;
      height: 28px;
      background: var(--bau-red);
      border-radius: 50%;
    }

    nav ul {
      display: flex;
      gap: 28px;
      list-style: none;
    }

    nav ul a {
      font-family: 'Jost', sans-serif;
      font-weight: 500;
      font-size: 0.85rem;
      color: var(--bau-black);
      text-decoration: none;
      text-transform: uppercase;
      letter-spacing: 0.06em;
      transition: color 0.2s;
    }

    nav ul a:hover { color: var(--bau-red); }

    /* Hero */
    .hero {
      display: flex;
      align-items: center;
      justify-content: space-between;
      max-width: 1200px;
      margin: 0 auto;
      padding: 80px 40px;
      gap: 40px;
    }

    .hero-content { flex: 1; max-width: 560px; }

    .hero h1 {
      font-size: clamp(3rem, 7vw, 5.5rem);
      font-weight: 900;
      margin-bottom: 1.5rem;
      line-height: 0.95;
    }

    .hero h1 span.red { color: var(--bau-red); }
    .hero h1 span.blue { color: var(--bau-blue); }

    .hero p {
      font-size: 1.1rem;
      color: var(--bau-dark-gray);
      margin-bottom: 2rem;
      max-width: 400px;
    }

    .btn {
      display: inline-block;
      background: var(--bau-black);
      color: var(--bau-white);
      border: 3px solid var(--bau-black);
      padding: 14px 36px;
      font-family: 'Jost', sans-serif;
      font-weight: 700;
      font-size: 0.9rem;
      text-transform: uppercase;
      letter-spacing: 0.06em;
      text-decoration: none;
      cursor: pointer;
      transition: background 0.2s, color 0.2s;
    }

    .btn:hover {
      background: var(--bau-red);
      border-color: var(--bau-red);
    }

    .hero-visual {
      flex: 1;
      display: flex;
      justify-content: center;
    }

    /* Features */
    .features {
      background: var(--bau-bg-secondary);
      padding: 80px 0;
      border-top: 4px solid var(--bau-black);
      border-bottom: 4px solid var(--bau-black);
    }

    .features h2 {
      font-size: 2.5rem;
      max-width: 1200px;
      margin: 0 auto;
      padding: 0 40px 48px;
    }

    .features-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
      gap: 32px;
      max-width: 1200px;
      margin: 0 auto;
      padding: 0 40px;
    }

    .feature {
      background: var(--bau-white);
      border: 3px solid var(--bau-black);
      padding: 32px;
    }

    .feature .shape {
      width: 44px;
      height: 44px;
      margin-bottom: 20px;
    }

    .shape-circle { background: var(--bau-blue); border-radius: 50%; }
    .shape-square { background: var(--bau-red); }
    .shape-triangle {
      width: 0 !important; height: 0 !important;
      border-left: 22px solid transparent;
      border-right: 22px solid transparent;
      border-bottom: 44px solid var(--bau-yellow);
      background: transparent !important;
    }

    .feature h3 { font-size: 1.1rem; margin-bottom: 0.5rem; }
    .feature p { color: var(--bau-dark-gray); font-size: 0.95rem; }

    /* Statement */
    .statement {
      background: var(--bau-red);
      color: var(--bau-white);
      text-align: center;
      padding: 80px 40px;
    }

    .statement h2 {
      font-size: clamp(2rem, 5vw, 3.5rem);
      font-weight: 900;
      margin-bottom: 1.5rem;
    }

    .statement p {
      font-size: 1.15rem;
      max-width: 500px;
      margin: 0 auto 2rem;
      opacity: 0.9;
    }

    .statement .btn {
      background: var(--bau-white);
      color: var(--bau-red);
      border-color: var(--bau-white);
    }

    .statement .btn:hover {
      background: var(--bau-black);
      color: var(--bau-white);
      border-color: var(--bau-black);
    }

    /* Footer */
    footer {
      background: var(--bau-black);
      color: var(--bau-warm-gray);
      text-align: center;
      padding: 40px;
      font-size: 0.85rem;
    }

    @media (max-width: 768px) {
      .hero {
        flex-direction: column;
        text-align: center;
        padding: 60px 24px;
      }
      nav { padding: 20px 24px; }
      nav ul { gap: 16px; }
      .features h2 { padding: 0 24px 40px; }
      .features-grid { padding: 0 24px; }
    }
  </style>
</head>
<body>
  <nav>
    <a href="#" class="logo">
      <div class="logo-circle"></div>
      Bauhaus
    </a>
    <ul>
      <li><a href="#">Manifest</a></li>
      <li><a href="#">Work</a></li>
      <li><a href="#">Archive</a></li>
      <li><a href="#">Contact</a></li>
    </ul>
  </nav>

  <section class="hero">
    <div class="hero-content">
      <h1><span class="red">Form</span> Follows <span class="blue">Function</span></h1>
      <p>Design reduced to its geometric essence. Every shape, every color, every line exists for a reason.</p>
      <a href="#" class="btn">Explore</a>
    </div>
    <div class="hero-visual">
      <svg width="360" height="360" viewBox="0 0 360 360" fill="none" xmlns="http://www.w3.org/2000/svg">
        <circle cx="200" cy="120" r="90" fill="#003DA5"/>
        <rect x="40" y="180" width="140" height="140" fill="#E3000B"/>
        <polygon points="240,360 320,200 400,360" fill="#FFD700"/>
        <line x1="20" y1="160" x2="340" y2="160" stroke="#000000" stroke-width="4"/>
        <line x1="180" y1="20" x2="180" y2="340" stroke="#000000" stroke-width="4"/>
      </svg>
    </div>
  </section>

  <section class="features">
    <h2>Principles</h2>
    <div class="features-grid">
      <div class="feature">
        <div class="shape shape-circle"></div>
        <h3>Unity</h3>
        <p>Art and technology united. Design that serves industry without sacrificing beauty.</p>
      </div>
      <div class="feature">
        <div class="shape shape-square"></div>
        <h3>Function</h3>
        <p>Every element justified by purpose. Ornament is eliminated; honesty remains.</p>
      </div>
      <div class="feature">
        <div class="shape shape-triangle"></div>
        <h3>Geometry</h3>
        <p>Circle, square, triangle. The universal vocabulary of form, reduced to fundamentals.</p>
      </div>
    </div>
  </section>

  <section class="statement">
    <h2>Less But Better</h2>
    <p>The Bauhaus taught us that design is not about adding more, but about finding what is essential.</p>
    <a href="#" class="btn">Read Manifesto</a>
  </section>

  <footer>
    <p>Built on Bauhaus principles. Weimar 1919 -- Dessau 1925 -- Berlin 1932.</p>
  </footer>
</body>
</html>
```
