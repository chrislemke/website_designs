# Plakatstil Design Reference

Plakatstil (German: "Poster Style"), also known as Sachplakat ("Object Poster"), is an early modern graphic design movement that emerged in Germany around 1906. It represents a radical simplification of advertising imagery -- stripping away all non-essential elements to achieve **immediate, memorable visual impact** through a single isolated subject, flat bold colors, and minimal text. The style was a direct rejection of the ornate complexity of Art Nouveau, prioritizing **focus, clarity, directness, and readability** above all else. Pioneered by Lucian Bernhard, it became a foundational influence on Bauhaus, the International Typographic Style, and ultimately Flat Design.

---

## Visual Characteristics

### Core Design Traits

- **Single isolated subject** -- one product, object, or figure dominates the entire composition; nothing competes for attention
- **Flat, solid color fills** -- all surfaces are rendered in uniform, unmodulated color with no gradients, shading, or tonal variation
- **Extreme reduction** -- objects and figures are simplified to their most essential outlines and geometric forms; all non-essential detail is eliminated
- **Bold, high-contrast color** -- a limited palette of 2-4 strong hues creates immediate visual punch; colors are saturated and poster-grade
- **Plain, uncluttered backgrounds** -- backgrounds are a single flat color field with no scenery, texture, or decoration
- **Generous negative space** -- open background area is a deliberate compositional strategy, not wasted space; it isolates and elevates the subject
- **No ornamentation** -- no decorative borders, flourishes, patterns, or embellishments of any kind
- **Brand name as design element** -- the product or brand name is the only text, rendered in bold lettering that is compositionally integrated with the image rather than layered on top
- **Geometric simplification of forms** -- people, objects, and scenes are reduced to basic shapes and clean outlines
- **Poster-scale legibility** -- every element is designed to read instantly at large scale and from a distance

### Design Principles

- Strip away everything that does not directly serve recognition and impact
- The product is the hero -- it should be the first and only thing the viewer sees
- Color is structural, not decorative -- each color area defines a shape or form
- Typography is part of the composition, not a caption added afterward
- Negative space creates focus -- the emptier the background, the stronger the subject
- Communicate in a single glance -- if the viewer needs more than one second, the design has failed
- Flat rendering is a deliberate choice, not a limitation -- it creates bold graphic power
- Simplicity is not emptiness; every remaining element carries maximum weight

---

## Color Palette

### Primary Palette

Plakatstil uses severely limited palettes of 2-4 bold, high-contrast colors. The palette is always dominated by one strong background color and one or two accent colors for the subject and text.

| Color Name | Hex | Role / Usage |
|------------|-----|-------------|
| **Poster Red** | `#C8102E` | Primary accent, bold subjects, brand text |
| **Deep Red** | `#8B1A1A` | Darker red variant, secondary forms |
| **Signal Blue** | `#003E7E` | Primary accent alternative, backgrounds |
| **Royal Blue** | `#1B3A6B` | Darker blue, subject rendering |
| **Olive** | `#5B6236` | Earth-tone accent, military/industrial subjects |
| **Dark Olive** | `#3D4125` | Deeper olive for contrast |
| **Lamp Black** | `#1A1A1A` | Text, outlines, dark subjects, backgrounds |
| **Rich Black** | `#0D0D0D` | Maximum-contrast backgrounds |
| **Warm White** | `#F5F0E1` | Light backgrounds (evokes aged paper) |
| **Cream** | `#FFFDD0` | Softer light background alternative |
| **Ochre Yellow** | `#CC7722` | Warm accent, highlights on dark backgrounds |
| **Goldenrod** | `#DAA520` | Secondary warm accent, brand text on dark |
| **Forest Green** | `#2D5F2D` | Subject accent, product rendering |
| **Burnt Orange** | `#BF5700` | Warm accent, attention-drawing highlight |

### Suggested CSS Custom Properties

```css
:root {
  /* Core palette */
  --plakat-black: #1a1a1a;
  --plakat-rich-black: #0d0d0d;
  --plakat-cream: #f5f0e1;
  --plakat-warm-white: #fffdd0;

  /* Bold accents */
  --plakat-red: #c8102e;
  --plakat-red-dark: #8b1a1a;
  --plakat-blue: #003e7e;
  --plakat-blue-dark: #1b3a6b;
  --plakat-olive: #5b6236;
  --plakat-olive-dark: #3d4125;

  /* Secondary accents */
  --plakat-ochre: #cc7722;
  --plakat-goldenrod: #daa520;
  --plakat-green: #2d5f2d;
  --plakat-orange: #bf5700;

  /* Functional assignments */
  --plakat-bg-primary: var(--plakat-cream);
  --plakat-bg-dark: var(--plakat-rich-black);
  --plakat-text-primary: var(--plakat-black);
  --plakat-text-inverse: var(--plakat-cream);
  --plakat-accent: var(--plakat-red);
}
```

### Color Usage Guidelines

- **Maximum 3-4 colors per composition** -- this is the defining constraint; every additional color dilutes impact
- **One dominant background color** fills the entire page or section; subjects and text sit on top in contrasting flat color
- **Dark backgrounds with bright subjects** is the most characteristic combination (black or deep blue background with red, ochre, or cream subject)
- **Light backgrounds (cream/warm white) with bold dark subjects** is the secondary classic approach
- Never use gradients, color transitions, or opacity effects -- all fills are flat solids at 100%
- Color boundaries are hard and clean -- no feathering, blending, or anti-aliased color transitions
- Each color area defines a distinct shape; color IS the drawing tool
- Avoid pastels, muted tones, or desaturated hues -- Plakatstil demands bold, poster-grade saturation

---

## Typography

### Typeface Characteristics

Plakatstil typography is defined by:

- **Bold, blocky sans-serif letterforms** -- thick strokes, high visual weight, designed for instant legibility at distance
- **Minimal text** -- typically only the brand or product name; no taglines, slogans, or body copy
- **Typography as composition** -- letters are sized, placed, and colored as graphic elements equal in importance to the image
- **Uppercase-dominant** -- headlines and brand names are rendered in all capitals for maximum poster impact
- **Tight, compact letterspacing** at display sizes -- letters sit close together, forming a solid typographic block
- **No decorative or serif typefaces** -- letterforms are stripped to their geometric essence, matching the reductive philosophy
- **Hand-lettered quality** -- original Plakatstil type had a custom, hand-drawn character; web implementations should favor geometric sans-serifs with strong personality
- **High stroke contrast against background** -- text must be immediately legible against the flat background color

### Recommended Web Fonts (Google Fonts)

| Font | Style | Best For |
|------|-------|----------|
| **Bebas Neue** | Bold condensed uppercase | Headlines, brand names -- closest to classic Plakatstil lettering |
| **Oswald** | Condensed geometric sans | Headlines, strong vertical emphasis |
| **Anton** | Black-weight condensed | Maximum-impact display text, poster headlines |
| **Archivo Black** | Black-weight grotesque | Bold headlines, punchy single-word displays |
| **Barlow Condensed** | Condensed grotesque, multiple weights | Headlines and supporting text |
| **Chivo** | Strong grotesque, confident character | Display text, brand names |
| **Fjalla One** | Bold condensed, Nordic character | Headlines with distinctive personality |
| **DM Sans** | Clean geometric sans | Supporting text, secondary labels |
| **Work Sans** | Geometric, screen-optimized | Body text when longer copy is needed |

### Font Pairing Suggestions

| Heading Font | Body Font | Character |
|-------------|-----------|-----------|
| **Bebas Neue** (400) | **DM Sans** (400) | Classic poster impact with clean supporting text |
| **Anton** (400) | **Work Sans** (400) | Maximum headline boldness, readable body |
| **Oswald** (700) | **Barlow Condensed** (400) | Condensed consistency, strong hierarchy through weight |
| **Archivo Black** (400) | **DM Sans** (400) | Punchy grotesque headlines, geometric body text |

### Typography CSS Example

```css
/* Import fonts */
@import url('https://fonts.googleapis.com/css2?family=Bebas+Neue&family=DM+Sans:wght@400;500;700&display=swap');

/* Headlines -- bold, condensed, poster-scale */
h1, h2, h3 {
  font-family: 'Bebas Neue', 'Anton', 'Oswald', sans-serif;
  text-transform: uppercase;
  letter-spacing: 0.05em;
  color: var(--plakat-accent);
  font-weight: 400;
  line-height: 0.95;
}

/* Display / Hero text -- maximum poster impact */
.plakat-display {
  font-family: 'Bebas Neue', 'Anton', sans-serif;
  font-size: clamp(4rem, 12vw, 10rem);
  letter-spacing: 0.08em;
  line-height: 0.9;
  text-transform: uppercase;
}

/* Brand name / product label */
.plakat-brand {
  font-family: 'Bebas Neue', 'Archivo Black', sans-serif;
  font-size: clamp(2rem, 6vw, 5rem);
  letter-spacing: 0.12em;
  text-transform: uppercase;
  text-align: center;
}

/* Body text (used sparingly) */
body {
  font-family: 'DM Sans', 'Work Sans', sans-serif;
  font-weight: 400;
  font-size: 1rem;
  line-height: 1.6;
  color: var(--plakat-text-primary);
}

/* Caption / minimal label */
.plakat-caption {
  font-family: 'DM Sans', sans-serif;
  font-weight: 500;
  font-size: 0.8rem;
  letter-spacing: 0.08em;
  text-transform: uppercase;
  color: var(--plakat-text-primary);
  opacity: 0.7;
}
```

---

## Layout Principles

### Composition and Structure

Plakatstil layout follows the logic of a poster -- a single focal point surrounded by empty space, with text anchored to the composition as a graphic block.

- **Central or near-central subject** -- the main image dominates the composition, typically occupying 40-60% of the visual field
- **Flat, monochrome backgrounds** -- the background is one unbroken color field; no panels, no gradients, no divisions
- **Text anchored to top or bottom** -- the brand name sits at the top or bottom of the composition, never floating in the middle or crowding the subject
- **Asymmetry within balance** -- the subject may be slightly off-center for visual interest, but the overall composition feels stable and deliberate
- **Extreme scale contrast** -- the subject is large, the text is large; there is nothing at medium scale to create clutter
- **No borders or frames** -- the color field extends to the edges; no containing lines, no decorative borders
- **Vertical orientation** -- the classic poster format is portrait/vertical, with content stacked: text block, subject, text block
- **No grid complexity** -- unlike Swiss Style, Plakatstil uses simple, intuitive placement rather than mathematical grids

### Section Organization

- **Hero / Poster area**: Full-viewport section with a single large graphic element centered on a flat color background, with the brand/title in bold condensed type above or below
- **Content sections**: Each section should feel like its own poster -- one idea, one visual, one color scheme per section
- **Transitions**: Hard color-block transitions between sections (full-width background color changes), never gradual fades or gradients
- **Feature areas**: Instead of multi-column grids, present features as a sequence of full-width poster-like panels, each with a single icon/illustration and short text
- **Call-to-action**: Bold, flat-colored button or text block in a contrasting accent color, isolated with generous surrounding space
- **Footer**: Minimal, flat-colored strip with small text; functions as the "bottom border" of the poster

### Responsive Approach

- The poster-like simplicity of Plakatstil translates naturally to mobile -- single-column layouts with large type and centered subjects
- Scale typography aggressively using `clamp()` -- headlines should be enormous on desktop, still bold on mobile
- Maintain the flat color block structure at all breakpoints
- Ensure the subject image/graphic scales proportionally and remains the dominant visual element
- Never add complexity at larger breakpoints -- Plakatstil is inherently single-column and stacked

---

## CSS / Design Techniques

### Full-Viewport Poster Section

```css
.plakat-poster {
  min-height: 100vh;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  background: var(--plakat-bg-dark);
  color: var(--plakat-text-inverse);
  text-align: center;
  padding: 4rem 2rem;
  position: relative;
  overflow: hidden;
}

.plakat-poster__title {
  font-family: 'Bebas Neue', sans-serif;
  font-size: clamp(4rem, 12vw, 10rem);
  text-transform: uppercase;
  letter-spacing: 0.1em;
  line-height: 0.9;
  color: var(--plakat-cream);
  position: relative;
  z-index: 2;
}

.plakat-poster__subject {
  max-width: 50vw;
  max-height: 50vh;
  object-fit: contain;
  margin: 2rem 0;
  position: relative;
  z-index: 2;
}

.plakat-poster__brand {
  font-family: 'Bebas Neue', sans-serif;
  font-size: clamp(1.5rem, 4vw, 3rem);
  text-transform: uppercase;
  letter-spacing: 0.2em;
  color: var(--plakat-accent);
  position: relative;
  z-index: 2;
}
```

### Color Block Sections

```css
/* Each section is a distinct color poster panel */
.plakat-section {
  padding: 6rem 2rem;
  text-align: center;
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 2rem;
}

.plakat-section--dark {
  background: var(--plakat-rich-black);
  color: var(--plakat-cream);
}

.plakat-section--red {
  background: var(--plakat-red);
  color: var(--plakat-cream);
}

.plakat-section--blue {
  background: var(--plakat-blue);
  color: var(--plakat-cream);
}

.plakat-section--cream {
  background: var(--plakat-cream);
  color: var(--plakat-black);
}

.plakat-section--olive {
  background: var(--plakat-olive);
  color: var(--plakat-cream);
}

/* Headings adapt to section color */
.plakat-section--dark h2,
.plakat-section--red h2,
.plakat-section--blue h2,
.plakat-section--olive h2 {
  color: var(--plakat-cream);
}

.plakat-section--cream h2 {
  color: var(--plakat-red);
}
```

### Simplified Object / Icon Style

```css
/* Icons and illustrations should be flat, single-color silhouettes */
.plakat-icon {
  width: 120px;
  height: 120px;
  display: flex;
  align-items: center;
  justify-content: center;
}

.plakat-icon svg {
  fill: currentColor;
  width: 100%;
  height: 100%;
}

/* Icon on a contrasting flat background */
.plakat-icon-block {
  width: 160px;
  height: 160px;
  background: var(--plakat-accent);
  display: flex;
  align-items: center;
  justify-content: center;
  /* No border-radius -- sharp corners only */
}

.plakat-icon-block svg {
  fill: var(--plakat-cream);
  width: 60%;
  height: 60%;
}
```

### Flat Button (Poster Style)

```css
.plakat-button {
  display: inline-block;
  background: var(--plakat-accent);
  color: var(--plakat-cream);
  border: none;
  border-radius: 0; /* Sharp corners -- poster aesthetic */
  padding: 16px 48px;
  font-family: 'Bebas Neue', sans-serif;
  font-size: 1.25rem;
  letter-spacing: 0.15em;
  text-transform: uppercase;
  cursor: pointer;
  text-decoration: none;
  transition: background 0.15s ease;
}

.plakat-button:hover {
  background: var(--plakat-red-dark);
}

/* Inverted button for dark backgrounds */
.plakat-button--inverse {
  background: var(--plakat-cream);
  color: var(--plakat-black);
}

.plakat-button--inverse:hover {
  background: var(--plakat-warm-white);
}

/* Outline button */
.plakat-button--outline {
  background: transparent;
  color: var(--plakat-accent);
  border: 3px solid var(--plakat-accent);
}

.plakat-button--outline:hover {
  background: var(--plakat-accent);
  color: var(--plakat-cream);
}
```

### Feature Panel (Poster Card)

```css
/* Each feature is its own mini-poster */
.plakat-feature {
  background: var(--plakat-bg-dark);
  color: var(--plakat-cream);
  padding: 4rem 2rem;
  text-align: center;
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 1.5rem;
}

.plakat-feature__icon {
  width: 96px;
  height: 96px;
}

.plakat-feature__icon svg {
  fill: var(--plakat-accent);
  width: 100%;
  height: 100%;
}

.plakat-feature__title {
  font-family: 'Bebas Neue', sans-serif;
  font-size: 1.75rem;
  text-transform: uppercase;
  letter-spacing: 0.1em;
  color: var(--plakat-cream);
}

.plakat-feature__text {
  font-family: 'DM Sans', sans-serif;
  font-size: 0.95rem;
  line-height: 1.6;
  max-width: 40ch;
  opacity: 0.8;
}

/* Alternating feature colors */
.plakat-feature:nth-child(even) {
  background: var(--plakat-accent);
}

.plakat-feature:nth-child(even) .plakat-feature__icon svg {
  fill: var(--plakat-cream);
}
```

### Hard Color-Block Divider

```css
/* No gradients, no rules -- just a hard color stripe */
.plakat-stripe {
  height: 8px;
  background: var(--plakat-accent);
  width: 100%;
}

.plakat-stripe--thin {
  height: 4px;
}

.plakat-stripe--thick {
  height: 16px;
}
```

### Simplified Silhouette Illustration (CSS)

```css
/* A flat, geometric shape representing a product -- pure CSS */
.plakat-silhouette {
  width: 200px;
  height: 300px;
  background: var(--plakat-accent);
  clip-path: polygon(
    20% 0%, 80% 0%, 90% 10%, 90% 90%, 80% 100%, 20% 100%, 10% 90%, 10% 10%
  );
  /* Simplified bottle-like shape as example */
}

/* Circle silhouette for rounded products */
.plakat-silhouette--round {
  width: 200px;
  height: 200px;
  background: var(--plakat-accent);
  border-radius: 50%;
}
```

### Navigation (Minimal)

```css
.plakat-nav {
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 24px 48px;
  background: var(--plakat-bg-dark);
}

.plakat-nav__brand {
  font-family: 'Bebas Neue', sans-serif;
  font-size: 1.5rem;
  letter-spacing: 0.15em;
  text-transform: uppercase;
  color: var(--plakat-cream);
  text-decoration: none;
}

.plakat-nav__links {
  display: flex;
  gap: 32px;
  list-style: none;
  margin: 0;
  padding: 0;
}

.plakat-nav__links a {
  font-family: 'DM Sans', sans-serif;
  font-weight: 500;
  font-size: 0.85rem;
  letter-spacing: 0.08em;
  text-transform: uppercase;
  color: var(--plakat-cream);
  text-decoration: none;
  opacity: 0.7;
  transition: opacity 0.15s ease;
}

.plakat-nav__links a:hover {
  opacity: 1;
}

.plakat-nav__links a.active {
  opacity: 1;
  color: var(--plakat-accent);
}
```

---

## Design Do's and Don'ts

### Do

- Use flat, solid color fills for every surface -- no gradients, no shading, no textures
- Limit the palette to 2-4 bold, high-contrast colors per page or section
- Make the primary subject/image dramatically large and isolated
- Use condensed, bold, uppercase sans-serif type for all headlines
- Keep text to an absolute minimum -- ideally just a name or single phrase per section
- Use generous negative space to isolate and elevate the subject
- Create hard, clean transitions between color blocks
- Design each section as if it were a standalone poster
- Use sharp corners on all elements -- no border-radius
- Render icons and illustrations as flat silhouettes in a single color

### Don't

- Use gradients, shadows, bevels, or any 3D effects
- Add decorative borders, frames, ornamental lines, or flourishes
- Include busy backgrounds, patterns, or textures
- Use serif, script, or decorative typefaces
- Write long paragraphs of body copy -- Plakatstil communicates through image and brand name, not prose
- Use more than 4 colors in a single composition
- Add subtle, muted, or pastel colors -- every color must be poster-bold
- Use rounded corners or soft shapes on UI elements
- Layer multiple subjects or competing visual elements in one section
- Apply opacity or transparency effects between color areas

---

## Materials and Textures (Visual Metaphors for Web)

Physical Plakatstil materials and their web equivalents:

| Physical Material | Web Equivalent |
|-------------------|----------------|
| Lithographic ink on paper | Flat, solid CSS color fills with no texture |
| Aged poster stock | Warm cream/ivory background tones (`#f5f0e1`) |
| Block-printed letterforms | Bold condensed sans-serif web fonts at large scale |
| Flat gouache paint | Uniform CSS `background-color` with zero variation |
| Cut paper collage | Hard-edged `clip-path` shapes and CSS shape compositions |
| Reduction woodcut | SVG silhouettes with single flat `fill` color |

---

## Related Aesthetics

| Aesthetic | Relationship to Plakatstil |
|-----------|---------------------------|
| **Art Nouveau** | Direct predecessor that Plakatstil reacted against; Plakatstil stripped away Art Nouveau's organic ornamentation in favor of radical simplicity |
| **Bauhaus** | Direct descendant; inherited Plakatstil's reductive approach to form and function, extending it into architecture, product design, and systematic visual language |
| **International Typographic Style** | Evolutionary successor; took Plakatstil's flat color and bold sans-serif typography and formalized it into grid-based, objective communication design |
| **Constructivism** | Contemporary parallel; shared commitment to geometric abstraction and design as a social/commercial communication tool |
| **Flat Design** | Modern digital descendant; the 2010s digital interface aesthetic directly echoes Plakatstil's flat color, bold shapes, and elimination of decorative detail |
| **Minimalism** | Broader parent philosophy; Plakatstil applied minimalist reduction specifically to commercial poster art over a century before digital minimalism |
| **Art Deco** | Shared era and some geometric sensibility, but Art Deco embraced ornamentation and luxury that Plakatstil deliberately rejected |
| **Heroic Realism** | Some Plakatstil artists (notably Hohlwein) moved toward propaganda poster styles that fed into Heroic Realism's bold, simplified figurative imagery |
| **Corporate Memphis** | Distant descendant; shares flat color fills and geometric figure simplification, though with a playful, illustrative character foreign to Plakatstil's serious directness |

---

## Quick-Start: Minimal Plakatstil Page Template

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Plakatstil Page</title>
  <link href="https://fonts.googleapis.com/css2?family=Bebas+Neue&family=DM+Sans:wght@400;500;700&display=swap" rel="stylesheet">
  <style>
    :root {
      --plakat-black: #1a1a1a;
      --plakat-rich-black: #0d0d0d;
      --plakat-cream: #f5f0e1;
      --plakat-warm-white: #fffdd0;
      --plakat-red: #c8102e;
      --plakat-red-dark: #8b1a1a;
      --plakat-blue: #003e7e;
      --plakat-olive: #5b6236;
      --plakat-ochre: #cc7722;
    }

    * { margin: 0; padding: 0; box-sizing: border-box; }

    body {
      background: var(--plakat-rich-black);
      color: var(--plakat-cream);
      font-family: 'DM Sans', sans-serif;
      font-weight: 400;
      line-height: 1.6;
    }

    h1, h2, h3 {
      font-family: 'Bebas Neue', sans-serif;
      text-transform: uppercase;
      letter-spacing: 0.08em;
      line-height: 0.95;
    }

    /* Navigation */
    nav {
      display: flex;
      align-items: center;
      justify-content: space-between;
      padding: 24px 48px;
      background: var(--plakat-rich-black);
    }

    nav a.brand {
      font-family: 'Bebas Neue', sans-serif;
      font-size: 1.5rem;
      letter-spacing: 0.15em;
      text-transform: uppercase;
      color: var(--plakat-cream);
      text-decoration: none;
    }

    nav ul {
      display: flex;
      gap: 32px;
      list-style: none;
    }

    nav ul a {
      font-family: 'DM Sans', sans-serif;
      font-weight: 500;
      font-size: 0.85rem;
      letter-spacing: 0.08em;
      text-transform: uppercase;
      color: var(--plakat-cream);
      text-decoration: none;
      opacity: 0.7;
      transition: opacity 0.15s ease;
    }

    nav ul a:hover { opacity: 1; }

    /* Hero -- full-viewport poster */
    .hero {
      min-height: 100vh;
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      background: var(--plakat-rich-black);
      text-align: center;
      padding: 4rem 2rem;
      gap: 2rem;
    }

    .hero h1 {
      font-size: clamp(4rem, 12vw, 10rem);
      color: var(--plakat-cream);
      letter-spacing: 0.1em;
    }

    .hero .subject {
      width: clamp(120px, 30vw, 300px);
      height: clamp(180px, 45vw, 450px);
      background: var(--plakat-red);
      clip-path: polygon(
        30% 0%, 70% 0%, 75% 5%, 75% 85%, 100% 85%, 100% 100%, 0% 100%, 0% 85%, 25% 85%, 25% 5%
      );
    }

    .hero .brand-name {
      font-family: 'Bebas Neue', sans-serif;
      font-size: clamp(1.5rem, 4vw, 3rem);
      letter-spacing: 0.25em;
      text-transform: uppercase;
      color: var(--plakat-ochre);
    }

    /* Color block section */
    .poster-section {
      padding: 6rem 2rem;
      text-align: center;
      display: flex;
      flex-direction: column;
      align-items: center;
      gap: 2rem;
    }

    .poster-section--red {
      background: var(--plakat-red);
      color: var(--plakat-cream);
    }

    .poster-section--cream {
      background: var(--plakat-cream);
      color: var(--plakat-black);
    }

    .poster-section--blue {
      background: var(--plakat-blue);
      color: var(--plakat-cream);
    }

    .poster-section h2 {
      font-size: clamp(2rem, 6vw, 5rem);
    }

    .poster-section--cream h2 {
      color: var(--plakat-red);
    }

    .poster-section p {
      font-size: 1.1rem;
      max-width: 50ch;
      opacity: 0.85;
    }

    /* Feature panels */
    .features {
      display: flex;
      flex-direction: column;
    }

    .feature {
      padding: 5rem 2rem;
      text-align: center;
      display: flex;
      flex-direction: column;
      align-items: center;
      gap: 1.5rem;
    }

    .feature:nth-child(1) { background: var(--plakat-rich-black); color: var(--plakat-cream); }
    .feature:nth-child(2) { background: var(--plakat-red); color: var(--plakat-cream); }
    .feature:nth-child(3) { background: var(--plakat-blue); color: var(--plakat-cream); }

    .feature-icon {
      width: 80px;
      height: 80px;
    }

    .feature h3 {
      font-size: 1.75rem;
      letter-spacing: 0.12em;
    }

    .feature p {
      font-size: 0.95rem;
      max-width: 40ch;
      opacity: 0.8;
    }

    /* CTA */
    .cta {
      background: var(--plakat-cream);
      color: var(--plakat-black);
      text-align: center;
      padding: 6rem 2rem;
    }

    .cta h2 {
      font-size: clamp(2.5rem, 7vw, 6rem);
      color: var(--plakat-red);
      margin-bottom: 2rem;
    }

    .btn {
      display: inline-block;
      background: var(--plakat-red);
      color: var(--plakat-cream);
      border: none;
      border-radius: 0;
      padding: 16px 48px;
      font-family: 'Bebas Neue', sans-serif;
      font-size: 1.25rem;
      letter-spacing: 0.15em;
      text-transform: uppercase;
      text-decoration: none;
      cursor: pointer;
      transition: background 0.15s ease;
    }

    .btn:hover { background: var(--plakat-red-dark); }

    /* Stripe divider */
    .stripe {
      height: 8px;
      background: var(--plakat-ochre);
      width: 100%;
    }

    /* Footer */
    footer {
      background: var(--plakat-rich-black);
      color: var(--plakat-cream);
      text-align: center;
      padding: 32px;
      font-size: 0.8rem;
      letter-spacing: 0.06em;
      text-transform: uppercase;
      opacity: 0.5;
    }

    @media (max-width: 768px) {
      nav { padding: 16px 20px; }
      nav ul { gap: 20px; }
      .hero { padding: 3rem 1.5rem; }
      .poster-section { padding: 4rem 1.5rem; }
      .feature { padding: 3rem 1.5rem; }
      .cta { padding: 4rem 1.5rem; }
    }
  </style>
</head>
<body>
  <nav>
    <a href="#" class="brand">Plakat</a>
    <ul>
      <li><a href="#">Work</a></li>
      <li><a href="#">About</a></li>
      <li><a href="#">Contact</a></li>
    </ul>
  </nav>

  <section class="hero">
    <h1>Sachplakat</h1>
    <div class="subject"></div>
    <div class="brand-name">Object Poster</div>
  </section>

  <div class="stripe"></div>

  <section class="poster-section poster-section--cream">
    <h2>Focus and Clarity</h2>
    <p>One subject. Flat color. Bold type. Nothing more. The power of reduction creates immediate, unforgettable impact.</p>
  </section>

  <div class="features">
    <div class="feature">
      <svg class="feature-icon" viewBox="0 0 80 80" fill="none"><rect x="15" y="10" width="50" height="60" fill="#c8102e"/></svg>
      <h3>Radical Simplicity</h3>
      <p>Every non-essential element is eliminated. What remains carries maximum visual weight.</p>
    </div>
    <div class="feature">
      <svg class="feature-icon" viewBox="0 0 80 80" fill="none"><circle cx="40" cy="40" r="30" fill="#f5f0e1"/></svg>
      <h3>Bold Color</h3>
      <p>Two to four saturated hues create poster-grade impact that commands attention instantly.</p>
    </div>
    <div class="feature">
      <svg class="feature-icon" viewBox="0 0 80 80" fill="none"><text x="10" y="55" font-family="sans-serif" font-size="40" font-weight="bold" fill="#f5f0e1">Aa</text></svg>
      <h3>Type as Image</h3>
      <p>Bold sans-serif letterforms are compositional elements equal in power to the illustration itself.</p>
    </div>
  </div>

  <div class="stripe"></div>

  <section class="cta">
    <h2>Make It Direct</h2>
    <a href="#" class="btn">See the Work</a>
  </section>

  <footer>
    <p>Designed in the Plakatstil tradition. Flat color. Sharp focus. Nothing wasted.</p>
  </footer>
</body>
</html>
```
