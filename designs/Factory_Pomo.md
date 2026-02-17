# Factory Pomo Design Reference

Factory Pomo is a design aesthetic that coalesced in the late 1980s, merging the **clean, referential forms of Memphis-Milano**, emerging **CAD computer graphics** visual languages, and revivals of **Bauhaus, Russian Constructivism, WPA graphics**, and **early-to-mid 20th century industrial vernacular**. It synthesizes postmodern playfulness with industrial seriousness, producing a look of **futuro-industrial machinery rendered through geometric abstraction and bold primary color contrasts**. Factory Pomo peaked from the mid-1980s to mid-1990s before giving way to Cyber Gen-X Corporate and Y2K Futurism aesthetics.

---

## Visual Characteristics

### Core Motifs and Patterns

- **Gears and cogs** -- oversized decorative gear shapes, both as illustrations and structural design elements
- **Metal ridging** -- parallel raised lines evoking corrugated metal, factory textures, and industrial surfaces
- **Isometric technical drawings** -- factory assembly lines, conveyor belts, and machinery rendered in isometric projection
- **Atomic and nuclear symbology** -- radiation symbols, atom diagrams, electron orbits
- **Radio waves and transmission towers** -- broadcasting iconography, concentric signal arcs
- **Radar and instrumentation graphics** -- sweep lines, scope circles, technical readouts
- **1950s TV test patterns** -- color bars, geometric calibration targets
- **Hazard tape patterns** -- diagonal stripe warning tape in high-contrast color pairs
- **Technical arrows and jagged forms** -- sharp directional indicators, lightning-bolt shapes
- **Exposed structural elements** -- steel beams, space-frame trusses, pipe railings with mesh infill
- **CRT monitors and screens** -- banks of television monitors as decorative/informational elements
- **Rotating globe sculptures** -- wire-frame or structural steel world globes

### Design Principles

- **Strong emphasis on symmetry** -- balanced, mirrored compositions as a primary organizational method
- **Color inversion as a compositional tool** -- symmetrical layouts where one half inverts the color scheme of the other
- **Simple, bold geometric shapes** -- circles, triangles, rectangles used as primary building blocks
- **Industrial tangibility meets digital abstraction** -- physical factory objects rendered through early digital design tools
- **Contrasting colors at high saturation** -- bold juxtapositions rather than gradual transitions
- **Layered complexity** -- mechanical elements, typography, and geometric shapes overlapping in dense compositions
- **Retro-futurist tension** -- Depression-era and Constructivist visual language repurposed for a digital age

---

## Color Palette

### Primary Scheme

Factory Pomo is **primary-color-heavy with brown accents**. The palette draws from industrial safety colors, Constructivist posters, and early desktop publishing capabilities.

| Role | Colors |
|------|--------|
| **Primary base** | Bold red, blue, yellow at full saturation |
| **Accents** | Brown, amber, industrial orange |
| **Neutrals** | Black, steel gray, harsh fluorescent white |
| **Secondaries** | Electric purple, teal (especially late 1980s-early 1990s additions) |

### Detailed Color Table

| Color | Hex (suggested) | Usage |
|-------|-----------------|-------|
| Industrial Red | `#CC2222`, `#E03030` | Primary accent, hazard elements, bold headings |
| Constructivist Blue | `#1A4B8C`, `#2255AA` | Backgrounds, structural elements, secondary panels |
| Signal Yellow | `#F5C518`, `#FFCC00` | Warning accents, highlights, gear fills |
| Factory Brown | `#6B4226`, `#8B5E3C` | Earthy counterpoint, backgrounds, borders |
| Industrial Orange | `#D4652F`, `#E87020` | Secondary accent, hazard tape, warm highlights |
| Electric Purple | `#7B2D8E`, `#9040A0` | Late-80s accent, display elements |
| Teal | `#008080`, `#1A9E9E` | Cool counterbalance, secondary accent |
| Steel Gray | `#71797E`, `#8A9098` | Structural elements, metal textures |
| Charcoal | `#2B2B2B`, `#333333` | Dark backgrounds, contrast base |
| Fluorescent White | `#E8EDF2`, `#F0F4FA` | Harsh, bluish-white lighting effect |
| Black | `#111111`, `#1A1A1A` | Deep background, text, maximum contrast |

### Suggested CSS Custom Properties

```css
:root {
  /* Primary industrial colors */
  --fp-red: #cc2222;
  --fp-red-bright: #e03030;
  --fp-blue: #1a4b8c;
  --fp-blue-bright: #2255aa;
  --fp-yellow: #f5c518;
  --fp-yellow-bright: #ffcc00;

  /* Secondary accents */
  --fp-brown: #6b4226;
  --fp-brown-light: #8b5e3c;
  --fp-orange: #d4652f;
  --fp-purple: #7b2d8e;
  --fp-teal: #008080;

  /* Neutrals */
  --fp-black: #111111;
  --fp-charcoal: #2b2b2b;
  --fp-steel: #71797e;
  --fp-steel-light: #8a9098;
  --fp-fluorescent-white: #e8edf2;
  --fp-white: #f0f4fa;

  /* Functional assignments */
  --fp-bg-primary: var(--fp-charcoal);
  --fp-bg-secondary: var(--fp-black);
  --fp-text-primary: var(--fp-fluorescent-white);
  --fp-text-heading: var(--fp-yellow);
  --fp-accent-primary: var(--fp-red);
  --fp-accent-secondary: var(--fp-blue);
  --fp-border: var(--fp-steel);
}
```

### Color Approaches

- **High-contrast complementary pairs** -- red/blue, yellow/black, orange/teal placed in direct opposition
- **Color inversion across symmetry axes** -- identical layout mirrored with swapped foreground/background colors
- **Primary color dominance** -- restrict palette to 3-4 bold primaries; avoid pastels entirely
- **Industrial warning combinations** -- yellow/black hazard stripes, red/white danger signals
- **Flat, ungraded fills** -- solid color blocks rather than gradients, echoing early screen-printing and CAD output

---

## Typography

### Typeface Characteristics

Factory Pomo typography is defined by two landmark digital typefaces from the late 1980s:

- **Modula** (Emigre, Zuzana Licko) -- heavy weights, tall letterforms, geometric slab serifs; resembles metal factory signage digitally sharpened into clean precision
- **Industria** (Neville Brody) -- geometric, condensed industrial feel; sharp, clean, digitally transformed

Shared characteristics of Factory Pomo type:
- **Heavy slab serifs** or bold geometric sans-serifs
- **Tall, closely-spaced letterforms** evoking factory signage and stamped metal
- **Digitally sharpened geometry** -- cleaner and more experimental than their historical inspirations
- **Strong vertical proportions** -- letters that emphasize height and narrow width
- **Uppercase-dominant** display usage
- **Art Deco influence filtered through digital tools** -- geometric precision impossible in hand-lettering

### Recommended Web Fonts (Google Fonts / Free)

| Font | Style | Usage | Why it fits |
|------|-------|-------|-------------|
| **Archivo Black** | Heavy geometric sans | Display headlines, titles | Bold industrial weight, geometric construction |
| **Oswald** | Condensed sans-serif | Headlines, subheadings | Tall, narrow proportions like factory signage |
| **Roboto Slab** | Geometric slab serif | Headlines, section titles | Clean slab serifs echoing Modula |
| **Arvo** | Geometric slab serif | Headings, accent text | Sturdy slab serifs with industrial weight |
| **Bebas Neue** | Condensed uppercase sans | Large display text, banners | Tall, tight letterforms; Constructivist feel |
| **Barlow Condensed** | Condensed sans | Subheadings, UI labels | Industrial precision, narrow proportions |
| **Saira** | Geometric sans (wide weight range) | Body text, technical labels | Clean digital geometry, multiple weights |
| **Share Tech Mono** | Monospaced, technical | Technical data, readouts, captions | Evokes CRT displays and computer terminals |
| **Rajdhani** | Geometric, angular | Body text, technical content | Sharp, mechanical feel with good readability |
| **DM Sans** | Clean geometric sans | Body copy | Neutral, digital, highly readable |

### Typography CSS Example

```css
@import url('https://fonts.googleapis.com/css2?family=Archivo+Black&family=Oswald:wght@400;600;700&family=Roboto+Slab:wght@400;700;900&family=Barlow+Condensed:wght@400;600;700&family=Share+Tech+Mono&family=DM+Sans:wght@300;400;500&display=swap');

/* Display / Hero text */
.fp-display {
  font-family: 'Archivo Black', 'Oswald', sans-serif;
  font-size: clamp(3rem, 8vw, 8rem);
  text-transform: uppercase;
  letter-spacing: 0.08em;
  line-height: 0.95;
  color: var(--fp-yellow);
}

/* Headlines */
h1, h2, h3 {
  font-family: 'Oswald', 'Barlow Condensed', sans-serif;
  text-transform: uppercase;
  letter-spacing: 0.1em;
  color: var(--fp-text-heading);
  font-weight: 700;
}

/* Slab serif alternate headings */
.fp-heading-slab {
  font-family: 'Roboto Slab', 'Arvo', serif;
  font-weight: 900;
  text-transform: uppercase;
  letter-spacing: 0.05em;
}

/* Body text */
body {
  font-family: 'DM Sans', 'Rajdhani', sans-serif;
  font-weight: 400;
  letter-spacing: 0.02em;
  line-height: 1.6;
  color: var(--fp-fluorescent-white);
}

/* Technical / readout text */
.fp-tech-text {
  font-family: 'Share Tech Mono', monospace;
  font-size: 0.85rem;
  letter-spacing: 0.05em;
  color: var(--fp-teal);
  text-transform: uppercase;
}
```

---

## Layout Principles

### Grid and Structure

- **Symmetrical, centered compositions** -- bilateral symmetry is the dominant organizational strategy
- **Isometric and axonometric grids** -- tilted perspectives for technical illustration sections, evoking CAD and engineering drawings
- **Dense, layered layouts** -- overlapping geometric elements, gears, type, and illustration unlike minimalist approaches
- **Modular grid with industrial rhythm** -- repeating units sized like factory tiles or control panels
- **Strong horizontal and vertical axes** -- content aligns to a rigid structural grid, as if mounted on steel beams

### Section Organization

- Use **industrial dividers** between sections (pipe/beam motifs, hazard stripe bars, gear-tooth borders)
- Create **panel-based layouts** resembling control rooms, factory floors, or technical schematics
- Apply **asymmetric information density within symmetric frames** -- the overall frame is symmetrical, but content within panels can vary
- Employ **inset panels and bordered containers** -- content framed in steel-like borders with corner rivets or bolt details
- Use **contrasting background colors** per section to create visual rhythm and separation

### Spatial Characteristics

- **Tightly packed** -- Factory Pomo favors density over whitespace
- **Flat depth** -- elements exist on the same plane or in clearly separated layers; no subtle shadows
- **Hard edges** -- crisp boundaries between elements, no feathering or blur
- **Full-bleed color blocks** -- sections extend edge-to-edge in bold solid colors

---

## CSS/Design Techniques

### Gear Shape (CSS-only)

```css
.fp-gear {
  width: 120px;
  height: 120px;
  background: var(--fp-steel);
  border-radius: 50%;
  position: relative;
  display: flex;
  align-items: center;
  justify-content: center;
}

.fp-gear::before {
  content: '';
  position: absolute;
  width: 140px;
  height: 140px;
  background:
    conic-gradient(
      from 0deg,
      var(--fp-steel) 0deg 15deg,
      transparent 15deg 30deg,
      var(--fp-steel) 30deg 45deg,
      transparent 45deg 60deg,
      var(--fp-steel) 60deg 75deg,
      transparent 75deg 90deg,
      var(--fp-steel) 90deg 105deg,
      transparent 105deg 120deg,
      var(--fp-steel) 120deg 135deg,
      transparent 135deg 150deg,
      var(--fp-steel) 150deg 165deg,
      transparent 165deg 180deg,
      var(--fp-steel) 180deg 195deg,
      transparent 195deg 210deg,
      var(--fp-steel) 210deg 225deg,
      transparent 225deg 240deg,
      var(--fp-steel) 240deg 255deg,
      transparent 255deg 270deg,
      var(--fp-steel) 270deg 285deg,
      transparent 285deg 300deg,
      var(--fp-steel) 300deg 315deg,
      transparent 315deg 330deg,
      var(--fp-steel) 330deg 345deg,
      transparent 345deg 360deg
    );
  border-radius: 50%;
  z-index: -1;
}

.fp-gear::after {
  content: '';
  width: 40px;
  height: 40px;
  background: var(--fp-charcoal);
  border-radius: 50%;
  border: 3px solid var(--fp-steel-light);
}
```

### Hazard Stripe Border

```css
.fp-hazard-border {
  border: 4px solid transparent;
  background:
    linear-gradient(var(--fp-charcoal), var(--fp-charcoal)) padding-box,
    repeating-linear-gradient(
      -45deg,
      var(--fp-yellow) 0px,
      var(--fp-yellow) 10px,
      var(--fp-black) 10px,
      var(--fp-black) 20px
    ) border-box;
}

/* Standalone hazard stripe divider */
.fp-hazard-divider {
  height: 12px;
  background: repeating-linear-gradient(
    -45deg,
    var(--fp-yellow) 0px,
    var(--fp-yellow) 10px,
    var(--fp-black) 10px,
    var(--fp-black) 20px
  );
  margin: 2rem 0;
}
```

### Metal Ridging Texture

```css
.fp-metal-ridged {
  background:
    repeating-linear-gradient(
      0deg,
      rgba(255,255,255,0.06) 0px,
      rgba(255,255,255,0.06) 1px,
      transparent 1px,
      transparent 4px
    ),
    linear-gradient(
      180deg,
      var(--fp-steel) 0%,
      #5a6268 50%,
      var(--fp-steel) 100%
    );
}

/* Corrugated metal variant */
.fp-corrugated {
  background:
    repeating-linear-gradient(
      90deg,
      rgba(255,255,255,0.08) 0px,
      rgba(0,0,0,0.05) 3px,
      rgba(255,255,255,0.08) 6px
    ),
    var(--fp-steel);
}
```

### Color-Inverted Symmetry Panel

```css
.fp-inversion-panel {
  display: grid;
  grid-template-columns: 1fr 1fr;
}

.fp-inversion-panel .fp-left {
  background: var(--fp-red);
  color: var(--fp-fluorescent-white);
  padding: 3rem;
}

.fp-inversion-panel .fp-right {
  background: var(--fp-fluorescent-white);
  color: var(--fp-red);
  padding: 3rem;
}

/* Ensure headings also invert */
.fp-inversion-panel .fp-left h2 { color: var(--fp-fluorescent-white); }
.fp-inversion-panel .fp-right h2 { color: var(--fp-red); }
```

### Industrial Panel / Control Card

```css
.fp-panel {
  background: var(--fp-charcoal);
  border: 2px solid var(--fp-steel);
  padding: 2rem;
  position: relative;
}

/* Corner rivets */
.fp-panel::before,
.fp-panel::after {
  content: '';
  position: absolute;
  width: 12px;
  height: 12px;
  background: radial-gradient(
    circle at 40% 40%,
    var(--fp-steel-light) 0%,
    var(--fp-steel) 50%,
    #555 100%
  );
  border-radius: 50%;
  border: 1px solid #555;
}

.fp-panel::before { top: 8px; left: 8px; }
.fp-panel::after { top: 8px; right: 8px; }

/* Additional rivets via inner element */
.fp-panel .fp-panel-inner::before,
.fp-panel .fp-panel-inner::after {
  content: '';
  position: absolute;
  width: 12px;
  height: 12px;
  background: radial-gradient(
    circle at 40% 40%,
    var(--fp-steel-light) 0%,
    var(--fp-steel) 50%,
    #555 100%
  );
  border-radius: 50%;
  border: 1px solid #555;
}

.fp-panel .fp-panel-inner::before { bottom: 8px; left: 8px; }
.fp-panel .fp-panel-inner::after { bottom: 8px; right: 8px; }
```

### Constructivist Diagonal Layout

```css
.fp-diagonal-section {
  position: relative;
  overflow: hidden;
  padding: 4rem 2rem;
}

.fp-diagonal-section::before {
  content: '';
  position: absolute;
  top: 0;
  left: -10%;
  width: 120%;
  height: 100%;
  background: var(--fp-red);
  transform: skewY(-4deg);
  transform-origin: top left;
  z-index: -1;
}
```

### Animated Gear Rotation

```css
@keyframes fp-rotate {
  from { transform: rotate(0deg); }
  to { transform: rotate(360deg); }
}

@keyframes fp-rotate-reverse {
  from { transform: rotate(360deg); }
  to { transform: rotate(0deg); }
}

.fp-gear-spin { animation: fp-rotate 12s linear infinite; }
.fp-gear-spin-reverse { animation: fp-rotate-reverse 12s linear infinite; }
```

### Fluorescent Lighting Glow Effect

```css
/* Simulates harsh overhead fluorescent lighting */
.fp-fluorescent-glow {
  box-shadow:
    0 0 30px rgba(232, 237, 242, 0.15),
    0 0 60px rgba(232, 237, 242, 0.05);
}

/* Text with fluorescent buzz effect */
.fp-neon-text {
  color: var(--fp-fluorescent-white);
  text-shadow:
    0 0 5px rgba(232, 237, 242, 0.6),
    0 0 15px rgba(232, 237, 242, 0.3);
}
```

### Pipe/Beam Section Divider

```css
.fp-pipe-divider {
  height: 8px;
  background: linear-gradient(
    180deg,
    var(--fp-steel-light) 0%,
    var(--fp-steel) 40%,
    #555 60%,
    var(--fp-steel) 100%
  );
  border-top: 1px solid rgba(255,255,255,0.15);
  margin: 2rem 0;
  position: relative;
}

/* Bolt accents on pipe divider */
.fp-pipe-divider::before,
.fp-pipe-divider::after {
  content: '';
  position: absolute;
  top: 50%;
  transform: translateY(-50%);
  width: 16px;
  height: 16px;
  background: radial-gradient(circle, var(--fp-steel-light), var(--fp-steel));
  border-radius: 50%;
  border: 1px solid #555;
}

.fp-pipe-divider::before { left: 20px; }
.fp-pipe-divider::after { right: 20px; }
```

### Radar / Scope Background Animation

```css
@keyframes fp-radar-sweep {
  from { transform: rotate(0deg); }
  to { transform: rotate(360deg); }
}

.fp-radar-bg {
  position: relative;
  background: var(--fp-black);
  border-radius: 50%;
  overflow: hidden;
}

.fp-radar-bg::before {
  content: '';
  position: absolute;
  top: 0;
  left: 50%;
  width: 50%;
  height: 50%;
  background: conic-gradient(
    from 0deg at 0% 100%,
    rgba(0, 128, 128, 0.4) 0deg,
    transparent 60deg
  );
  transform-origin: bottom left;
  animation: fp-radar-sweep 4s linear infinite;
}

/* Concentric scope rings */
.fp-radar-bg::after {
  content: '';
  position: absolute;
  inset: 10%;
  border: 1px solid rgba(0, 128, 128, 0.3);
  border-radius: 50%;
  box-shadow:
    inset 0 0 0 20px transparent,
    inset 0 0 0 21px rgba(0, 128, 128, 0.2),
    inset 0 0 0 50px transparent,
    inset 0 0 0 51px rgba(0, 128, 128, 0.15);
}
```

---

## Materials and Textures (Visual Metaphors for Web)

Physical Factory Pomo materials and their web equivalents:

| Physical Material | Web Equivalent |
|-------------------|----------------|
| Corrugated steel / metal ridging | Repeating linear gradients with alternating light/dark bands |
| Exposed steel I-beams | Heavy rectangular borders with metallic gradients |
| Industrial mesh / perforated metal | Dot-pattern backgrounds, small repeating radial gradients |
| Hazard/warning tape | Diagonal-striped repeating linear gradients (yellow/black) |
| Brushed aluminum | Subtle horizontal linear gradient with light streaks |
| Cast iron gears | Conic gradients with tooth patterns, dark metallic fills |
| Concrete / factory floor | Subtle noise overlay textures in gray tones |
| Fluorescent tube lighting | White/blue box-shadow glow, high-brightness overlays |
| CRT screen glass | Dark backgrounds with subtle scan-line patterns |
| Rivets and bolts | Small radial-gradient circles with highlight and shadow |
| Wire mesh panels | Grid backgrounds with thin lines and transparent fills |

---

## Influences and Design Lineage

Factory Pomo draws from these historical movements and reinterprets them through late-1980s digital tools:

| Influence | What Factory Pomo borrows |
|-----------|--------------------------|
| **Russian Constructivism** | Diagonal compositions, bold geometric typography, red/black/white palettes, propaganda poster aesthetics |
| **Bauhaus** | Geometric purity, primary color commitment, form-follows-function reinterpreted as form-follows-machine |
| **Art Deco** | Symmetry, decorative geometry, stylized industrial imagery, stepped/tiered forms |
| **WPA Poster Art** | Heroic worker figures, strong flat color areas, industrial pride imagery |
| **Diego Rivera murals** | Factory floor panoramas, celebration of industrial labor, machine-human integration |
| **Memphis-Milano** | Bold color, geometric playfulness, postmodern irreverence, anti-minimalism |
| **Streamline Moderne** | Aerodynamic curves, chrome finishes, futuristic machine aesthetic |
| **High-tech architecture** | Exposed structural systems (Centre Pompidou, Lloyd's Building), colorful ducts, visible mechanical systems |
| **Early CAD graphics** | Clean vector geometry, isometric views, limited-palette digital rendering |

---

## Related Aesthetics

| Aesthetic | Relationship to Factory Pomo |
|-----------|------------------------------|
| **Memphis Lite** | Lighter, more consumer-friendly version of the same postmodern design impulse |
| **Wacky Pomo** | Shares postmodern irreverence but leans more playful and less industrial |
| **Decoplex** | Overlaps in Art Deco revival and geometric precision |
| **Early Cyber** | Shares CAD-influenced digital aesthetic and technological optimism |
| **Cyberdelia** | Overlaps in psychedelic-digital visual language of the early 1990s |
| **Silicon Dreams** | Shares the utopian technology narrative expressed through digital design |
| **Raygun Gothic** | Overlaps in retro-futurism and mid-century industrial nostalgia |
| **Constructivism** | Direct ancestor; Factory Pomo is essentially digital neo-Constructivism |
| **Art Deco** | Foundational influence on symmetry, geometry, and decorative industrial motifs |
| **Memphis Design** | Parent movement; Factory Pomo is the industrial-focused branch of 80s postmodernism |

---

## Quick-Start: Minimal Factory Pomo Page Template

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Factory Pomo Page</title>
  <link href="https://fonts.googleapis.com/css2?family=Archivo+Black&family=Oswald:wght@400;600;700&family=Roboto+Slab:wght@700;900&family=Barlow+Condensed:wght@400;600&family=Share+Tech+Mono&family=DM+Sans:wght@300;400;500&display=swap" rel="stylesheet">
  <style>
    :root {
      --fp-red: #cc2222;
      --fp-blue: #1a4b8c;
      --fp-yellow: #f5c518;
      --fp-brown: #6b4226;
      --fp-orange: #d4652f;
      --fp-teal: #008080;
      --fp-black: #111111;
      --fp-charcoal: #2b2b2b;
      --fp-steel: #71797e;
      --fp-steel-light: #8a9098;
      --fp-white: #e8edf2;
    }

    * { margin: 0; padding: 0; box-sizing: border-box; }

    body {
      background: var(--fp-charcoal);
      color: var(--fp-white);
      font-family: 'DM Sans', sans-serif;
      font-weight: 400;
      line-height: 1.6;
    }

    /* Hazard stripe header border */
    .hero {
      text-align: center;
      padding: 5rem 2rem 4rem;
      background: var(--fp-black);
      border-bottom: 12px solid transparent;
      background-clip: padding-box;
      position: relative;
    }

    .hero::after {
      content: '';
      position: absolute;
      bottom: 0;
      left: 0;
      right: 0;
      height: 12px;
      background: repeating-linear-gradient(
        -45deg,
        var(--fp-yellow) 0px, var(--fp-yellow) 10px,
        var(--fp-black) 10px, var(--fp-black) 20px
      );
    }

    .hero h1 {
      font-family: 'Archivo Black', sans-serif;
      font-size: clamp(3rem, 8vw, 7rem);
      text-transform: uppercase;
      letter-spacing: 0.08em;
      color: var(--fp-yellow);
      line-height: 0.95;
    }

    .hero .subtitle {
      font-family: 'Share Tech Mono', monospace;
      text-transform: uppercase;
      letter-spacing: 0.15em;
      color: var(--fp-teal);
      margin-top: 1rem;
      font-size: 0.9rem;
    }

    /* Color-inverted two-column section */
    .inversion-section {
      display: grid;
      grid-template-columns: 1fr 1fr;
    }

    .inversion-section .col-left {
      background: var(--fp-red);
      color: var(--fp-white);
      padding: 3rem;
    }

    .inversion-section .col-right {
      background: var(--fp-white);
      color: var(--fp-red);
      padding: 3rem;
    }

    .inversion-section h2 {
      font-family: 'Oswald', sans-serif;
      text-transform: uppercase;
      letter-spacing: 0.1em;
      font-weight: 700;
      margin-bottom: 1rem;
    }

    /* Industrial panel section */
    section.panel {
      max-width: 900px;
      margin: 3rem auto;
      padding: 2.5rem;
      border: 2px solid var(--fp-steel);
      background: var(--fp-charcoal);
    }

    section.panel h2 {
      font-family: 'Roboto Slab', serif;
      text-transform: uppercase;
      letter-spacing: 0.05em;
      color: var(--fp-yellow);
      font-weight: 900;
      margin-bottom: 1rem;
    }

    /* Pipe divider */
    .pipe-divider {
      height: 8px;
      background: linear-gradient(180deg, var(--fp-steel-light), var(--fp-steel), #555, var(--fp-steel));
      border-top: 1px solid rgba(255,255,255,0.15);
      margin: 0;
    }
  </style>
</head>
<body>
  <div class="hero">
    <h1>Title Here</h1>
    <p class="subtitle">// System status: operational //</p>
  </div>
  <div class="pipe-divider"></div>
  <div class="inversion-section">
    <div class="col-left">
      <h2>Section A</h2>
      <p>Content with primary color background.</p>
    </div>
    <div class="col-right">
      <h2>Section B</h2>
      <p>Same content, inverted color scheme.</p>
    </div>
  </div>
  <div class="pipe-divider"></div>
  <section class="panel">
    <h2>Industrial Panel</h2>
    <p>Content framed in steel-bordered industrial panel styling.</p>
  </section>
</body>
</html>
```
