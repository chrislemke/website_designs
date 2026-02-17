# De Stijl

Mondrian rectangles in red, yellow, blue on white with strict horizontal and vertical black lines. De Stijl ("The Style"), founded in the Netherlands in 1917 by Theo van Doesburg and Piet Mondrian, is a radical reductionist art movement that strips visual composition down to its absolute essentials: straight lines (exclusively horizontal and vertical), rectangular planes, and the three primary colors plus black, white, and gray. No curves, no diagonals, no ornament -- only pure geometric abstraction expressing universal harmony through asymmetric balance.

---

## Visual Characteristics

### Core Design Traits

- **Strict horizontal and vertical lines only** -- no diagonals, no curves, no angles; every line is either perfectly horizontal or perfectly vertical
- **Rectangular planes of primary color** -- red, yellow, and blue blocks of varying size arranged on a white ground
- **Thick black grid lines** -- heavy black rules (4-8px) delineate and separate the rectangular color planes
- **Asymmetric balance** -- compositions feel balanced through proportional weight distribution, never through mirror symmetry
- **White as the dominant field** -- white occupies the majority of the composition; color blocks are strategic accents, not backgrounds
- **No representational imagery** -- purely abstract; no photographs, no illustrations, no icons that depict real-world objects
- **No gradients, no textures, no shadows** -- every surface is a flat, solid color with no depth simulation
- **Open-ended compositions** -- Mondrian's compositions often suggest extension beyond the canvas edge; grids imply continuation
- **Mathematical proportions** -- relationships between rectangles follow harmonic ratios, creating visual music
- **Limited palette, maximum expression** -- the restriction to three primaries plus neutrals forces compositional mastery

### Design Principles

- Reduce to the absolute universal elements: horizontal, vertical, primary color, neutral
- Seek dynamic equilibrium through asymmetric arrangement of unequal parts
- Eliminate the individual and particular in favor of the universal and absolute
- Every line and plane must be necessary; if it can be removed, it should be
- Tension between elements creates visual rhythm; static symmetry is avoided
- Color blocks carry visual weight proportional to their area and saturation
- The grid is the composition -- it is not a scaffold beneath the design, it is the design itself
- White space is active and compositional, never passive or leftover

---

## Color Palette

### De Stijl Core Palette

The De Stijl palette is the most restricted of any design movement: three primary colors, black, white, and optionally gray. Every other color is excluded.

| Color Name | Hex | Role / Usage |
|------------|-----|-------------|
| **Mondrian Red** | `#D40000` | Primary accent blocks, key interactive elements |
| **Mondrian Yellow** | `#FFD200` | Secondary accent blocks, highlights, smaller planes |
| **Mondrian Blue** | `#0047AB` | Tertiary accent blocks, links, supporting color planes |
| **Grid Black** | `#000000` | Grid lines, text, structural rules, borders |
| **Field White** | `#FFFFFF` | Dominant background, majority of the composition |
| **Off-White** | `#F7F5F0` | Slightly warm alternative background for screens |
| **Light Gray** | `#D9D9D9` | Optional neutral plane, subtle section separation |
| **Mid Gray** | `#808080` | Occasional neutral block, secondary text |

### CSS Custom Properties

```css
:root {
  /* Primary triad */
  --ds-red: #d40000;
  --ds-yellow: #ffd200;
  --ds-blue: #0047ab;

  /* Hover/active states */
  --ds-red-dark: #a80000;
  --ds-yellow-dark: #ccaa00;
  --ds-blue-dark: #003580;

  /* Neutrals */
  --ds-black: #000000;
  --ds-white: #ffffff;
  --ds-off-white: #f7f5f0;
  --ds-light-gray: #d9d9d9;
  --ds-mid-gray: #808080;

  /* Grid */
  --ds-grid-width: 6px;
  --ds-grid-color: #000000;

  /* Text */
  --ds-text-primary: #000000;
  --ds-text-secondary: #808080;
}
```

### Color Usage Guidelines

- **Only use red, yellow, and blue** -- no green, no orange, no purple, no secondary or tertiary colors
- White dominates; color blocks are accents that occupy perhaps 15-30% of the total composition
- Red carries the most visual weight and should be used for the most important elements
- Yellow is visually lighter and works for secondary accents and smaller blocks
- Blue recedes and serves well for supporting areas and links
- Black is exclusively structural: grid lines, text, and borders
- Gray may appear as an occasional neutral block but should not dominate
- Color blocks should be rectangular and aligned to the grid; never circular or irregular

---

## Typography

### Typeface Characteristics

De Stijl typography is:

- **Geometric sans-serif** -- stripped of any calligraphic or decorative quality
- **Blocky and structural** -- letterforms echo the rectangular geometry of the compositions
- **Uppercase or small-caps preferred** -- uniformity of letter height reinforces the grid
- **Tight or normal tracking** -- letters form dense, cohesive blocks of text
- **Weight as the only variation** -- hierarchy created through size and weight, never through style (italic) or decoration
- **Aligned to the grid** -- text blocks positioned along grid lines like any other rectangular element

### Recommended Web Fonts (Google Fonts)

| Font | Style | Best For |
|------|-------|----------|
| **Jost** | Geometric sans (Futura-like) | Display headings, hero text |
| **Archivo** | Grotesque geometric | Headings and body text, versatile |
| **Barlow** | Slightly condensed geometric | Navigation, labels, compact layouts |
| **DM Sans** | Low-contrast geometric | Body text, readable at small sizes |
| **Work Sans** | Geometric grotesque | Body text, editorial content |
| **Poppins** | Pure geometric circles | Modern interpretation of geometric purity |
| **Inter** | Screen-optimized humanist | Body text, UI elements |
| **Bebas Neue** | Condensed uppercase display | Large display text, poster-style headings |
| **Oswald** | Condensed gothic | Uppercase headings, navigational labels |
| **Archivo Black** | Ultra-bold grotesque | Maximum-impact display text |

### Font Pairing Suggestions

| Heading Font | Body Font | Character |
|-------------|-----------|-----------|
| **Bebas Neue** (400) | **Work Sans** (400) | Bold, architectural display |
| **Jost** (700) | **DM Sans** (400) | Geometric precision |
| **Archivo Black** (400) | **Inter** (400) | Ultra-bold structural impact |
| **Oswald** (600) | **Barlow** (400) | Condensed, efficient |
| **Poppins** (700) | **Work Sans** (400) | Clean geometric consistency |

### Typography CSS Example

```css
/* Import fonts */
@import url('https://fonts.googleapis.com/css2?family=Bebas+Neue&family=Work+Sans:wght@400;500;600&display=swap');

/* Headings */
h1, h2, h3, h4, h5, h6 {
  font-family: 'Bebas Neue', 'Impact', sans-serif;
  font-weight: 400;
  color: var(--ds-text-primary);
  line-height: 1.0;
  letter-spacing: 0.04em;
  text-transform: uppercase;
}

/* Display / Hero text */
.ds-display {
  font-family: 'Bebas Neue', sans-serif;
  font-size: clamp(4rem, 10vw, 8rem);
  letter-spacing: 0.06em;
  line-height: 0.9;
  text-transform: uppercase;
}

/* Body text */
body {
  font-family: 'Work Sans', sans-serif;
  font-weight: 400;
  font-size: 1rem;
  line-height: 1.7;
  color: var(--ds-text-primary);
}

/* Labels and navigation */
.ds-label {
  font-family: 'Bebas Neue', sans-serif;
  font-weight: 400;
  font-size: 0.9rem;
  letter-spacing: 0.1em;
  text-transform: uppercase;
}

/* Caption */
.ds-caption {
  font-family: 'Work Sans', sans-serif;
  font-weight: 400;
  font-size: 0.85rem;
  color: var(--ds-mid-gray);
  line-height: 1.5;
}
```

---

## Layout Principles

### Grid and Structure

- **The Mondrian grid** -- the layout itself is a De Stijl composition; thick black lines divide the page into rectangular zones of varying sizes
- **No equal divisions** -- rectangles are deliberately unequal to create dynamic asymmetric tension
- **CSS Grid as the primary tool** -- `grid-template-columns` and `grid-template-rows` with explicit track sizes mirror the Mondrian grid
- **Thick black gaps/borders** -- grid gaps are rendered as 4-8px black lines using borders or gaps with a black background container
- **Color blocks as sections** -- some grid cells are filled with primary colors; most remain white
- **Content constrained to cells** -- text and interactive elements live within their assigned grid cells, never overlapping boundaries
- **Edge-to-edge grid** -- the composition can extend to the viewport edges, implying continuation beyond the screen

### Section Organization

- **Navigation**: A horizontal black-bordered bar; logo text in one cell, links in adjacent cells, separated by vertical black rules
- **Hero**: The largest grid cell; oversized headline text with one or two color block accents in adjacent cells
- **Features**: Multiple grid cells of varying sizes, each containing a feature; cells bordered by thick black lines
- **Content**: Text occupies white cells; adjacent color cells provide visual accent without containing content
- **CTA**: A primary-color-filled cell with contrasting text and button
- **Footer**: A narrow horizontal row at the bottom of the grid composition, black background

### Responsive Approach

- Grid simplifies from complex multi-cell compositions to stacked rectangles on mobile
- Black borders and grid lines maintain their weight at all sizes
- Color block proportions shift but the palette remains constant
- Typography scales with `clamp()` while maintaining grid alignment
- The grid metaphor is preserved even in single-column layouts through bordered sections

---

## CSS / Design Techniques

### Mondrian Grid Layout

```css
.ds-grid {
  display: grid;
  grid-template-columns: 2fr 1fr 1fr;
  grid-template-rows: auto auto auto;
  gap: 0;
  border: 6px solid var(--ds-black);
  max-width: 1200px;
  margin: 0 auto;
}

.ds-grid > * {
  border: 3px solid var(--ds-black);
  padding: 32px;
}

/* Color block cells */
.ds-cell--red { background: var(--ds-red); color: var(--ds-white); }
.ds-cell--yellow { background: var(--ds-yellow); color: var(--ds-black); }
.ds-cell--blue { background: var(--ds-blue); color: var(--ds-white); }
.ds-cell--white { background: var(--ds-white); color: var(--ds-black); }
.ds-cell--gray { background: var(--ds-light-gray); color: var(--ds-black); }
```

### De Stijl Card Component

```css
.ds-card {
  background: var(--ds-white);
  border: 4px solid var(--ds-black);
  padding: 32px;
  position: relative;
}

/* Color accent bar on card edge */
.ds-card--red-accent::before {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  width: 8px;
  height: 100%;
  background: var(--ds-red);
}

.ds-card--blue-accent::before {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 8px;
  background: var(--ds-blue);
}

.ds-card-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
  border: 4px solid var(--ds-black);
}

.ds-card-grid .ds-card {
  border: 2px solid var(--ds-black);
}
```

### De Stijl Button

```css
.ds-button {
  display: inline-block;
  background: var(--ds-black);
  color: var(--ds-white);
  border: none;
  border-radius: 0;
  padding: 14px 40px;
  font-family: 'Bebas Neue', sans-serif;
  font-size: 1.1rem;
  letter-spacing: 0.1em;
  text-transform: uppercase;
  cursor: pointer;
  text-decoration: none;
  transition: background 0.2s ease;
}

.ds-button:hover {
  background: var(--ds-red);
}

/* Primary color variants */
.ds-button--red {
  background: var(--ds-red);
}

.ds-button--red:hover {
  background: var(--ds-red-dark);
}

.ds-button--blue {
  background: var(--ds-blue);
}

.ds-button--blue:hover {
  background: var(--ds-blue-dark);
}

/* Outline variant */
.ds-button--outline {
  background: transparent;
  color: var(--ds-black);
  border: 4px solid var(--ds-black);
  padding: 10px 36px;
}

.ds-button--outline:hover {
  background: var(--ds-black);
  color: var(--ds-white);
}
```

### Navigation Bar

```css
.ds-nav {
  display: flex;
  align-items: stretch;
  border: 4px solid var(--ds-black);
  border-bottom-width: 6px;
  max-width: 1200px;
  margin: 0 auto;
}

.ds-nav__logo {
  display: flex;
  align-items: center;
  padding: 16px 32px;
  background: var(--ds-red);
  font-family: 'Bebas Neue', sans-serif;
  font-size: 1.5rem;
  color: var(--ds-white);
  text-decoration: none;
  letter-spacing: 0.08em;
  border-right: 4px solid var(--ds-black);
}

.ds-nav__links {
  display: flex;
  align-items: stretch;
  list-style: none;
  margin: 0;
  padding: 0;
  flex: 1;
}

.ds-nav__links li {
  border-right: 4px solid var(--ds-black);
}

.ds-nav__links li:last-child {
  border-right: none;
}

.ds-nav__links a {
  display: flex;
  align-items: center;
  padding: 16px 28px;
  font-family: 'Bebas Neue', sans-serif;
  font-size: 1rem;
  color: var(--ds-black);
  text-decoration: none;
  letter-spacing: 0.08em;
  text-transform: uppercase;
  transition: background 0.2s ease, color 0.2s ease;
}

.ds-nav__links a:hover {
  background: var(--ds-yellow);
}
```

### Hero Section

```css
.ds-hero {
  display: grid;
  grid-template-columns: 3fr 1fr;
  grid-template-rows: 1fr auto;
  border: 4px solid var(--ds-black);
  border-top: none;
  max-width: 1200px;
  margin: 0 auto;
}

.ds-hero__content {
  padding: 80px 60px;
  border-right: 4px solid var(--ds-black);
  grid-row: span 2;
}

.ds-hero__content h1 {
  font-size: clamp(3.5rem, 8vw, 7rem);
  margin-bottom: 1.5rem;
  line-height: 0.9;
}

.ds-hero__content p {
  font-size: 1.1rem;
  max-width: 480px;
  margin-bottom: 2.5rem;
  color: var(--ds-mid-gray);
  line-height: 1.7;
}

.ds-hero__block-blue {
  background: var(--ds-blue);
  min-height: 120px;
  border-bottom: 4px solid var(--ds-black);
}

.ds-hero__block-yellow {
  background: var(--ds-yellow);
  min-height: 80px;
}

@media (max-width: 768px) {
  .ds-hero {
    grid-template-columns: 1fr;
  }
  .ds-hero__content {
    border-right: none;
    border-bottom: 4px solid var(--ds-black);
    padding: 60px 28px;
  }
  .ds-hero__block-blue { min-height: 40px; }
  .ds-hero__block-yellow { min-height: 30px; }
}
```

### Feature Grid (Mondrian-style)

```css
.ds-features {
  display: grid;
  grid-template-columns: 1fr 1fr 1fr;
  border: 4px solid var(--ds-black);
  border-top: none;
  max-width: 1200px;
  margin: 0 auto;
}

.ds-feature {
  padding: 40px 32px;
  border-right: 4px solid var(--ds-black);
}

.ds-feature:last-child {
  border-right: none;
}

.ds-feature__accent {
  width: 40px;
  height: 8px;
  margin-bottom: 24px;
}

.ds-feature h3 {
  font-size: 1.3rem;
  margin-bottom: 0.75rem;
}

.ds-feature p {
  font-size: 0.95rem;
  color: var(--ds-mid-gray);
  line-height: 1.6;
}

@media (max-width: 768px) {
  .ds-features {
    grid-template-columns: 1fr;
  }
  .ds-feature {
    border-right: none;
    border-bottom: 4px solid var(--ds-black);
  }
  .ds-feature:last-child {
    border-bottom: none;
  }
}
```

---

## Design Do's and Don'ts

### Do

- Use only horizontal and vertical lines -- this is the most fundamental rule of De Stijl
- Restrict the palette to red, yellow, blue, black, white, and gray exclusively
- Create asymmetric compositions where no two adjacent rectangles are the same size
- Use thick black lines (4-8px) as the structural grid
- Let white dominate the composition; use primary colors as strategic accents
- Treat the grid as the design itself, not as a hidden scaffold
- Reference Mondrian's compositional principles of dynamic equilibrium
- Use uppercase geometric sans-serif typography aligned to the grid

### Don't

- Use diagonal lines, curves, or circles -- these violate the core De Stijl principle
- Introduce secondary colors (green, orange, purple) or any non-primary hues
- Create symmetrical layouts -- De Stijl demands dynamic asymmetry
- Use thin or invisible grid lines; the black rules are a visible, defining element
- Add shadows, gradients, textures, or any depth simulation
- Include representational imagery, illustrations, or photographs
- Use serif, script, or decorative typefaces
- Fill the entire composition with color -- white must remain the dominant field
- Round any corners; every element is a sharp rectangle

---

## Related Aesthetics

| Aesthetic | Relationship to De Stijl |
|-----------|-------------------------|
| **Bauhaus** | Contemporary sibling; shared reductive geometry and primary colors but allowed diagonals and circles |
| **Minimalism** | Philosophical descendant; took De Stijl's reductive impulse further, eliminating even the primary colors |
| **International Typographic Style** | Successor movement; formalized the grid system De Stijl pioneered into a comprehensive typographic methodology |
| **Flat Design** | Digital echo; shares flat color and geometric simplicity but without De Stijl's strict compositional rules |
| **Constructivism** | Parallel avant-garde; shared the geometric abstraction but embraced diagonals and revolutionary politics |
| **Modernisme** | Architectural parallel; shared the belief in pure form and rational construction |
| **Neubrutalism** | Shares thick borders and bold structure but embraces rawness over De Stijl's harmonic precision |
| **Memphis Design** | Postmodern reaction; deliberately violated De Stijl's rules with curves, patterns, and pastels |
| **Material Design** | Google's system borrows grid discipline and flat color while adding shadow layers for hierarchy |
| **Mondrian (fashion/product)** | Direct commercial application of De Stijl compositions to clothing, furniture, and product surfaces |

---

## Quick-Start: Minimal De Stijl Page Template

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>De Stijl Page</title>
  <link href="https://fonts.googleapis.com/css2?family=Bebas+Neue&family=Work+Sans:wght@400;500;600&display=swap" rel="stylesheet">
  <style>
    :root {
      --ds-red: #d40000;
      --ds-yellow: #ffd200;
      --ds-blue: #0047ab;
      --ds-black: #000000;
      --ds-white: #ffffff;
      --ds-light-gray: #d9d9d9;
      --ds-mid-gray: #808080;
      --ds-border: 4px solid #000000;
    }

    * { margin: 0; padding: 0; box-sizing: border-box; }

    body {
      background: var(--ds-white);
      color: var(--ds-black);
      font-family: 'Work Sans', sans-serif;
      font-weight: 400;
      line-height: 1.7;
    }

    h1, h2, h3 {
      font-family: 'Bebas Neue', sans-serif;
      font-weight: 400;
      text-transform: uppercase;
      letter-spacing: 0.04em;
      line-height: 0.95;
    }

    .page {
      max-width: 1200px;
      margin: 0 auto;
      border-left: 6px solid var(--ds-black);
      border-right: 6px solid var(--ds-black);
    }

    /* Navigation */
    nav {
      display: flex;
      align-items: stretch;
      border-top: 6px solid var(--ds-black);
      border-bottom: var(--ds-border);
    }

    nav a.logo {
      display: flex;
      align-items: center;
      padding: 16px 32px;
      background: var(--ds-red);
      color: var(--ds-white);
      font-family: 'Bebas Neue', sans-serif;
      font-size: 1.6rem;
      text-decoration: none;
      letter-spacing: 0.1em;
      border-right: var(--ds-border);
    }

    nav ul {
      display: flex;
      list-style: none;
      flex: 1;
    }

    nav ul li {
      border-right: var(--ds-border);
    }

    nav ul li:last-child { border-right: none; }

    nav ul a {
      display: flex;
      align-items: center;
      padding: 16px 24px;
      font-family: 'Bebas Neue', sans-serif;
      font-size: 1rem;
      color: var(--ds-black);
      text-decoration: none;
      letter-spacing: 0.08em;
      text-transform: uppercase;
      transition: background 0.2s;
    }

    nav ul a:hover { background: var(--ds-yellow); }

    /* Hero - Mondrian grid */
    .hero {
      display: grid;
      grid-template-columns: 3fr 1fr;
      grid-template-rows: 1fr auto;
    }

    .hero-content {
      padding: 80px 60px;
      border-right: var(--ds-border);
      border-bottom: var(--ds-border);
      grid-row: span 2;
    }

    .hero h1 {
      font-size: clamp(3.5rem, 8vw, 6.5rem);
      margin-bottom: 1.5rem;
    }

    .hero h1 .red { color: var(--ds-red); }
    .hero h1 .blue { color: var(--ds-blue); }

    .hero p {
      font-size: 1.1rem;
      color: var(--ds-mid-gray);
      max-width: 480px;
      margin-bottom: 2.5rem;
    }

    .btn {
      display: inline-block;
      background: var(--ds-black);
      color: var(--ds-white);
      padding: 14px 40px;
      font-family: 'Bebas Neue', sans-serif;
      font-size: 1.1rem;
      letter-spacing: 0.1em;
      text-transform: uppercase;
      text-decoration: none;
      transition: background 0.2s;
    }

    .btn:hover { background: var(--ds-red); }

    .hero-block-blue {
      background: var(--ds-blue);
      border-bottom: var(--ds-border);
      min-height: 140px;
    }

    .hero-block-yellow {
      background: var(--ds-yellow);
      min-height: 80px;
    }

    /* Features */
    .features {
      display: grid;
      grid-template-columns: 1fr 1fr 1fr;
      border-bottom: var(--ds-border);
    }

    .feature {
      padding: 48px 32px;
      border-right: var(--ds-border);
    }

    .feature:last-child { border-right: none; }

    .feature-accent {
      width: 36px;
      height: 8px;
      margin-bottom: 24px;
    }

    .feature h3 { font-size: 1.4rem; margin-bottom: 0.75rem; }
    .feature p { color: var(--ds-mid-gray); font-size: 0.95rem; }

    /* CTA - color block section */
    .cta {
      display: grid;
      grid-template-columns: 1fr auto;
      border-bottom: var(--ds-border);
    }

    .cta-content {
      padding: 60px;
      border-right: var(--ds-border);
    }

    .cta h2 { font-size: 2.5rem; margin-bottom: 1rem; }
    .cta p { color: var(--ds-mid-gray); margin-bottom: 2rem; max-width: 400px; }

    .cta-block {
      background: var(--ds-red);
      width: 180px;
    }

    /* Footer */
    footer {
      display: grid;
      grid-template-columns: auto 1fr auto;
      background: var(--ds-black);
      color: var(--ds-light-gray);
    }

    .footer-block {
      background: var(--ds-yellow);
      width: 60px;
      border-right: var(--ds-border);
    }

    .footer-text {
      padding: 28px 32px;
      font-size: 0.85rem;
      border-right: var(--ds-border);
    }

    .footer-block-blue {
      background: var(--ds-blue);
      width: 40px;
    }

    @media (max-width: 768px) {
      .hero {
        grid-template-columns: 1fr;
      }
      .hero-content {
        border-right: none;
        border-bottom: var(--ds-border);
        padding: 60px 28px;
      }
      .hero-block-blue { min-height: 40px; }
      .hero-block-yellow { min-height: 30px; }
      .features {
        grid-template-columns: 1fr;
      }
      .feature {
        border-right: none;
        border-bottom: var(--ds-border);
      }
      .feature:last-child { border-bottom: none; }
      .cta { grid-template-columns: 1fr; }
      .cta-content { border-right: none; }
      .cta-block { width: 100%; height: 40px; }
      nav { flex-wrap: wrap; }
    }
  </style>
</head>
<body>
  <div class="page">
    <nav>
      <a href="#" class="logo">De Stijl</a>
      <ul>
        <li><a href="#">Manifest</a></li>
        <li><a href="#">Works</a></li>
        <li><a href="#">Archive</a></li>
        <li><a href="#">Contact</a></li>
      </ul>
    </nav>

    <section class="hero">
      <div class="hero-content">
        <h1><span class="red">Pure</span> Form<br><span class="blue">Pure</span> Color</h1>
        <p>Horizontal. Vertical. Red. Yellow. Blue. The universal language of visual harmony, reduced to its absolute essence.</p>
        <a href="#" class="btn">Explore</a>
      </div>
      <div class="hero-block-blue"></div>
      <div class="hero-block-yellow"></div>
    </section>

    <section class="features">
      <div class="feature">
        <div class="feature-accent" style="background: var(--ds-red);"></div>
        <h3>Reduction</h3>
        <p>Strip away everything that is not essential. What remains is the universal truth of form and color.</p>
      </div>
      <div class="feature">
        <div class="feature-accent" style="background: var(--ds-blue);"></div>
        <h3>Equilibrium</h3>
        <p>Dynamic balance through asymmetry. Unequal parts in perfect tension create visual harmony.</p>
      </div>
      <div class="feature">
        <div class="feature-accent" style="background: var(--ds-yellow);"></div>
        <h3>Universality</h3>
        <p>Three colors, two directions, one truth. The simplest elements express the deepest order.</p>
      </div>
    </section>

    <section class="cta">
      <div class="cta-content">
        <h2>The New Plastic Art</h2>
        <p>Composition in line and color. The style that seeks nothing less than the visual expression of universal harmony.</p>
        <a href="#" class="btn">Read Manifesto</a>
      </div>
      <div class="cta-block"></div>
    </section>

    <footer>
      <div class="footer-block"></div>
      <div class="footer-text">
        Built on De Stijl principles. Leiden 1917.
      </div>
      <div class="footer-block-blue"></div>
    </footer>
  </div>
</body>
</html>
```
