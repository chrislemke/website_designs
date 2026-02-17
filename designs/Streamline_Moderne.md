# Streamline Moderne Design Reference

Streamline Moderne (also known as Art Moderne) is an evolution of Art Deco architecture and design that emerged in the 1930s and remained popular through the 1940s. It represents **speed, efficiency, modernity, technology, motion**, and **functionality**. Born from Depression-era austerity, it replaced Art Deco's lavish ornamentation with a clean, machine-inspired aesthetic. Forms are drawn from transportation design -- ocean liners, airplanes, trains, and automobiles -- applying aerodynamic streamlining to everything from buildings to toasters. The result is smooth, horizontal, forward-moving, and unadorned: progress expressed through the curve of a line rather than the richness of a surface.

---

## Visual Characteristics

### Core Motifs and Patterns

- **Speed lines** -- long horizontal grooves and striping that convey motion and velocity; the defining Streamline Moderne motif
- **Rounded / teardrop forms** -- aerodynamic profiles inspired by wind-tunnel-tested transportation design
- **Bullet and cylinder shapes** -- elongated tubular forms with hemispherical or tapered ends
- **Curved corners** -- all right angles are softened into smooth radii
- **Porthole windows** -- circular nautical-inspired openings, a signature architectural element
- **Horizontal banding** -- three or more parallel lines wrapping around surfaces to accentuate length and movement
- **Smooth, unadorned surfaces** -- clean planes without applied ornament; form itself is the decoration
- **Nautical references** -- ocean liner styling including railings, deck-like platforms, and rounded bridge forms

### Design Principles

- **Horizontal emphasis** over verticality -- compositions stretch wide and low, suggesting forward motion
- **Aerodynamic, curvilinear construction** -- every edge is rounded, every corner radiused
- **Functional minimalism** -- ornament is stripped away; beauty comes from form and proportion
- **Machine-inspired precision** -- smooth, manufactured surfaces suggesting industrial perfection
- **Directional movement** created through horizontal lines and tapered forms
- **Symmetrical but flowing** -- bilateral symmetry combined with sweeping horizontal curves
- **Monolithic unity** -- elements merge into continuous surfaces rather than being assembled from separate parts

---

## Color Palette

### Primary Scheme

| Role | Colors |
|------|--------|
| **Base** | White, cream, pale earth tones |
| **Primary accents** | Chrome silver, steel gray |
| **Secondary accents** | Teal, ocean blue, muted red |
| **Contrast** | Black or charcoal for trim and typography |

### Suggested Hex Values

| Color | Hex (suggested) | Usage |
|-------|-----------------|-------|
| Ivory White | `#F5F2EB`, `#FAFAF5` | Primary backgrounds, large surfaces |
| Warm Cream | `#EDE8D8`, `#E8E2D0` | Secondary backgrounds, panels |
| Chrome Silver | `#C8CDD0`, `#D6DADC` | Metallic accents, borders, highlights |
| Steel Gray | `#6B7178`, `#8A9098` | Structural elements, secondary text |
| Ocean Teal | `#3D7B8A`, `#2D6B7A` | Accent color, feature highlights |
| Muted Red | `#B84C4C`, `#A03C3C` | Accent details, call-to-action elements |
| Deco Black | `#1E2024`, `#2A2D32` | Dark backgrounds, typography, trim |
| Pale Blue | `#D4DEE4`, `#C0CED8` | Subtle backgrounds, tinted surfaces |
| Brass / Gold | `#B8A060`, `#C4AC6C` | Occasional warm metallic accent |

### Suggested CSS Custom Properties

```css
:root {
  /* Base */
  --moderne-white: #fafaf5;
  --moderne-ivory: #f5f2eb;
  --moderne-cream: #ede8d8;
  --moderne-black: #1e2024;
  --moderne-charcoal: #2a2d32;

  /* Metallics */
  --moderne-chrome: #c8cdd0;
  --moderne-chrome-light: #d6dadc;
  --moderne-steel: #6b7178;
  --moderne-steel-light: #8a9098;
  --moderne-brass: #b8a060;

  /* Accents */
  --moderne-teal: #3d7b8a;
  --moderne-teal-light: #5a9aaa;
  --moderne-red: #b84c4c;
  --moderne-pale-blue: #d4dee4;

  /* Functional */
  --moderne-bg-primary: var(--moderne-ivory);
  --moderne-bg-secondary: var(--moderne-cream);
  --moderne-text-primary: var(--moderne-charcoal);
  --moderne-text-secondary: var(--moderne-steel);
  --moderne-accent: var(--moderne-teal);
  --moderne-border: var(--moderne-chrome);
}
```

### Approaches

- **Light, airy palette dominated by white and cream** -- clean and open, like a freshly painted 1930s building
- **Chrome and steel as structural accents** -- metallic silver tones for borders, dividers, and highlights
- **Selective bold accents** -- a single teal or muted red element against a pale background for contrast
- **Dark variant** -- charcoal/black base with chrome borders and pale text, evoking a polished appliance or car dashboard
- **Minimal color count** -- restrict to 2-3 colors plus chrome for clean, uncluttered impact

---

## Typography

### Typeface Characteristics

Streamline Moderne typography features:

- **Geometric, sans-serif typefaces** with clean, even strokes
- **Rounded letterforms** -- soft terminals and curved geometry, not sharp or angular
- **Extended / wide proportions** -- letters stretched horizontally to echo the aesthetic's horizontal emphasis
- **Uniform stroke weight** -- monolinear construction for a clean, engineered appearance
- **Uppercase-forward** usage for headlines and labels, echoing architectural signage
- **Generous letter-spacing** -- airy, open tracking that reinforces the horizontal line
- **No serifs, no ornamental details** -- pure geometric simplicity

### Recommended Web Fonts (Google Fonts / Free)

| Font | Style | Usage |
|------|-------|-------|
| **Raleway** | Geometric, thin-to-bold range | Headlines, subheadings |
| **Jost** | Geometric sans inspired by 1920s-30s | All-purpose, clean headlines |
| **Tenor Sans** | Clean geometric sans | Body text, UI elements |
| **Josefin Sans** | Geometric, vintage 1930s feel | Headlines, display text |
| **Nunito** | Rounded geometric sans | Body text, softer applications |
| **Quicksand** | Rounded geometric | Casual headings, labels |
| **Work Sans** | Clean geometric with slight warmth | Body copy |
| **DM Sans** | Geometric sans with clean proportions | Body text, subheadings |
| **Fahkwang** | Extended geometric with art deco echo | Display headlines |

### Typography CSS Example

```css
/* Headlines */
h1, h2, h3 {
  font-family: 'Raleway', 'Jost', sans-serif;
  text-transform: uppercase;
  letter-spacing: 0.18em;
  color: var(--moderne-charcoal);
  font-weight: 300;
  line-height: 1.2;
}

/* Display / Hero text */
.moderne-display {
  font-family: 'Josefin Sans', 'Fahkwang', sans-serif;
  font-size: clamp(2.5rem, 7vw, 7rem);
  letter-spacing: 0.25em;
  line-height: 1.05;
  font-weight: 200;
  text-transform: uppercase;
}

/* Body text */
body {
  font-family: 'Work Sans', 'Tenor Sans', 'DM Sans', sans-serif;
  font-weight: 300;
  letter-spacing: 0.02em;
  line-height: 1.75;
  color: var(--moderne-charcoal);
}
```

---

## Layout Principles

### Grid and Structure

- **Horizontal, wide-format layouts** -- content stretches across the viewport, emphasizing breadth over height
- **Symmetrical composition** -- center-aligned with balanced left-right weight
- **Rounded containers** -- all panels, cards, and content boxes use generous border-radius
- **Layered horizontal bands** -- full-width sections stacked vertically, each a distinct horizontal stripe
- **Low, wide proportions** -- hero sections and cards are wider than they are tall
- **Generous whitespace** -- clean, open spacing that lets smooth surfaces breathe

### Section Organization

- Use **horizontal line dividers** between sections (triple-line speed rules, chrome-colored separators)
- Apply **wide padding** -- generous horizontal margins reflecting the expansive, aerodynamic feel
- Create **hierarchy through weight and spacing** -- thin, widely-spaced large headings vs. compact body text
- Employ **rounded panel containers** -- cards and content blocks with substantial border-radius
- **Full-width bands** -- alternating light and slightly darker horizontal sections spanning the viewport

---

## CSS/Design Techniques

### Chrome / Metallic Gradient Effects

```css
/* Chrome metallic gradient for headers or accents */
.moderne-chrome-text {
  background: linear-gradient(
    135deg,
    #a8b0b8, #d6dadc, #8a9098, #c8cdd0, #b0b8c0
  );
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  background-clip: text;
}

/* Chrome metallic border */
.moderne-chrome-border {
  border: 2px solid transparent;
  border-image: linear-gradient(
    90deg,
    #8a9098, #d6dadc, #c8cdd0, #d6dadc, #8a9098
  ) 1;
}

/* Brushed steel surface */
.moderne-steel-surface {
  background: linear-gradient(
    180deg,
    #c8cdd0 0%,
    #d6dadc 25%,
    #b8bfc4 50%,
    #d0d4d8 75%,
    #c0c6cc 100%
  );
}
```

### Speed Line Dividers

```css
/* Triple horizontal speed line divider */
.moderne-speed-lines {
  display: flex;
  flex-direction: column;
  gap: 4px;
  width: 70%;
  margin: 2.5rem auto;
  align-items: center;
}

.moderne-speed-lines::before,
.moderne-speed-lines::after {
  content: '';
  height: 1px;
  width: 85%;
  background: linear-gradient(
    90deg,
    transparent,
    var(--moderne-chrome) 15%,
    var(--moderne-chrome) 85%,
    transparent
  );
}

.moderne-speed-lines::after {
  width: 70%;
}

/* Center speed line (thicker) */
.moderne-divider {
  height: 2px;
  width: 100%;
  background: linear-gradient(
    90deg,
    transparent,
    var(--moderne-steel) 10%,
    var(--moderne-steel) 90%,
    transparent
  );
  border: none;
  margin: 2rem auto;
}
```

### Rounded Moderne Panel / Card

```css
.moderne-card {
  background: var(--moderne-white);
  border: 1px solid var(--moderne-chrome);
  border-radius: 20px;
  padding: 2.5rem;
  position: relative;
  overflow: hidden;
  box-shadow: 0 2px 12px rgba(30, 32, 36, 0.06);
  transition: box-shadow 0.3s ease;
}

.moderne-card:hover {
  box-shadow: 0 4px 24px rgba(30, 32, 36, 0.1);
}

/* Horizontal speed line accent at top of card */
.moderne-card::before {
  content: '';
  position: absolute;
  top: 0;
  left: 10%;
  right: 10%;
  height: 3px;
  background: linear-gradient(
    90deg,
    transparent,
    var(--moderne-teal) 20%,
    var(--moderne-teal) 80%,
    transparent
  );
  border-radius: 0 0 2px 2px;
}
```

### Porthole Window Element

```css
/* Circular porthole-style frame for images or decorative use */
.moderne-porthole {
  width: 180px;
  height: 180px;
  border-radius: 50%;
  border: 4px solid var(--moderne-chrome);
  box-shadow:
    inset 0 0 0 3px var(--moderne-white),
    inset 0 0 0 5px var(--moderne-steel-light),
    0 4px 16px rgba(30, 32, 36, 0.1);
  overflow: hidden;
  display: flex;
  align-items: center;
  justify-content: center;
}

/* Cross-bar detail inside porthole */
.moderne-porthole::after {
  content: '';
  position: absolute;
  width: 100%;
  height: 2px;
  background: var(--moderne-chrome);
}
```

### Glass Block Effect

```css
/* Grid simulating glass block walls */
.moderne-glass-block {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(80px, 1fr));
  gap: 3px;
  background: var(--moderne-chrome);
  border-radius: 12px;
  overflow: hidden;
  padding: 3px;
}

.moderne-glass-block > * {
  background: rgba(212, 222, 228, 0.5);
  backdrop-filter: blur(4px);
  padding: 1rem;
  border-radius: 4px;
  aspect-ratio: 1;
}
```

### Horizontal Banding / Speed Stripe Background

```css
/* Subtle horizontal stripe texture */
.moderne-stripe-bg {
  background-color: var(--moderne-ivory);
  background-image: repeating-linear-gradient(
    0deg,
    transparent,
    transparent 18px,
    rgba(200, 205, 208, 0.2) 18px,
    rgba(200, 205, 208, 0.2) 19px
  );
}

/* Bold horizontal bands */
.moderne-bands {
  background: linear-gradient(
    180deg,
    var(--moderne-ivory) 0%,
    var(--moderne-ivory) 30%,
    var(--moderne-cream) 30%,
    var(--moderne-cream) 34%,
    var(--moderne-ivory) 34%,
    var(--moderne-ivory) 66%,
    var(--moderne-cream) 66%,
    var(--moderne-cream) 70%,
    var(--moderne-ivory) 70%
  );
}
```

### Streamlined Shadow / Depth

```css
/* Soft, horizontal-biased shadow suggesting aerodynamic form */
.moderne-shadow {
  box-shadow:
    0 2px 6px rgba(30, 32, 36, 0.04),
    0 8px 24px rgba(30, 32, 36, 0.06);
}

/* Polished chrome inset effect */
.moderne-inset {
  box-shadow:
    inset 0 1px 3px rgba(30, 32, 36, 0.1),
    inset 0 -1px 2px rgba(255, 255, 255, 0.6);
}
```

### Curved Corner Container

```css
/* Container with exaggerated Streamline Moderne rounded corners */
.moderne-container {
  background: var(--moderne-white);
  border-radius: 30px;
  padding: 3rem 4rem;
  border: 1px solid var(--moderne-chrome-light);
  position: relative;
}

/* Accent stripe wrapping around container */
.moderne-container::before {
  content: '';
  position: absolute;
  top: 50%;
  left: 0;
  right: 0;
  height: 2px;
  background: var(--moderne-chrome);
  transform: translateY(-50%);
  pointer-events: none;
}
```

### Background Texture Pattern

```css
/* Subtle brushed steel texture */
.moderne-brushed-bg {
  background-color: var(--moderne-ivory);
  background-image:
    repeating-linear-gradient(
      90deg,
      transparent,
      transparent 2px,
      rgba(200, 205, 208, 0.03) 2px,
      rgba(200, 205, 208, 0.03) 3px
    );
}

/* Soft gradient suggesting a curved surface */
.moderne-curved-surface {
  background: radial-gradient(
    ellipse 120% 80% at 50% 0%,
    var(--moderne-white) 0%,
    var(--moderne-cream) 100%
  );
}
```

---

## Materials and Textures (Visual Metaphors for Web)

Physical Streamline Moderne materials and their web equivalents:

| Physical Material | Web Equivalent |
|-------------------|----------------|
| Chrome plating | Linear metallic silver gradients, reflective borders |
| Stainless steel | Steel-gray solid fills with subtle vertical grain (repeating-linear-gradient) |
| Glass block | Translucent grid panels with frosted blur (`backdrop-filter: blur`) |
| Polished lacquer | Deep solid backgrounds with subtle sheen gradient overlay |
| White enamel | Clean white/ivory backgrounds with minimal shadow for depth |
| Bakelite plastic | Smooth, solid muted-color fills (cream, teal, muted red) |
| Varnished brass | Warm gold-toned gradient accents, sparingly applied |
| Terrazzo flooring | Speckled subtle noise texture overlay on light surfaces |
| Curved glass | Transparent overlays with radial gradient suggesting curvature |
| Polished concrete | Light gray backgrounds with very subtle texture noise |

---

## Related Aesthetics

| Aesthetic | Relationship to Streamline Moderne |
|-----------|-------------------------------------|
| **Art Deco** | Direct predecessor; Streamline Moderne replaces Deco's angular ornament with aerodynamic curves |
| **Mid-Century Modern** | Direct successor; carries forward clean lines and functional design into the 1950s-60s |
| **Googie** | Exuberant descendant; takes Moderne's curves to flamboyant, space-age extremes |
| **Dieselpunk** | Retro-futuristic fiction aesthetic rooted in the 1930s-40s industrial era |
| **Decopunk** | Speculative aesthetic blending Art Deco and Streamline Moderne visual language |
| **Raygun Gothic** | Retro-futurism inspired by streamlined 1930s-50s visions of the future |
| **Atompunk** | Shares the optimistic machine-age spirit, but set in the atomic 1950s |
| **Factory Pomo** | Industrial design descendant with postmodern reinterpretation |

---

## Quick-Start: Minimal Streamline Moderne Page Template

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Streamline Moderne Page</title>
  <link href="https://fonts.googleapis.com/css2?family=Raleway:wght@200;300;400;600&family=Josefin+Sans:wght@200;300;400&family=Work+Sans:wght@300;400&display=swap" rel="stylesheet">
  <style>
    :root {
      --moderne-white: #fafaf5;
      --moderne-ivory: #f5f2eb;
      --moderne-cream: #ede8d8;
      --moderne-charcoal: #2a2d32;
      --moderne-chrome: #c8cdd0;
      --moderne-steel: #6b7178;
      --moderne-teal: #3d7b8a;
    }

    * { margin: 0; padding: 0; box-sizing: border-box; }

    body {
      background: var(--moderne-ivory);
      color: var(--moderne-charcoal);
      font-family: 'Work Sans', sans-serif;
      font-weight: 300;
      letter-spacing: 0.02em;
      line-height: 1.75;
    }

    h1, h2, h3 {
      font-family: 'Raleway', sans-serif;
      text-transform: uppercase;
      letter-spacing: 0.18em;
      color: var(--moderne-charcoal);
      font-weight: 300;
    }

    .hero {
      text-align: center;
      padding: 6rem 2rem;
      background: radial-gradient(
        ellipse 120% 80% at 50% 0%,
        var(--moderne-white) 0%,
        var(--moderne-ivory) 100%
      );
    }

    .hero h1 {
      font-family: 'Josefin Sans', sans-serif;
      font-size: clamp(2.5rem, 7vw, 6rem);
      letter-spacing: 0.25em;
      font-weight: 200;
    }

    /* Triple speed line divider */
    .moderne-divider {
      display: flex;
      flex-direction: column;
      align-items: center;
      gap: 4px;
      width: 60%;
      margin: 2rem auto;
    }

    .moderne-divider span {
      display: block;
      height: 1px;
      background: linear-gradient(
        90deg, transparent,
        var(--moderne-chrome) 15%,
        var(--moderne-chrome) 85%,
        transparent
      );
    }

    .moderne-divider span:nth-child(1) { width: 100%; }
    .moderne-divider span:nth-child(2) { width: 85%; height: 2px; background: linear-gradient(90deg, transparent, var(--moderne-steel) 15%, var(--moderne-steel) 85%, transparent); }
    .moderne-divider span:nth-child(3) { width: 70%; }

    section {
      max-width: 900px;
      margin: 0 auto;
      padding: 4rem 2rem;
      text-align: center;
    }

    section h2 {
      margin-bottom: 1.5rem;
    }

    .moderne-card {
      background: var(--moderne-white);
      border: 1px solid var(--moderne-chrome);
      border-radius: 20px;
      padding: 2.5rem;
      box-shadow: 0 2px 12px rgba(30, 32, 36, 0.06);
    }
  </style>
</head>
<body>
  <div class="hero">
    <h1>Title Here</h1>
    <div class="moderne-divider">
      <span></span><span></span><span></span>
    </div>
    <p>Subtitle in clean, geometric Work Sans</p>
  </div>
  <section>
    <h2>Section Heading</h2>
    <div class="moderne-card">
      <p>Content with Streamline Moderne styling applied. Clean surfaces, rounded corners, and horizontal emphasis create a sense of aerodynamic forward motion.</p>
    </div>
  </section>
</body>
</html>
```
