# Neo-Vectorheart

A pseudo-revival of the Vectorheart aesthetic that emerged in the late 2010s as part of the
broader Neo-Y2K movement. Neo-Vectorheart fuses the angular vector geometry and monochromatic
rigor of the original Vectorheart style (pioneered by The Designers Republic and Bionic Systems)
with Neubrutalist design language and gamer-grunge maximalism. The result is sleek, dynamic, and
visually aggressive -- striking vector shapes and sharp diagonal compositions rendered in
predominantly black-and-white palettes with bold accent color punctuation. It is less abstract
than original Vectorheart and more grounded in contemporary digital culture, particularly
gaming, logo design, and cyberpunk-influenced graphics.

---

## Color Palette

### Primary Scheme

Neo-Vectorheart is fundamentally **monochromatic**. Black and white are the dominant colors;
all other hues function as accent/complementary colors rather than primary ones. This
high-contrast monochrome foundation is what gives the aesthetic its sharp, logo-ready quality.

| Role | Colors | Hex (suggested) |
|------|--------|-----------------|
| **Primary background** | Pure black, near-black | `#000000`, `#0A0A0A`, `#0D0D0D` |
| **Secondary background** | Dark charcoal | `#141414`, `#1A1A1A` |
| **Surface / panels** | Off-black, dark gray | `#1E1E1E`, `#242424` |
| **Primary text / shapes** | Pure white, near-white | `#FFFFFF`, `#F0F0F0` |
| **Secondary text** | Mid-gray | `#888888`, `#999999` |
| **Muted elements** | Dark gray | `#555555`, `#666666` |
| **Borders / hard edges** | White or near-white | `#FFFFFF`, `#E0E0E0` |
| **Accent (electric)** | Single vivid hue -- pick one per composition | See accent palette below |

### Accent Color Palette

Accents are used sparingly -- a single vivid color per composition or section, never multiple
competing hues. The accent color should feel like a deliberate, high-voltage interruption of
the monochrome field.

| Accent Name | Hex | Usage |
|-------------|-----|-------|
| Volt Green | `#00FF66`, `#39FF14` | Gaming-inflected energy, terminal glow, active states |
| Electric Cyan | `#00FFFF`, `#00D4FF` | Tech-forward, cyberpunk undertones |
| Hot Magenta | `#FF00FF`, `#FF0066` | Aggressive, attention-grabbing highlights |
| Signal Red | `#FF0033`, `#FF1A1A` | Alert states, aggressive emphasis |
| Acid Yellow | `#CCFF00`, `#DFFF00` | High-visibility labels, caution elements |
| UV Purple | `#BF00FF`, `#9B30FF` | Cyberpunk accent, glow effects |

### Color Guidelines

- **Black and white dominate** -- resist adding color; the monochromatic scheme is the aesthetic
- **One accent per composition** -- choose a single vivid accent and use it consistently
- Accent colors work best on **small, high-impact elements**: outlines, icons, a single word, a divider line
- **No gradients on primary surfaces** -- gradients are minimal and reserved for subtle glow or accent effects
- High-contrast relationships are mandatory -- avoid mid-tone pairings that reduce sharpness
- The inverted palette (white background, black shapes) is equally valid

### Suggested CSS Custom Properties

```css
:root {
  /* Monochrome base */
  --nv-black: #000000;
  --nv-near-black: #0a0a0a;
  --nv-dark: #141414;
  --nv-surface: #1e1e1e;
  --nv-mid-dark: #242424;
  --nv-gray: #555555;
  --nv-mid-gray: #888888;
  --nv-light-gray: #cccccc;
  --nv-near-white: #f0f0f0;
  --nv-white: #ffffff;

  /* Single accent -- swap per composition */
  --nv-accent: #00FF66;
  --nv-accent-dim: rgba(0, 255, 102, 0.3);
  --nv-accent-glow: rgba(0, 255, 102, 0.15);

  /* Functional mappings */
  --nv-bg-primary: var(--nv-black);
  --nv-bg-secondary: var(--nv-dark);
  --nv-bg-surface: var(--nv-surface);
  --nv-text-primary: var(--nv-white);
  --nv-text-secondary: var(--nv-mid-gray);
  --nv-text-muted: var(--nv-gray);
  --nv-border: var(--nv-white);
  --nv-border-subtle: var(--nv-mid-dark);
}
```

---

## Typography

### Typeface Characteristics

Neo-Vectorheart typography is futuristic, geometric, and bold:

- **Futuristic display typefaces** -- angular, geometric, tech-forward fonts that feel engineered and digitally precise
- **Bold, uppercase, condensed** -- headlines are loud, compressed, and commanding
- **Tight or negative letter-spacing on headlines** -- creates density and visual force
- **All-caps as default for headings and labels** -- industrial, utilitarian, tech-aggressive
- **Neubrutalist influence on type** -- stretched, grotesque, or deliberately unconventional typefaces alongside cleaner options
- **Monospaced accents** -- code-style fonts for decorative data overlays and technical annotations
- **White text on black (or inverted)** -- high contrast is non-negotiable; no mid-tone type on mid-tone backgrounds
- **No serif fonts** -- the aesthetic is entirely sans-serif and monospace

### Recommended Web Fonts (Google Fonts)

| Font | Style | Usage |
|------|-------|-------|
| **Orbitron** | Square, geometric, tech-forward | Hero titles, display headings, logo-style text |
| **Chakra Petch** | Angular, semi-condensed, mechanical | Headlines, section titles, navigation |
| **Bebas Neue** | Tall condensed sans-serif | Large display text, impactful uppercase headings |
| **Rajdhani** | Semi-condensed, technical, clean | Subheadings, labels, UI text |
| **Space Grotesk** | Geometric grotesque | Body text, mid-weight headings |
| **Exo 2** | Geometric, futuristic sans | Section titles, medium-weight display |
| **Share Tech Mono** | Technical monospace | Data overlays, annotations, decorative code |
| **Inter** | Neutral neo-grotesque | Body text, paragraphs |
| **Audiowide** | Wide, futuristic, bold | Impactful display text, brand-style headings |
| **Bruno Ace** | Mechanical, futuristic | Display headlines, accent text |

### Typography CSS Example

```css
@import url('https://fonts.googleapis.com/css2?family=Orbitron:wght@400;700;900&family=Chakra+Petch:wght@400;600;700&family=Bebas+Neue&family=Rajdhani:wght@400;500;600&family=Inter:wght@300;400;500&family=Share+Tech+Mono&display=swap');

/* Display / Hero text */
.nv-display {
  font-family: 'Orbitron', 'Bebas Neue', sans-serif;
  font-size: clamp(3rem, 9vw, 8rem);
  font-weight: 900;
  letter-spacing: -0.02em;
  line-height: 0.9;
  text-transform: uppercase;
  color: var(--nv-white);
}

/* Headlines */
h1, h2, h3 {
  font-family: 'Chakra Petch', 'Rajdhani', sans-serif;
  font-weight: 700;
  letter-spacing: 0.06em;
  text-transform: uppercase;
  color: var(--nv-white);
  line-height: 1.05;
}

/* Body text */
body {
  font-family: 'Inter', 'Space Grotesk', sans-serif;
  font-weight: 400;
  font-size: 1rem;
  line-height: 1.6;
  color: var(--nv-text-secondary);
  -webkit-font-smoothing: antialiased;
}

/* Technical label / overline */
.nv-label {
  font-family: 'Rajdhani', 'Chakra Petch', sans-serif;
  font-size: 0.7rem;
  text-transform: uppercase;
  letter-spacing: 0.2em;
  color: var(--nv-text-muted);
}

/* Monospaced decorative text */
.nv-mono {
  font-family: 'Share Tech Mono', monospace;
  font-size: 0.65rem;
  letter-spacing: 0.08em;
  color: var(--nv-accent);
  opacity: 0.5;
}

/* Accent-colored text with glow */
.nv-accent-text {
  color: var(--nv-accent);
  text-shadow:
    0 0 8px var(--nv-accent-dim),
    0 0 24px var(--nv-accent-glow);
}
```

---

## Key Design Elements and Motifs

### Defining Visual Elements

- **45-degree and 60-degree diagonal lines** -- the signature structural motif; slashes, chevrons, and angled dividers appear everywhere, creating aggressive directional energy
- **Striking vector shapes** -- hard-edged, flat geometric forms (triangles, parallelograms, chevrons, abstract polygons) rendered as clean vectors, not organic or hand-drawn
- **Monochromatic compositions** -- black and white dominate with clinical precision; color is an event, not a default
- **Bold outlines and hard borders** -- Neubrutalist influence: thick, visible borders on elements instead of soft shadows
- **Hard 45-degree shadows** -- flat, offset shadows (not diffused drop shadows) in the Neubrutalist tradition
- **Trademark / copyright symbols** -- liberal decorative use of TM, (C), (R) symbols inherited from original Vectorheart
- **Logo abundance** -- repeated, rotated, and stacked logo-like elements as compositional texture
- **Silhouettes and icons** -- bold, flat, iconographic forms used as graphic accents
- **Japanese-influenced typography** -- occasional kanji characters or anime-inflected graphical elements (inherited from Vectorheart)
- **Technical annotations** -- monospaced data strings, coordinates, and alphanumeric codes used decoratively
- **Anti-establishment messaging** -- ironic slogans, exaggerated consumer-culture references, cyberpunk undertones

### Patterns vs. Original Vectorheart

Neo-Vectorheart uses **less abstract patterns** than original Vectorheart. Where the original favored purely abstract geometric arrangements, the neo variant tends toward more recognizable, purposeful compositions -- logo-like constructs, identifiable angular symbols, and structured diagonal layouts rather than pure geometric abstraction.

---

## Composition and Layout Principles

### Structure and Geometry

- **Diagonal dominance** -- major layout divisions follow 45-degree or 60-degree angles; sections are sliced diagonally, not horizontally
- **Angular containers** -- use `clip-path` and `transform: skew()` to create non-rectangular panels, cards, and sections
- **Asymmetric, dynamic compositions** -- off-center layouts with strong directional thrust; nothing feels static
- **Maximum-minimalist philosophy** -- visually complex compositions built from minimal, precisely placed elements (inherited from original Vectorheart)
- **Hard-edge flat design** -- no rounded corners, no soft gradients, no blur effects; everything is crisp and geometric
- **Grid-breaking energy** -- while underlying structure may use a grid, visible elements deliberately break and overlap grid lines
- **Full-bleed backgrounds** -- sections fill the viewport edge-to-edge; no contained, centered content boxes
- **Overlapping and layered elements** -- shapes, text, and graphics stack and intersect to create visual density

### Neubrutalist Layout Influence

- **Thick visible borders** -- elements are outlined with bold strokes (2-4px solid white or black)
- **Flat, offset box-shadows** -- hard shadows at fixed angles (typically 4-8px offset at 45 degrees) instead of diffused drops
- **Geometric blocks** -- content contained in stark rectangular or angular blocks with visible edges
- **Deliberate visual tension** -- intentionally challenging compositions that feel energetic and confrontational
- **Random or asymmetric placement** -- elements may appear deliberately "off" from expected positions

### Section Organization

- **Diagonal dividers between sections** -- use angled `clip-path` or SVG shapes to create slashed transitions
- **High contrast section alternation** -- alternate between black-on-white and white-on-black sections
- **Angular accent bars** -- thin diagonal lines or bands of accent color as section markers
- **Dense header zones** -- concentrated visual information at the top of sections, with more breathing room below
- **Floating vector shapes** -- decorative geometric elements positioned at section edges and intersections

---

## CSS/Design Techniques

### Diagonal Section Divider

```css
/* Angled section transition using clip-path */
.nv-section {
  position: relative;
  padding: 6rem 2rem;
  clip-path: polygon(0 0, 100% 4%, 100% 96%, 0 100%);
}

/* Alternative: steeper 60-degree-style cut */
.nv-section--steep {
  clip-path: polygon(0 0, 100% 8%, 100% 92%, 0 100%);
}

/* Inverted black/white section pairing */
.nv-section--dark {
  background: var(--nv-black);
  color: var(--nv-white);
}

.nv-section--light {
  background: var(--nv-white);
  color: var(--nv-black);
}
```

### Hard 45-Degree Shadow (Neubrutalist)

```css
/* Signature flat offset shadow */
.nv-brutalist-shadow {
  box-shadow: 6px 6px 0 var(--nv-white);
  border: 2px solid var(--nv-white);
}

/* Inverted for light sections */
.nv-brutalist-shadow--inverted {
  box-shadow: 6px 6px 0 var(--nv-black);
  border: 2px solid var(--nv-black);
}

/* Accent-colored shadow variant */
.nv-brutalist-shadow--accent {
  box-shadow: 6px 6px 0 var(--nv-accent);
  border: 2px solid var(--nv-accent);
}
```

### Diagonal Line Accents

```css
/* 45-degree decorative line */
.nv-diagonal-line {
  position: absolute;
  width: 200%;
  height: 2px;
  background: var(--nv-white);
  transform: rotate(-45deg);
  transform-origin: 0 0;
  pointer-events: none;
}

/* 60-degree variant */
.nv-diagonal-line--steep {
  transform: rotate(-60deg);
}

/* Accent-colored diagonal */
.nv-diagonal-line--accent {
  background: var(--nv-accent);
  box-shadow: 0 0 10px var(--nv-accent-dim);
}

/* Diagonal stripe pattern overlay */
.nv-diagonal-stripes {
  background: repeating-linear-gradient(
    45deg,
    transparent,
    transparent 10px,
    rgba(255, 255, 255, 0.03) 10px,
    rgba(255, 255, 255, 0.03) 12px
  );
  pointer-events: none;
}
```

### Angular Vector Shape Elements

```css
/* Chevron / arrow shape */
.nv-chevron {
  width: 60px;
  height: 60px;
  clip-path: polygon(0 0, 50% 0, 100% 50%, 50% 100%, 0 100%, 50% 50%);
  background: var(--nv-white);
}

/* Parallelogram panel */
.nv-parallelogram {
  transform: skewX(-12deg);
  background: var(--nv-surface);
  border: 2px solid var(--nv-white);
  padding: 2rem 2.5rem;
}

.nv-parallelogram > * {
  transform: skewX(12deg); /* Counter-skew content */
}

/* Triangular accent */
.nv-triangle {
  width: 0;
  height: 0;
  border-left: 40px solid transparent;
  border-right: 40px solid transparent;
  border-bottom: 70px solid var(--nv-accent);
}

/* Angular clip container */
.nv-clipped-panel {
  clip-path: polygon(0 0, calc(100% - 30px) 0, 100% 30px, 100% 100%, 30px 100%, 0 calc(100% - 30px));
  background: var(--nv-surface);
  border: 2px solid var(--nv-white);
  padding: 2.5rem;
}
```

### Bold Border Card (Neubrutalist Influence)

```css
.nv-card {
  background: var(--nv-surface);
  border: 3px solid var(--nv-white);
  padding: 2rem;
  position: relative;
}

/* Hard offset shadow */
.nv-card::after {
  content: '';
  position: absolute;
  top: 6px;
  left: 6px;
  width: 100%;
  height: 100%;
  border: 3px solid var(--nv-white);
  z-index: -1;
  pointer-events: none;
}

/* Card with accent corner mark */
.nv-card--marked::before {
  content: '';
  position: absolute;
  top: 0;
  right: 0;
  width: 20px;
  height: 20px;
  background: var(--nv-accent);
  clip-path: polygon(0 0, 100% 0, 100% 100%);
}
```

### Trademark / Symbol Decorations

```css
/* Decorative TM/copyright symbols in the Vectorheart tradition */
.nv-tm::after {
  content: '\2122';  /* TM symbol */
  font-size: 0.45em;
  vertical-align: super;
  opacity: 0.6;
  margin-left: 0.15em;
  font-weight: 400;
}

.nv-reg::after {
  content: '\00AE';  /* Registered symbol */
  font-size: 0.4em;
  vertical-align: super;
  opacity: 0.5;
  margin-left: 0.1em;
}

/* Repeated logo/brand stamp pattern overlay */
.nv-logo-pattern {
  background-image: repeating-linear-gradient(
    45deg,
    transparent,
    transparent 40px,
    rgba(255, 255, 255, 0.02) 40px,
    rgba(255, 255, 255, 0.02) 42px
  );
  pointer-events: none;
}
```

### Accent Glow Effect

```css
/* Neon glow on accent-colored elements */
.nv-glow {
  box-shadow:
    0 0 4px var(--nv-accent),
    0 0 16px var(--nv-accent-dim),
    0 0 40px var(--nv-accent-glow);
}

/* Glow text */
.nv-glow-text {
  color: var(--nv-accent);
  text-shadow:
    0 0 6px var(--nv-accent-dim),
    0 0 20px var(--nv-accent-glow);
}

/* Accent-colored horizontal rule */
.nv-accent-rule {
  border: none;
  height: 3px;
  background: var(--nv-accent);
  box-shadow: 0 0 12px var(--nv-accent-dim);
}
```

### Neo-Vectorheart Button

```css
.nv-button {
  display: inline-block;
  padding: 0.8rem 2.5rem;
  border: 3px solid var(--nv-white);
  background: transparent;
  color: var(--nv-white);
  font-family: 'Chakra Petch', 'Rajdhani', sans-serif;
  font-size: 0.85rem;
  font-weight: 700;
  letter-spacing: 0.15em;
  text-transform: uppercase;
  cursor: pointer;
  position: relative;
  transition: all 0.15s ease;
}

.nv-button:hover {
  background: var(--nv-white);
  color: var(--nv-black);
}

/* Skewed / angular button variant */
.nv-button--skewed {
  transform: skewX(-8deg);
}

.nv-button--skewed:hover {
  background: var(--nv-accent);
  border-color: var(--nv-accent);
  color: var(--nv-black);
}

/* Brutalist shadow button */
.nv-button--brutal {
  box-shadow: 4px 4px 0 var(--nv-white);
  transition: all 0.1s ease;
}

.nv-button--brutal:hover {
  transform: translate(2px, 2px);
  box-shadow: 2px 2px 0 var(--nv-white);
}

/* Accent border button */
.nv-button--accent {
  border-color: var(--nv-accent);
  color: var(--nv-accent);
}

.nv-button--accent:hover {
  background: var(--nv-accent);
  color: var(--nv-black);
}
```

### Navigation

```css
.nv-nav {
  position: fixed;
  top: 0;
  left: 0;
  right: 0;
  z-index: 100;
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 1rem 2.5rem;
  background: var(--nv-black);
  border-bottom: 2px solid var(--nv-white);
}

.nv-nav-brand {
  font-family: 'Orbitron', sans-serif;
  font-weight: 700;
  font-size: 1rem;
  letter-spacing: 0.1em;
  text-transform: uppercase;
  color: var(--nv-white);
  text-decoration: none;
}

.nv-nav-links {
  display: flex;
  gap: 2rem;
  list-style: none;
}

.nv-nav-links a {
  color: var(--nv-text-secondary);
  text-decoration: none;
  font-family: 'Rajdhani', sans-serif;
  font-size: 0.8rem;
  font-weight: 600;
  letter-spacing: 0.15em;
  text-transform: uppercase;
  transition: color 0.15s ease;
}

.nv-nav-links a:hover {
  color: var(--nv-accent);
}
```

---

## Animation and Motion

- **Minimal, sharp transitions** -- no ease-in-out curves; use `ease` or `linear` with short durations (100-200ms)
- **Snap transformations** -- elements translate or rotate to precise positions, not fluid arcs
- **Diagonal slide-ins** -- elements enter the viewport along 45-degree or 60-degree paths
- **Accent pulse** -- subtle pulsing glow on accent-colored elements
- **No organic motion** -- everything moves mechanically and precisely; no bounce, wobble, or spring physics

```css
/* Diagonal slide-in */
@keyframes nv-slide-diagonal {
  from {
    transform: translate(-40px, 40px);
    opacity: 0;
  }
  to {
    transform: translate(0, 0);
    opacity: 1;
  }
}

.nv-animate-in {
  animation: nv-slide-diagonal 0.3s ease forwards;
}

/* Accent glow pulse */
@keyframes nv-pulse-glow {
  0%, 100% { box-shadow: 0 0 4px var(--nv-accent), 0 0 16px var(--nv-accent-dim); }
  50% { box-shadow: 0 0 8px var(--nv-accent), 0 0 30px var(--nv-accent-dim); }
}

.nv-pulse {
  animation: nv-pulse-glow 2s ease-in-out infinite;
}
```

---

## Cultural References and Influences

The following define the Neo-Vectorheart visual lineage:

- **The Designers Republic** -- pioneering Sheffield studio whose angular, logo-saturated, ironic-corporate vector work defined original Vectorheart
- **Bionic Systems** -- early 2000s design firm producing maximalist vector compositions
- **Peter Saville** -- Factory Records album art with its Swiss-influenced typographic precision
- **Gaming culture** -- esports branding, tournament graphics, streamer overlays, gamer-grunge maximalism
- **Cyberpunk media** -- dark, high-contrast, tech-dystopian visual language
- **Logo design communities** -- behance/dribbble monochromatic logo culture of the late 2010s
- **Neo-Y2K movement** -- broader revival of late-1990s/early-2000s digital aesthetics through a contemporary lens
- **Swiss modernism / International Typographic Style** -- grid precision and typographic hierarchy
- **Neubrutalism** -- bold borders, flat shadows, geometric blocks, confrontational layout

---

## Related Aesthetics

| Aesthetic | Relationship to Neo-Vectorheart |
|-----------|--------------------------------|
| **Vectorheart** | Direct ancestor; Neo-Vectorheart is the contemporary revival of this early-2000s aesthetic |
| **Neo-Y2K** | Parent movement; Neo-Vectorheart is one expression within the broader Neo-Y2K revival |
| **Neubrutalism** | Key influence; contributes bold borders, flat shadows, and confrontational layout language |
| **Cyberpunk** | Related; shares dark, high-contrast, tech-dystopian visual sensibility |
| **Acid Design** | Sibling; shares neon accents on dark backgrounds and rave-adjacent visual energy |
| **Cyberminimalism** | Related; shares monochromatic precision and digital sleekness, but Neo-Vectorheart is more maximalist |
| **Gamer** | Related; gamer-grunge maximalism is a primary influence on Neo-Vectorheart compositions |
| **Hexatron** | Related; shares geometric precision and tech-futurist dark aesthetics |
| **Vectorbloom** | Sibling; organic vector art from the same design lineage |
| **Metalheart** | Related; shares dark, angular, tech-aggressive design language but emphasizes 3D metallic forms |

---

## Quick-Start: Minimal Neo-Vectorheart Page Template

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Neo-Vectorheart Page</title>
  <link href="https://fonts.googleapis.com/css2?family=Orbitron:wght@400;700;900&family=Chakra+Petch:wght@400;600;700&family=Rajdhani:wght@400;500;600&family=Inter:wght@300;400;500&family=Share+Tech+Mono&display=swap" rel="stylesheet">
  <style>
    :root {
      --nv-black: #000000;
      --nv-dark: #141414;
      --nv-surface: #1e1e1e;
      --nv-gray: #555555;
      --nv-mid-gray: #888888;
      --nv-white: #ffffff;
      --nv-accent: #00FF66;
      --nv-accent-dim: rgba(0, 255, 102, 0.3);
      --nv-accent-glow: rgba(0, 255, 102, 0.15);
    }

    * { margin: 0; padding: 0; box-sizing: border-box; }

    body {
      background: var(--nv-black);
      color: var(--nv-white);
      font-family: 'Inter', sans-serif;
      font-weight: 400;
      font-size: 1rem;
      line-height: 1.6;
      -webkit-font-smoothing: antialiased;
      overflow-x: hidden;
    }

    h1, h2, h3 {
      font-family: 'Chakra Petch', sans-serif;
      font-weight: 700;
      letter-spacing: 0.06em;
      text-transform: uppercase;
      line-height: 1.05;
    }

    /* Navigation with hard border */
    nav {
      display: flex;
      justify-content: space-between;
      align-items: center;
      padding: 1rem 2.5rem;
      border-bottom: 2px solid var(--nv-white);
    }

    .brand {
      font-family: 'Orbitron', sans-serif;
      font-weight: 700;
      font-size: 1rem;
      letter-spacing: 0.1em;
      text-transform: uppercase;
    }

    .brand span {
      color: var(--nv-accent);
    }

    nav a {
      color: var(--nv-mid-gray);
      text-decoration: none;
      font-family: 'Rajdhani', sans-serif;
      font-size: 0.8rem;
      font-weight: 600;
      letter-spacing: 0.15em;
      text-transform: uppercase;
      transition: color 0.15s;
    }

    nav a:hover { color: var(--nv-accent); }

    /* Hero with diagonal composition */
    .hero {
      min-height: 85vh;
      display: flex;
      flex-direction: column;
      justify-content: center;
      padding: 6rem 3rem;
      position: relative;
      overflow: hidden;
    }

    /* Diagonal line accent across hero */
    .hero::before {
      content: '';
      position: absolute;
      top: 0;
      left: -20%;
      width: 140%;
      height: 2px;
      background: var(--nv-accent);
      transform: rotate(-45deg);
      transform-origin: top left;
      opacity: 0.5;
      box-shadow: 0 0 12px var(--nv-accent-dim);
    }

    /* Diagonal stripe pattern */
    .hero::after {
      content: '';
      position: absolute;
      inset: 0;
      background: repeating-linear-gradient(
        45deg,
        transparent,
        transparent 40px,
        rgba(255, 255, 255, 0.015) 40px,
        rgba(255, 255, 255, 0.015) 42px
      );
      pointer-events: none;
    }

    .hero h1 {
      font-family: 'Orbitron', sans-serif;
      font-size: clamp(3rem, 9vw, 8rem);
      font-weight: 900;
      letter-spacing: -0.02em;
      line-height: 0.9;
      text-transform: uppercase;
      position: relative;
      z-index: 1;
    }

    .hero h1 .accent { color: var(--nv-accent); }

    .hero p {
      margin-top: 1.5rem;
      color: var(--nv-mid-gray);
      font-size: 0.9rem;
      letter-spacing: 0.1em;
      text-transform: uppercase;
      font-family: 'Rajdhani', sans-serif;
      position: relative;
      z-index: 1;
    }

    /* Decorative data tag */
    .data-tag {
      font-family: 'Share Tech Mono', monospace;
      font-size: 0.6rem;
      color: var(--nv-accent);
      opacity: 0.5;
      letter-spacing: 0.08em;
    }

    /* TM symbol decoration */
    .tm::after {
      content: '\2122';
      font-size: 0.45em;
      vertical-align: super;
      opacity: 0.6;
      margin-left: 0.1em;
    }

    /* Diagonal section divider */
    .divider {
      height: 80px;
      background: var(--nv-black);
      clip-path: polygon(0 0, 100% 100%, 100% 100%, 0 100%);
      position: relative;
    }

    .divider::after {
      content: '';
      position: absolute;
      bottom: 0;
      left: 0;
      right: 0;
      height: 2px;
      background: var(--nv-white);
    }

    /* Content section */
    section {
      padding: 5rem 3rem;
      max-width: 1100px;
      margin: 0 auto;
      position: relative;
    }

    /* Brutalist card with offset shadow */
    .card {
      background: var(--nv-surface);
      border: 3px solid var(--nv-white);
      padding: 2.5rem;
      position: relative;
      box-shadow: 6px 6px 0 var(--nv-white);
      margin-bottom: 2rem;
    }

    .card h3 {
      margin-bottom: 0.75rem;
    }

    .card p {
      color: var(--nv-mid-gray);
      font-size: 0.9rem;
    }

    /* Accent corner mark */
    .card::before {
      content: '';
      position: absolute;
      top: 0;
      right: 0;
      width: 18px;
      height: 18px;
      background: var(--nv-accent);
      clip-path: polygon(0 0, 100% 0, 100% 100%);
    }

    /* Skewed button */
    .btn {
      display: inline-block;
      padding: 0.8rem 2.5rem;
      border: 3px solid var(--nv-white);
      background: transparent;
      color: var(--nv-white);
      font-family: 'Chakra Petch', sans-serif;
      font-size: 0.85rem;
      font-weight: 700;
      letter-spacing: 0.15em;
      text-transform: uppercase;
      text-decoration: none;
      transform: skewX(-8deg);
      transition: all 0.15s;
      cursor: pointer;
    }

    .btn:hover {
      background: var(--nv-accent);
      border-color: var(--nv-accent);
      color: var(--nv-black);
    }

    /* Vector shape decoration */
    .vector-shape {
      position: fixed;
      pointer-events: none;
      z-index: 0;
    }

    .vector-shape--chevron {
      width: 120px;
      height: 120px;
      clip-path: polygon(0 0, 50% 0, 100% 50%, 50% 100%, 0 100%, 50% 50%);
      background: var(--nv-white);
      opacity: 0.03;
      top: 20%;
      right: 5%;
      transform: rotate(45deg);
    }

    .vector-shape--triangle {
      width: 0;
      height: 0;
      border-left: 60px solid transparent;
      border-right: 60px solid transparent;
      border-bottom: 100px solid var(--nv-accent);
      opacity: 0.06;
      bottom: 15%;
      left: 3%;
      transform: rotate(-15deg);
    }

    /* Footer */
    footer {
      border-top: 2px solid var(--nv-white);
      padding: 2rem 2.5rem;
      display: flex;
      justify-content: space-between;
      align-items: center;
    }

    footer p {
      font-family: 'Rajdhani', sans-serif;
      font-size: 0.75rem;
      letter-spacing: 0.15em;
      text-transform: uppercase;
      color: var(--nv-gray);
    }

    @media (max-width: 768px) {
      .hero { padding: 4rem 1.5rem; }
      section { padding: 3rem 1.5rem; }
      nav { padding: 1rem 1.5rem; }
      .card { box-shadow: 4px 4px 0 var(--nv-white); }
    }
  </style>
</head>
<body>
  <!-- Decorative vector shapes -->
  <div class="vector-shape vector-shape--chevron"></div>
  <div class="vector-shape vector-shape--triangle"></div>

  <nav>
    <span class="brand">VECTOR<span>//</span>SYS</span>
    <a href="#">ABOUT</a>
  </nav>

  <section class="hero">
    <span class="data-tag">NEO-VH // 2024.REV.03</span>
    <h1>DESIGN<br><span class="accent">VECTOR</span><br>FORWARD<span class="tm"></span></h1>
    <p>Angular precision meets gamer-grunge maximalism</p>
    <div style="margin-top: 2rem; position: relative; z-index: 1;">
      <a href="#" class="btn">ENGAGE</a>
    </div>
  </section>

  <section>
    <div class="card">
      <span class="data-tag" style="display: block; margin-bottom: 1rem;">MODULE :: 001</span>
      <h3>DIAGONAL ENERGY</h3>
      <p>45-degree and 60-degree lines define every composition. Sharp, angular, vectorized -- never soft, never curved.</p>
    </div>

    <div class="card">
      <span class="data-tag" style="display: block; margin-bottom: 1rem;">MODULE :: 002</span>
      <h3>MONO + ACCENT</h3>
      <p>Black and white dominate. Color is an event -- a single vivid accent deployed with surgical precision.</p>
    </div>
  </section>

  <footer>
    <p>NEO-VECTORHEART &copy; 2024</p>
    <span class="data-tag">SYS.STATUS // ACTIVE</span>
  </footer>
</body>
</html>
```
