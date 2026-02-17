# Cyberminimalism Design Reference

Cyberminimalism is a hyper-minimalistic digital aesthetic that emerged in the late 2010s, coined by designer Alex Edwards (also known as "Cyberbougie"). It extends minimalism beyond Flat Design principles into extreme reductionism. At its most distilled, a Cyberminimalist design comprises **sans-serif words, color gradients, a design grid, and little to nothing else**. The style places extreme emphasis on a particular form of "sleekness" -- stripping interfaces to their absolute essentials while maintaining a polished, high-tech feel.

---

## Visual Characteristics

### Core Design Traits

- **Extreme reductionism** -- remove every element that does not serve a direct functional or communicative purpose; if in doubt, leave it out
- **Sleekness above all** -- every surface, transition, and edge should feel precision-engineered; no rough textures, no hand-drawn elements, no ornamentation
- **Sans-serif typography as primary visual element** -- text itself becomes the design; large, confident type on open space
- **Color gradients as the sole decorative device** -- standard smooth gradients or grainy/noisy gradient textures provide the only visual richness
- **Strict grid alignment** -- every element sits on a deliberate, mathematical grid; nothing is placed "by feel"
- **Simple, symmetrical geometric shapes** -- squares, circles, and rectangles; no complex illustrations or icons
- **High contrast, monochromatic foundations** -- black and white dominate, with color used sparingly and intentionally
- **Flat design UI elements** -- no skeuomorphism, no drop shadows (or only minimal ones), no bevels
- **Bento-style grid layouts** -- modular, compartmentalized card grids popularized by Apple's 2022 product presentations
- **Neumorphism and Glassmorphism as occasional accent techniques** -- subtle frosted-glass panels or soft-extruded elements can appear but remain subordinate to the minimalist framework

### Design Principles

- Negative space is not empty -- it is a structural element that gives content room to command attention
- Visual hierarchy is achieved through size contrast and spatial relationships, not through decoration
- Every pixel must justify its existence; ornamental elements are eliminated
- Interactions should feel instant, precise, and invisible -- micro-animations are subtle if present at all
- Content density is low; each screen or section communicates one idea clearly
- Symmetry and alignment create order; asymmetry is used only when it serves a deliberate focal point
- Design should feel "expensive" -- the restraint itself communicates sophistication

---

## Color Palette

### Primary Scheme

Cyberminimalism is fundamentally **monochromatic**. Black and white form the backbone, with gradients providing the only chromatic expression. Text is almost exclusively black or white; colored text is rare and intentional.

| Role | Colors | Hex (suggested) |
|------|--------|-----------------|
| **Background (dark mode)** | Pure black, near-black | `#000000`, `#0A0A0A`, `#111111` |
| **Background (light mode)** | Pure white, off-white | `#FFFFFF`, `#FAFAFA`, `#F5F5F5` |
| **Text on dark** | Pure white, near-white | `#FFFFFF`, `#F0F0F0`, `#E0E0E0` |
| **Text on light** | Pure black, near-black | `#000000`, `#0A0A0A`, `#1A1A1A` |
| **Muted text** | Medium grays | `#888888`, `#999999`, `#666666` |
| **Borders / dividers** | Subtle grays | `#222222` (dark), `#E5E5E5` (light) |
| **Gradient start** | Deep violet, deep blue | `#6C00FF`, `#0066FF`, `#FF0080` |
| **Gradient end** | Cyan, pink, warm amber | `#00D4FF`, `#FF6B6B`, `#FFB800` |
| **Accent (minimal)** | Single vibrant hue | `#5B5BFF`, `#00C2FF`, `#FF3366` |

### Gradient Palette

Gradients are the signature decorative element. They range from smooth linear/radial gradients to grainy, dithered textures.

| Gradient Name | From | To | Hex Pair |
|---------------|------|----|----------|
| **Violet-Cyan** | Deep purple | Electric cyan | `#6C00FF` to `#00D4FF` |
| **Sunset** | Hot pink | Warm amber | `#FF0080` to `#FFB800` |
| **Ocean** | Deep blue | Teal | `#0036FF` to `#00D4AA` |
| **Monochrome** | Dark gray | Light gray | `#333333` to `#CCCCCC` |
| **Neon** | Electric blue | Magenta | `#00C2FF` to `#FF00AA` |
| **Frost** | White | Light blue-gray | `#FFFFFF` to `#D0E0F0` |

### Suggested CSS Custom Properties

```css
:root {
  /* Base (dark mode default) */
  --cm-bg-primary: #000000;
  --cm-bg-secondary: #0a0a0a;
  --cm-bg-tertiary: #111111;
  --cm-bg-elevated: #1a1a1a;

  /* Text */
  --cm-text-primary: #ffffff;
  --cm-text-secondary: #999999;
  --cm-text-muted: #666666;

  /* Borders */
  --cm-border: #222222;
  --cm-border-subtle: #1a1a1a;

  /* Gradients */
  --cm-gradient-primary: linear-gradient(135deg, #6c00ff, #00d4ff);
  --cm-gradient-secondary: linear-gradient(135deg, #ff0080, #ffb800);
  --cm-gradient-subtle: linear-gradient(135deg, #1a1a1a, #333333);

  /* Accent */
  --cm-accent: #5b5bff;
  --cm-accent-hover: #7a7aff;
}

/* Light mode overrides */
@media (prefers-color-scheme: light) {
  :root {
    --cm-bg-primary: #ffffff;
    --cm-bg-secondary: #fafafa;
    --cm-bg-tertiary: #f5f5f5;
    --cm-bg-elevated: #ffffff;

    --cm-text-primary: #000000;
    --cm-text-secondary: #666666;
    --cm-text-muted: #999999;

    --cm-border: #e5e5e5;
    --cm-border-subtle: #f0f0f0;
  }
}
```

### Color Guidelines

- **Default to black and white** -- resist the urge to add color; the absence of color is the aesthetic
- Gradients should appear on **one focal element per section** at most -- a hero background, a single button, or an accent shape
- When using gradients on text, apply them via `background-clip: text` for a striking but controlled effect
- Grainy gradients add texture and depth without breaking the minimalist ethos
- Colored text is used sparingly and only for interactive states or critical emphasis
- Dark mode is the canonical Cyberminimalist presentation; light mode is an acceptable variant

---

## Typography

### Typeface Characteristics

Cyberminimalism typography is defined by:

- **Grotesque and neo-grotesque sans-serifs** -- clean, neutral, and precisely constructed
- **Slab serifs as a secondary option** -- when a more assertive, editorial tone is needed
- **Large scale, bold weight** -- headlines dominate the page; type is the primary visual element
- **Tight or negative letter-spacing on headlines** -- creates density and visual impact
- **Generous letter-spacing on labels and small text** -- improves legibility and adds sophistication
- **Minimal font variation** -- one family for everything, two at most; weight contrast provides hierarchy

### Recommended Web Fonts (Google Fonts)

| Font | Style | Usage |
|------|-------|-------|
| **Inter** | Neo-grotesque sans, designed for screens | Body text, UI labels, all-purpose (the canonical Cyberminimalist choice) |
| **Space Grotesk** | Geometric grotesque with technical feel | Headlines, display text, technical interfaces |
| **DM Sans** | Clean geometric sans | Body text, paragraphs, smaller UI copy |
| **Outfit** | Modern geometric sans, variable weight | Headlines and body, single-font systems |
| **Syne** | Bold, expressive geometric sans | Display headings, hero sections |
| **IBM Plex Sans** | Corporate neo-grotesque | Body text, professional contexts |
| **Roboto Mono** | Monospace | Code snippets, data labels, technical accents |
| **Roboto Slab** | Slab serif | Editorial headlines, secondary headings |
| **Albert Sans** | Clean geometric, wide weight range | Headlines through body text |
| **Darker Grotesque** | Condensed grotesque | Large display text, impactful headlines |

### Typography CSS Example

```css
/* Import fonts */
@import url('https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700&family=Space+Grotesk:wght@400;500;600;700&display=swap');

/* Headlines -- large, tight, commanding */
h1, h2, h3 {
  font-family: 'Space Grotesk', 'Inter', sans-serif;
  font-weight: 700;
  color: var(--cm-text-primary);
  line-height: 1.05;
  letter-spacing: -0.03em;
}

/* Display / Hero text */
.cm-display {
  font-family: 'Space Grotesk', sans-serif;
  font-size: clamp(3rem, 8vw, 7rem);
  font-weight: 700;
  letter-spacing: -0.04em;
  line-height: 0.95;
}

/* Body text */
body {
  font-family: 'Inter', sans-serif;
  font-weight: 400;
  font-size: 1rem;
  line-height: 1.6;
  color: var(--cm-text-primary);
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}

/* Overline / label text */
.cm-label {
  font-family: 'Inter', sans-serif;
  font-weight: 500;
  font-size: 0.75rem;
  letter-spacing: 0.12em;
  text-transform: uppercase;
  color: var(--cm-text-secondary);
}

/* Monospace accent */
.cm-mono {
  font-family: 'Roboto Mono', monospace;
  font-size: 0.875rem;
  letter-spacing: 0.02em;
  color: var(--cm-text-secondary);
}

/* Gradient text effect */
.cm-gradient-text {
  background: var(--cm-gradient-primary);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  background-clip: text;
}
```

---

## Layout Principles

### Grid and Structure

- **Strict grid system** -- every element sits on a defined grid; CSS Grid or explicit column systems are preferred over freeform positioning
- **Bento-style grids** -- modular, compartmentalized layouts where each cell contains one piece of content (popularized by Apple's 2022 keynote presentations)
- **Symmetrical composition** -- centered layouts, mirrored arrangements, and balanced visual weight
- **Extreme whitespace** -- margins and padding are generous; empty space is a deliberate design choice, not wasted area
- **Full-viewport sections** -- each section often fills the entire viewport height, creating a presentation-like scroll experience
- **Max-width containers** (1200-1440px) prevent content from spreading too wide on large displays
- **Consistent spacing scale** -- use a mathematical spacing system (e.g., 4px base: 8, 16, 24, 32, 48, 64, 96, 128)

### Section Organization

- **One idea per screen** -- avoid cramming multiple concepts into a single viewport
- **No decorative dividers** -- sections are separated by whitespace alone, or by a change in background (black to white)
- **Content is centered** -- both horizontally and often vertically within its section
- **Typography creates hierarchy** -- size differences between heading and body text should be dramatic (3:1 or greater ratio)
- **Cards and containers have minimal or no visible borders** -- differentiation comes from background color shifts or subtle elevation
- **Navigation is reduced** -- minimal nav items, no mega-menus, often just a wordmark and one or two links

### Bento Grid Pattern

```css
.cm-bento {
  display: grid;
  grid-template-columns: repeat(4, 1fr);
  grid-auto-rows: minmax(200px, auto);
  gap: 1px;  /* hairline gaps or small gaps */
  max-width: 1200px;
  margin: 0 auto;
}

.cm-bento-cell {
  background: var(--cm-bg-elevated);
  padding: 2.5rem;
  display: flex;
  flex-direction: column;
  justify-content: flex-end;
}

.cm-bento-cell--wide {
  grid-column: span 2;
}

.cm-bento-cell--tall {
  grid-row: span 2;
}

.cm-bento-cell--featured {
  grid-column: span 2;
  grid-row: span 2;
  background: var(--cm-gradient-primary);
  color: #ffffff;
}
```

---

## CSS/Design Techniques

### Grainy Gradient Technique

The grainy/noisy gradient is a signature Cyberminimalist texture. It adds analog warmth to the otherwise purely digital aesthetic.

```css
/* Grainy gradient using SVG noise filter */
.cm-grainy-gradient {
  position: relative;
  background: linear-gradient(135deg, #6c00ff, #00d4ff);
}

.cm-grainy-gradient::after {
  content: '';
  position: absolute;
  inset: 0;
  background-image: url("data:image/svg+xml,%3Csvg viewBox='0 0 256 256' xmlns='http://www.w3.org/2000/svg'%3E%3Cfilter id='noise'%3E%3CfeTurbulence type='fractalNoise' baseFrequency='0.65' numOctaves='3' stitchTiles='stitch'/%3E%3C/filter%3E%3Crect width='100%25' height='100%25' filter='url(%23noise)' opacity='0.25'/%3E%3C/svg%3E");
  background-size: 256px 256px;
  pointer-events: none;
  mix-blend-mode: overlay;
  opacity: 0.4;
}
```

### Smooth Gradient Backgrounds

```css
/* Subtle gradient background for sections */
.cm-gradient-bg {
  background: linear-gradient(
    180deg,
    var(--cm-bg-primary) 0%,
    #0a0a1a 50%,
    var(--cm-bg-primary) 100%
  );
}

/* Radial gradient spotlight effect */
.cm-spotlight {
  background: radial-gradient(
    ellipse at 50% 0%,
    rgba(108, 0, 255, 0.15) 0%,
    transparent 70%
  );
}
```

### Minimal Card

```css
.cm-card {
  background: var(--cm-bg-elevated);
  border: 1px solid var(--cm-border);
  border-radius: 16px;
  padding: 2rem;
  transition: border-color 0.2s ease;
}

.cm-card:hover {
  border-color: var(--cm-text-muted);
}
```

### Minimal Button

```css
.cm-button {
  display: inline-flex;
  align-items: center;
  justify-content: center;
  background: var(--cm-text-primary);
  color: var(--cm-bg-primary);
  border: none;
  border-radius: 999px;
  padding: 12px 28px;
  font-family: 'Inter', sans-serif;
  font-weight: 500;
  font-size: 0.9rem;
  letter-spacing: 0.01em;
  cursor: pointer;
  transition: opacity 0.2s ease;
}

.cm-button:hover {
  opacity: 0.85;
}

/* Ghost / outline variant */
.cm-button--ghost {
  background: transparent;
  color: var(--cm-text-primary);
  border: 1px solid var(--cm-border);
}

.cm-button--ghost:hover {
  border-color: var(--cm-text-primary);
}

/* Gradient accent button */
.cm-button--gradient {
  background: var(--cm-gradient-primary);
  color: #ffffff;
  border: none;
}
```

### Glassmorphism Accent Panel

```css
.cm-glass {
  background: rgba(255, 255, 255, 0.05);
  backdrop-filter: blur(20px);
  -webkit-backdrop-filter: blur(20px);
  border: 1px solid rgba(255, 255, 255, 0.08);
  border-radius: 20px;
  padding: 2rem;
}
```

### Neumorphism Accent (Subtle)

```css
/* Use sparingly -- only for special interactive elements */
.cm-neomorphic {
  background: var(--cm-bg-secondary);
  border-radius: 16px;
  padding: 2rem;
  box-shadow:
    8px 8px 24px rgba(0, 0, 0, 0.4),
    -8px -8px 24px rgba(255, 255, 255, 0.03);
}
```

### Hairline Grid Dividers

```css
/* Grid with hairline dividers between cells */
.cm-grid-dividers {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  border-top: 1px solid var(--cm-border);
  border-left: 1px solid var(--cm-border);
}

.cm-grid-dividers > * {
  padding: 2.5rem;
  border-right: 1px solid var(--cm-border);
  border-bottom: 1px solid var(--cm-border);
}
```

### Scroll-Snap Sections

```css
/* Full-viewport scroll-snap for presentation-like browsing */
html {
  scroll-snap-type: y mandatory;
  scroll-behavior: smooth;
}

.cm-section {
  min-height: 100vh;
  scroll-snap-align: start;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  padding: 4rem 2rem;
}
```

### Minimal Navigation

```css
.cm-nav {
  position: fixed;
  top: 0;
  left: 0;
  right: 0;
  z-index: 100;
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 1.25rem 2.5rem;
  background: rgba(0, 0, 0, 0.6);
  backdrop-filter: blur(12px);
  -webkit-backdrop-filter: blur(12px);
  border-bottom: 1px solid var(--cm-border-subtle);
}

.cm-nav-brand {
  font-family: 'Space Grotesk', sans-serif;
  font-weight: 700;
  font-size: 1.125rem;
  color: var(--cm-text-primary);
  text-decoration: none;
}

.cm-nav-links {
  display: flex;
  gap: 2rem;
  list-style: none;
}

.cm-nav-links a {
  color: var(--cm-text-secondary);
  text-decoration: none;
  font-size: 0.875rem;
  font-weight: 400;
  transition: color 0.2s ease;
}

.cm-nav-links a:hover {
  color: var(--cm-text-primary);
}
```

### Responsive Considerations

```css
/* Tablet */
@media (max-width: 1024px) {
  .cm-bento {
    grid-template-columns: repeat(2, 1fr);
  }

  .cm-display {
    font-size: clamp(2.5rem, 6vw, 5rem);
    letter-spacing: -0.03em;
  }
}

/* Mobile */
@media (max-width: 640px) {
  .cm-bento {
    grid-template-columns: 1fr;
  }

  .cm-bento-cell--wide,
  .cm-bento-cell--featured {
    grid-column: span 1;
  }

  .cm-display {
    font-size: clamp(2rem, 10vw, 3.5rem);
    letter-spacing: -0.02em;
  }

  .cm-nav {
    padding: 1rem 1.5rem;
  }
}
```

---

## Notable Examples

Brands and products that exemplify Cyberminimalism:

| Example | Year | Notes |
|---------|------|-------|
| **Linear** (app) | 2021 | Dark UI, gradient accents, sparse layout, grotesque typography |
| **Nothing OS** | 2022 | Dot-matrix-inspired minimalism, monochromatic with geometric accents |
| **Apple product pages** (Bento era) | 2022+ | Bento grids, black backgrounds, massive typography, gradient highlights |
| **frame.io** redesign | 2023 | Dark mode, restrained palette, grid-based layout |
| **Attio** | 2024 | Monochromatic dark UI with selective gradient accents |
| **AWS re:Invent** branding | 2024 | Gradient typography on black, extreme simplicity |
| **Eurovision** branding | 2024 | Bold geometric grid, gradient fills, sans-serif dominance |
| **Datalands** | 2019 | Early example of the aesthetic with data-driven minimal layouts |
| **Delegated** (app) | 2019 | Clean, grid-based interface with restrained color |
| **iPhone 16 / iPad Air M2 presentations** | 2024 | Apple's keynote slides as canonical Cyberminimalist design |

---

## Related Aesthetics

| Aesthetic | Relationship to Cyberminimalism |
|-----------|-------------------------------|
| **Flat Design** | Direct ancestor; Cyberminimalism takes Flat Design's anti-skeuomorphic principles and pushes them to an extreme |
| **Minimalism** | Parent aesthetic; Cyberminimalism is specifically the digital/tech-industry expression of minimalism |
| **International Typographic Style (Swiss Style)** | Shares the grid obsession, sans-serif dominance, and belief that form follows function |
| **Glassmorphism** | A compatible accent technique; frosted-glass panels can appear within a Cyberminimalist layout as subtle depth cues |
| **Neumorphism** | An alternative approach to minimal UI; occasionally blended into Cyberminimalist designs for soft-extruded interactive elements |

---

## Quick-Start: Minimal Cyberminimalism Page Template

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Cyberminimalism Page</title>
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700&family=Space+Grotesk:wght@400;500;600;700&display=swap" rel="stylesheet">
  <style>
    :root {
      --cm-bg: #000000;
      --cm-bg-elevated: #111111;
      --cm-text: #ffffff;
      --cm-text-secondary: #888888;
      --cm-border: #222222;
      --cm-gradient: linear-gradient(135deg, #6c00ff, #00d4ff);
    }

    * { margin: 0; padding: 0; box-sizing: border-box; }

    body {
      background: var(--cm-bg);
      color: var(--cm-text);
      font-family: 'Inter', sans-serif;
      font-weight: 400;
      font-size: 1rem;
      line-height: 1.6;
      -webkit-font-smoothing: antialiased;
    }

    /* Navigation */
    nav {
      display: flex;
      justify-content: space-between;
      align-items: center;
      padding: 1.5rem 3rem;
      border-bottom: 1px solid var(--cm-border);
    }

    nav a {
      color: var(--cm-text-secondary);
      text-decoration: none;
      font-size: 0.875rem;
      transition: color 0.2s;
    }

    nav a:hover { color: var(--cm-text); }

    .brand {
      font-family: 'Space Grotesk', sans-serif;
      font-weight: 700;
      font-size: 1.125rem;
      color: var(--cm-text);
    }

    /* Hero */
    .hero {
      min-height: 80vh;
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      text-align: center;
      padding: 4rem 2rem;
      gap: 1.5rem;
    }

    .hero h1 {
      font-family: 'Space Grotesk', sans-serif;
      font-size: clamp(3rem, 8vw, 7rem);
      font-weight: 700;
      line-height: 0.95;
      letter-spacing: -0.04em;
    }

    .hero .gradient-text {
      background: var(--cm-gradient);
      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent;
      background-clip: text;
    }

    .hero p {
      color: var(--cm-text-secondary);
      font-size: 1.125rem;
      max-width: 480px;
    }

    .hero-cta {
      display: inline-flex;
      align-items: center;
      gap: 0.5rem;
      background: var(--cm-text);
      color: var(--cm-bg);
      border: none;
      border-radius: 999px;
      padding: 14px 32px;
      font-family: 'Inter', sans-serif;
      font-weight: 500;
      font-size: 0.9rem;
      cursor: pointer;
      transition: opacity 0.2s;
      text-decoration: none;
    }

    .hero-cta:hover { opacity: 0.85; }

    /* Bento Grid */
    .bento {
      display: grid;
      grid-template-columns: repeat(3, 1fr);
      gap: 1px;
      max-width: 1200px;
      margin: 0 auto;
      padding: 0 2rem;
    }

    .bento-cell {
      background: var(--cm-bg-elevated);
      padding: 3rem;
      display: flex;
      flex-direction: column;
      justify-content: flex-end;
      gap: 0.75rem;
      min-height: 280px;
    }

    .bento-cell h3 {
      font-family: 'Space Grotesk', sans-serif;
      font-weight: 600;
      font-size: 1.25rem;
    }

    .bento-cell p {
      color: var(--cm-text-secondary);
      font-size: 0.875rem;
      line-height: 1.5;
    }

    .bento-cell--accent {
      background: var(--cm-gradient);
      grid-column: span 2;
    }

    /* Footer */
    footer {
      border-top: 1px solid var(--cm-border);
      padding: 3rem;
      text-align: center;
      color: var(--cm-text-secondary);
      font-size: 0.8rem;
      margin-top: 6rem;
    }

    @media (max-width: 768px) {
      .bento {
        grid-template-columns: 1fr;
      }
      .bento-cell--accent {
        grid-column: span 1;
      }
      nav { padding: 1rem 1.5rem; }
    }
  </style>
</head>
<body>
  <nav>
    <span class="brand">Project</span>
    <a href="#">About</a>
  </nav>

  <section class="hero">
    <h1>Build <span class="gradient-text">something</span><br>remarkable.</h1>
    <p>A hyper-minimal interface where content speaks for itself. No noise, no clutter, just clarity.</p>
    <a href="#" class="hero-cta">Get Started</a>
  </section>

  <section class="bento">
    <div class="bento-cell bento-cell--accent">
      <h3>Gradient Accent</h3>
      <p>The sole decorative element in the entire design system. Use sparingly.</p>
    </div>
    <div class="bento-cell">
      <h3>Grid Precision</h3>
      <p>Every element aligned to a strict mathematical grid.</p>
    </div>
    <div class="bento-cell">
      <h3>Monochrome</h3>
      <p>Black and white as the foundation. Color is earned, not given.</p>
    </div>
    <div class="bento-cell">
      <h3>Sans-Serif</h3>
      <p>Typography is the primary design element.</p>
    </div>
    <div class="bento-cell">
      <h3>Negative Space</h3>
      <p>Emptiness as a deliberate structural choice.</p>
    </div>
  </section>

  <footer>
    <p>Designed with nothing but intention.</p>
  </footer>
</body>
</html>
```
