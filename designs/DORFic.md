# DORFic Design Reference

DORFic stands for **Daylight, Orange, Red, Futurism, and Graphic** (shortened to "-fic"). It is an aesthetic featuring **Abstract Tech-esque minimalist imagery** that was popular from the **mid-to-late 2000s to the mid-2010s**. The style is **industrial and highly minimalist**, featuring **stark white cityscapes** primarily accented with **bright oranges and grey**. It combines **sterile scientific gear** with **military and factory iconography**, presenting a sanitized technological vision that is clean, sharp, and futuristic without relying on neon or holographic excess. The aesthetic closely overlaps with Frutiger Aero but emphasizes industrialism over natural elements, and shares cyberpunk's technological focus while remaining "majorly more sanitized and less dependent on neon gear and holographics."

---

## Visual Characteristics

### Core Motifs and Patterns

- **Stark white environments** -- clean, bright cityscapes and interiors bathed in daylight
- **Bright orange as the dominant accent** -- the signature color that defines DORFic, used for highlights, UI elements, and graphic overlays
- **Parallel and symmetric geometry** -- rigid structural compositions with strong geometric repetition
- **Low polygonal composition** -- faceted, angular 3D forms and surfaces
- **Glass and tech patterns** -- transparent, reflective panels and technological surface treatments
- **Office spaces and robotics** -- sterile, corporate-futuristic environments
- **Sunlight and cleanliness emphasis** -- bright, naturally-lit scenes that feel hygienic and optimistic
- **Sterile scientific gear** -- lab equipment, protective equipment, precision instruments
- **Military and factory iconography** -- industrial symbols, utilitarian labeling, functional graphics
- **Goggles, visors, and protective gear** -- techwear accessories as visual motifs
- **Explosive visuals** -- dynamic, high-energy 3D compositions and motion graphics
- **Monochromatic base with selective color pops** -- near-grayscale environments punctuated by vivid orange and red

### Design Principles

- **Industrial minimalism** -- stripped-down, functional design with no decorative excess
- **Sanitized futurism** -- technology portrayed as clean, controlled, and orderly (not gritty or dystopian)
- **Daylight-driven illumination** -- bright, white-dominant lighting that feels natural and open
- **High contrast between white space and orange accents** -- the tension between neutral base and vivid color
- **Geometric precision** -- every element is aligned, symmetrical, and intentional
- **Abstract tech imagery** -- technology represented through stylized graphics, not photorealism
- **Bordering on monochromatic** -- minimal color usage beyond the white/gray/orange core
- **Sharp, clean, and casual** -- professional but not stiff; technical but approachable

---

## Color Palette

### Primary Scheme

| Role | Colors |
|------|--------|
| **Base / Background** | White, off-white, light gray |
| **Primary accent** | Bright orange, amber orange |
| **Secondary accent** | Red, warm red-orange |
| **Neutral structure** | Gray, charcoal, steel gray |
| **Tertiary accent** | Blue (used sparingly for tech/interface elements) |
| **High contrast** | Black (used in dark variant) |

### Detailed Palette

| Color | Hex (suggested) | Usage |
|-------|-----------------|-------|
| Pure White | `#FFFFFF`, `#FAFAFA` | Primary backgrounds, open space |
| Soft White | `#F0F2F5`, `#E8EAED` | Secondary backgrounds, card surfaces |
| DORFic Orange | `#FF6600`, `#FF7A1A` | Primary accent, highlights, CTAs, key UI elements |
| Warm Amber | `#FF8C00`, `#FFA033` | Secondary accent, gradients with orange |
| Signal Red | `#E03020`, `#CC2A1A` | Tertiary accent, alerts, emphasis markers |
| Light Gray | `#C0C4CC`, `#B0B4BC` | Borders, subtle UI elements, secondary text |
| Medium Gray | `#808690`, `#6E7480` | Body text, structural lines |
| Charcoal | `#3A3E48`, `#2E3240` | Headlines on white, dark UI panels |
| Near Black | `#1A1E28`, `#12161E` | Dark variant backgrounds, maximum contrast |
| Tech Blue | `#0074D9`, `#1A8CFF` | Interface accents, links, tech indicators |

### Dark Variant Palette

DORFic has a recognized dark alternate where black replaces white backgrounds, leaning toward Cyberpunk and Dark Aero:

| Color | Hex (suggested) | Usage |
|-------|-----------------|-------|
| Dark Base | `#0D0F14`, `#141820` | Primary dark background |
| Dark Surface | `#1E222C`, `#262B38` | Card backgrounds, panels |
| Dark Border | `#3A3E48` | Subtle dividers and edges |
| Orange on Dark | `#FF6600`, `#FF7A1A` | Accent (same orange, higher contrast on dark) |

### Suggested CSS Custom Properties

```css
:root {
  /* Whites and neutrals */
  --dorfic-white: #ffffff;
  --dorfic-off-white: #f0f2f5;
  --dorfic-soft-white: #e8eaed;
  --dorfic-light-gray: #c0c4cc;
  --dorfic-mid-gray: #808690;
  --dorfic-charcoal: #3a3e48;
  --dorfic-near-black: #1a1e28;

  /* Orange accent spectrum */
  --dorfic-orange: #ff6600;
  --dorfic-orange-light: #ff8c33;
  --dorfic-orange-bright: #ff7a1a;
  --dorfic-amber: #ff8c00;
  --dorfic-orange-glow: rgba(255, 102, 0, 0.3);
  --dorfic-orange-subtle: rgba(255, 102, 0, 0.08);

  /* Red accent */
  --dorfic-red: #e03020;
  --dorfic-red-light: #ff4433;

  /* Blue accent */
  --dorfic-blue: #0074d9;
  --dorfic-blue-light: #1a8cff;

  /* Functional mappings (light mode) */
  --dorfic-bg-primary: var(--dorfic-white);
  --dorfic-bg-secondary: var(--dorfic-off-white);
  --dorfic-bg-surface: var(--dorfic-soft-white);
  --dorfic-text-primary: var(--dorfic-charcoal);
  --dorfic-text-secondary: var(--dorfic-mid-gray);
  --dorfic-accent: var(--dorfic-orange);
  --dorfic-accent-hover: var(--dorfic-orange-bright);
  --dorfic-border: var(--dorfic-light-gray);
}

/* Dark variant override */
[data-theme="dark"] {
  --dorfic-bg-primary: #0d0f14;
  --dorfic-bg-secondary: #141820;
  --dorfic-bg-surface: #1e222c;
  --dorfic-text-primary: #e8eaed;
  --dorfic-text-secondary: #808690;
  --dorfic-border: #3a3e48;
}
```

### Approaches

- **White-dominant base with orange punches** -- vast white or light gray fields interrupted by vivid orange elements
- **Near-monochromatic gray structure** -- charcoal-to-white gradient range for all structural elements
- **Orange as navigation and emphasis only** -- never used for large background areas; always a focused accent
- **Red for secondary emphasis** -- sparing use alongside orange for alerts or important callouts
- **Daylight warmth** -- slight warm tint to whites (not cold/blue-white) to evoke sunlit environments

---

## Typography

### Typeface Characteristics

DORFic typography reflects mid-2000s corporate tech and industrial design:

- **Clean, geometric sans-serif typefaces** -- functional and technical without ornamentation
- **Medium to bold weights for headings** -- strong, authoritative presence
- **Condensed or semi-condensed proportions** -- space-efficient, industrial feel
- **Uppercase for labels and navigation** -- utilitarian, military-influenced labeling
- **Wide letter-spacing on display text** -- creates an airy, futuristic quality
- **No serifs** -- everything is modern, technical, forward-looking
- **Orange-accented type** -- key words or numbers rendered in DORFic orange against white/gray
- **Small technical labels** -- spec-sheet style text for secondary information

### Recommended Web Fonts (Google Fonts / Free)

| Font | Style | Usage |
|------|-------|-------|
| **Rajdhani** | Semi-condensed, technical, geometric | Headlines, navigation, labels |
| **Exo 2** | Geometric, futuristic sans | Display headings, feature titles |
| **Barlow** | Slightly condensed, industrial grotesk | Headlines, body text |
| **Barlow Condensed** | Narrow industrial grotesk | Labels, navigation, utility text |
| **Inter** | Clean, neutral, modern sans | Body text, paragraphs |
| **Source Sans 3** | Adobe open-source, technical clarity | Body text, UI elements |
| **Titillium Web** | Angular, tech-forward | Headlines, interface text |
| **Saira** | Wide, geometric, industrial | Display headings, numbers |
| **Chakra Petch** | Angular, tech-industrial | Display text, data labels |
| **Oswald** | Condensed, strong | Section headings, uppercase labels |

### Typography CSS Example

```css
/* Headlines */
h1, h2, h3 {
  font-family: 'Rajdhani', 'Barlow', sans-serif;
  font-weight: 600;
  letter-spacing: 0.06em;
  color: var(--dorfic-charcoal);
  line-height: 1.15;
}

/* Display / Hero text */
.dorfic-display {
  font-family: 'Exo 2', 'Saira', sans-serif;
  font-size: clamp(2.5rem, 6vw, 5.5rem);
  font-weight: 700;
  letter-spacing: 0.08em;
  text-transform: uppercase;
  line-height: 1.05;
  color: var(--dorfic-charcoal);
}

/* Orange accent text */
.dorfic-accent-text {
  color: var(--dorfic-orange);
  font-weight: 700;
}

/* Body text */
body {
  font-family: 'Inter', 'Source Sans 3', sans-serif;
  font-weight: 400;
  letter-spacing: 0.01em;
  line-height: 1.65;
  color: var(--dorfic-text-secondary);
}

/* Industrial label text */
.dorfic-label {
  font-family: 'Barlow Condensed', 'Oswald', sans-serif;
  font-size: 0.7rem;
  font-weight: 600;
  text-transform: uppercase;
  letter-spacing: 0.2em;
  color: var(--dorfic-mid-gray);
}

/* Technical / data text */
.dorfic-tech {
  font-family: 'Chakra Petch', 'Titillium Web', monospace;
  font-size: 0.85rem;
  letter-spacing: 0.05em;
  color: var(--dorfic-mid-gray);
}
```

---

## Layout Principles

### Grid and Structure

- **Rigid, symmetric grid layouts** -- parallel lines, equal spacing, engineered precision
- **White space as a primary design element** -- vast open areas that evoke sterile, sunlit environments
- **Wide, horizontal compositions** -- landscape-oriented sections reflecting widescreen interfaces
- **Strong vertical and horizontal axes** -- everything aligns to a visible or implied grid
- **Full-width sections with constrained content** -- content centered within expansive white fields
- **Geometric containers** -- rectangular and angular panels, not rounded or organic

### Section Organization

- Use **bold orange dividers or accent lines** to separate sections
- Apply **angular geometric shapes** as section backgrounds or decorative elements
- Create **hierarchy through scale and color** -- larger elements and orange elements draw attention first
- Employ **card-style panels with subtle gray borders** -- clean, flat, minimal elevation
- Use **asymmetric layouts with strong alignment** -- offset content that still respects the grid
- Include **industrial-style numbering or labeling** -- "01 / OVERVIEW" style section markers
- Apply **generous padding** -- breathing room that evokes clean, clinical environments

### Compositional Patterns

- **Split layouts** -- half white, half image/content, divided by an orange accent line
- **Overlapping geometric panels** -- layered rectangles and parallelograms creating depth
- **Data-dashboard style grids** -- modular, evenly-spaced card layouts
- **Full-bleed photography with geometric overlays** -- photos of cityscapes or tech masked by angular shapes

---

## CSS/Design Techniques

### Orange Accent Bar / Stripe

```css
/* Signature DORFic accent bar */
.dorfic-accent-bar {
  width: 60px;
  height: 4px;
  background: var(--dorfic-orange);
  margin: 1rem 0;
}

/* Full-width accent divider */
.dorfic-divider {
  width: 100%;
  height: 3px;
  background: linear-gradient(
    90deg,
    var(--dorfic-orange) 0%,
    var(--dorfic-orange) 30%,
    var(--dorfic-light-gray) 30%,
    var(--dorfic-light-gray) 100%
  );
}

/* Partial accent divider (industrial style) */
.dorfic-divider-partial {
  height: 2px;
  background: linear-gradient(
    90deg,
    var(--dorfic-orange) 0%,
    var(--dorfic-orange) 120px,
    transparent 120px
  );
}
```

### Industrial Panel / Card

```css
/* Clean DORFic card on white background */
.dorfic-card {
  background: var(--dorfic-white);
  border: 1px solid var(--dorfic-light-gray);
  border-left: 4px solid var(--dorfic-orange);
  padding: 2rem;
  position: relative;
}

/* Card with orange top accent */
.dorfic-card-top {
  background: var(--dorfic-white);
  border: 1px solid var(--dorfic-light-gray);
  border-top: 4px solid var(--dorfic-orange);
  padding: 2rem;
  box-shadow: 0 2px 8px rgba(0, 0, 0, 0.04);
}

/* Dark variant card */
.dorfic-card-dark {
  background: var(--dorfic-bg-surface, #1e222c);
  border: 1px solid rgba(255, 102, 0, 0.15);
  border-left: 4px solid var(--dorfic-orange);
  padding: 2rem;
  color: #e8eaed;
}
```

### Geometric Overlay / Angular Clip

```css
/* Angular section divider (parallelogram shape) */
.dorfic-angle-divider {
  width: 100%;
  height: 80px;
  background: var(--dorfic-off-white);
  clip-path: polygon(0 0, 100% 30%, 100% 100%, 0 70%);
}

/* Angular accent block */
.dorfic-angle-block {
  position: relative;
  overflow: hidden;
}

.dorfic-angle-block::before {
  content: '';
  position: absolute;
  top: 0;
  right: -5%;
  width: 40%;
  height: 100%;
  background: var(--dorfic-orange);
  clip-path: polygon(20% 0, 100% 0, 100% 100%, 0% 100%);
  opacity: 0.08;
  pointer-events: none;
}

/* Low-poly geometric background pattern */
.dorfic-geometric-bg {
  background:
    linear-gradient(135deg, transparent 40%, rgba(255, 102, 0, 0.03) 40%, rgba(255, 102, 0, 0.03) 60%, transparent 60%),
    linear-gradient(225deg, transparent 40%, rgba(58, 62, 72, 0.03) 40%, rgba(58, 62, 72, 0.03) 60%, transparent 60%);
  background-size: 120px 120px;
}
```

### Orange Glow and Highlight Effects

```css
/* Orange glow for interactive elements */
.dorfic-glow {
  box-shadow:
    0 0 8px rgba(255, 102, 0, 0.3),
    0 0 24px rgba(255, 102, 0, 0.1);
}

/* Orange highlight border on hover */
.dorfic-highlight {
  transition: all 0.25s ease;
  border-left: 4px solid transparent;
}

.dorfic-highlight:hover {
  border-left: 4px solid var(--dorfic-orange);
  background: var(--dorfic-orange-subtle);
}

/* Orange underline accent for text */
.dorfic-underline {
  text-decoration: none;
  position: relative;
}

.dorfic-underline::after {
  content: '';
  position: absolute;
  bottom: -2px;
  left: 0;
  width: 100%;
  height: 2px;
  background: var(--dorfic-orange);
  transform: scaleX(0);
  transform-origin: left;
  transition: transform 0.3s ease;
}

.dorfic-underline:hover::after {
  transform: scaleX(1);
}
```

### Industrial Section Marker

```css
/* Numbered section label (e.g., "01 / OVERVIEW") */
.dorfic-section-marker {
  display: flex;
  align-items: center;
  gap: 0.75rem;
  margin-bottom: 2rem;
}

.dorfic-section-marker .number {
  font-family: 'Saira', 'Exo 2', sans-serif;
  font-size: 2rem;
  font-weight: 700;
  color: var(--dorfic-orange);
  line-height: 1;
}

.dorfic-section-marker .separator {
  width: 1px;
  height: 24px;
  background: var(--dorfic-light-gray);
}

.dorfic-section-marker .title {
  font-family: 'Barlow Condensed', sans-serif;
  font-size: 0.75rem;
  font-weight: 600;
  text-transform: uppercase;
  letter-spacing: 0.25em;
  color: var(--dorfic-mid-gray);
}
```

### DORFic Button Styles

```css
/* Primary orange button */
.dorfic-button {
  display: inline-block;
  padding: 0.75rem 2rem;
  background: var(--dorfic-orange);
  color: var(--dorfic-white);
  border: none;
  font-family: 'Barlow Condensed', 'Rajdhani', sans-serif;
  font-size: 0.85rem;
  font-weight: 600;
  text-transform: uppercase;
  letter-spacing: 0.15em;
  cursor: pointer;
  transition: all 0.2s ease;
}

.dorfic-button:hover {
  background: var(--dorfic-orange-bright);
  box-shadow: 0 4px 16px rgba(255, 102, 0, 0.3);
}

/* Ghost / outline button */
.dorfic-button-ghost {
  display: inline-block;
  padding: 0.7rem 2rem;
  background: transparent;
  color: var(--dorfic-orange);
  border: 2px solid var(--dorfic-orange);
  font-family: 'Barlow Condensed', 'Rajdhani', sans-serif;
  font-size: 0.85rem;
  font-weight: 600;
  text-transform: uppercase;
  letter-spacing: 0.15em;
  cursor: pointer;
  transition: all 0.2s ease;
}

.dorfic-button-ghost:hover {
  background: var(--dorfic-orange);
  color: var(--dorfic-white);
}
```

### Glass / Tech Panel Effect

```css
/* Frosted glass panel (DORFic tech style) */
.dorfic-glass {
  background: rgba(255, 255, 255, 0.7);
  backdrop-filter: blur(12px);
  -webkit-backdrop-filter: blur(12px);
  border: 1px solid rgba(192, 196, 204, 0.4);
  box-shadow: 0 2px 12px rgba(0, 0, 0, 0.06);
}

/* Dark variant glass */
.dorfic-glass-dark {
  background: rgba(30, 34, 44, 0.8);
  backdrop-filter: blur(12px);
  -webkit-backdrop-filter: blur(12px);
  border: 1px solid rgba(255, 102, 0, 0.1);
}
```

### Sterile Grid Background

```css
/* Fine technical grid (blueprint/schematic feel) */
.dorfic-grid-bg {
  background-image:
    linear-gradient(rgba(192, 196, 204, 0.15) 1px, transparent 1px),
    linear-gradient(90deg, rgba(192, 196, 204, 0.15) 1px, transparent 1px);
  background-size: 40px 40px;
}

/* Grid with orange accent lines */
.dorfic-grid-accent {
  background-image:
    linear-gradient(rgba(192, 196, 204, 0.1) 1px, transparent 1px),
    linear-gradient(90deg, rgba(192, 196, 204, 0.1) 1px, transparent 1px),
    linear-gradient(rgba(255, 102, 0, 0.06) 1px, transparent 1px),
    linear-gradient(90deg, rgba(255, 102, 0, 0.06) 1px, transparent 1px);
  background-size: 40px 40px, 40px 40px, 200px 200px, 200px 200px;
}
```

---

## Materials and Textures (Visual Metaphors for Web)

Physical DORFic materials and their web equivalents:

| Physical Material | Web Equivalent |
|-------------------|----------------|
| Stark white architecture | `#FFFFFF` or `#FAFAFA` backgrounds with generous whitespace |
| Industrial orange paint | Flat `#FF6600` fills on buttons, bars, and accent elements |
| Matte gray steel | Flat mid-gray (`#808690`) borders and dividers, no gradients |
| Scientific glass panels | `backdrop-filter: blur()` with semi-transparent white background |
| Factory signage | Uppercase condensed sans-serif labels with wide letter-spacing |
| Low-poly 3D surfaces | Angular `clip-path` shapes and geometric SVG patterns |
| Protective visor glass | Gradient from transparent to slightly tinted overlay |
| Daylight illumination | Subtle warm box-shadows and bright, open layouts |
| Technical schematics | Fine grid backgrounds with thin gray lines |

---

## Era-Defining Products and Influences

The following products, brands, and media define the DORFic visual language and serve as design references:

- **Microsoft Office 2003-2010** -- orange-accented UI, clean white panels, geometric icons
- **Xbox 360 LIVE** -- white/green/gray interface with bold accent colors and clean geometry
- **Mirror's Edge** (2008) -- stark white cityscapes with vivid red/orange accents, the quintessential DORFic game
- **SUPERHOT** (2016) -- minimalist white environments with red geometric shapes
- **Intel Pentium 4 branding** (with Blue Man Group) -- clean tech imagery with bold color accents
- **Android 1.0** -- early mobile UI with functional, minimalist design language
- **Nintendo eShop** -- clean, bright digital storefront with structured grid layout
- **Rocket League** -- bright, clean sci-fi sports aesthetic
- **Halo series** -- futuristic military-industrial design with clean geometry
- **Orangetheory Fitness** -- brand identity built on DORFic orange-on-white principles
- **Avast Antivirus** -- orange accent on white/gray clean tech interface

---

## Related Aesthetics

| Aesthetic | Relationship to DORFic |
|-----------|----------------------|
| **Frutiger Aero** | Closest overlap; DORFic replaces Frutiger Aero's natural elements with industrial/military motifs |
| **Abstract Tech** | Parent influence; DORFic is essentially Abstract Tech with a specific orange/white palette |
| **Corporate** | Shares the clean, professional, sterile sensibility but DORFic adds futurism and bold color |
| **Cyberpunk** | DORFic's dark variant approaches Cyberpunk but remains more sanitized, less neon |
| **Dark Aero** | The dark variant of DORFic overlaps significantly with Dark Aero |
| **Minimalism** | Foundational influence; DORFic is minimalism with industrial and tech overlays |
| **Skeuomorphism** | Temporal overlap (same era); DORFic tends toward flatter, less ornate treatments |
| **Technozen** | Shares clean tech sensibility; Technozen is calmer and more zen, DORFic is more industrial |
| **Y2K Futurism** | Predecessor; DORFic carries Y2K's optimistic futurism into the late 2000s |
| **Vectorheart** | Related graphic style; shares clean vector aesthetics and geometric precision |

---

## Quick-Start: Minimal DORFic Page Template

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>DORFic Page</title>
  <link href="https://fonts.googleapis.com/css2?family=Rajdhani:wght@400;600;700&family=Exo+2:wght@400;700&family=Barlow+Condensed:wght@400;600&family=Inter:wght@300;400&display=swap" rel="stylesheet">
  <style>
    :root {
      --dorfic-white: #ffffff;
      --dorfic-off-white: #f0f2f5;
      --dorfic-light-gray: #c0c4cc;
      --dorfic-mid-gray: #808690;
      --dorfic-charcoal: #3a3e48;
      --dorfic-orange: #ff6600;
      --dorfic-orange-bright: #ff7a1a;
      --dorfic-orange-glow: rgba(255, 102, 0, 0.3);
      --dorfic-orange-subtle: rgba(255, 102, 0, 0.08);
    }

    * { margin: 0; padding: 0; box-sizing: border-box; }

    body {
      background: var(--dorfic-white);
      color: var(--dorfic-mid-gray);
      font-family: 'Inter', sans-serif;
      font-weight: 400;
      letter-spacing: 0.01em;
      line-height: 1.65;
    }

    h1, h2, h3 {
      font-family: 'Rajdhani', sans-serif;
      font-weight: 600;
      letter-spacing: 0.06em;
      color: var(--dorfic-charcoal);
    }

    .hero {
      text-align: center;
      padding: 8rem 2rem 6rem;
      background: var(--dorfic-off-white);
      position: relative;
      overflow: hidden;
    }

    .hero::before {
      content: '';
      position: absolute;
      top: 0;
      right: -5%;
      width: 40%;
      height: 100%;
      background: var(--dorfic-orange);
      clip-path: polygon(20% 0, 100% 0, 100% 100%, 0% 100%);
      opacity: 0.06;
    }

    .hero h1 {
      font-family: 'Exo 2', sans-serif;
      font-size: clamp(2.5rem, 6vw, 5rem);
      font-weight: 700;
      text-transform: uppercase;
      letter-spacing: 0.08em;
      line-height: 1.05;
    }

    .hero h1 span {
      color: var(--dorfic-orange);
    }

    .dorfic-accent-bar {
      width: 60px;
      height: 4px;
      background: var(--dorfic-orange);
      margin: 1.5rem auto;
    }

    .hero p {
      max-width: 500px;
      margin: 0 auto;
      color: var(--dorfic-mid-gray);
    }

    section {
      max-width: 900px;
      margin: 0 auto;
      padding: 5rem 2rem;
    }

    .section-marker {
      display: flex;
      align-items: center;
      gap: 0.75rem;
      margin-bottom: 2rem;
    }

    .section-marker .num {
      font-family: 'Exo 2', sans-serif;
      font-size: 2rem;
      font-weight: 700;
      color: var(--dorfic-orange);
    }

    .section-marker .sep {
      width: 1px;
      height: 24px;
      background: var(--dorfic-light-gray);
    }

    .section-marker .label {
      font-family: 'Barlow Condensed', sans-serif;
      font-size: 0.75rem;
      font-weight: 600;
      text-transform: uppercase;
      letter-spacing: 0.25em;
      color: var(--dorfic-mid-gray);
    }

    .dorfic-card {
      background: var(--dorfic-white);
      border: 1px solid var(--dorfic-light-gray);
      border-left: 4px solid var(--dorfic-orange);
      padding: 2rem;
      margin-bottom: 1.5rem;
    }

    .dorfic-card h3 {
      margin-bottom: 0.5rem;
    }

    .dorfic-button {
      display: inline-block;
      padding: 0.75rem 2rem;
      background: var(--dorfic-orange);
      color: #fff;
      border: none;
      font-family: 'Barlow Condensed', sans-serif;
      font-size: 0.85rem;
      font-weight: 600;
      text-transform: uppercase;
      letter-spacing: 0.15em;
      cursor: pointer;
      transition: all 0.2s ease;
      text-decoration: none;
    }

    .dorfic-button:hover {
      background: var(--dorfic-orange-bright);
      box-shadow: 0 4px 16px var(--dorfic-orange-glow);
    }
  </style>
</head>
<body>
  <div class="hero">
    <h1>Title <span>Here</span></h1>
    <div class="dorfic-accent-bar"></div>
    <p>Subtitle in clean Inter with industrial precision and DORFic clarity</p>
  </div>
  <section>
    <div class="section-marker">
      <span class="num">01</span>
      <span class="sep"></span>
      <span class="label">Overview</span>
    </div>
    <div class="dorfic-card">
      <h3>Section Heading</h3>
      <p>Content styled with the DORFic industrial minimalist aesthetic. Clean, precise, orange-accented.</p>
    </div>
    <a href="#" class="dorfic-button">Explore More</a>
  </section>
</body>
</html>
```
