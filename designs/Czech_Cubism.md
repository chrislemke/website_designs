# Czech Cubism Design Reference

Czech Cubism (1910-1925) is a uniquely Bohemian adaptation of Cubist aesthetics centered in Prague. Unlike French Cubism, which remained primarily a painting movement, Czech Cubism extended geometric fragmentation into **architecture, furniture, ceramics, lighting, and decorative arts**. The movement's core philosophy held that objects possess an **inner energy** that can be released by breaking down their surfaces into **dynamic, geometric planes**. It rejected Art Nouveau's organic fluidity in favor of **crystalline forms, sharp angles, and oblique force lines**, drawing spiritual significance from the geometry of inorganic crystals as Platonic solids.

---

## Visual Characteristics

### Core Motifs and Patterns

- **Crystalline / prismatic forms** -- faceted surfaces inspired by the geometry of natural crystals; the defining visual signature
- **Sharp angular planes** -- surfaces intersecting at dramatic oblique angles, creating visual dynamism
- **Zig-zag patterns** -- angular, jagged lines used as borders, ornamental bands, and surface decoration
- **Oblique force lines** -- diagonal cuts through vertical and horizontal masses, releasing "inner energy"
- **Pyramid and prism shapes** -- three-dimensional geometric solids applied to architectural volumes and object forms
- **Faceted, multidirectional surfaces** -- broken planes that catch light and shadow differently across the face of an object
- **Beveled edges** -- chamfered corners and sliced planes replacing smooth curves or right angles
- **Diamond and rhombus tessellations** -- repeating angular shapes used in railings, grates, and decorative panels

### Design Principles

- **Geometric fragmentation** of all surfaces -- no plane remains flat or unbroken
- **Oblique lines dominate** over horizontals and verticals (per Pavel Janak's 1911 theoretical text "The Prism and the Pyramid")
- **Light and shadow as material** -- faceted surfaces are designed to interact with natural light, creating shifting shadows
- **Spiritual geometry** -- crystalline forms carry philosophical weight as expressions of natural order
- **Unity across scales** -- the same geometric vocabulary applies from building facades down to porcelain cups
- **Austere expressiveness** -- ornament derived from structure, not applied decoration
- **Dynamic tension** -- visual energy created by the collision of angular planes
- **Rejection of curves** -- deliberate opposition to Art Nouveau's organic, flowing lines

---

## Color Palette

### Primary Scheme

| Role | Colors |
|------|--------|
| **Base surfaces** | Warm whites, cream, stone gray |
| **Structural contrast** | Black outlines, dark charcoal edges |
| **Earth tones** | Ochre, sienna, warm brown, terracotta |
| **High contrast** | White surfaces with bold black edges |

### Accent and Decorative Colors

| Color | Hex (suggested) | Usage |
|-------|-----------------|-------|
| Stone White | `#F2EDE4`, `#E8E0D0` | Primary surface backgrounds |
| Warm Cream | `#F5F0E1`, `#EDE6D6` | Light panels, text backgrounds |
| Ochre | `#C8A951`, `#B8962E` | Accent borders, heading highlights |
| Sienna / Terracotta | `#A0522D`, `#8B4513` | Warm accent blocks, decorative bands |
| Charcoal | `#2D2D2D`, `#3A3A3A` | Text, structural outlines |
| Deep Black | `#1A1A1A`, `#0D0D0D` | Edge lines, high-contrast borders |
| Muted Blue | `#3B5998`, `#4A6FA5` | Sparse ceramic-inspired accents |
| Dusty Red | `#8B3A3A`, `#A04040` | National color accents (Rondocubist influence) |
| Dark Bronze | `#6B5B3E`, `#7D6E52` | Metalwork-inspired accents |

### Suggested CSS Custom Properties

```css
:root {
  /* Base surfaces */
  --cubism-white: #f2ede4;
  --cubism-cream: #f5f0e1;
  --cubism-stone: #d6cfc2;
  --cubism-stone-dark: #b8b0a0;

  /* Structural darks */
  --cubism-charcoal: #2d2d2d;
  --cubism-black: #1a1a1a;
  --cubism-edge: #0d0d0d;

  /* Earth tones */
  --cubism-ochre: #c8a951;
  --cubism-ochre-dark: #b8962e;
  --cubism-sienna: #a0522d;
  --cubism-terracotta: #8b4513;
  --cubism-brown: #5c4033;
  --cubism-bronze: #6b5b3e;

  /* Sparse accents */
  --cubism-blue: #3b5998;
  --cubism-red: #8b3a3a;

  /* Functional mappings */
  --cubism-bg-primary: var(--cubism-white);
  --cubism-bg-secondary: var(--cubism-cream);
  --cubism-bg-dark: var(--cubism-charcoal);
  --cubism-text-primary: var(--cubism-charcoal);
  --cubism-text-light: var(--cubism-cream);
  --cubism-accent: var(--cubism-ochre);
  --cubism-border: var(--cubism-black);
  --cubism-border-light: var(--cubism-stone-dark);
}
```

### Approaches

- **High-contrast structural lines** -- bold black edges on light stone/cream surfaces, mimicking architectural facade detailing
- **Earth-tone warmth** -- ochre, sienna, and brown as the primary accent palette, reflecting Prague's building materials
- **Monochromatic with geometric interest** -- rely on shape and shadow rather than color variety
- **Sparse color punctuation** -- use blue or red only as rare focal accents, as in Czech Cubist ceramics

---

## Typography

### Typeface Characteristics

Czech Cubism typography features:

- **Geometric, angular letterforms** with sharp vertices and faceted construction
- **Strong diagonal strokes** reflecting the oblique-line philosophy
- **Constructed / architectural feel** -- letters that look built rather than drawn
- **Sans-serif dominance** for modernist authority
- **Condensed proportions** conveying vertical energy
- **Uppercase-heavy usage** for headlines, echoing architectural inscriptions
- **Angular serifs** when serifs are used -- pointed, not rounded

### Recommended Web Fonts (Google Fonts / Free)

| Font | Style | Usage |
|------|-------|-------|
| **Josefin Sans** | Geometric, angular, vintage | Headlines, display text |
| **Bebas Neue** | Bold, condensed, uppercase | Hero titles, banners |
| **Oswald** | Condensed, strong vertical rhythm | Section headings |
| **Archivo Black** | Bold geometric sans | Display headings |
| **Staatliches** | Condensed, architectural display | Large feature titles |
| **Barlow Condensed** | Clean condensed geometric | Subheadings, navigation |
| **Source Sans 3** | Neutral geometric sans | Body text |
| **IBM Plex Sans** | Constructed, precise geometric | Body text, UI elements |
| **Cormorant Garamond** | Angular, high-contrast serif | Decorative body text, quotes |
| **Playfair Display** | Sharp, angular transitional serif | Formal headings (serif variant) |

### Typography CSS Example

```css
/* Headlines -- angular, constructed, uppercase */
h1, h2, h3 {
  font-family: 'Josefin Sans', 'Bebas Neue', sans-serif;
  text-transform: uppercase;
  letter-spacing: 0.12em;
  color: var(--cubism-charcoal);
  font-weight: 700;
  line-height: 1.1;
}

/* Display / Hero text */
.cubism-display {
  font-family: 'Bebas Neue', 'Staatliches', sans-serif;
  font-size: clamp(3rem, 8vw, 8rem);
  letter-spacing: 0.15em;
  line-height: 0.95;
  color: var(--cubism-black);
}

/* Body text */
body {
  font-family: 'Source Sans 3', 'IBM Plex Sans', sans-serif;
  font-weight: 400;
  letter-spacing: 0.02em;
  line-height: 1.7;
  color: var(--cubism-text-primary);
}

/* Captions / small text */
.cubism-caption {
  font-family: 'Barlow Condensed', sans-serif;
  text-transform: uppercase;
  letter-spacing: 0.08em;
  font-size: 0.85rem;
  color: var(--cubism-stone-dark);
}
```

---

## Layout Principles

### Grid and Structure

- **Asymmetric angular grids** -- avoid perfectly regular grids; introduce deliberate diagonal offsets and angular breaks
- **Faceted sectioning** -- divide the page into panels that suggest crystalline planes, not uniform rectangles
- **Strong diagonal axes** -- content areas and dividers placed at oblique angles
- **Vertical emphasis** -- tall, narrow content columns echoing the prismatic verticality of Czech Cubist architecture
- **Overlapping planes** -- content panels that overlap slightly, suggesting depth and spatial interpenetration
- **Modular but dynamic spacing** -- consistent spacing units, but with angular disruptions

### Section Organization

- Use **angular geometric dividers** between sections (zig-zag lines, faceted borders, beveled separators)
- Apply **generous negative space** around angular elements to let their geometry breathe
- Create **hierarchy through angular scale** -- large faceted hero sections stepping down to smaller crystalline panels
- Employ **beveled containers** -- panels with clipped corners or angled edges rather than rounded corners
- Use **structural black outlines** to define and separate geometric regions, mimicking architectural edge detailing

---

## CSS/Design Techniques

### Faceted / Clipped Containers

```css
/* Beveled panel -- corners clipped at angles */
.cubism-panel {
  background: var(--cubism-cream);
  clip-path: polygon(
    3% 0%, 97% 0%, 100% 4%, 100% 96%,
    97% 100%, 3% 100%, 0% 96%, 0% 4%
  );
  padding: 3rem 2.5rem;
  border: 2px solid var(--cubism-border);
}

/* Diamond-shaped accent element */
.cubism-diamond {
  width: 60px;
  height: 60px;
  background: var(--cubism-ochre);
  transform: rotate(45deg);
  margin: 1rem auto;
}

/* Angled section divider */
.cubism-angle-divider {
  width: 100%;
  height: 60px;
  background: linear-gradient(
    to bottom right,
    var(--cubism-bg-primary) 49.5%,
    var(--cubism-border) 49.5%,
    var(--cubism-border) 50.5%,
    var(--cubism-bg-secondary) 50.5%
  );
}
```

### Crystalline Border Effects

```css
/* Multi-layered angular border */
.cubism-crystal-border {
  border: 3px solid var(--cubism-black);
  outline: 1px solid var(--cubism-stone-dark);
  outline-offset: 5px;
  position: relative;
}

.cubism-crystal-border::before {
  content: '';
  position: absolute;
  inset: -10px;
  border: 1px solid var(--cubism-stone-dark);
  pointer-events: none;
}

/* Zig-zag border using repeating gradient */
.cubism-zigzag-border {
  background-image:
    linear-gradient(135deg, var(--cubism-black) 25%, transparent 25%),
    linear-gradient(225deg, var(--cubism-black) 25%, transparent 25%);
  background-size: 20px 20px;
  background-position: 0 0;
  background-repeat: repeat-x;
  height: 10px;
  width: 100%;
}
```

### Angular Shadow / Depth

```css
/* Sharp geometric shadow -- no blur, hard edges */
.cubism-shadow {
  box-shadow:
    6px 6px 0 0 var(--cubism-charcoal),
    12px 12px 0 0 var(--cubism-stone-dark);
}

/* Oblique shadow suggesting angled light */
.cubism-oblique-shadow {
  box-shadow:
    8px 4px 0 0 var(--cubism-black);
  position: relative;
}

/* Layered plane depth effect */
.cubism-depth {
  position: relative;
}

.cubism-depth::after {
  content: '';
  position: absolute;
  top: 8px;
  left: 8px;
  right: -8px;
  bottom: -8px;
  background: var(--cubism-stone-dark);
  z-index: -1;
}
```

### Zig-Zag and Angular Decorative Elements

```css
/* Zig-zag divider using clip-path */
.cubism-zigzag {
  width: 100%;
  height: 30px;
  background: var(--cubism-ochre);
  clip-path: polygon(
    0% 0%, 5% 100%, 10% 0%, 15% 100%, 20% 0%,
    25% 100%, 30% 0%, 35% 100%, 40% 0%, 45% 100%,
    50% 0%, 55% 100%, 60% 0%, 65% 100%, 70% 0%,
    75% 100%, 80% 0%, 85% 100%, 90% 0%, 95% 100%, 100% 0%
  );
}

/* Prismatic background pattern */
.cubism-prism-bg {
  background-color: var(--cubism-white);
  background-image:
    linear-gradient(60deg, var(--cubism-stone) 25%, transparent 25%),
    linear-gradient(-60deg, var(--cubism-stone) 25%, transparent 25%),
    linear-gradient(60deg, transparent 75%, var(--cubism-stone) 75%),
    linear-gradient(-60deg, transparent 75%, var(--cubism-stone) 75%);
  background-size: 40px 70px;
  background-position: 0 0, 0 0, 20px 35px, 20px 35px;
}
```

### Diagonal / Oblique Section Layout

```css
/* Angled section -- content on a diagonal plane */
.cubism-angled-section {
  position: relative;
  padding: 6rem 2rem;
  background: var(--cubism-cream);
}

.cubism-angled-section::before {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  height: 80px;
  background: var(--cubism-bg-primary);
  clip-path: polygon(0 0, 100% 0, 100% 20%, 0 100%);
}

/* Skewed container for dynamic angular feel */
.cubism-skew-container {
  transform: skewY(-2deg);
  padding: 4rem 2rem;
  background: var(--cubism-charcoal);
  color: var(--cubism-text-light);
}

.cubism-skew-container > * {
  transform: skewY(2deg); /* counter-skew content */
}
```

### Card / Panel Component

```css
.cubism-card {
  background: var(--cubism-white);
  border: 2px solid var(--cubism-black);
  padding: 2rem;
  position: relative;
  clip-path: polygon(
    0% 3%, 3% 0%, 97% 0%, 100% 3%,
    100% 97%, 97% 100%, 3% 100%, 0% 97%
  );
}

/* Structural line accent at top */
.cubism-card::before {
  content: '';
  position: absolute;
  top: 0;
  left: 10%;
  right: 10%;
  height: 4px;
  background: var(--cubism-ochre);
}

/* Angular highlight corner */
.cubism-card::after {
  content: '';
  position: absolute;
  top: 0;
  right: 0;
  width: 30px;
  height: 30px;
  background: linear-gradient(
    225deg,
    var(--cubism-ochre) 50%,
    transparent 50%
  );
}
```

### Crystal Texture Overlay

```css
/* Faceted crystal texture overlay for backgrounds */
.cubism-crystal-texture {
  position: relative;
}

.cubism-crystal-texture::after {
  content: '';
  position: absolute;
  inset: 0;
  background:
    linear-gradient(30deg, rgba(0,0,0,0.03) 25%, transparent 25%),
    linear-gradient(150deg, rgba(0,0,0,0.03) 25%, transparent 25%),
    linear-gradient(210deg, rgba(0,0,0,0.03) 25%, transparent 25%),
    linear-gradient(330deg, rgba(0,0,0,0.03) 25%, transparent 25%);
  background-size: 60px 100px;
  pointer-events: none;
}
```

---

## Materials and Textures (Visual Metaphors for Web)

Physical Czech Cubist materials and their web equivalents:

| Physical Material | Web Equivalent |
|-------------------|----------------|
| Cut stone / Limestone | Light textured backgrounds with subtle grain overlay |
| Brick facades with geometric relief | Repeating geometric background patterns in earth tones |
| Stoneware porcelain | Clean white surfaces with bold black geometric outlines |
| Dark wood furniture | Deep brown panels, warm dark backgrounds |
| Metal railings and grates | Angular geometric border patterns, dark metallic gradients |
| Cast concrete | Light gray matte surfaces with minimal texture |
| Bronze fittings | Dark metallic bronze gradients for accent elements |
| Ceramic glaze | Subtle sheen gradients on colored accent panels |

---

## Sub-styles and Variations

### Early Czech Cubism (1911-1914)

- The purest phase of the movement
- Strict adherence to crystalline and prismatic geometry
- Monochromatic and austere color palettes (black, white, stone)
- Architects: Josef Gocar (House of the Black Madonna), Josef Chochol (Hodek Apartment House, Kovarovic Villa)
- Focus on facades, furniture, and porcelain

### Rondocubism (1920s)

- Post-war evolution incorporating **rounded forms** alongside angular geometry
- **National style** reflecting the new Czechoslovak Republic identity
- More **colorful** than early Czech Cubism, with dichromatic facades in **red and ochre/yellow**
- Folk art influences blended with geometric abstraction
- Exemplified by Pavel Janak's Legiobank and the Palace of Trade Fairs
- Bridges Czech Cubism toward Art Deco

---

## Related Aesthetics

| Aesthetic | Relationship to Czech Cubism |
|-----------|------------------------------|
| **Cubism** | Parent movement; Czech Cubism extends Cubist painting principles into three-dimensional design |
| **Art Nouveau** | Direct predecessor and opposite; Czech Cubism rejected Art Nouveau's organic curves |
| **Art Deco** | Successor influenced by Czech Cubism's geometric vocabulary and applied arts approach |
| **Expressionism** | Contemporary; shared interest in expressing inner energy through form |
| **Modernism** | Broader movement; Czech Cubism is an early Modernist experiment in total design |
| **Bauhaus** | Later contemporary; shares geometric construction but favors minimalism over crystalline ornament |
| **De Stijl** | Parallel movement; both use geometric abstraction, but De Stijl restricts to orthogonal forms |
| **Constructivism** | Shares emphasis on geometric structure and the unity of art and functional design |

---

## Quick-Start: Minimal Czech Cubism Page Template

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Czech Cubism Page</title>
  <link href="https://fonts.googleapis.com/css2?family=Josefin+Sans:wght@400;700&family=Bebas+Neue&family=Source+Sans+3:wght@400;600&display=swap" rel="stylesheet">
  <style>
    :root {
      --cubism-white: #f2ede4;
      --cubism-cream: #f5f0e1;
      --cubism-stone: #d6cfc2;
      --cubism-charcoal: #2d2d2d;
      --cubism-black: #1a1a1a;
      --cubism-ochre: #c8a951;
      --cubism-sienna: #a0522d;
      --cubism-bronze: #6b5b3e;
    }

    * { margin: 0; padding: 0; box-sizing: border-box; }

    body {
      background: var(--cubism-white);
      color: var(--cubism-charcoal);
      font-family: 'Source Sans 3', sans-serif;
      font-weight: 400;
      letter-spacing: 0.02em;
      line-height: 1.7;
    }

    h1, h2, h3 {
      font-family: 'Josefin Sans', sans-serif;
      text-transform: uppercase;
      letter-spacing: 0.12em;
      font-weight: 700;
    }

    /* Hero with angular geometry */
    .hero {
      text-align: center;
      padding: 6rem 2rem 4rem;
      background: var(--cubism-charcoal);
      color: var(--cubism-cream);
      position: relative;
    }

    .hero h1 {
      font-family: 'Bebas Neue', sans-serif;
      font-size: clamp(3rem, 8vw, 7rem);
      letter-spacing: 0.15em;
      color: var(--cubism-white);
    }

    .hero p {
      color: var(--cubism-stone);
      margin-top: 1rem;
      letter-spacing: 0.08em;
      text-transform: uppercase;
      font-size: 0.9rem;
    }

    /* Angled divider below hero */
    .hero-divider {
      width: 100%;
      height: 60px;
      background: linear-gradient(
        to bottom right,
        var(--cubism-charcoal) 49.5%,
        var(--cubism-black) 49.5%,
        var(--cubism-black) 50.5%,
        var(--cubism-white) 50.5%
      );
    }

    /* Zig-zag accent band */
    .zigzag-band {
      width: 100%;
      height: 20px;
      background: var(--cubism-ochre);
      clip-path: polygon(
        0% 0%, 4% 100%, 8% 0%, 12% 100%, 16% 0%,
        20% 100%, 24% 0%, 28% 100%, 32% 0%, 36% 100%,
        40% 0%, 44% 100%, 48% 0%, 52% 100%, 56% 0%,
        60% 100%, 64% 0%, 68% 100%, 72% 0%, 76% 100%,
        80% 0%, 84% 100%, 88% 0%, 92% 100%, 96% 0%, 100% 100%
      );
    }

    section {
      max-width: 900px;
      margin: 0 auto;
      padding: 4rem 2rem;
    }

    section h2 {
      margin-bottom: 1.5rem;
      padding-bottom: 0.5rem;
      border-bottom: 3px solid var(--cubism-black);
    }

    /* Beveled card */
    .card {
      background: var(--cubism-cream);
      border: 2px solid var(--cubism-black);
      padding: 2rem;
      clip-path: polygon(
        0% 3%, 3% 0%, 97% 0%, 100% 3%,
        100% 97%, 97% 100%, 3% 100%, 0% 97%
      );
      margin: 1.5rem 0;
      box-shadow: 6px 6px 0 0 var(--cubism-charcoal);
    }
  </style>
</head>
<body>
  <div class="hero">
    <h1>Title Here</h1>
    <p>Crystalline geometry in digital form</p>
  </div>
  <div class="hero-divider"></div>
  <div class="zigzag-band"></div>
  <section>
    <h2>Section Heading</h2>
    <div class="card">
      <p>Content styled with Czech Cubist geometric principles -- angular, faceted, structurally expressive.</p>
    </div>
  </section>
</body>
</html>
```
