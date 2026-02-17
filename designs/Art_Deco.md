# Art Deco Design Reference

Art Deco (also known as Style Moderne) is a decorative art and design movement that emerged in the 1910s-1930s. It represents **luxury, glamour, modernity, progress, faith in technology**, the **machine aesthetic**, and **speed**. The style celebrates technological advancement through geometric abstraction, luxury through material richness, forward momentum via dynamic angular composition, and industrial precision balanced with decorative opulence.

---

## Visual Characteristics

### Core Motifs and Patterns

- **Chevrons** -- V-shaped angular patterns, often repeated in rows or borders
- **Sunbursts / Radiating lines** -- Fan-shaped rays emanating from a central point; a signature Art Deco motif
- **Zig-zag patterns** -- Sharp, angular repetitions used as borders, dividers, and background fills
- **Stepped forms** -- Tiered, pyramid-like shapes inspired by Mesoamerican and Egyptian architecture
- **Stylized natural forms** -- Abstracted/geometric versions of plants, animals, and human figures
- **Symmetry** -- Strong bilateral or radial symmetry throughout all compositions
- **Geometric fans and arches** -- Semi-circular fan shapes with internal geometric divisions
- **Repeating geometric pattern backgrounds** -- Tessellated grids of triangles, hexagons, and diamonds

### Design Principles

- **Angular, geometric construction** emphasizing verticality
- **Streamlined, aerodynamic curves** (especially in the later Streamline Moderne variant)
- **Symmetrical composition** throughout all design elements
- **Strong focal points** using angular emphasis and radiating patterns
- **Directional movement** created through chevron and sunburst patterns
- **Lavish ornamentation** -- rich decorative detail, never minimalist
- **Verticality** used for prestige, technological advancement, and dramatic effect

---

## Color Palette

### Primary Scheme

| Role | Colors |
|------|--------|
| **Base** | Black, deep charcoal |
| **Primary accents** | Gold, silver, chrome |
| **High contrast** | Black paired with gold, silver, or chrome |

### Secondary / Jewel Tones

| Color | Hex (suggested) | Usage |
|-------|-----------------|-------|
| Emerald | `#046307`, `#2E8B57` | Accent panels, decorative elements |
| Sapphire | `#0F52BA`, `#1E3A5F` | Secondary backgrounds, highlights |
| Ruby | `#9B111E`, `#8B0000` | Accent text, call-to-action elements |
| Amber / Gold | `#D4AF37`, `#C5A03F` | Borders, headings, ornamental details |
| Silver / Platinum | `#C0C0C0`, `#A9A9A9` | Secondary metallic accents |
| Ivory / Cream | `#FFFFF0`, `#F5F5DC` | Light backgrounds, text on dark |

### Suggested CSS Custom Properties

```css
:root {
  /* Base */
  --deco-black: #1a1a1a;
  --deco-charcoal: #2d2d2d;
  --deco-cream: #f5f0e1;
  --deco-ivory: #fffff0;

  /* Metallics */
  --deco-gold: #d4af37;
  --deco-gold-light: #e8d48b;
  --deco-silver: #c0c0c0;
  --deco-chrome: #dbe4eb;

  /* Jewel tones */
  --deco-emerald: #046307;
  --deco-sapphire: #0f52ba;
  --deco-ruby: #9b111e;
  --deco-amethyst: #6b3fa0;

  /* Functional */
  --deco-bg-primary: var(--deco-black);
  --deco-bg-secondary: var(--deco-charcoal);
  --deco-text-primary: var(--deco-cream);
  --deco-accent: var(--deco-gold);
  --deco-border: var(--deco-gold);
}
```

### Approaches

- **Monochromatic with high contrast gradients** -- e.g., black to dark gray with gold accents
- **Metallic finishes as primary design elements** -- gradients mimicking gold, chrome, brass
- **High contrast combinations** -- always pair dark bases with bright metallics
- **Limited color separation for bold impact** -- restrict palette to 3-4 colors maximum

---

## Typography

### Typeface Characteristics

Art Deco typography features:

- **Geometric, sans-serif typefaces** with streamlined characteristics
- **Bold, angular letterforms** with sharp terminals
- **Inline / engraved effects** -- letters with internal lines or decorative strokes
- **Strong vertical emphasis** -- tall, narrow proportions
- **Uniform stroke weight** or dramatic thick/thin contrast
- **Uppercase-heavy** usage for headlines and display text
- **Decorative capitals** with geometric embellishments

### Recommended Web Fonts (Google Fonts / Free)

| Font | Style | Usage |
|------|-------|-------|
| **Poiret One** | Geometric, thin, elegant | Headlines, display text |
| **Josefin Sans** | Geometric, vintage feel | Headlines, subheadings |
| **Bebas Neue** | Bold, condensed, uppercase | Headlines, banners |
| **Raleway** | Thin geometric with elegant weight range | Body text, subheadings |
| **Cinzel** | Serif with classical proportion | Formal headings |
| **Cinzel Decorative** | Ornamental serif | Feature titles, logos |
| **Tenor Sans** | Clean geometric sans | Body copy |
| **Limelight** | Art Deco display font | Large display headlines |
| **Metropolis** (self-hosted) | Geometric sans inspired by 1920s | All-purpose |

### Typography CSS Example

```css
/* Headlines */
h1, h2, h3 {
  font-family: 'Poiret One', 'Josefin Sans', sans-serif;
  text-transform: uppercase;
  letter-spacing: 0.15em;
  color: var(--deco-gold);
  font-weight: 400;
}

/* Display / Hero text */
.deco-display {
  font-family: 'Bebas Neue', 'Limelight', sans-serif;
  font-size: clamp(3rem, 8vw, 8rem);
  letter-spacing: 0.2em;
  line-height: 1.1;
}

/* Body text */
body {
  font-family: 'Raleway', 'Tenor Sans', sans-serif;
  font-weight: 300;
  letter-spacing: 0.03em;
  line-height: 1.7;
  color: var(--deco-cream);
}
```

---

## Layout Principles

### Grid and Structure

- **Grid-based systematic organization** -- use modular grids with strong alignment
- **Symmetrical layouts** -- center-aligned content, mirrored columns
- **Strong vertical axis** -- content flows along a central vertical spine
- **Stepped/tiered sections** -- content blocks arranged in pyramid or ziggurat formations
- **Careful alignment and rhythm** using modular spacing units

### Section Organization

- Use **geometric dividers** between sections (chevron lines, sunburst separators, stepped borders)
- Apply **generous whitespace** (or dark space) around ornamented elements
- Create **hierarchy through scale** -- oversized headings, medium subheadings, refined body text
- Employ **angular containers** -- frames, borders, and panels with geometric embellishment

---

## CSS/Design Techniques

### Metallic Gradient Effects

```css
/* Gold metallic gradient for headings or accents */
.deco-gold-text {
  background: linear-gradient(
    135deg,
    #bf953f, #fcf6ba, #b38728, #fbf5b7, #aa771c
  );
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  background-clip: text;
}

/* Gold metallic border */
.deco-gold-border {
  border: 2px solid transparent;
  border-image: linear-gradient(
    135deg,
    #bf953f, #fcf6ba, #b38728
  ) 1;
}

/* Chrome/silver gradient */
.deco-chrome {
  background: linear-gradient(
    135deg,
    #c0c0c0, #e8e8e8, #a9a9a9, #d4d4d4, #b0b0b0
  );
}
```

### Geometric Borders and Dividers

```css
/* Stepped border effect */
.deco-stepped-border {
  border: 3px solid var(--deco-gold);
  outline: 1px solid var(--deco-gold);
  outline-offset: 6px;
  padding: 2rem;
}

/* Double-line geometric divider */
.deco-divider {
  height: 0;
  border: none;
  border-top: 3px solid var(--deco-gold);
  border-bottom: 1px solid var(--deco-gold);
  margin: 2rem auto;
  width: 60%;
  position: relative;
}

/* Chevron separator using CSS */
.deco-chevron::after {
  content: '';
  display: block;
  width: 40px;
  height: 40px;
  border-right: 3px solid var(--deco-gold);
  border-bottom: 3px solid var(--deco-gold);
  transform: rotate(45deg);
  margin: -20px auto 0;
}
```

### Sunburst / Radiating Pattern (CSS-only)

```css
.deco-sunburst {
  background: repeating-conic-gradient(
    var(--deco-gold) 0deg 5deg,
    transparent 5deg 10deg
  );
  opacity: 0.1;
  position: absolute;
  inset: 0;
  pointer-events: none;
}
```

### Art Deco Card / Panel

```css
.deco-card {
  background: var(--deco-charcoal);
  border: 1px solid var(--deco-gold);
  padding: 2rem;
  position: relative;
  text-align: center;
}

/* Corner ornaments */
.deco-card::before,
.deco-card::after {
  content: '';
  position: absolute;
  width: 30px;
  height: 30px;
  border-color: var(--deco-gold);
  border-style: solid;
}

.deco-card::before {
  top: 8px;
  left: 8px;
  border-width: 2px 0 0 2px;
}

.deco-card::after {
  bottom: 8px;
  right: 8px;
  border-width: 0 2px 2px 0;
}
```

### Fan/Arch Decorative Element

```css
.deco-fan {
  width: 200px;
  height: 100px;
  background: conic-gradient(
    from 180deg at 50% 100%,
    var(--deco-gold) 0deg,
    transparent 20deg,
    var(--deco-gold) 40deg,
    transparent 60deg,
    var(--deco-gold) 80deg,
    transparent 100deg,
    var(--deco-gold) 120deg,
    transparent 140deg,
    var(--deco-gold) 160deg,
    transparent 180deg
  );
  border-radius: 200px 200px 0 0;
  opacity: 0.3;
}
```

### Geometric Shadow/Depth

```css
/* Sharp geometric shadow (not soft box-shadow) */
.deco-shadow {
  box-shadow:
    4px 4px 0 0 var(--deco-gold),
    8px 8px 0 0 var(--deco-charcoal);
}
```

### Background Texture Pattern

```css
/* Repeating diamond/rhombus pattern */
.deco-pattern-bg {
  background-color: var(--deco-black);
  background-image:
    linear-gradient(45deg, var(--deco-gold) 25%, transparent 25%),
    linear-gradient(-45deg, var(--deco-gold) 25%, transparent 25%),
    linear-gradient(45deg, transparent 75%, var(--deco-gold) 75%),
    linear-gradient(-45deg, transparent 75%, var(--deco-gold) 75%);
  background-size: 20px 20px;
  background-position: 0 0, 0 10px, 10px -10px, -10px 0px;
  opacity: 0.05;
}
```

---

## Materials and Textures (Visual Metaphors for Web)

Physical Art Deco materials and their web equivalents:

| Physical Material | Web Equivalent |
|-------------------|----------------|
| Polished marble | Subtle noise texture overlay on light surfaces |
| Chrome / Brushed steel | Linear metallic gradients (silver/gray) |
| Gilt / Gold leaf | Gold gradient text, gold borders |
| Lacquer (high-gloss black) | Deep black backgrounds with subtle sheen gradients |
| Exotic wood grain | Warm brown textured backgrounds (subtle) |
| Stained glass | Jewel-tone color blocks with dark leading-style borders |
| Onyx | Dark translucent overlays with depth |
| Ivory / Bone | Off-white / cream tones for light themes |

---

## Sub-styles and Variations

### Early Art Deco (1910s-1920s)
- More ornamental and handcrafted
- Influenced by Cubism, Fauvism, and non-Western art (Egyptian, African, Mesoamerican)
- Rich surface decoration and exotic materials
- Heavier, more opulent feel

### Neo-Egyptian Art Deco
- Incorporates Egyptian motifs: scarabs, lotus flowers, papyrus columns, pyramidal forms
- Sparked by the discovery of Tutankhamun's tomb (1922)
- Geometric interpretation of Egyptian hieroglyphs and symbols

### Streamline Moderne (1930s)
- Evolved, later form of Art Deco
- Emphasizes **aerodynamic curves** over angular geometry
- Horizontal lines, rounded corners, nautical references
- Cleaner, less ornamented, more futuristic
- Chrome and glass over gold and exotic materials

---

## Related Aesthetics

| Aesthetic | Relationship to Art Deco |
|-----------|--------------------------|
| **Art Nouveau** | Predecessor; organic curves vs. Art Deco's geometry |
| **Bauhaus** | Contemporary; shares geometric focus, but Bauhaus is minimalist and functional |
| **Cubism** | Major influence; geometric abstraction of natural forms |
| **Futurism** | Shared fascination with speed, technology, and dynamism |
| **Decopunk** | Speculative fiction aesthetic based on Art Deco visual language |
| **Dieselpunk** | Retro-futuristic style drawing from 1920s-1940s industrial design |
| **Flapper** | Cultural companion aesthetic (1920s fashion and lifestyle) |
| **Streamline Moderne** | Direct evolution of Art Deco into softer, more aerodynamic forms |

---

## Quick-Start: Minimal Art Deco Page Template

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Art Deco Page</title>
  <link href="https://fonts.googleapis.com/css2?family=Poiret+One&family=Raleway:wght@300;400;600&family=Bebas+Neue&display=swap" rel="stylesheet">
  <style>
    :root {
      --deco-black: #1a1a1a;
      --deco-charcoal: #2d2d2d;
      --deco-cream: #f5f0e1;
      --deco-gold: #d4af37;
      --deco-gold-light: #e8d48b;
    }

    * { margin: 0; padding: 0; box-sizing: border-box; }

    body {
      background: var(--deco-black);
      color: var(--deco-cream);
      font-family: 'Raleway', sans-serif;
      font-weight: 300;
      letter-spacing: 0.03em;
      line-height: 1.7;
    }

    h1, h2, h3 {
      font-family: 'Poiret One', sans-serif;
      text-transform: uppercase;
      letter-spacing: 0.15em;
      color: var(--deco-gold);
    }

    .hero {
      text-align: center;
      padding: 6rem 2rem;
      border-bottom: 3px solid var(--deco-gold);
    }

    .hero h1 {
      font-family: 'Bebas Neue', sans-serif;
      font-size: clamp(3rem, 8vw, 7rem);
      letter-spacing: 0.2em;
    }

    .deco-divider {
      width: 60%;
      margin: 2rem auto;
      border: none;
      border-top: 3px solid var(--deco-gold);
      position: relative;
    }

    section {
      max-width: 900px;
      margin: 0 auto;
      padding: 4rem 2rem;
      text-align: center;
    }
  </style>
</head>
<body>
  <div class="hero">
    <h1>Title Here</h1>
    <hr class="deco-divider">
    <p>Subtitle or tagline in elegant Raleway</p>
  </div>
  <section>
    <h2>Section Heading</h2>
    <p>Content with Art Deco styling applied.</p>
  </section>
</body>
</html>
```
