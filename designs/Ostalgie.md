# Ostalgie -- Design Reference

> An aesthetic rooted in nostalgia for East Germany (the GDR, 1949--1990), expressed through
> the visual culture of socialist-era consumer goods, state graphic design, prefabricated
> architecture, and the quiet charm of constrained industrial production. Also known as
> **GDR Nostalgia**, **DDR-Nostalgie**, or **Ost-Nostalgie**. The term blends "Ost" (east)
> with "Nostalgie" (nostalgia), coined in 1992 by comedian Uwe Steimle.

---

## Visual Characteristics

- **Tone:** Warm, bittersweet, wistfully retro. A sentimental fondness for everyday objects and graphic design produced under material constraint. Not ironic kitsch -- sincere affection for simplicity and familiarity.
- **Design philosophy:** Functional, durable, unpretentious mass-production aesthetics. Objects and graphics designed within strict state constraints, resulting in a distinctive look born from limited materials and centralized oversight.
- **Packaging and label design:** Period-specific product labels from the 1950s--1980s with simple typography, limited color runs, and utilitarian layouts. Brands like Club-Cola, Rondo coffee, Juwel cigarettes, and Spreewald pickles define the visual vernacular.
- **Graphic style:** Flat color fields, limited palette (often 2--4 hues per composition), bold simplified shapes, and functional clarity. Influenced by Bauhaus principles filtered through socialist production constraints.
- **Propaganda graphics:** Political posters, banners, FDJ (Free German Youth) materials, state coat of arms, and organizational insignia used as decorative elements and cultural signifiers.
- **Material culture icons:** Trabant automobiles, Ampelmannchen (East German pedestrian traffic light figures), Plattenbau (prefabricated concrete apartment blocks), Sandmannchen (TV character), and DEFA film materials.
- **Architectural references:** Prefabricated housing blocks (Plattenbau), socialist classicism, post-Bauhaus functionalism, monumental civic buildings, and the distinctive geometric abstraction of GDR public spaces.
- **Interior references:** Authentic GDR-era domestic furnishings -- simple wooden furniture, synthetic Dederon fabrics, patterned wallpaper in muted floral or geometric prints, and functional household objects with minimal ornamentation.
- **Texture and materiality:** Rough concrete, synthetic textiles (Dederon), bakelite plastics, printed paper with visible halftone grain, weathered signage, and machine-carved lettering on composite materials.

## Color Palette

The Ostalgie palette is defined by desaturated, muted tones reflecting the materials and printing limitations of GDR consumer goods. Warm browns and oranges ground the palette, punctuated by institutional blues and greens. Nothing is vivid -- everything feels slightly faded, as if recalled from memory.

### Primary Palette

| Role            | Colors                                                        |
|-----------------|---------------------------------------------------------------|
| Warm base tones | Ochre brown, sand beige, warm tan, mustard yellow             |
| Cool accents    | Muted teal, institutional blue, slate grey-blue               |
| State colors    | Socialist red, deep navy, hammer gold                         |
| Neutrals        | Concrete grey, warm off-white, dark charcoal, faded cream     |
| Earth tones     | Olive green, muted rust orange, dusty terracotta              |

### CSS Custom Properties

```css
:root {
  /* Warm Browns & Ochres */
  --ost-ochre:            #B8860B;
  --ost-sand:             #D2B48C;
  --ost-tan:              #C4A882;
  --ost-warm-brown:       #8B6914;
  --ost-mustard:          #C9A830;

  /* Blues & Teals */
  --ost-teal:             #5F8A8B;
  --ost-institutional-blue: #4A6D8C;
  --ost-slate-blue:       #607B8B;
  --ost-navy:             #2C3E50;
  --ost-faded-blue:       #7B9BAA;

  /* State Reds & Golds */
  --ost-socialist-red:    #B83230;
  --ost-deep-red:         #8B2323;
  --ost-hammer-gold:      #D4A017;
  --ost-banner-red:       #C0392B;

  /* Greens & Olives */
  --ost-olive:            #6B7B3A;
  --ost-muted-green:      #7D8B6A;
  --ost-sage:             #8F9B7A;

  /* Earth & Rust */
  --ost-rust:             #B7613F;
  --ost-terracotta:       #C47A5A;
  --ost-burnt-orange:     #A0522D;

  /* Neutrals */
  --ost-concrete:         #9B9B8E;
  --ost-dark-concrete:    #6B6B60;
  --ost-charcoal:         #3C3C34;
  --ost-cream:            #F2EADB;
  --ost-off-white:        #EDE6D6;
  --ost-warm-white:       #FAF6EE;
  --ost-paper:            #E8DFD0;
}
```

### Color Usage Guidelines

- **Backgrounds:** Use warm neutrals -- cream, off-white, paper, or sand. For contrast sections use concrete grey or charcoal. The overall feeling should be like aged packaging or printed ephemera from the 1970s.
- **Headlines and bold text:** Charcoal or dark concrete on light backgrounds. Socialist red for emphasis. Institutional blue for secondary headings.
- **Accent elements:** Socialist red and hammer gold for badges, borders, and state-symbol decorations. Use sparingly -- these are punctuation, not wallpaper.
- **Cards and panels:** Sand, tan, or paper tones with subtle borders in concrete grey. Alternating warm and cool neutrals between sections.
- **Overall feeling:** Muted, warm, and slightly faded. High saturation is absent. Colors feel like they were printed on rough paper with limited ink, then aged for 30 years. Nostalgic without being grey and depressing -- there is warmth and sincerity in the palette.

## Typography

### Font Characteristics

GDR typography was produced by VEB Typoart Dresden, the state type foundry, whose designers (Herbert Thannhaeuser, Albert Kapr) created faces rooted in traditional German book design and printing culture. The result is typography that is functional, slightly condensed, and grounded in classical European sans-serif and slab-serif traditions -- similar to Western counterparts but with a distinctly restrained, utilitarian character.

- **Headlines:** Bold, condensed sans-serifs or geometric grotesks. Uppercase with moderate letter-spacing. Functional and commanding without being flashy. Reminiscent of state signage and product labels.
- **Body text:** Clean, highly legible sans-serifs with a slightly mechanical character. Warm and readable, referencing the functional clarity of GDR book design.
- **Accent text:** Condensed or narrow-width faces for labels, badges, and product-style callouts. Slab-serifs for a more institutional or official tone.
- **Display / nostalgic:** Rounded or geometric faces that evoke 1960s--1970s Eastern Bloc product packaging and signage.

### Recommended Web Fonts

| Role        | Fonts (Google Fonts / System)                                    |
|-------------|------------------------------------------------------------------|
| Display     | Oswald (Bold), Bebas Neue, Barlow Condensed (Bold)               |
| Headings    | Roboto Condensed (Bold), DM Sans (Bold), Barlow (SemiBold)       |
| Body        | Source Sans 3, IBM Plex Sans, Work Sans, Inter                   |
| Labels      | Roboto Condensed, Barlow Condensed, Space Grotesk                |
| Nostalgic   | Jost, Rubik, Nunito (for softer, rounded GDR packaging feel)     |

### CSS Typography Example

```css
@import url('https://fonts.googleapis.com/css2?family=Oswald:wght@500;700&family=Roboto+Condensed:wght@400;700&family=Source+Sans+3:wght@400;600&family=Jost:wght@400;500&display=swap');

h1, h2, h3 {
  font-family: 'Oswald', 'Arial Narrow', sans-serif;
  font-weight: 700;
  text-transform: uppercase;
  letter-spacing: 0.06em;
  line-height: 1.15;
  color: var(--ost-charcoal);
}

h1 {
  font-size: clamp(2.5rem, 5vw, 4rem);
  letter-spacing: 0.1em;
  color: var(--ost-socialist-red);
}

h2 {
  font-family: 'Roboto Condensed', sans-serif;
  font-size: clamp(1.5rem, 3vw, 2.2rem);
  color: var(--ost-institutional-blue);
}

body {
  font-family: 'Source Sans 3', 'IBM Plex Sans', sans-serif;
  font-weight: 400;
  line-height: 1.65;
  color: var(--ost-charcoal);
}

.label, .badge-text {
  font-family: 'Roboto Condensed', sans-serif;
  font-weight: 700;
  text-transform: uppercase;
  letter-spacing: 0.12em;
  font-size: 0.8rem;
  color: var(--ost-dark-concrete);
}
```

## Key Design Elements and Motifs

### Recurring Visual Motifs

- **Ampelmannchen** -- the distinctive East German pedestrian signal figure (hat-wearing, arm-outstretched walking man or standing figure); used as icons, decorative elements, and identity markers
- **Trabant silhouette** -- the iconic boxy car outline; used as decorative illustrations and nostalgic symbols
- **State coat of arms elements** -- compass, wheat wreath, and hammer motifs adapted as decorative borders and badges
- **Plattenbau grid** -- the repetitive window grid of prefabricated apartment blocks; used as background patterns and section dividers
- **Product label frames** -- rectangular or oval frames with simple borders mimicking period packaging design
- **Five-pointed stars** -- state symbols used as bullet points, decorative accents, and hierarchical markers
- **Wheat sheaves** -- socialist abundance motifs for borders and badge decorations
- **FDJ sun emblem** -- rising sun with radiating lines, adapted as background decoration
- **Geometric wallpaper patterns** -- repeating abstract or simplified floral motifs in muted tones
- **Compass and gear symbols** -- industry and progress motifs from state iconography
- **Banner ribbons** -- simple flat ribbons containing text, mimicking state ceremony and propaganda banners

### Decorative CSS Patterns

```css
/* Plattenbau window grid pattern */
.plattenbau-grid {
  background-color: var(--ost-concrete);
  background-image:
    repeating-linear-gradient(
      0deg,
      transparent,
      transparent 38px,
      var(--ost-dark-concrete) 38px,
      var(--ost-dark-concrete) 40px
    ),
    repeating-linear-gradient(
      90deg,
      transparent,
      transparent 28px,
      var(--ost-dark-concrete) 28px,
      var(--ost-dark-concrete) 30px
    );
}

/* Product label / packaging frame */
.ost-label-frame {
  border: 2px solid var(--ost-charcoal);
  outline: 1px solid var(--ost-charcoal);
  outline-offset: 4px;
  padding: 1.5rem 2rem;
  text-align: center;
  position: relative;
}

.ost-label-frame::before {
  content: '';
  position: absolute;
  inset: -8px;
  border: 1px solid var(--ost-concrete);
}

/* State banner ribbon */
.ost-banner {
  background: var(--ost-socialist-red);
  color: var(--ost-warm-white);
  font-family: 'Oswald', sans-serif;
  font-weight: 700;
  text-transform: uppercase;
  letter-spacing: 0.08em;
  padding: 0.6rem 2.5rem;
  display: inline-block;
  text-align: center;
  position: relative;
}

.ost-banner::before,
.ost-banner::after {
  content: '';
  position: absolute;
  top: 0;
  border-style: solid;
  border-color: var(--ost-socialist-red);
  height: 100%;
}

.ost-banner::before {
  left: -1.2rem;
  border-width: 1.2rem 1.2rem 1.2rem 0;
  border-left-color: transparent;
}

.ost-banner::after {
  right: -1.2rem;
  border-width: 1.2rem 0 1.2rem 1.2rem;
  border-right-color: transparent;
}

/* Five-pointed star accent */
.ost-star {
  display: inline-block;
  width: 24px;
  height: 24px;
  background: var(--ost-socialist-red);
  clip-path: polygon(
    50% 0%, 61% 35%, 98% 35%, 68% 57%,
    79% 91%, 50% 70%, 21% 91%, 32% 57%,
    2% 35%, 39% 35%
  );
}

/* GDR-style geometric wallpaper pattern */
.ost-wallpaper {
  background-color: var(--ost-cream);
  background-image:
    radial-gradient(
      circle at 25% 25%,
      var(--ost-sand) 2px,
      transparent 2px
    ),
    radial-gradient(
      circle at 75% 75%,
      var(--ost-sand) 2px,
      transparent 2px
    );
  background-size: 30px 30px;
}

/* Horizontal stripe divider (state ceremony style) */
.ost-stripe-divider {
  height: 6px;
  background: linear-gradient(
    to right,
    var(--ost-socialist-red) 0%,
    var(--ost-socialist-red) 33%,
    var(--ost-hammer-gold) 33%,
    var(--ost-hammer-gold) 67%,
    var(--ost-socialist-red) 67%,
    var(--ost-socialist-red) 100%
  );
}
```

## Textures and Materials

- **Concrete and Plattenbau surfaces** -- raw, unfinished concrete with visible panel seams evoking prefabricated housing. Cool grey with warm undertones.
- **Aged packaging paper** -- slightly yellowed, rough-textured paper with visible fiber. The substrate for all nostalgic product label designs.
- **Dederon synthetic fabric** -- smooth, slightly shiny synthetic textile characteristic of GDR textile production. A subtle sheen texture.
- **Bakelite plastic** -- warm, dark-toned plastic with a slight translucency. Used in household objects, radios, and telephones.
- **Machine-carved composite signage** -- the distinctive weather-resistant black-and-white plastic composite of East Berlin street signs with technical, condensed letterforms.
- **Halftone print grain** -- coarse printing artifacts visible on mass-produced packaging and posters.
- **Wallpaper patterns** -- abstract floral or geometric motifs in ochre, beige, brown, and muted green on textured paper.

### CSS Texture Techniques

```css
/* Aged packaging paper */
.ost-aged-paper {
  background-color: var(--ost-paper);
  background-image:
    radial-gradient(
      ellipse at 30% 20%,
      rgba(184, 134, 11, 0.06) 0%,
      transparent 50%
    ),
    radial-gradient(
      ellipse at 70% 80%,
      rgba(139, 105, 20, 0.04) 0%,
      transparent 40%
    ),
    linear-gradient(
      to bottom,
      rgba(60, 60, 52, 0.03) 0%,
      transparent 15%,
      transparent 85%,
      rgba(60, 60, 52, 0.04) 100%
    );
}

/* Concrete / Plattenbau surface */
.ost-concrete-surface {
  background-color: var(--ost-concrete);
  background-image:
    linear-gradient(
      to bottom,
      rgba(0, 0, 0, 0.04) 0%,
      rgba(0, 0, 0, 0.01) 50%,
      rgba(0, 0, 0, 0.05) 100%
    );
}

/* Halftone print overlay */
.ost-halftone::after {
  content: '';
  position: absolute;
  inset: 0;
  background-image: radial-gradient(
    circle, rgba(60, 60, 52, 0.1) 1px, transparent 1px
  );
  background-size: 3px 3px;
  pointer-events: none;
  mix-blend-mode: multiply;
}

/* Dederon fabric sheen */
.ost-dederon {
  background: linear-gradient(
    135deg,
    var(--ost-faded-blue) 0%,
    color-mix(in srgb, var(--ost-faded-blue) 85%, white) 40%,
    var(--ost-faded-blue) 60%,
    color-mix(in srgb, var(--ost-faded-blue) 90%, white) 100%
  );
}

/* Subtle wallpaper texture for backgrounds */
.ost-wallpaper-texture {
  background-color: var(--ost-cream);
  background-image:
    repeating-linear-gradient(
      45deg,
      transparent,
      transparent 10px,
      rgba(184, 134, 11, 0.03) 10px,
      rgba(184, 134, 11, 0.03) 11px
    ),
    repeating-linear-gradient(
      -45deg,
      transparent,
      transparent 10px,
      rgba(107, 123, 58, 0.03) 10px,
      rgba(107, 123, 58, 0.03) 11px
    );
}
```

## Layout Principles

### Structure

- **Functional and grid-based** -- compositions follow a clear, utilitarian grid reminiscent of state-published materials. Content is organized in orderly blocks with defined boundaries.
- **Centered and symmetrical** -- a preference for bilateral symmetry reflecting institutional and official design conventions. Center-aligned headings and balanced card layouts.
- **Modular repetition** -- the Plattenbau philosophy extends to layout: repeating uniform modules (cards, panels, sections) arranged in predictable grids.
- **Clear hierarchy** -- state-influenced information design with unambiguous heading levels, labeled sections, and structured content flow.
- **Generous borders and frames** -- content enclosed in visible frames and double-line borders evoking product labels and official documents.
- **Horizontal banding** -- sections separated by colored stripe dividers or border rules, creating a layered, band-like composition.

### Grid and Spacing

```css
.ost-layout {
  display: grid;
  grid-template-columns: 1fr;
  gap: 0;
  max-width: 1200px;
  margin: 0 auto;
  background: var(--ost-cream);
}

.ost-section {
  padding: 3.5rem 2.5rem;
  position: relative;
  border-bottom: 2px solid var(--ost-concrete);
}

.ost-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
  gap: 2rem;
  padding: 2.5rem;
}

.ost-card {
  background: var(--ost-warm-white);
  border: 2px solid var(--ost-charcoal);
  padding: 2rem 1.5rem;
  text-align: center;
  position: relative;
}

/* Double-frame product label effect */
.ost-card::before {
  content: '';
  position: absolute;
  inset: 4px;
  border: 1px solid var(--ost-concrete);
  pointer-events: none;
}

/* Section label badge */
.ost-section-label {
  display: inline-block;
  background: var(--ost-charcoal);
  color: var(--ost-warm-white);
  font-family: 'Roboto Condensed', sans-serif;
  font-weight: 700;
  font-size: 0.75rem;
  text-transform: uppercase;
  letter-spacing: 0.15em;
  padding: 0.3rem 1.2rem;
  margin-bottom: 1.5rem;
}

/* Horizontal section divider */
.ost-divider {
  height: 4px;
  background: var(--ost-charcoal);
  position: relative;
}

.ost-divider::after {
  content: '';
  position: absolute;
  top: 6px;
  left: 0;
  right: 0;
  height: 1px;
  background: var(--ost-concrete);
}
```

### Header / Hero Section

```css
.ost-hero {
  background: var(--ost-charcoal);
  text-align: center;
  padding: 5rem 2rem 4rem;
  position: relative;
  overflow: hidden;
  border-bottom: 4px solid var(--ost-socialist-red);
}

/* Subtle Plattenbau grid overlay */
.ost-hero::before {
  content: '';
  position: absolute;
  inset: 0;
  background-image:
    repeating-linear-gradient(
      0deg,
      transparent,
      transparent 58px,
      rgba(155, 155, 142, 0.08) 58px,
      rgba(155, 155, 142, 0.08) 60px
    ),
    repeating-linear-gradient(
      90deg,
      transparent,
      transparent 78px,
      rgba(155, 155, 142, 0.08) 78px,
      rgba(155, 155, 142, 0.08) 80px
    );
  pointer-events: none;
}

.ost-hero h1 {
  position: relative;
  z-index: 1;
  font-family: 'Oswald', sans-serif;
  font-size: clamp(3rem, 6vw, 5rem);
  font-weight: 700;
  color: var(--ost-warm-white);
  text-transform: uppercase;
  letter-spacing: 0.12em;
  margin-bottom: 0.5rem;
}

.ost-hero .subtitle {
  position: relative;
  z-index: 1;
  font-family: 'Roboto Condensed', sans-serif;
  font-weight: 400;
  font-size: 1.2rem;
  text-transform: uppercase;
  letter-spacing: 0.2em;
  color: var(--ost-sand);
  border-top: 1px solid var(--ost-concrete);
  border-bottom: 1px solid var(--ost-concrete);
  display: inline-block;
  padding: 0.5rem 2rem;
  margin-top: 1.5rem;
}

/* Red star accent above title */
.ost-hero .star-accent {
  position: relative;
  z-index: 1;
  display: inline-block;
  width: 30px;
  height: 30px;
  background: var(--ost-socialist-red);
  clip-path: polygon(
    50% 0%, 61% 35%, 98% 35%, 68% 57%,
    79% 91%, 50% 70%, 21% 91%, 32% 57%,
    2% 35%, 39% 35%
  );
  margin-bottom: 1.5rem;
}
```

### Call-to-Action / Button

```css
.ost-button {
  display: inline-block;
  font-family: 'Oswald', sans-serif;
  font-weight: 700;
  font-size: 1rem;
  text-transform: uppercase;
  letter-spacing: 0.08em;
  color: var(--ost-warm-white);
  background: var(--ost-socialist-red);
  border: 2px solid var(--ost-deep-red);
  padding: 0.8rem 2.5rem;
  cursor: pointer;
  transition: all 0.2s ease;
  text-decoration: none;
}

.ost-button:hover {
  background: var(--ost-deep-red);
  box-shadow: 0 2px 8px rgba(60, 60, 52, 0.3);
}

.ost-button--secondary {
  background: var(--ost-charcoal);
  border-color: var(--ost-dark-concrete);
  color: var(--ost-cream);
}

.ost-button--secondary:hover {
  background: var(--ost-dark-concrete);
}

.ost-button--outline {
  background: transparent;
  border: 2px solid var(--ost-charcoal);
  color: var(--ost-charcoal);
}

.ost-button--outline:hover {
  background: var(--ost-charcoal);
  color: var(--ost-cream);
}
```

## Design Techniques Summary

| Technique                    | Implementation                                                          |
|------------------------------|-------------------------------------------------------------------------|
| Plattenbau grid              | `repeating-linear-gradient()` in both axes creating window-like pattern |
| Product label frames         | Double borders using `border` + `outline` or nested `::before` pseudo   |
| Aged paper texture           | Layered `radial-gradient()` with warm semi-transparent tints            |
| State banner ribbon          | Pseudo-elements with angled borders forming ribbon tails                |
| Five-pointed star            | CSS `clip-path: polygon()` in socialist red                             |
| Red-gold stripe dividers     | `linear-gradient()` with hard color stops                               |
| Muted color desaturation     | All accent colors kept at low-to-medium saturation, warm undertones     |
| Halftone print grain         | Tiny `radial-gradient` dots with `mix-blend-mode: multiply`             |
| Section label badges         | Dark background + white condensed uppercase text, small and rectangular |
| Double-line borders          | `border` + `::before` inset to create period packaging frame effect     |
| Concrete texture             | Subtle vertical `linear-gradient` with low-opacity dark tints           |
| Institutional color coding   | Socialist red for primary emphasis, institutional blue for secondary     |

## Related Aesthetics

These aesthetics share visual DNA with Ostalgie and can be blended or referenced:

| Aesthetic              | Relationship                                                                |
|------------------------|-----------------------------------------------------------------------------|
| **Brutalism**          | Shares the raw concrete materiality and monumental civic architecture       |
| **Socialist Realism**  | The propagandistic visual language that Ostalgie recontextualizes           |
| **Heroic Realism**     | Propaganda poster techniques that inform the state-graphic elements         |
| **Sovietwave**         | Digital, vaporwave-inflected nostalgia for Soviet-era aesthetics            |
| **Soviet Nostalgia**   | Broader Eastern Bloc nostalgia movement; Ostalgie is the German variant     |
| **Yugo-Nostalgia**     | Yugoslav parallel -- same mechanism of post-socialist nostalgia             |
| **Mid-Century Modern** | Shares the 1950s--1960s functional design origins and Bauhaus lineage       |
| **Retrofuturism**      | GDR's optimistic space-age and industrial imagery shares retrofuturist DNA  |
| **Kitsch**             | The affectionate embrace of mass-produced, low-prestige consumer objects    |
| **Plakatstil**         | German poster tradition -- flat colors, bold type, simplified forms         |

## Quick-Start Template Skeleton

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Ostalgie Page</title>
  <link href="https://fonts.googleapis.com/css2?family=Oswald:wght@500;700&family=Roboto+Condensed:wght@400;700&family=Source+Sans+3:wght@400;600&display=swap" rel="stylesheet">
  <style>
    :root {
      --ost-ochre:              #B8860B;
      --ost-sand:               #D2B48C;
      --ost-tan:                #C4A882;
      --ost-mustard:            #C9A830;
      --ost-teal:               #5F8A8B;
      --ost-institutional-blue: #4A6D8C;
      --ost-navy:               #2C3E50;
      --ost-socialist-red:      #B83230;
      --ost-deep-red:           #8B2323;
      --ost-hammer-gold:        #D4A017;
      --ost-olive:              #6B7B3A;
      --ost-muted-green:        #7D8B6A;
      --ost-rust:               #B7613F;
      --ost-concrete:           #9B9B8E;
      --ost-dark-concrete:      #6B6B60;
      --ost-charcoal:           #3C3C34;
      --ost-cream:              #F2EADB;
      --ost-off-white:          #EDE6D6;
      --ost-warm-white:         #FAF6EE;
      --ost-paper:              #E8DFD0;
    }

    * { box-sizing: border-box; margin: 0; padding: 0; }

    body {
      font-family: 'Source Sans 3', 'Helvetica Neue', sans-serif;
      background: var(--ost-cream);
      color: var(--ost-charcoal);
      line-height: 1.65;
    }

    header {
      background: var(--ost-charcoal);
      text-align: center;
      padding: 5rem 2rem 4rem;
      position: relative;
      overflow: hidden;
      border-bottom: 4px solid var(--ost-socialist-red);
    }

    /* Plattenbau grid overlay */
    header::before {
      content: '';
      position: absolute;
      inset: 0;
      background-image:
        repeating-linear-gradient(
          0deg, transparent, transparent 58px,
          rgba(155,155,142,0.08) 58px, rgba(155,155,142,0.08) 60px
        ),
        repeating-linear-gradient(
          90deg, transparent, transparent 78px,
          rgba(155,155,142,0.08) 78px, rgba(155,155,142,0.08) 80px
        );
      pointer-events: none;
    }

    header h1 {
      position: relative; z-index: 1;
      font-family: 'Oswald', sans-serif;
      font-size: clamp(3rem, 6vw, 5rem);
      font-weight: 700;
      color: var(--ost-warm-white);
      text-transform: uppercase;
      letter-spacing: 0.12em;
    }

    header p {
      position: relative; z-index: 1;
      font-family: 'Roboto Condensed', sans-serif;
      font-weight: 400;
      font-size: 1.1rem;
      text-transform: uppercase;
      letter-spacing: 0.2em;
      color: var(--ost-sand);
      border-top: 1px solid var(--ost-concrete);
      border-bottom: 1px solid var(--ost-concrete);
      display: inline-block;
      padding: 0.5rem 2rem;
      margin-top: 1.5rem;
    }

    /* Red-gold-red stripe divider */
    .divider {
      height: 6px;
      background: linear-gradient(
        to right,
        var(--ost-socialist-red) 0%, var(--ost-socialist-red) 33%,
        var(--ost-hammer-gold) 33%, var(--ost-hammer-gold) 67%,
        var(--ost-socialist-red) 67%, var(--ost-socialist-red) 100%
      );
    }

    main {
      max-width: 1100px;
      margin: 0 auto;
      padding: 3.5rem 2rem;
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
      gap: 2rem;
    }

    .card {
      background: var(--ost-warm-white);
      border: 2px solid var(--ost-charcoal);
      padding: 2rem 1.5rem;
      text-align: center;
      position: relative;
    }

    /* Inner frame line for packaging feel */
    .card::before {
      content: '';
      position: absolute;
      inset: 4px;
      border: 1px solid var(--ost-concrete);
      pointer-events: none;
    }

    .card h2 {
      font-family: 'Roboto Condensed', sans-serif;
      font-weight: 700;
      font-size: 1.3rem;
      text-transform: uppercase;
      letter-spacing: 0.06em;
      color: var(--ost-institutional-blue);
      margin-bottom: 1rem;
    }

    .card p {
      color: var(--ost-charcoal);
      line-height: 1.7;
      font-size: 0.95rem;
    }

    footer {
      background: var(--ost-charcoal);
      color: var(--ost-concrete);
      text-align: center;
      padding: 2rem;
      font-family: 'Roboto Condensed', sans-serif;
      text-transform: uppercase;
      letter-spacing: 0.1em;
      font-size: 0.85rem;
      border-top: 4px solid var(--ost-socialist-red);
    }
  </style>
</head>
<body>
  <header>
    <h1>Page Title Here</h1>
    <p>A Subtitle in the Spirit of the East</p>
  </header>
  <div class="divider"></div>
  <main>
    <div class="card">
      <h2>Section One</h2>
      <p>Content goes here. Simple, functional, and sincere.</p>
    </div>
    <div class="card">
      <h2>Section Two</h2>
      <p>Content goes here. Every element earns its place.</p>
    </div>
    <div class="card">
      <h2>Section Three</h2>
      <p>Content goes here. Warmth through restraint.</p>
    </div>
  </main>
  <footer>
    <p>Built with care and a touch of nostalgia</p>
  </footer>
</body>
</html>
```
