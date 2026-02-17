# Four Colors Design Reference

Four Colors is a color scheme and design aesthetic that dominated consumer products and consumer technology from the mid-2000s to the mid-2010s. It first gained prominence around 2004 through Apple's iPod "Silhouette" advertising campaign. The style is characterized by **flat visuals that predominantly use four colors** -- electric lime, sky blue, hot pink, and neon orange -- applied to products, packaging, and promotional materials. It functions as a subgenre bridging **Superflat Pop** and **Frutiger Aero**, emphasizing personalization, bold saturation, and eye-catching consumer appeal. The four colors reference Japanese seasonal symbolism: pink (spring), green (summer), orange (autumn), blue (winter).

---

## Visual Characteristics

### Core Motifs and Elements

- **Four-color constraint** -- designs predominantly use exactly four saturated colors (electric lime, sky blue, hot pink, neon orange) as the organizing principle
- **Flat, non-dimensional rendering** -- no gradients, drop shadows, or 3D effects; all surfaces are solid color fills
- **Bold saturation** -- colors are pushed to maximum vibrancy and chroma; muted tones are avoided entirely
- **Consumer product focus** -- the aesthetic originates from and is most at home on physical products, packaging, and advertising
- **Silhouette compositions** -- human or object silhouettes placed against vivid solid-color backgrounds (directly from the iPod campaign)
- **Color variant systems** -- the same product or design offered in each of the four colors, encouraging personalization and collection
- **Clean, minimal surfaces** -- products and designs feature smooth, unadorned surfaces where the color itself is the primary design element
- **Rainbow extensions** -- the four core colors occasionally expand into wider rainbow arrangements while maintaining the original four as anchors

### Design Principles

- **Color as identity** -- each of the four hues serves as a distinct identity marker; products are differentiated by color alone
- **Flat composition without texture** -- surfaces are smooth and plastic-like; no noise, grain, or material texture
- **Personalization through color choice** -- the aesthetic empowers the consumer to express individuality via color selection
- **Eye-catching adjacency** -- the four colors are placed in direct proximity for maximum visual impact and energy
- **Youthful, optimistic tone** -- the palette and its application communicate fun, energy, and accessibility
- **Seasonal/cyclical balance** -- the four colors form a balanced system representing completeness (four seasons, four directions)
- **Product photography as design** -- the product itself, rendered in one of the four colors against a contrasting solid background, constitutes the complete visual composition

---

## Color Palette

### Primary Four Colors

| Color | Hex (suggested) | Usage |
|-------|-----------------|-------|
| Electric Lime | `#7FFF00`, `#ADFF2F` | Primary accent, spring/summer energy, backgrounds |
| Sky Blue | `#00BFFF`, `#38BDF8` | Cool accent, winter tone, tech-forward panels |
| Hot Pink | `#FF1493`, `#FF69B4` | Warm accent, spring tone, highlight elements |
| Neon Orange | `#FF6600`, `#FF8C00` | Warm accent, autumn tone, call-to-action elements |

### Extended Rainbow Variant

| Color | Hex (suggested) | Usage |
|-------|-----------------|-------|
| Vivid Red | `#FF0033`, `#EF4444` | Expanded palette accent, alerts, emphasis |
| Bright Yellow | `#FFD700`, `#FACC15` | Expanded palette accent, highlights, badges |
| True Purple | `#8B00FF`, `#A855F7` | Expanded palette accent, premium/special elements |

### Supporting / Neutral Colors

| Color | Hex (suggested) | Usage |
|-------|-----------------|-------|
| Pure White | `#FFFFFF` | Product backgrounds, text on colored panels |
| Near-Black | `#1A1A1A`, `#111111` | Silhouette figures, text, dark backgrounds |
| Black | `#000000` | Silhouette figures, iPod-style compositions |
| Light Gray | `#F5F5F5`, `#E5E5E5` | Neutral section backgrounds, UI chrome |
| Silver | `#C0C0C0`, `#A3A3A3` | Product accents, metallic references (iPod body) |

### Suggested CSS Custom Properties

```css
:root {
  /* Primary Four Colors */
  --fc-lime: #7FFF00;
  --fc-lime-soft: #ADFF2F;
  --fc-sky: #00BFFF;
  --fc-sky-soft: #38BDF8;
  --fc-pink: #FF1493;
  --fc-pink-soft: #FF69B4;
  --fc-orange: #FF6600;
  --fc-orange-soft: #FF8C00;

  /* Extended Rainbow */
  --fc-red: #FF0033;
  --fc-yellow: #FFD700;
  --fc-purple: #8B00FF;

  /* Neutrals */
  --fc-white: #FFFFFF;
  --fc-light-gray: #F5F5F5;
  --fc-silver: #C0C0C0;
  --fc-dark: #1A1A1A;
  --fc-black: #000000;

  /* Functional */
  --fc-bg-primary: var(--fc-white);
  --fc-bg-secondary: var(--fc-light-gray);
  --fc-text-primary: var(--fc-dark);
  --fc-text-on-color: var(--fc-white);
  --fc-accent-1: var(--fc-lime);
  --fc-accent-2: var(--fc-sky);
  --fc-accent-3: var(--fc-pink);
  --fc-accent-4: var(--fc-orange);
}
```

### Color Usage Approaches

- **Solid flat fills only** -- no gradients, no blending between colors; each surface is a single hue
- **Maximum saturation** -- use the purest, most vivid versions of each color; never desaturate
- **Four-color rotation** -- cycle through the four colors systematically across cards, sections, and elements
- **High-contrast pairings** -- place lime against pink, sky blue against orange for maximum visual energy
- **White or black as ground** -- products and elements sit on pure white or pure black; no colored backgrounds behind colored objects
- **Seasonal symbolism** -- when assigning colors to categories, consider the Japanese seasonal mapping (pink=spring, green=summer, orange=autumn, blue=winter)

---

## Typography

### Typeface Characteristics

Four Colors typography reflects the mid-2000s to mid-2010s consumer tech era:

- **Clean, modern sans-serif typefaces** -- matching the smooth, flat product surfaces
- **Medium-weight, confident letterforms** -- not too thin (unlike minimalism), not too heavy (unlike grunge)
- **Wide tracking on display text** -- airy, product-catalog feel
- **Legibility at all sizes** -- designed for packaging, advertising, and screen use
- **Slightly rounded terminals** -- softened forms that reference the friendly, consumer-oriented tone
- **Avoid decorative or serif typefaces** -- the style is emphatically modern and sans-serif

### Recommended Web Fonts (Google Fonts / Free)

| Font | Style | Usage |
|------|-------|-------|
| **Inter** | Modern geometric sans | Body text, UI elements, product descriptions |
| **Montserrat** | Geometric sans, confident | Headlines, hero text, product names |
| **Poppins** | Geometric sans, friendly | Headlines, subheadings, buttons |
| **Outfit** | Clean modern sans | All-purpose, slightly rounded |
| **Nunito Sans** | Humanist sans, approachable | Body text, paragraphs |
| **DM Sans** | Clean geometric sans | Body copy, secondary text |
| **Sora** | Modern geometric | Display headlines, bold statements |
| **Lexend** | Optimized for readability | Body text, UI labels |

### Typography CSS Example

```css
/* Google Fonts import */
@import url('https://fonts.googleapis.com/css2?family=Montserrat:wght@400;600;700;800&family=Inter:wght@400;500;600&display=swap');

/* Headlines */
h1, h2, h3 {
  font-family: 'Montserrat', 'Poppins', sans-serif;
  font-weight: 700;
  letter-spacing: 0.03em;
  text-transform: uppercase;
  color: var(--fc-dark);
}

/* Display / Hero text */
.fc-display {
  font-family: 'Montserrat', sans-serif;
  font-size: clamp(2.5rem, 7vw, 5.5rem);
  font-weight: 800;
  letter-spacing: 0.05em;
  text-transform: uppercase;
  line-height: 1.1;
}

/* Body text */
body {
  font-family: 'Inter', 'Nunito Sans', sans-serif;
  font-weight: 400;
  letter-spacing: 0.01em;
  line-height: 1.65;
  color: var(--fc-dark);
}

/* Product label / badge text */
.fc-label {
  font-family: 'Montserrat', sans-serif;
  font-weight: 600;
  font-size: 0.85rem;
  letter-spacing: 0.08em;
  text-transform: uppercase;
}
```

---

## Layout Principles

### Grid and Structure

- **Product-grid layout** -- items displayed in a uniform grid where each cell features one of the four colors
- **Generous whitespace** -- products and colored elements float in open white space, catalog-style
- **Four-column structure** -- naturally suited to four-column grids (one column per color)
- **Centered compositions** -- individual product/element presentations are centered on their solid-color background
- **Flat, poster-like sections** -- each section resembles a print advertisement or product poster
- **No visible borders or dividers** -- sections are separated by color changes alone

### Section Organization

- Use **alternating solid-color backgrounds** between sections, cycling through the four colors
- Apply **ample padding** within colored sections (minimum 4rem vertical padding) so content does not feel cramped
- Create **visual hierarchy through color intensity** -- the most important content gets the most vivid color background
- Employ a **silhouette-on-color pattern** for hero areas -- dark figures or product outlines on saturated backgrounds
- Use **white breathing sections** between colored sections to prevent visual fatigue
- Organize product/feature showcases as **color-coded card grids** where each card is a different color from the palette

### Responsive Considerations

- The four-column grid collapses to two columns on tablet and one column on mobile
- Colored sections maintain their full-bleed backgrounds at all breakpoints
- Typography scales down but retains uppercase treatment and wide tracking
- Silhouette compositions simplify to smaller, centered arrangements on narrow viewports

---

## CSS/Design Techniques

### Solid Color Section Panels

```css
/* Color-coded full-width sections */
.fc-section {
  padding: 5rem 2rem;
  text-align: center;
}

.fc-section-lime {
  background: var(--fc-lime);
  color: var(--fc-dark);
}

.fc-section-sky {
  background: var(--fc-sky);
  color: var(--fc-white);
}

.fc-section-pink {
  background: var(--fc-pink);
  color: var(--fc-white);
}

.fc-section-orange {
  background: var(--fc-orange);
  color: var(--fc-white);
}
```

### Four-Color Card Grid

```css
/* Product/feature card grid cycling through four colors */
.fc-card-grid {
  display: grid;
  grid-template-columns: repeat(4, 1fr);
  gap: 1.5rem;
  padding: 3rem 2rem;
  max-width: 1280px;
  margin: 0 auto;
}

@media (max-width: 1024px) {
  .fc-card-grid {
    grid-template-columns: repeat(2, 1fr);
  }
}

@media (max-width: 640px) {
  .fc-card-grid {
    grid-template-columns: 1fr;
  }
}

.fc-card {
  padding: 2.5rem 2rem;
  text-align: center;
  color: var(--fc-white);
  transition: transform 0.2s ease;
}

.fc-card:hover {
  transform: scale(1.03);
}

/* Assign colors in rotation */
.fc-card:nth-child(4n+1) { background: var(--fc-lime); color: var(--fc-dark); }
.fc-card:nth-child(4n+2) { background: var(--fc-sky); }
.fc-card:nth-child(4n+3) { background: var(--fc-pink); }
.fc-card:nth-child(4n+4) { background: var(--fc-orange); }
```

### iPod Silhouette Hero Pattern

```css
/* Silhouette-on-color hero area inspired by iPod campaign */
.fc-hero {
  position: relative;
  background: var(--fc-pink);
  color: var(--fc-white);
  min-height: 80vh;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  text-align: center;
  padding: 4rem 2rem;
  overflow: hidden;
}

.fc-hero-silhouette {
  /* Dark silhouette figure overlaid on vivid background */
  position: absolute;
  bottom: 0;
  right: 10%;
  width: 40%;
  max-width: 400px;
  filter: brightness(0); /* Forces any image to pure black silhouette */
  opacity: 0.9;
}

.fc-hero h1 {
  font-family: 'Montserrat', sans-serif;
  font-size: clamp(3rem, 8vw, 6rem);
  font-weight: 800;
  text-transform: uppercase;
  letter-spacing: 0.06em;
  position: relative;
  z-index: 1;
}
```

### Color Swatch / Variant Selector

```css
/* Product color variant selector (iPod/iPhone style) */
.fc-color-selector {
  display: flex;
  gap: 0.75rem;
  justify-content: center;
  padding: 1.5rem 0;
}

.fc-swatch {
  width: 2.5rem;
  height: 2.5rem;
  border-radius: 50%;
  border: 3px solid transparent;
  cursor: pointer;
  transition: border-color 0.2s ease, transform 0.15s ease;
}

.fc-swatch:hover {
  transform: scale(1.15);
}

.fc-swatch.active {
  border-color: var(--fc-dark);
}

.fc-swatch--lime { background: var(--fc-lime); }
.fc-swatch--sky { background: var(--fc-sky); }
.fc-swatch--pink { background: var(--fc-pink); }
.fc-swatch--orange { background: var(--fc-orange); }
```

### Flat Button System

```css
/* Flat, bold buttons matching the Four Colors ethos */
.fc-button {
  display: inline-block;
  padding: 0.85rem 2.5rem;
  border: none;
  font-family: 'Montserrat', sans-serif;
  font-weight: 700;
  font-size: 0.9rem;
  letter-spacing: 0.06em;
  text-transform: uppercase;
  text-decoration: none;
  cursor: pointer;
  transition: transform 0.15s ease, opacity 0.15s ease;
}

.fc-button:hover {
  transform: scale(1.05);
  opacity: 0.92;
}

/* Pill variant */
.fc-button--pill {
  border-radius: 999px;
}

/* Square variant */
.fc-button--square {
  border-radius: 0;
}

/* Color variants */
.fc-button--lime { background: var(--fc-lime); color: var(--fc-dark); }
.fc-button--sky { background: var(--fc-sky); color: var(--fc-white); }
.fc-button--pink { background: var(--fc-pink); color: var(--fc-white); }
.fc-button--orange { background: var(--fc-orange); color: var(--fc-white); }
```

### Four-Color Stripe / Divider

```css
/* Horizontal four-color stripe divider */
.fc-stripe {
  display: flex;
  height: 6px;
  width: 100%;
}

.fc-stripe > span {
  flex: 1;
}

.fc-stripe > span:nth-child(1) { background: var(--fc-lime); }
.fc-stripe > span:nth-child(2) { background: var(--fc-sky); }
.fc-stripe > span:nth-child(3) { background: var(--fc-pink); }
.fc-stripe > span:nth-child(4) { background: var(--fc-orange); }

/* CSS-only gradient stripe alternative */
.fc-stripe-gradient {
  height: 6px;
  background: linear-gradient(
    90deg,
    var(--fc-lime) 0%,
    var(--fc-lime) 25%,
    var(--fc-sky) 25%,
    var(--fc-sky) 50%,
    var(--fc-pink) 50%,
    var(--fc-pink) 75%,
    var(--fc-orange) 75%,
    var(--fc-orange) 100%
  );
}
```

### Color-Background Swap Animation

```css
/* Cycling background color animation (iPod ad style) */
@keyframes fc-color-cycle {
  0%   { background-color: var(--fc-lime); }
  25%  { background-color: var(--fc-sky); }
  50%  { background-color: var(--fc-pink); }
  75%  { background-color: var(--fc-orange); }
  100% { background-color: var(--fc-lime); }
}

.fc-cycle-bg {
  animation: fc-color-cycle 8s ease-in-out infinite;
}
```

### Product Showcase Card

```css
/* Clean product card on white background */
.fc-product-card {
  background: var(--fc-white);
  padding: 2rem;
  text-align: center;
  border: none;
  box-shadow: none; /* No shadows in flat design */
}

.fc-product-card img {
  max-width: 200px;
  height: auto;
  margin: 0 auto 1.5rem;
  display: block;
}

.fc-product-card h3 {
  font-family: 'Montserrat', sans-serif;
  font-weight: 700;
  font-size: 1.1rem;
  text-transform: uppercase;
  letter-spacing: 0.04em;
  margin-bottom: 0.5rem;
}

.fc-product-card .price {
  font-family: 'Inter', sans-serif;
  font-weight: 600;
  font-size: 1.25rem;
  color: var(--fc-pink);
}
```

---

## Applications by Medium

### Consumer Electronics and Products

- Apple iPod Nano/Shuffle (2005) -- the origin point, with each model available in lime, sky blue, pink, and orange
- iPhone 5C (2013) -- extended the Four Colors philosophy to smartphones
- Nintendo 64 "Funtastic Series" (1996) -- translucent colored console variants
- Nintendo Wii accessories (2006) -- colored controller jackets and accessories
- Motorola Pebl (2005) -- colored flip phone variants
- BlendJet blenders, iLuv Bubblegum earphones, Post-it Notes -- consumer goods adopting the four-color variant system
- PlayStation 2 and 3 -- limited-edition color variants

### Games and Interactive Media

- Katamari series (2004-2023) -- vibrant four-color flat compositions
- Just Dance series (2009-2024) -- neon silhouettes on saturated color backgrounds
- Wii Party (2010) -- four-player color coding matching the aesthetic

### Television and Entertainment

- The Fresh Beat Band (2009-2013) -- each character assigned one of the four colors
- The Backyardigans (2004-2013) -- colorful flat backgrounds and character design
- Eurovision Song Contest 2007 -- stage and branding design
- Life Lessons with Uramichi Oniisan -- anime color palette reference

### Packaging and Advertising

- Daiso, Fujifilm, Sony -- Japanese consumer brands extensively using the four-color system
- Product catalog layouts with white backgrounds and color-coded product variants
- Advertising campaigns featuring silhouettes on solid color fields

---

## Related Aesthetics

| Aesthetic | Relationship to Four Colors |
|-----------|----------------------------|
| **Superflat Pop** | Parent aesthetic; Four Colors is a subgenre of Superflat Pop's flat, saturated color fields |
| **Frutiger Aero** | Parent aesthetic; Four Colors bridges into Frutiger Aero's optimistic, nature-referencing consumer tech design |
| **Bright Tertiaries** | Closest relative; shares flat color-block approach, similar palette, and consumer-friendly design language |
| **Flat Design** | Shared commitment to flat rendering with no gradients, shadows, or 3D effects |
| **Corporate** | Shared clean, product-focused visual language for branding and marketing materials |
| **Dollar Store Vernacular** | Shares the mass-produced consumer product context and bright color packaging |
| **McBling** | Overlapping era (mid-2000s) and shared emphasis on bold, flashy consumer aesthetics |
| **Pop Art** | Shared use of bold, flat color and consumer culture as subject matter |
| **Technozen** | Overlapping tech-forward optimism and clean product design |
| **Vectordelia** | Shared vibrant color palette and flat vector design approach |
| **Old Web** | Shared era of bright, unrestrained color usage in digital contexts |
| **Figuration Narrative** | Connection through flat, illustrative design language |
| **UrBling** | Overlapping era and shared consumer product/fashion color boldness |

---

## Quick-Start: Minimal Four Colors Page Template

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Four Colors Page</title>
  <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@400;600;700;800&family=Inter:wght@400;500;600&display=swap" rel="stylesheet">
  <style>
    :root {
      --fc-lime: #7FFF00;
      --fc-sky: #00BFFF;
      --fc-pink: #FF1493;
      --fc-orange: #FF6600;
      --fc-white: #FFFFFF;
      --fc-dark: #1A1A1A;
      --fc-black: #000000;
    }

    * { margin: 0; padding: 0; box-sizing: border-box; }

    body {
      background: var(--fc-white);
      color: var(--fc-dark);
      font-family: 'Inter', sans-serif;
      font-weight: 400;
      line-height: 1.65;
    }

    h1, h2, h3 {
      font-family: 'Montserrat', sans-serif;
      font-weight: 700;
      letter-spacing: 0.03em;
      text-transform: uppercase;
    }

    /* Four-color stripe header */
    .stripe {
      display: flex;
      height: 6px;
    }
    .stripe span { flex: 1; }
    .stripe span:nth-child(1) { background: var(--fc-lime); }
    .stripe span:nth-child(2) { background: var(--fc-sky); }
    .stripe span:nth-child(3) { background: var(--fc-pink); }
    .stripe span:nth-child(4) { background: var(--fc-orange); }

    /* Hero with cycling background */
    .hero {
      background: var(--fc-pink);
      color: var(--fc-white);
      text-align: center;
      padding: 6rem 2rem;
      position: relative;
      overflow: hidden;
    }

    .hero h1 {
      font-size: clamp(2.5rem, 7vw, 5.5rem);
      font-weight: 800;
      letter-spacing: 0.06em;
      color: var(--fc-white);
    }

    .hero p {
      font-size: 1.2rem;
      margin-top: 1rem;
      opacity: 0.9;
    }

    /* Four-color card grid */
    .cards {
      display: grid;
      grid-template-columns: repeat(4, 1fr);
      gap: 0;
      max-width: 1280px;
      margin: 0 auto;
    }

    @media (max-width: 1024px) {
      .cards { grid-template-columns: repeat(2, 1fr); }
    }
    @media (max-width: 640px) {
      .cards { grid-template-columns: 1fr; }
    }

    .card {
      padding: 3rem 2rem;
      text-align: center;
      color: var(--fc-white);
    }

    .card:nth-child(4n+1) { background: var(--fc-lime); color: var(--fc-dark); }
    .card:nth-child(4n+2) { background: var(--fc-sky); }
    .card:nth-child(4n+3) { background: var(--fc-pink); }
    .card:nth-child(4n+4) { background: var(--fc-orange); }

    .card h2 {
      font-size: 1.3rem;
      margin-bottom: 0.75rem;
    }

    /* Content section */
    .content {
      max-width: 900px;
      margin: 0 auto;
      padding: 5rem 2rem;
      text-align: center;
    }

    .content h2 {
      margin-bottom: 1.5rem;
    }

    /* Flat button */
    .btn {
      display: inline-block;
      padding: 0.85rem 2.5rem;
      background: var(--fc-sky);
      color: var(--fc-white);
      font-family: 'Montserrat', sans-serif;
      font-weight: 700;
      font-size: 0.9rem;
      letter-spacing: 0.06em;
      text-transform: uppercase;
      text-decoration: none;
      border: none;
      border-radius: 999px;
      cursor: pointer;
      margin-top: 1.5rem;
    }
  </style>
</head>
<body>
  <div class="stripe">
    <span></span><span></span><span></span><span></span>
  </div>
  <div class="hero">
    <h1>Title Here</h1>
    <p>Subtitle in clean Inter type</p>
  </div>
  <div class="cards">
    <div class="card">
      <h2>Lime</h2>
      <p>Content in a flat color panel.</p>
    </div>
    <div class="card">
      <h2>Sky Blue</h2>
      <p>Content in a flat color panel.</p>
    </div>
    <div class="card">
      <h2>Hot Pink</h2>
      <p>Content in a flat color panel.</p>
    </div>
    <div class="card">
      <h2>Neon Orange</h2>
      <p>Content in a flat color panel.</p>
    </div>
  </div>
  <div class="content">
    <h2>Section Heading</h2>
    <p>Content with Four Colors styling applied. The aesthetic emphasizes bold, flat, saturated color as the primary design element.</p>
    <br>
    <a href="#" class="btn">Call to Action</a>
  </div>
  <div class="stripe">
    <span></span><span></span><span></span><span></span>
  </div>
</body>
</html>
```
