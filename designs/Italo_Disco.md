# Italo Disco Design Reference

Italo Disco is a music genre and associated visual aesthetic that originated in Italy in the late 1970s and peaked during the mid-1980s. Its visual identity is **futuristic, romantic, and often unabashedly campy**, presenting a **polished, aspirational, and often surreal fantasy world**. The aesthetic is defined by soft **airbrushed illustration**, **neon-lit cityscapes**, **chrome and metallic surfaces**, **laser grids**, and **glamorous figures** in stylized sci-fi settings. It combines **romantic melancholy** with **futuristic wonder**, filtered through a distinctly European sensibility -- escapist, sincere, and unapologetically kitsch.

---

## Visual Characteristics

### Core Motifs and Patterns

- **Soft airbrushed illustration** -- dreamy, hyper-real quality inspired by 12-inch vinyl sleeve artwork by artists like Giampaolo Cecchini
- **Neon lights and neon-lit cityscapes** -- glowing urban skylines, illuminated signage, electric horizons
- **Laser grids and geometric patterns** -- perspective grids receding into infinity, wireframe landscapes, grid floors
- **Chrome and metallic surfaces** -- reflective silver elements, polished metal textures, gleaming accents
- **Cosmic and space backgrounds** -- starfields, nebulae, planetary horizons, deep space gradients
- **Palm trees and tropical elements** -- exotic, escapist landscape motifs silhouetted against sunset skies
- **Glamorous fashion figures** -- elegantly dressed, often melancholic characters in stylized poses
- **Sci-fi machinery** -- robots, futuristic vehicles, space stations, synthesizers rendered in airbrush
- **Sunset and sunrise gradients** -- warm-to-cool transitions across dramatic skies
- **Bold, high-contrast color schemes** -- vivid neons against deep darks

### Design Principles

- **Escapism-driven design philosophy** -- every element transports the viewer to an idealized, fantastical world
- **Romantic sincerity paired with kitsch sensibility** -- glamour is earnest, not ironic
- **Retrofuturistic optimism** -- the future imagined through 1980s European eyes, full of wonder
- **High contrast and saturation** -- bold neons against dark or deep-toned backgrounds
- **Airbrushed smoothness** -- soft gradients, no hard edges, everything blends and glows
- **Layered atmospheric depth** -- foreground figures, midground architecture, background cosmos
- **Centered, symmetrical hero compositions** -- figures and focal elements dominate the center
- **Blend of high fashion and science fiction** -- couture meets cosmos
- **Melancholic grandeur** -- beauty tinged with wistfulness and longing

---

## Color Palette

### Primary Scheme

| Role | Colors |
|------|--------|
| **Background** | Deep midnight blue, black, dark purple |
| **Primary neon accents** | Hot magenta/pink, electric cyan, vivid violet |
| **Warm accents** | Neon orange, sunset gold, coral pink |
| **Metallic elements** | Chrome silver, polished gold, brushed steel |
| **Atmospheric** | Soft lavender, pale turquoise, dusky rose |

### Detailed Palette

| Color | Hex | Usage |
|-------|-----|-------|
| Midnight Black | `#0A0A14` | Deep backgrounds, space voids |
| Cosmic Navy | `#0D0B2E` | Primary dark background, night sky base |
| Deep Purple | `#1A0533` | Secondary background, depth layering |
| Hot Magenta | `#FF2975` | Primary neon accent, highlights, glows |
| Electric Cyan | `#00E5FF` | Laser grids, neon outlines, tech elements |
| Vivid Violet | `#8C1EFF` | Secondary neon accent, cosmic elements |
| Neon Orange | `#FF901F` | Sunset accents, warm neon highlights |
| Sunset Gold | `#FFD319` | Golden hour glow, luxury accents |
| Coral Pink | `#FF6B8A` | Romantic elements, soft neon warmth |
| Soft Lavender | `#C4A1FF` | Atmospheric haze, airbrushed transitions |
| Pale Turquoise | `#6DF1D8` | Cool atmospheric glow, secondary neon |
| Chrome Silver | `#C0C0C0` | Metallic surfaces, chrome text |
| Bright Chrome | `#E8E8E8` | Metallic highlights, reflective peaks |
| Dusky Rose | `#B8506E` | Muted romantic accent, figure elements |
| Palm Silhouette | `#1B0A2E` | Tropical silhouettes against gradients |

### Suggested CSS Custom Properties

```css
:root {
  /* Deep backgrounds */
  --italo-black: #0a0a14;
  --italo-navy: #0d0b2e;
  --italo-purple-deep: #1a0533;
  --italo-purple-dark: #2a0845;

  /* Neon accents */
  --italo-magenta: #ff2975;
  --italo-cyan: #00e5ff;
  --italo-violet: #8c1eff;
  --italo-orange: #ff901f;
  --italo-gold: #ffd319;
  --italo-coral: #ff6b8a;

  /* Atmospheric tones */
  --italo-lavender: #c4a1ff;
  --italo-turquoise: #6df1d8;
  --italo-rose: #b8506e;
  --italo-sky: #5c2c6d;

  /* Metallics */
  --italo-chrome: #c0c0c0;
  --italo-chrome-bright: #e8e8e8;
  --italo-chrome-dark: #808080;
  --italo-gold-metallic: #d4a843;

  /* Neon glows (for box-shadow / text-shadow) */
  --italo-glow-magenta: rgba(255, 41, 117, 0.6);
  --italo-glow-cyan: rgba(0, 229, 255, 0.6);
  --italo-glow-violet: rgba(140, 30, 255, 0.5);
  --italo-glow-orange: rgba(255, 144, 31, 0.5);

  /* Functional mappings */
  --italo-bg-primary: var(--italo-navy);
  --italo-bg-secondary: var(--italo-purple-deep);
  --italo-bg-surface: var(--italo-purple-dark);
  --italo-text-primary: var(--italo-chrome-bright);
  --italo-text-secondary: var(--italo-lavender);
  --italo-accent-primary: var(--italo-magenta);
  --italo-accent-secondary: var(--italo-cyan);
  --italo-border: rgba(140, 30, 255, 0.3);
}
```

### Approaches

- **Dark-to-vivid contrast** -- deep navy/purple backgrounds with neon accents that pop aggressively
- **Sunset gradient sweeps** -- gold to magenta to violet to navy horizontal or diagonal gradients
- **Neon-on-dark** -- bright line elements and text glowing against near-black backgrounds
- **Chrome metallic accents** -- silver and gold gradients for text and decorative elements
- **Atmospheric color layering** -- soft lavender and turquoise washes creating depth and haze
- **Complementary neon pairing** -- magenta + cyan as the iconic dual-neon combination

---

## Typography

### Typeface Characteristics

Italo Disco typography combines several distinct modes drawn from its vinyl cover art heritage:

- **Bold, condensed sans-serifs** -- high-impact display type for titles (Futura Extra Bold Condensed was used on original covers)
- **Flowing script and brush typefaces** -- romantic, cursive lettering for artist names and subtitles (Brush Script appeared on original covers)
- **Geometric display fonts** -- clean, futuristic letterforms for technological/space themes
- **Extended and wide-set tracking** -- airy, aspirational spacing on headlines
- **Metallic and neon text effects** -- chrome gradients, glowing outlines, and neon tube styling
- **Italic and oblique variants** -- conveying speed, movement, and dynamism
- **Mixed case with dramatic sizing** -- large display text paired with delicate secondary type
- **ALL CAPS for impact** -- display headlines shouting with disco energy

### Recommended Web Fonts (Google Fonts)

| Font | Style | Usage |
|------|-------|-------|
| **Syncopate** | Wide, geometric, uppercase-feeling | Primary headlines, hero display |
| **Orbitron** | Geometric, square, futuristic | Futuristic/tech headings, numbers |
| **Righteous** | Rounded, retro, display | Section titles, warm retro feel |
| **Pacifico** | Flowing script, brush-like | Romantic accents, script overlays |
| **Dancing Script** | Elegant cursive | Artist-name-style script elements |
| **Montserrat** | Geometric sans, versatile | Subheadings, UI text |
| **Jost** | Geometric, Futura-inspired | Body text, clean headlines |
| **Inter** | Clean, neutral, modern | Body text, readability |
| **Oswald** | Condensed, bold sans | Bold condensed headlines |
| **Exo 2** | Geometric, futuristic sans | Tech-themed headings, labels |

### Typography CSS Example

```css
/* Hero / Display headlines -- big, bold, neon-glowing */
.italo-display {
  font-family: 'Syncopate', 'Orbitron', sans-serif;
  font-size: clamp(2.5rem, 7vw, 6rem);
  font-weight: 700;
  letter-spacing: 0.12em;
  text-transform: uppercase;
  line-height: 1.1;
  color: var(--italo-chrome-bright);
  text-shadow:
    0 0 10px var(--italo-glow-magenta),
    0 0 40px var(--italo-glow-magenta),
    0 0 80px rgba(255, 41, 117, 0.3);
}

/* Section headlines */
h1, h2, h3 {
  font-family: 'Righteous', 'Jost', sans-serif;
  font-weight: 400;
  letter-spacing: 0.06em;
  color: var(--italo-chrome-bright);
}

/* Script / romantic accent text */
.italo-script {
  font-family: 'Pacifico', 'Dancing Script', cursive;
  font-size: clamp(1.5rem, 4vw, 3rem);
  font-weight: 400;
  font-style: normal;
  color: var(--italo-coral);
  text-shadow:
    0 0 8px var(--italo-glow-magenta),
    0 0 20px rgba(255, 107, 138, 0.3);
}

/* Body text */
body {
  font-family: 'Inter', 'Jost', sans-serif;
  font-weight: 300;
  letter-spacing: 0.02em;
  line-height: 1.7;
  color: var(--italo-text-secondary);
}

/* Chrome metallic text effect */
.italo-chrome-text {
  font-family: 'Oswald', 'Montserrat', sans-serif;
  font-weight: 700;
  letter-spacing: 0.08em;
  text-transform: uppercase;
  background: linear-gradient(
    180deg,
    #ffffff 0%,
    #e8e8e8 25%,
    #808080 50%,
    #c0c0c0 75%,
    #ffffff 100%
  );
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  background-clip: text;
}

/* Small technical/label text */
.italo-label {
  font-family: 'Exo 2', 'Montserrat', sans-serif;
  font-size: 0.75rem;
  text-transform: uppercase;
  letter-spacing: 0.25em;
  color: var(--italo-cyan);
  text-shadow: 0 0 6px var(--italo-glow-cyan);
}
```

---

## Layout Principles

### Grid and Structure

- **Full-bleed hero sections** -- dramatic, edge-to-edge visuals dominating above the fold
- **Centered, symmetrical compositions** -- content gravitates to center axis, mirroring album cover layouts
- **Generous vertical spacing** -- sections breathe with ample padding, evoking open cosmic spaces
- **Wide aspect ratios** -- landscape-oriented sections referencing widescreen cinematic framing
- **Layered parallax depth** -- background starfields, midground grids, foreground content create z-depth
- **Diagonal and angular dividers** -- slanted section breaks adding dynamism and movement
- **Grid floors / perspective grids** -- laser-grid elements as decorative section backgrounds

### Section Organization

- Use **neon gradient dividers** between sections (magenta-to-cyan fading lines)
- Apply **atmospheric background gradients** that shift color as user scrolls (navy to purple to deep black)
- Create **hierarchy through glow intensity** -- brighter neon glow = more important element
- Employ **card/panel layouts with neon borders** -- content contained in softly glowing frames
- Use **large typographic headers** -- oversized display text as section anchors
- Overlay **decorative grid patterns** at low opacity behind content sections
- Place **palm tree or cityscape silhouettes** as decorative section edges

### Responsive Considerations

- Hero display text scales fluidly with `clamp()` -- dramatic on desktop, still bold on mobile
- Neon glow effects can be reduced on mobile for performance (fewer shadow layers)
- Laser grid backgrounds can simplify to solid gradients on small screens
- Maintain generous padding -- the spacious, cosmic feel should not be lost at any breakpoint

---

## CSS/Design Techniques

### Neon Glow Text Effect

```css
/* Hot magenta neon text */
.neon-magenta {
  color: var(--italo-magenta);
  text-shadow:
    0 0 7px var(--italo-magenta),
    0 0 10px var(--italo-magenta),
    0 0 21px var(--italo-magenta),
    0 0 42px rgba(255, 41, 117, 0.5),
    0 0 82px rgba(255, 41, 117, 0.3),
    0 0 92px rgba(255, 41, 117, 0.2);
}

/* Electric cyan neon text */
.neon-cyan {
  color: var(--italo-cyan);
  text-shadow:
    0 0 7px var(--italo-cyan),
    0 0 10px var(--italo-cyan),
    0 0 21px var(--italo-cyan),
    0 0 42px rgba(0, 229, 255, 0.5),
    0 0 82px rgba(0, 229, 255, 0.3),
    0 0 92px rgba(0, 229, 255, 0.2);
}

/* Flickering neon animation */
@keyframes neon-flicker {
  0%, 19%, 21%, 23%, 25%, 54%, 56%, 100% {
    text-shadow:
      0 0 7px var(--italo-magenta),
      0 0 10px var(--italo-magenta),
      0 0 21px var(--italo-magenta),
      0 0 42px rgba(255, 41, 117, 0.5),
      0 0 82px rgba(255, 41, 117, 0.3);
  }
  20%, 24%, 55% {
    text-shadow: none;
  }
}

.neon-flicker {
  animation: neon-flicker 3s infinite alternate;
}
```

### Sunset Gradient Background

```css
/* Classic Italo Disco sunset sky */
.italo-sunset {
  background: linear-gradient(
    180deg,
    #0d0b2e 0%,       /* cosmic navy top */
    #1a0533 15%,       /* deep purple */
    #5c2c6d 30%,       /* dusky violet */
    #b8506e 45%,       /* rose horizon */
    #ff6b8a 55%,       /* coral pink band */
    #ff901f 65%,       /* neon orange glow */
    #ffd319 75%,       /* golden sun */
    #ff2975 85%,       /* magenta lower glow */
    #1a0533 100%       /* fade to deep */
  );
}

/* Simplified two-tone gradient for sections */
.italo-gradient-section {
  background: linear-gradient(
    135deg,
    var(--italo-navy) 0%,
    var(--italo-purple-deep) 50%,
    var(--italo-purple-dark) 100%
  );
}
```

### Laser Grid / Perspective Floor

```css
/* Perspective laser grid (classic 80s floor effect) */
.laser-grid {
  position: relative;
  overflow: hidden;
}

.laser-grid::after {
  content: '';
  position: absolute;
  bottom: 0;
  left: -50%;
  right: -50%;
  height: 50%;
  background:
    linear-gradient(
      rgba(0, 229, 255, 0.15) 1px,
      transparent 1px
    ),
    linear-gradient(
      90deg,
      rgba(0, 229, 255, 0.15) 1px,
      transparent 1px
    );
  background-size: 60px 40px;
  transform: perspective(400px) rotateX(60deg);
  transform-origin: bottom center;
  mask-image: linear-gradient(to top, rgba(0, 0, 0, 0.8), transparent);
  -webkit-mask-image: linear-gradient(to top, rgba(0, 0, 0, 0.8), transparent);
  pointer-events: none;
}
```

### Neon Border Card / Panel

```css
.italo-card {
  background: rgba(13, 11, 46, 0.85);
  border: 1px solid rgba(140, 30, 255, 0.3);
  border-radius: 4px;
  padding: 2.5rem;
  position: relative;
  overflow: hidden;
  box-shadow:
    0 0 15px rgba(140, 30, 255, 0.15),
    inset 0 0 30px rgba(13, 11, 46, 0.5);
  backdrop-filter: blur(10px);
}

/* Neon top-edge highlight */
.italo-card::before {
  content: '';
  position: absolute;
  top: 0;
  left: 5%;
  right: 5%;
  height: 1px;
  background: linear-gradient(
    90deg,
    transparent,
    var(--italo-magenta) 30%,
    var(--italo-cyan) 70%,
    transparent
  );
  box-shadow: 0 0 10px var(--italo-glow-magenta);
}

/* Hover glow intensification */
.italo-card:hover {
  border-color: rgba(255, 41, 117, 0.5);
  box-shadow:
    0 0 20px rgba(255, 41, 117, 0.2),
    0 0 40px rgba(140, 30, 255, 0.1),
    inset 0 0 30px rgba(13, 11, 46, 0.5);
  transition: all 0.4s ease;
}
```

### Chrome Metallic Gradient Effect

```css
/* Chrome text for display headings */
.italo-chrome-display {
  background: linear-gradient(
    180deg,
    #ffffff 0%,
    #e8e8e8 20%,
    #808080 45%,
    #b0b0b0 55%,
    #e0e0e0 80%,
    #ffffff 100%
  );
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  background-clip: text;
  filter: drop-shadow(0 2px 4px rgba(0, 0, 0, 0.5));
}

/* Gold metallic variant */
.italo-gold-display {
  background: linear-gradient(
    180deg,
    #ffd700 0%,
    #d4a843 30%,
    #8b6914 50%,
    #d4a843 70%,
    #ffd700 100%
  );
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  background-clip: text;
}
```

### Airbrushed Glow / Soft Light Effect

```css
/* Airbrushed radial glow -- place behind hero elements */
.airbrush-glow {
  position: absolute;
  width: 400px;
  height: 400px;
  border-radius: 50%;
  background: radial-gradient(
    circle,
    rgba(255, 41, 117, 0.3) 0%,
    rgba(140, 30, 255, 0.15) 40%,
    transparent 70%
  );
  filter: blur(60px);
  pointer-events: none;
  z-index: 0;
}

/* Secondary cyan glow */
.airbrush-glow-cyan {
  background: radial-gradient(
    circle,
    rgba(0, 229, 255, 0.25) 0%,
    rgba(109, 241, 216, 0.1) 40%,
    transparent 70%
  );
  filter: blur(80px);
}
```

### Neon Line Divider

```css
/* Magenta-to-cyan gradient divider */
.italo-divider {
  width: 60%;
  margin: 3rem auto;
  border: none;
  height: 2px;
  background: linear-gradient(
    90deg,
    transparent,
    var(--italo-magenta) 20%,
    var(--italo-cyan) 80%,
    transparent
  );
  box-shadow:
    0 0 8px var(--italo-glow-magenta),
    0 0 16px rgba(0, 229, 255, 0.3);
}
```

### Palm Tree Silhouette (CSS-only Decorative)

```css
/* Palm tree silhouette decoration (positioned absolutely) */
.palm-silhouette {
  position: absolute;
  bottom: 0;
  width: 120px;
  height: 200px;
  background: var(--italo-black);
  clip-path: polygon(
    50% 0%, 30% 15%, 5% 10%, 25% 25%, 0% 30%,
    20% 35%, 10% 45%, 30% 42%, 25% 55%, 38% 48%,
    45% 100%, 55% 100%, 62% 48%, 75% 55%, 70% 42%,
    90% 45%, 80% 35%, 100% 30%, 75% 25%, 95% 10%,
    70% 15%, 50% 0%
  );
  opacity: 0.6;
}
```

### Starfield Background Animation

```css
/* Twinkling starfield */
@keyframes twinkle {
  0%, 100% { opacity: 0.3; }
  50% { opacity: 1; }
}

.starfield {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  pointer-events: none;
  z-index: 0;
  background:
    radial-gradient(1px 1px at 10% 20%, rgba(255, 255, 255, 0.8), transparent),
    radial-gradient(1px 1px at 30% 60%, rgba(255, 255, 255, 0.6), transparent),
    radial-gradient(1px 1px at 50% 10%, rgba(255, 255, 255, 0.9), transparent),
    radial-gradient(1px 1px at 70% 40%, rgba(255, 255, 255, 0.5), transparent),
    radial-gradient(1px 1px at 85% 75%, rgba(255, 255, 255, 0.7), transparent),
    radial-gradient(1px 1px at 20% 80%, rgba(255, 255, 255, 0.4), transparent),
    radial-gradient(1px 1px at 60% 90%, rgba(255, 255, 255, 0.6), transparent),
    radial-gradient(1.5px 1.5px at 40% 35%, rgba(200, 180, 255, 0.8), transparent),
    radial-gradient(1.5px 1.5px at 90% 15%, rgba(180, 220, 255, 0.7), transparent);
  animation: twinkle 4s ease-in-out infinite alternate;
}
```

### Neon Button

```css
.italo-button {
  display: inline-block;
  padding: 0.8rem 2.5rem;
  border: 2px solid var(--italo-magenta);
  border-radius: 2px;
  background: transparent;
  color: var(--italo-magenta);
  font-family: 'Montserrat', 'Jost', sans-serif;
  font-size: 0.85rem;
  font-weight: 600;
  letter-spacing: 0.2em;
  text-transform: uppercase;
  cursor: pointer;
  text-decoration: none;
  transition: all 0.3s ease;
  box-shadow:
    0 0 8px var(--italo-glow-magenta),
    inset 0 0 8px rgba(255, 41, 117, 0.1);
}

.italo-button:hover {
  background: var(--italo-magenta);
  color: #ffffff;
  box-shadow:
    0 0 15px var(--italo-glow-magenta),
    0 0 40px rgba(255, 41, 117, 0.3),
    inset 0 0 15px rgba(255, 255, 255, 0.1);
}

/* Cyan variant */
.italo-button--cyan {
  border-color: var(--italo-cyan);
  color: var(--italo-cyan);
  box-shadow:
    0 0 8px var(--italo-glow-cyan),
    inset 0 0 8px rgba(0, 229, 255, 0.1);
}

.italo-button--cyan:hover {
  background: var(--italo-cyan);
  color: var(--italo-black);
  box-shadow:
    0 0 15px var(--italo-glow-cyan),
    0 0 40px rgba(0, 229, 255, 0.3),
    inset 0 0 15px rgba(255, 255, 255, 0.1);
}
```

---

## Materials and Textures (Visual Metaphors for Web)

Physical Italo Disco motifs and their web equivalents:

| Physical Reference | Web Equivalent |
|-------------------|----------------|
| Neon tube signage | Text with multi-layered `text-shadow` in neon colors, optional flicker animation |
| Airbrushed illustration | Large `radial-gradient` blurs, soft color transitions, `filter: blur()` on decorative elements |
| Laser grid floor | CSS grid pattern with `perspective` transform, fading with mask-image |
| Chrome/metallic surfaces | Multi-stop `linear-gradient` on text using `background-clip: text` |
| Cosmic starfield | Multiple `radial-gradient` dots at random positions, subtle twinkle animation |
| Sunset sky | Vertical `linear-gradient` with 6-8 color stops from gold through pink to deep purple |
| Palm tree silhouette | Dark `clip-path` shapes positioned absolutely against gradient backgrounds |
| Vinyl record grooves | Concentric `repeating-radial-gradient` circles at low opacity |
| Smoke machine haze | Semi-transparent `radial-gradient` overlays with high blur, low opacity |
| Disco ball reflections | Small bright dots scattered via `radial-gradient`, gentle animation |

---

## Imagery and Photography Guidelines

When sourcing or creating imagery for an Italo Disco styled site:

- **Favor airbrushed or digitally smoothed illustrations** over raw photography
- **Apply heavy color grading** to any photographs -- push toward magenta/cyan split-toning
- **Use silhouettes** of cityscapes, palm trees, and figures against gradient skies
- **Add lens flare and light leak effects** for authenticity
- **Feature geometric wireframe elements** layered over images
- **Incorporate retro-futuristic subjects** -- synthesizers, sports cars, skylines, space imagery
- **Keep human figures stylized** -- glamorous, fashion-forward, slightly idealized
- **Avoid stark realism** -- everything should feel slightly dreamlike and polished

---

## Related Aesthetics

| Aesthetic | Relationship to Italo Disco |
|-----------|----------------------------|
| **Disco** | Direct parent genre; Italo Disco inherits the glamour and dancefloor energy |
| **Synthwave** | Modern descendant; reinterprets Italo Disco visuals with contemporary tools |
| **Vaporwave** | Samples and recontextualizes Italo Disco's melodic synthetic qualities, more ironic |
| **Laser Grid** | Shares the perspective grid motif; more focused on the single visual element |
| **New Wave** | Contemporary movement; shares neon, angular design, and synth culture |
| **Paninaro** | Italian subcultural style overlapping with Italo Disco's fashion sensibility |
| **Retrofuturism** | Broader parent category encompassing the future-as-imagined-in-the-past motif |
| **Chromecore** | Shares metallic/chrome elements, though rooted in 2000s rather than 1980s |

---

## Quick-Start: Minimal Italo Disco Page Template

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Italo Disco Page</title>
  <link href="https://fonts.googleapis.com/css2?family=Syncopate:wght@400;700&family=Righteous&family=Pacifico&family=Inter:wght@300;400&family=Montserrat:wght@400;600&display=swap" rel="stylesheet">
  <style>
    :root {
      --italo-black: #0a0a14;
      --italo-navy: #0d0b2e;
      --italo-purple-deep: #1a0533;
      --italo-magenta: #ff2975;
      --italo-cyan: #00e5ff;
      --italo-violet: #8c1eff;
      --italo-coral: #ff6b8a;
      --italo-lavender: #c4a1ff;
      --italo-chrome-bright: #e8e8e8;
      --italo-glow-magenta: rgba(255, 41, 117, 0.6);
      --italo-glow-cyan: rgba(0, 229, 255, 0.6);
    }

    * { margin: 0; padding: 0; box-sizing: border-box; }

    body {
      background: linear-gradient(180deg, var(--italo-navy) 0%, var(--italo-purple-deep) 50%, var(--italo-black) 100%);
      color: var(--italo-lavender);
      font-family: 'Inter', sans-serif;
      font-weight: 300;
      letter-spacing: 0.02em;
      line-height: 1.7;
      min-height: 100vh;
    }

    .hero {
      text-align: center;
      padding: 8rem 2rem 6rem;
      position: relative;
      overflow: hidden;
    }

    /* Airbrushed glow behind title */
    .hero::before {
      content: '';
      position: absolute;
      top: 50%;
      left: 50%;
      transform: translate(-50%, -50%);
      width: 500px;
      height: 500px;
      border-radius: 50%;
      background: radial-gradient(circle, rgba(255, 41, 117, 0.2) 0%, rgba(140, 30, 255, 0.1) 40%, transparent 70%);
      filter: blur(60px);
      pointer-events: none;
    }

    .hero h1 {
      font-family: 'Syncopate', sans-serif;
      font-size: clamp(2rem, 6vw, 5rem);
      font-weight: 700;
      letter-spacing: 0.12em;
      text-transform: uppercase;
      color: var(--italo-chrome-bright);
      text-shadow:
        0 0 10px var(--italo-glow-magenta),
        0 0 40px var(--italo-glow-magenta),
        0 0 80px rgba(255, 41, 117, 0.2);
      position: relative;
      z-index: 1;
    }

    .hero .script-subtitle {
      font-family: 'Pacifico', cursive;
      font-size: clamp(1.2rem, 3vw, 2rem);
      color: var(--italo-coral);
      margin-top: 1rem;
      text-shadow: 0 0 12px rgba(255, 107, 138, 0.4);
      position: relative;
      z-index: 1;
    }

    .italo-divider {
      width: 50%;
      margin: 3rem auto;
      border: none;
      height: 2px;
      background: linear-gradient(90deg, transparent, var(--italo-magenta) 20%, var(--italo-cyan) 80%, transparent);
      box-shadow: 0 0 8px var(--italo-glow-magenta), 0 0 16px rgba(0, 229, 255, 0.3);
    }

    section {
      max-width: 900px;
      margin: 0 auto;
      padding: 4rem 2rem;
      text-align: center;
      position: relative;
      z-index: 1;
    }

    section h2 {
      font-family: 'Righteous', sans-serif;
      font-size: 1.8rem;
      letter-spacing: 0.06em;
      color: var(--italo-cyan);
      text-shadow: 0 0 8px var(--italo-glow-cyan);
      margin-bottom: 1.5rem;
    }

    .italo-card {
      background: rgba(13, 11, 46, 0.85);
      border: 1px solid rgba(140, 30, 255, 0.3);
      border-radius: 4px;
      padding: 2.5rem;
      position: relative;
      overflow: hidden;
      box-shadow: 0 0 15px rgba(140, 30, 255, 0.15);
      backdrop-filter: blur(10px);
    }

    .italo-card::before {
      content: '';
      position: absolute;
      top: 0;
      left: 5%;
      right: 5%;
      height: 1px;
      background: linear-gradient(90deg, transparent, var(--italo-magenta) 30%, var(--italo-cyan) 70%, transparent);
    }

    .italo-button {
      display: inline-block;
      margin-top: 2rem;
      padding: 0.8rem 2.5rem;
      border: 2px solid var(--italo-magenta);
      border-radius: 2px;
      background: transparent;
      color: var(--italo-magenta);
      font-family: 'Montserrat', sans-serif;
      font-size: 0.85rem;
      font-weight: 600;
      letter-spacing: 0.2em;
      text-transform: uppercase;
      text-decoration: none;
      cursor: pointer;
      transition: all 0.3s ease;
      box-shadow: 0 0 8px var(--italo-glow-magenta), inset 0 0 8px rgba(255, 41, 117, 0.1);
    }

    .italo-button:hover {
      background: var(--italo-magenta);
      color: #ffffff;
      box-shadow: 0 0 15px var(--italo-glow-magenta), 0 0 40px rgba(255, 41, 117, 0.3);
    }
  </style>
</head>
<body>
  <div class="hero">
    <h1>Title Here</h1>
    <p class="script-subtitle">una notte magica</p>
  </div>
  <hr class="italo-divider">
  <section>
    <div class="italo-card">
      <h2>Section Heading</h2>
      <p>Content styled with the Italo Disco aesthetic -- neon glows, deep cosmic backgrounds, and romantic European flair.</p>
      <a href="#" class="italo-button">Explore</a>
    </div>
  </section>
</body>
</html>
```
