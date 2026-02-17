# Seiz Breur Design Reference

Seiz Breur ("The Seven Brothers" in Breton) was a Breton artistic movement active from 1923 to 1947, founded by Jeanne Malivel. The movement synthesized **Art Deco geometry, Arts and Crafts philosophy, and Celtic/Breton cultural heritage** into a distinctive visual language. It rejected mass-produced tourist kitsch in favor of authentic, modern interpretations of traditional Breton forms. The aesthetic is defined by **bold wood-engraving linework, Celtic knotwork and spiral motifs, restrained earth-tone palettes with gold accents**, and a disciplined fusion of folk-art vitality with modernist structure.

---

## Visual Characteristics

### Core Motifs and Patterns

- **Triskelion (triskele)** -- the three-armed Celtic spiral symbol, used as a central decorative and symbolic device
- **Hermine (ermine)** -- the traditional symbol of Brittany, stylized as a repeating ornamental motif
- **Celtic knotwork** -- interlaced bands forming continuous, unbroken patterns; used for borders, dividers, and panel decoration
- **Saw-tooth patterns** -- sharp, angular zig-zag borders inspired by both Art Deco geometry and traditional Breton textile edging
- **Spirals** -- single and double spirals drawn from megalithic and Celtic stone carving traditions
- **Marine imagery** -- waves, fish, shells, and seaweed reflecting Brittany's Atlantic coastline
- **Peacock feathers and palmettes** -- stylized fan-shaped organic forms used as decorative fills
- **Religious and folkloric figures** -- saints, pilgrims, and legendary characters rendered in flat, emblematic compositions
- **Wood-engraving linework** -- bold, high-contrast black-and-white compositions with crisp, deliberate mark-making

### Design Principles

- **Cultural authenticity over decoration** -- every ornamental choice rooted in Breton heritage, never arbitrary
- **Modernist clarity with folk-art warmth** -- Art Deco's geometric discipline combined with the handcrafted vitality of traditional craft
- **High contrast, limited palette** -- visual impact through stark tonal relationships rather than chromatic variety
- **Flat, emblematic rendering** -- figures and forms abstracted into two-dimensional, poster-like compositions
- **Unity of disciplines** -- design principles applied consistently across architecture, furniture, ceramics, graphics, textiles, and liturgical objects
- **Adaptation to material** -- decorative forms shaped by the function and material of the object, not imposed onto it
- **Bold negative space** -- compositions balance dense patterning against generous open areas for visual breathing room

---

## Color Palette

### Primary Scheme

The palette is deliberately restrained, drawing from the Breton landscape (granite coast, dark forests, overcast Atlantic skies), traditional craft pigments, and the black-and-white dominance of wood-engraving prints.

| Role | Colors |
|------|--------|
| **Dominant** | Black, off-white, warm gray |
| **Earth tones** | Raw umber, burnt sienna, stone gray, slate |
| **Accent** | Antique gold, tarnished bronze |
| **Secondary** | Deep forest green, muted navy, charcoal brown |
| **Highlights** | Parchment cream, warm ivory |

### Detailed Color Table

| Color | Hex (suggested) | Usage |
|-------|-----------------|-------|
| Ink Black | `#1c1a17`, `#0f0e0c` | Primary text, linework, dominant backgrounds |
| Warm Off-White | `#f2ece0`, `#e8e0d0` | Page backgrounds, negative space |
| Granite Gray | `#6b6560`, `#7a746e` | Secondary text, mid-tone accents |
| Stone Gray | `#a09890`, `#8e857c` | Borders, subtle backgrounds |
| Raw Umber | `#5c4a38`, `#6b5542` | Dark accents, text on light backgrounds |
| Burnt Sienna | `#8a5a3c`, `#9b6344` | Warm accent details, decorative elements |
| Antique Gold | `#b8963e`, `#a6873a` | Headings, ornamental details, key accents |
| Tarnished Bronze | `#8c7a4e`, `#7d6e45` | Secondary metallic accents, borders |
| Forest Green | `#2c4a2e`, `#3a5a3c` | Accent panels, nature motifs |
| Muted Navy | `#2a3448`, `#344050` | Deep backgrounds, secondary dark tone |
| Parchment Cream | `#f5f0e1`, `#ede5d4` | Light backgrounds, text areas |
| Slate | `#4a4a4e`, `#555560` | Structural elements, dark mid-tones |

### Suggested CSS Custom Properties

```css
:root {
  /* Base / Backgrounds */
  --sb-ink-black: #1c1a17;
  --sb-charcoal: #2a2622;
  --sb-off-white: #f2ece0;
  --sb-parchment: #f5f0e1;
  --sb-warm-ivory: #ede5d4;

  /* Grays / Neutrals */
  --sb-granite: #6b6560;
  --sb-stone: #a09890;
  --sb-slate: #4a4a4e;

  /* Earth Tones */
  --sb-raw-umber: #5c4a38;
  --sb-burnt-sienna: #8a5a3c;
  --sb-dark-brown: #3e2e20;

  /* Metallics */
  --sb-antique-gold: #b8963e;
  --sb-bronze: #8c7a4e;
  --sb-gold-light: #d4bb6e;

  /* Accent Colors */
  --sb-forest-green: #2c4a2e;
  --sb-muted-navy: #2a3448;

  /* Functional */
  --sb-bg-primary: var(--sb-off-white);
  --sb-bg-secondary: var(--sb-parchment);
  --sb-bg-dark: var(--sb-ink-black);
  --sb-text-primary: var(--sb-ink-black);
  --sb-text-secondary: var(--sb-granite);
  --sb-accent: var(--sb-antique-gold);
  --sb-border: var(--sb-raw-umber);
}
```

### Color Approach

- **Black-and-white dominance** -- reflecting the wood-engraving and print heritage of the movement
- **Earth tones as the chromatic range** -- muted, natural pigment colors; never bright or synthetic
- **Gold as the singular luxury accent** -- used sparingly for headings and ornamental emphasis
- **High tonal contrast** -- dark ink tones against pale parchment, minimal mid-tone mudding
- **Monochromatic restraint** -- most compositions use only 2-3 colors at a time
- **Cool grays balanced by warm browns** -- the granite coast meets the hearth

---

## Typography

### Typeface Characteristics

Seiz Breur typography blends Celtic manuscript traditions with Art Deco's geometric boldness and the graphic clarity of woodcut lettering. Key characteristics:

- **Bold, angular letterforms** with strong vertical emphasis -- influenced by Art Deco display type
- **Celtic uncial influences** -- rounded, calligraphic forms derived from insular manuscript traditions
- **Condensed proportions** -- tall, narrow letters conveying both modernity and monumental weight
- **Uppercase-heavy display usage** -- headlines and titles set in all-caps with wide letter-spacing
- **Hand-lettered quality** -- letterforms that retain the mark of the engraver's tool
- **Strong stroke contrast** in display sizes; even weight in body text
- **Decorative initials** -- large ornamental capitals incorporating Celtic knotwork or spiral motifs

### Recommended Web Fonts (Google Fonts / Free)

| Font | Style | Usage |
|------|-------|-------|
| **Cinzel** | Classical inscriptional serif | Headlines, section titles |
| **Cinzel Decorative** | Ornamental inscriptional serif | Feature titles, display text |
| **Uncial Antiqua** | Celtic uncial display | Decorative headings, drop caps |
| **Bebas Neue** | Bold condensed sans | Banners, large display headlines |
| **Josefin Sans** | Geometric vintage sans | Subheadings, labels |
| **EB Garamond** | Humanist old-style serif | Body text, paragraphs |
| **Cormorant Garamond** | Elegant old-style serif | Body text, long passages |
| **Sorts Mill Goudy** | Arts and Crafts-era serif | Body copy, captions |
| **Cardo** | Scholarly old-style serif | Secondary body text |

### Typography CSS Example

```css
/* Import fonts */
@import url('https://fonts.googleapis.com/css2?family=Cinzel:wght@400;600;700&family=Cinzel+Decorative:wght@400;700&family=Uncial+Antiqua&family=EB+Garamond:ital,wght@0,400;0,600;0,700;1,400&family=Bebas+Neue&display=swap');

/* Headlines */
h1, h2, h3 {
  font-family: 'Cinzel', 'Georgia', serif;
  color: var(--sb-ink-black);
  font-weight: 700;
  letter-spacing: 0.08em;
  text-transform: uppercase;
  line-height: 1.2;
}

/* Display / Hero text */
.sb-display {
  font-family: 'Bebas Neue', 'Cinzel', sans-serif;
  font-size: clamp(3rem, 8vw, 7rem);
  letter-spacing: 0.15em;
  line-height: 1.05;
  color: var(--sb-ink-black);
}

/* Subtitle / accent headings */
.sb-subtitle {
  font-family: 'Josefin Sans', sans-serif;
  font-weight: 300;
  letter-spacing: 0.2em;
  text-transform: uppercase;
  color: var(--sb-antique-gold);
  font-size: 0.9rem;
}

/* Body text */
body {
  font-family: 'EB Garamond', 'Cormorant Garamond', 'Georgia', serif;
  font-size: 1.125rem;
  font-weight: 400;
  letter-spacing: 0.01em;
  line-height: 1.8;
  color: var(--sb-ink-black);
}

/* Celtic decorative drop cap */
.sb-dropcap::first-letter {
  font-family: 'Uncial Antiqua', serif;
  font-size: 4em;
  float: left;
  line-height: 0.75;
  margin-right: 0.1em;
  margin-top: 0.05em;
  color: var(--sb-antique-gold);
}
```

---

## Layout Principles

### Grid and Structure

- **Strong central axis** -- content organized along a vertical spine, reflecting monument and stele compositions
- **Symmetrical layouts** -- bilateral symmetry dominant, as in Celtic manuscript pages and Breton heraldic design
- **Generous margins and negative space** -- compositions breathe; density is localized to ornamental borders and headers
- **Modular, panel-based sections** -- content blocks framed like woodcut prints, each section a self-contained visual unit
- **Vertical emphasis** -- tall, narrow proportions in both layout and typography, conveying solemnity

### Section Organization

- Use **Celtic knotwork or saw-tooth dividers** between sections
- Apply **bordered panels** for key content -- double-line or knotwork-framed containers
- Create **hierarchy through weight and contrast** -- bold black headings, lighter body text, gold accent details
- Employ **banner-style headers** for major sections, echoing poster and print design
- **Footer colophons** with a small hermine or triskele ornament

---

## CSS/Design Techniques

### Celtic Knotwork Border

```css
/* Interlaced-style double border evoking knotwork */
.sb-knot-border {
  border: 3px solid var(--sb-ink-black);
  outline: 3px solid var(--sb-ink-black);
  outline-offset: 5px;
  padding: 2.5rem;
  position: relative;
  background: var(--sb-off-white);
}

/* Corner ornament squares */
.sb-knot-border::before,
.sb-knot-border::after {
  content: '';
  position: absolute;
  width: 14px;
  height: 14px;
  background: var(--sb-antique-gold);
  border: 2px solid var(--sb-ink-black);
}

.sb-knot-border::before {
  top: -5px;
  left: -5px;
}

.sb-knot-border::after {
  bottom: -5px;
  right: -5px;
}
```

### Saw-Tooth Divider

```css
/* Zig-zag / saw-tooth pattern divider */
.sb-sawtooth {
  height: 16px;
  width: 100%;
  background:
    linear-gradient(135deg, var(--sb-ink-black) 33.33%, transparent 33.33%) 0 0,
    linear-gradient(225deg, var(--sb-ink-black) 33.33%, transparent 33.33%) 0 0;
  background-size: 16px 16px;
  background-repeat: repeat-x;
  margin: 2rem 0;
}

/* Simpler single-line saw-tooth */
.sb-sawtooth-thin {
  height: 8px;
  width: 60%;
  margin: 2rem auto;
  background:
    linear-gradient(135deg, var(--sb-antique-gold) 33.33%, transparent 33.33%) 0 0,
    linear-gradient(225deg, var(--sb-antique-gold) 33.33%, transparent 33.33%) 0 0;
  background-size: 8px 8px;
  background-repeat: repeat-x;
}
```

### Triskele / Spiral Ornament (CSS-only)

```css
/* Decorative triple-spiral evocation */
.sb-triskele {
  width: 60px;
  height: 60px;
  margin: 1.5rem auto;
  position: relative;
}

.sb-triskele::before {
  content: '';
  position: absolute;
  inset: 0;
  background: conic-gradient(
    from 0deg,
    var(--sb-antique-gold) 0deg 40deg,
    transparent 40deg 120deg,
    var(--sb-antique-gold) 120deg 160deg,
    transparent 160deg 240deg,
    var(--sb-antique-gold) 240deg 280deg,
    transparent 280deg 360deg
  );
  border-radius: 50%;
  opacity: 0.7;
}
```

### Wood-Engraving Texture Overlay

```css
/* Subtle grain texture evoking woodcut printing */
.sb-woodgrain-bg {
  background-color: var(--sb-off-white);
  background-image:
    repeating-linear-gradient(
      0deg,
      transparent,
      transparent 2px,
      rgba(28, 26, 23, 0.02) 2px,
      rgba(28, 26, 23, 0.02) 3px
    );
}

/* Dark variant with engraved feel */
.sb-engraved-bg {
  background-color: var(--sb-ink-black);
  background-image:
    repeating-linear-gradient(
      90deg,
      transparent,
      transparent 1px,
      rgba(242, 236, 224, 0.03) 1px,
      rgba(242, 236, 224, 0.03) 2px
    );
}
```

### Ornamental Divider with Center Motif

```css
/* Horizontal rule with decorative hermine center */
.sb-divider {
  display: flex;
  align-items: center;
  gap: 1.2rem;
  margin: 2.5rem auto;
  width: 70%;
  color: var(--sb-antique-gold);
}

.sb-divider::before,
.sb-divider::after {
  content: '';
  flex: 1;
  height: 2px;
  background: var(--sb-ink-black);
}

.sb-divider span {
  font-size: 1.2rem;
  color: var(--sb-antique-gold);
  letter-spacing: 0.3em;
}
```

### Seiz Breur Card / Panel

```css
.sb-card {
  background: var(--sb-off-white);
  border: 2px solid var(--sb-ink-black);
  padding: 2.5rem;
  position: relative;
  max-width: 750px;
  margin: 2rem auto;
}

/* Inner gold accent border */
.sb-card-inner {
  border: 1px solid var(--sb-antique-gold);
  padding: 2rem;
}

.sb-card h3 {
  font-family: 'Cinzel', serif;
  text-align: center;
  text-transform: uppercase;
  letter-spacing: 0.1em;
  margin-bottom: 1rem;
  color: var(--sb-ink-black);
}
```

### Gold Accent Text

```css
/* Antique gold gradient for headings */
.sb-gold-text {
  background: linear-gradient(
    135deg,
    #8c7a4e, #b8963e, #d4bb6e, #b8963e, #8c7a4e
  );
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  background-clip: text;
}

/* Gold border accent */
.sb-gold-border {
  border: 2px solid transparent;
  border-image: linear-gradient(
    to right,
    var(--sb-bronze),
    var(--sb-antique-gold),
    var(--sb-gold-light),
    var(--sb-antique-gold),
    var(--sb-bronze)
  ) 1;
}
```

### Dark Variant (Ink / Engraved)

```css
.sb-dark {
  background: var(--sb-ink-black);
  color: var(--sb-off-white);
}

.sb-dark h1, .sb-dark h2, .sb-dark h3 {
  color: var(--sb-antique-gold);
}

.sb-dark .sb-knot-border {
  background: var(--sb-charcoal);
  border-color: var(--sb-antique-gold);
  outline-color: var(--sb-antique-gold);
}

.sb-dark .sb-divider::before,
.sb-dark .sb-divider::after {
  background: var(--sb-antique-gold);
}
```

### Geometric Shadow

```css
/* Sharp, print-block-style shadow */
.sb-shadow {
  box-shadow:
    3px 3px 0 0 var(--sb-ink-black),
    6px 6px 0 0 rgba(28, 26, 23, 0.15);
}
```

---

## Materials and Textures (Visual Metaphors for Web)

Physical Seiz Breur materials and their web equivalents:

| Physical Material | Web Equivalent |
|-------------------|----------------|
| Wood-engraved print | High-contrast black-and-white sections with fine linear texture overlays |
| Granite (Breton coast) | Cool gray textured backgrounds with subtle grain |
| Parchment / handmade paper | Warm off-white backgrounds with subtle noise |
| Gold leaf / gilt | Antique gold gradient text and borders |
| Carved stone (menhirs, crosses) | Heavy, monumental typography with deep letter-spacing |
| Embroidered textile | Dense ornamental borders and repeating pattern bands |
| Faience / glazed ceramic | Muted color panels with dark outline borders |
| Stained glass | Jewel-tone accent panels with heavy dark leading-style dividers |
| Wrought iron | Dark structural frames and grid lines |
| Celtic metalwork | Interlaced knotwork border patterns |

---

## Iconic Design Examples

### Representative Works (Visual Reference)

- **Wood engravings by Jeanne Malivel** -- stark black-and-white compositions with Celtic motifs, flat figure rendering, and bold negative space; the foundational visual language of the movement
- **Posters and postcards** -- Art Deco-influenced graphic design with Breton symbols; condensed uppercase type, central symmetrical compositions, limited color
- **Kornog magazine covers** -- modernist layouts combining Celtic ornamentation with clean typographic hierarchy
- **Embroidered banners** -- textile works featuring hermine and triskele patterns in traditional needlework translated to modern graphic design
- **Faience figurines** -- ceramic works depicting Breton saints and folk characters in simplified, geometric forms
- **Stained glass panels** -- religious works by Xavier de Langlais combining Celtic knotwork borders with figurative scenes in deep, muted tones
- **Furniture and architectural detail** -- carved wood panels and stone elements featuring saw-tooth and spiral motifs integrated into functional structures

---

## Related Aesthetics

| Aesthetic | Relationship to Seiz Breur |
|-----------|---------------------------|
| **Art Deco** | Primary formal influence; geometric structure, bold symmetry, condensed typography |
| **Arts and Crafts** | Philosophical kinship; anti-industrial ethos, handcraft values, unity of art and utility |
| **Bauhaus** | Contemporary parallel; shared interest in integrating art, craft, and industry; functional modernism |
| **Celtic Revival** | Cultural root; Celtic knotwork, spirals, manuscript traditions, and mythological subject matter |
| **Regionalism** | Broader movement context; valorization of local culture against centralizing homogenization |

---

## Quick-Start: Minimal Seiz Breur Page Template

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Seiz Breur Page</title>
  <link href="https://fonts.googleapis.com/css2?family=Cinzel:wght@400;600;700&family=EB+Garamond:ital,wght@0,400;0,600;0,700;1,400&family=Bebas+Neue&family=Uncial+Antiqua&display=swap" rel="stylesheet">
  <style>
    :root {
      --sb-ink-black: #1c1a17;
      --sb-charcoal: #2a2622;
      --sb-off-white: #f2ece0;
      --sb-parchment: #f5f0e1;
      --sb-raw-umber: #5c4a38;
      --sb-antique-gold: #b8963e;
      --sb-granite: #6b6560;
    }

    * { margin: 0; padding: 0; box-sizing: border-box; }

    body {
      background: var(--sb-off-white);
      color: var(--sb-ink-black);
      font-family: 'EB Garamond', 'Georgia', serif;
      font-size: 1.125rem;
      line-height: 1.8;
      letter-spacing: 0.01em;
    }

    h1, h2, h3 {
      font-family: 'Cinzel', serif;
      font-weight: 700;
      text-transform: uppercase;
      letter-spacing: 0.08em;
    }

    .hero {
      text-align: center;
      padding: 6rem 2rem 5rem;
      border-bottom: 3px solid var(--sb-ink-black);
      background: var(--sb-off-white);
    }

    .hero h1 {
      font-family: 'Bebas Neue', sans-serif;
      font-size: clamp(3rem, 8vw, 7rem);
      letter-spacing: 0.15em;
      color: var(--sb-ink-black);
    }

    .hero .subtitle {
      font-family: 'Cinzel', serif;
      font-weight: 400;
      letter-spacing: 0.2em;
      text-transform: uppercase;
      color: var(--sb-antique-gold);
      font-size: 0.9rem;
      margin-top: 1rem;
    }

    .sb-divider {
      display: flex;
      align-items: center;
      gap: 1rem;
      margin: 2rem auto;
      width: 50%;
    }

    .sb-divider::before,
    .sb-divider::after {
      content: '';
      flex: 1;
      height: 2px;
      background: var(--sb-ink-black);
    }

    .sb-divider span {
      color: var(--sb-antique-gold);
      font-size: 1.2rem;
    }

    section {
      max-width: 750px;
      margin: 0 auto;
      padding: 4rem 2rem;
      text-align: center;
    }

    section h2 {
      margin-bottom: 1.5rem;
    }

    .sb-dropcap::first-letter {
      font-family: 'Uncial Antiqua', serif;
      font-size: 4em;
      float: left;
      line-height: 0.75;
      margin-right: 0.1em;
      color: var(--sb-antique-gold);
    }
  </style>
</head>
<body>
  <div class="hero">
    <h1>Title Here</h1>
    <div class="sb-divider"><span>&#10038;</span></div>
    <p class="subtitle">Subtitle in Cinzel with gold accent</p>
  </div>
  <section>
    <h2>Section Heading</h2>
    <p class="sb-dropcap">Content styled in the Seiz Breur tradition, blending Celtic heritage with modernist clarity and the bold discipline of the woodcut print.</p>
  </section>
</body>
</html>
```
