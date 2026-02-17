# Fleischer Style Design Reference

The Fleischer Style is an animation and visual aesthetic that rose to prominence in the 1920s and 1930s, developed primarily by Fleischer Studios (creators of Betty Boop, Popeye, and Koko the Clown). It is defined by **rubber hose animation**, **surreal humor**, **gritty urban settings**, **musical synchronization**, and a blend of **whimsy with dark undercurrents**. The style prioritizes expressive, physics-defying motion over anatomical realism, using simplified character construction with elastic, jointless limbs. Its visual language bridges the Jazz Age and the Great Depression, combining Art Deco elegance with vaudeville irreverence.

---

## Visual Characteristics

### Core Motifs and Design Elements

- **Rubber hose limbs** -- Fluid, boneless arms and legs drawn as smooth curves without articulated joints (elbows, knees); the defining hallmark of the style
- **Pie-cut eyes** -- Large, round eyes with a wedge-shaped pupil cut from the circle, conveying innocence and expressiveness
- **White gloves** -- Oversized four-fingered gloves on characters, used for visual contrast against dark bodies
- **Oversized shoes** -- Comically large, rounded footwear that anchors characters to the ground plane
- **Sentient objects** -- Inanimate objects (buildings, furniture, musical instruments) that come alive, stretch, dance, and express emotion
- **Visual sound effects** -- Sound rendered as visible graphic elements directly within the scene (musical notes, impact stars, squiggly lines)
- **Gritty urban backdrops** -- City streets, tenements, docks, and industrial scenes rendered with atmospheric depth
- **Surreal transformations** -- Characters and objects morphing, splitting, stretching, and reassembling in dreamlike sequences
- **Ink-and-cel aesthetic** -- Visible brushstroke quality, imperfect line weight variation, and slight registration wobble that gives the style its handmade charm
- **Film grain and flicker** -- Artifacts of early film projection: dust, scratches, vignetting, and uneven exposure

### Design Principles

- **Expressiveness over realism** -- Every element is exaggerated and caricatured for maximum emotional impact
- **Flat, theatrical composition** -- Limited use of perspective; scenes composed like a stage set with a fixed viewpoint
- **Musical rhythm in layout** -- Compositions pulse and sway; elements are arranged to suggest rhythmic movement even in static form
- **Dark whimsy** -- Cheerful cartoon aesthetics layered over unsettling, surreal, or mildly grotesque content
- **High-contrast silhouettes** -- Characters designed to read as strong black shapes against light backgrounds (or vice versa)
- **Circular and rounded forms** -- Heads, bodies, eyes, buttons, and props all trend toward circles and ovals
- **Minimal color, maximum contrast** -- Originally black and white; when color is used, it is limited and bold
- **Depth through layering** -- Inspired by the Fleischer "Stereoptical" process that layered animation over 3D miniature sets; creates a parallax-like depth effect

---

## Color Palette

### Primary Scheme (Classic Black & White)

| Role | Colors |
|------|--------|
| **Ink black** | Deep true black for outlines, character bodies, and shadows |
| **Paper white** | Bright white for backgrounds, highlights, and glove details |
| **Mid grays** | Intermediate tones for shading, depth, and atmospheric effects |

### Extended Palette (Sepia / Aged Film)

| Color | Hex | Usage |
|-------|-----|-------|
| Ink Black | `#1a1a1a` | Primary outlines, character fills, strong shadows |
| Warm Black | `#2b2520` | Softer shadows, background depth |
| Dark Sepia | `#3e3229` | Panel backgrounds, dark accents |
| Burnt Umber | `#613323` | Warm shadow tones, border accents |
| Cocoa Brown | `#6b5446` | Secondary elements, muted fills |
| Parchment | `#f5e6c8` | Primary background (aged paper feel) |
| Antique Cream | `#f5f0e1` | Light backgrounds, text areas |
| Warm White | `#faf6ed` | Highlights, bright areas |

### Accent Colors (Colorized Fleischer / Cuphead-inspired)

| Color | Hex | Usage |
|-------|-----|-------|
| Old Film Amber | `#d4a54a` | Warm highlights, decorative borders |
| Dusty Rose | `#c97b7b` | Flesh tones, warm accents |
| Salmon Pink | `#fbafa4` | Character highlights, warm glow |
| Muted Gold | `#9a8820` | Vintage accent, button highlights |
| Faded Red | `#b84a3c` | Action highlights, danger elements |
| Teal Green | `#4a7c6f` | Cool contrast, environmental accents |
| Sage | `#73a089` | Background vegetation, muted nature |
| Soft Peach | `#f5cdb4` | Skin tones, warm midtones |
| Pale Yellow | `#fddda0` | Warm light, glow effects |
| Dusty Blue | `#6b8ea6` | Sky tones, cool accents |

### Suggested CSS Custom Properties

```css
:root {
  /* Ink & Paper (core black-and-white feel) */
  --fleischer-ink: #1a1a1a;
  --fleischer-warm-black: #2b2520;
  --fleischer-dark-sepia: #3e3229;
  --fleischer-charcoal: #4a4a4a;
  --fleischer-mid-gray: #888888;
  --fleischer-parchment: #f5e6c8;
  --fleischer-cream: #f5f0e1;
  --fleischer-warm-white: #faf6ed;

  /* Sepia / Aged Film */
  --fleischer-burnt-umber: #613323;
  --fleischer-cocoa: #6b5446;
  --fleischer-amber: #d4a54a;

  /* Colorized Accents */
  --fleischer-dusty-rose: #c97b7b;
  --fleischer-salmon: #fbafa4;
  --fleischer-faded-red: #b84a3c;
  --fleischer-teal: #4a7c6f;
  --fleischer-sage: #73a089;
  --fleischer-peach: #f5cdb4;
  --fleischer-pale-yellow: #fddda0;
  --fleischer-dusty-blue: #6b8ea6;
  --fleischer-muted-gold: #9a8820;

  /* Functional */
  --fleischer-bg-primary: var(--fleischer-parchment);
  --fleischer-bg-secondary: var(--fleischer-cream);
  --fleischer-bg-dark: var(--fleischer-ink);
  --fleischer-text-primary: var(--fleischer-ink);
  --fleischer-text-on-dark: var(--fleischer-parchment);
  --fleischer-accent: var(--fleischer-faded-red);
  --fleischer-border: var(--fleischer-ink);
}
```

### Palette Approaches

- **Classic monochrome** -- Pure black, white, and grays for authentic 1930s cartoon feel
- **Sepia-tinted** -- Warm browns and cream tones evoking aged nitrate film stock
- **Limited colorization** -- Muted, desaturated accent colors as if hand-painted onto film frames (never bright or saturated)
- **High contrast ink** -- Always maintain strong black outlines regardless of color scheme

---

## Typography

### Typeface Characteristics

Fleischer-era typography features:

- **Hand-lettered quality** -- Slightly irregular, as if drawn by an animator's brush or pen
- **Rounded, friendly letterforms** -- Matching the circular character design philosophy
- **Bold outlines** -- Letters often have visible stroke outlines, like cartoon characters themselves
- **Art Deco influence** -- Geometric construction with decorative flair, reflecting the era
- **Condensed display faces** -- Title cards use tall, narrow, attention-grabbing lettering
- **Bouncy baseline** -- Letters that sit unevenly, suggesting movement and rhythm
- **ALL CAPS for titles** -- Headlines and title cards rendered in uppercase with wide letter-spacing

### Recommended Web Fonts (Google Fonts)

| Font | Style | Usage |
|------|-------|-------|
| **Creepster** | Playful, cartoon horror | Feature titles, spooky/whimsical headers |
| **Bungee** | Bold, chunky display | Hero headlines, large titles |
| **Bungee Shade** | 3D shadow effect display | Decorative headers with retro depth |
| **Fascinate Inline** | Art Deco inline detailing | Elegant display text, section headers |
| **Poiret One** | Geometric, thin, elegant | Subheadings with Art Deco flavor |
| **Josefin Sans** | Geometric vintage sans | Subheadings, UI text |
| **Limelight** | 1920s Art Deco display | Large display headlines |
| **Special Elite** | Typewriter / hand-stamped | Body text with vintage feel |
| **Fredoka** | Rounded, friendly sans | Body text, approachable content |
| **Abril Fatface** | Bold Didone display | Pull quotes, statement text |

### Typography CSS Example

```css
/* Import fonts */
@import url('https://fonts.googleapis.com/css2?family=Bungee+Shade&family=Josefin+Sans:wght@300;400;600&family=Special+Elite&family=Fredoka:wght@300;400;500;600&display=swap');

/* Title card / Hero text */
.fleischer-title {
  font-family: 'Bungee Shade', 'Bungee', cursive;
  font-size: clamp(2.5rem, 7vw, 6rem);
  letter-spacing: 0.08em;
  line-height: 1.1;
  color: var(--fleischer-ink);
  text-align: center;
  text-shadow:
    3px 3px 0 var(--fleischer-amber),
    -1px -1px 0 var(--fleischer-charcoal);
}

/* Section headings */
h1, h2, h3 {
  font-family: 'Josefin Sans', sans-serif;
  text-transform: uppercase;
  letter-spacing: 0.12em;
  color: var(--fleischer-ink);
  font-weight: 600;
}

/* Body text */
body {
  font-family: 'Fredoka', 'Josefin Sans', sans-serif;
  font-weight: 400;
  letter-spacing: 0.02em;
  line-height: 1.7;
  color: var(--fleischer-ink);
}

/* Narrative / caption text (typewriter feel) */
.fleischer-caption {
  font-family: 'Special Elite', cursive;
  font-size: 1.1rem;
  letter-spacing: 0.04em;
  line-height: 1.6;
}
```

---

## Layout Principles

### Grid and Structure

- **Stage-like composition** -- Treat the viewport as a theater stage; content is centered with a clear "performance area"
- **Flat layered planes** -- Foreground, midground, and background as distinct horizontal layers (parallax scrolling is a natural fit)
- **Centered, single-column flow** -- Content stacks vertically along a central axis, like animation cels on a timeline
- **Generous padding and borders** -- Thick black outlines around content areas echo the ink-heavy cartoon aesthetic
- **Rounded containers** -- Panels and cards use border-radius to match the rounded character design language
- **Vignette framing** -- Content areas darken or fade at the edges, evoking the projected-film look

### Section Organization

- Use **thick ink-line dividers** between sections (3-5px solid black rules)
- Apply **film-frame borders** around key content (double-line or dashed borders suggesting sprocket holes)
- Create **title cards** as full-width interstitial sections between content (mimicking intertitles from silent film)
- Employ **circular and oval frames** for images and character portraits
- Use **slight rotation or skew** on elements to suggest hand-drawn imprecision

---

## CSS/Design Techniques

### Film Grain Overlay

```css
/* Animated film grain noise overlay */
.fleischer-grain::after {
  content: '';
  position: fixed;
  inset: 0;
  pointer-events: none;
  z-index: 9999;
  opacity: 0.06;
  background-image: url("data:image/svg+xml,%3Csvg viewBox='0 0 256 256' xmlns='http://www.w3.org/2000/svg'%3E%3Cfilter id='noise'%3E%3CfeTurbulence type='fractalNoise' baseFrequency='0.9' numOctaves='4' stitchTiles='stitch'/%3E%3C/filter%3E%3Crect width='100%25' height='100%25' filter='url(%23noise)'/%3E%3C/svg%3E");
  background-size: 256px 256px;
  mix-blend-mode: multiply;
  animation: fleischer-grain-shift 0.3s steps(4) infinite;
}

@keyframes fleischer-grain-shift {
  0% { transform: translate(0, 0); }
  25% { transform: translate(-2px, 1px); }
  50% { transform: translate(1px, -2px); }
  75% { transform: translate(-1px, 2px); }
  100% { transform: translate(2px, -1px); }
}
```

### Vignette Effect

```css
/* Dark vignette edges like an old film projector */
.fleischer-vignette::before {
  content: '';
  position: fixed;
  inset: 0;
  pointer-events: none;
  z-index: 9998;
  background: radial-gradient(
    ellipse at center,
    transparent 50%,
    rgba(26, 26, 26, 0.4) 100%
  );
}
```

### Thick Ink Outline Borders

```css
/* Cartoon-style thick ink outlines on containers */
.fleischer-panel {
  background: var(--fleischer-cream);
  border: 4px solid var(--fleischer-ink);
  border-radius: 16px;
  padding: 2rem;
  position: relative;
  box-shadow: 6px 6px 0 var(--fleischer-ink);
}

/* Double-outline effect for emphasis */
.fleischer-panel-double {
  background: var(--fleischer-cream);
  border: 4px solid var(--fleischer-ink);
  border-radius: 16px;
  padding: 2rem;
  outline: 2px solid var(--fleischer-ink);
  outline-offset: 4px;
  border-radius: 18px;
}
```

### Rubber Hose Divider (SVG via CSS)

```css
/* Wavy, rubber-hose-style section divider */
.fleischer-divider {
  width: 100%;
  height: 40px;
  background: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 800 40'%3E%3Cpath d='M0 20 Q100 0 200 20 Q300 40 400 20 Q500 0 600 20 Q700 40 800 20' fill='none' stroke='%231a1a1a' stroke-width='4' stroke-linecap='round'/%3E%3C/svg%3E") no-repeat center;
  background-size: 100% 100%;
  margin: 2rem 0;
}
```

### Title Card (Silent Film Intertitle)

```css
/* Full-width interstitial title card */
.fleischer-title-card {
  background: var(--fleischer-ink);
  color: var(--fleischer-parchment);
  text-align: center;
  padding: 4rem 2rem;
  border-top: 6px solid var(--fleischer-charcoal);
  border-bottom: 6px solid var(--fleischer-charcoal);
  position: relative;
}

.fleischer-title-card h2 {
  font-family: 'Bungee Shade', cursive;
  font-size: clamp(2rem, 5vw, 4rem);
  letter-spacing: 0.1em;
  color: var(--fleischer-parchment);
  text-shadow: 2px 2px 0 var(--fleischer-amber);
}

/* Decorative corner brackets */
.fleischer-title-card::before,
.fleischer-title-card::after {
  content: '';
  position: absolute;
  width: 40px;
  height: 40px;
  border-color: var(--fleischer-parchment);
  border-style: solid;
}
.fleischer-title-card::before {
  top: 16px; left: 16px;
  border-width: 3px 0 0 3px;
}
.fleischer-title-card::after {
  bottom: 16px; right: 16px;
  border-width: 0 3px 3px 0;
}
```

### Pie-Cut Eye Decorative Element

```css
/* Iconic pie-eye as a decorative CSS element */
.fleischer-pie-eye {
  width: 60px;
  height: 60px;
  background: var(--fleischer-warm-white);
  border: 4px solid var(--fleischer-ink);
  border-radius: 50%;
  position: relative;
  display: inline-block;
}

.fleischer-pie-eye::after {
  content: '';
  position: absolute;
  top: 50%;
  left: 50%;
  width: 24px;
  height: 24px;
  background: var(--fleischer-ink);
  border-radius: 50%;
  transform: translate(-50%, -50%);
  /* Pie-cut highlight */
  box-shadow: -3px -3px 0 2px var(--fleischer-warm-white);
}
```

### Bouncy Animation (Squash & Stretch)

```css
/* Rubber hose bounce animation for interactive elements */
@keyframes fleischer-bounce {
  0%, 100% {
    transform: scaleY(1) scaleX(1);
  }
  30% {
    transform: scaleY(0.85) scaleX(1.1);
  }
  50% {
    transform: scaleY(1.15) scaleX(0.9);
  }
  70% {
    transform: scaleY(0.95) scaleX(1.03);
  }
}

.fleischer-bounce:hover {
  animation: fleischer-bounce 0.6s ease-in-out;
  transform-origin: bottom center;
}

/* Wobble for idle animation */
@keyframes fleischer-wobble {
  0%, 100% { transform: rotate(0deg); }
  25% { transform: rotate(-2deg); }
  75% { transform: rotate(2deg); }
}

.fleischer-wobble {
  animation: fleischer-wobble 3s ease-in-out infinite;
}
```

### Sepia / Aged Paper Background

```css
/* Aged paper texture background */
.fleischer-aged-bg {
  background-color: var(--fleischer-parchment);
  background-image:
    radial-gradient(
      ellipse at 20% 50%,
      rgba(97, 51, 35, 0.08) 0%,
      transparent 50%
    ),
    radial-gradient(
      ellipse at 80% 20%,
      rgba(97, 51, 35, 0.05) 0%,
      transparent 40%
    ),
    radial-gradient(
      ellipse at 50% 80%,
      rgba(97, 51, 35, 0.06) 0%,
      transparent 45%
    );
}
```

### Film Flicker Effect

```css
/* Subtle brightness flicker like old film projection */
@keyframes fleischer-flicker {
  0%, 100% { opacity: 1; }
  4% { opacity: 0.97; }
  8% { opacity: 1; }
  12% { opacity: 0.98; }
  24% { opacity: 1; }
  28% { opacity: 0.96; }
  32% { opacity: 1; }
  56% { opacity: 0.99; }
  60% { opacity: 0.97; }
  64% { opacity: 1; }
  80% { opacity: 0.98; }
  84% { opacity: 1; }
}

.fleischer-flicker {
  animation: fleischer-flicker 4s linear infinite;
}
```

### Spotlight / Radial Light Effect

```css
/* Theatrical spotlight effect (Stereoptical depth feel) */
.fleischer-spotlight {
  position: relative;
}

.fleischer-spotlight::before {
  content: '';
  position: absolute;
  inset: 0;
  pointer-events: none;
  background: radial-gradient(
    circle at 50% 30%,
    rgba(245, 230, 200, 0.15) 0%,
    transparent 60%
  );
  z-index: 1;
}
```

---

## Materials and Textures (Visual Metaphors for Web)

| Physical Material | Web Equivalent |
|-------------------|----------------|
| Nitrate film stock | Film grain overlay + vignette + flicker animation |
| Animation cel acetate | Semi-transparent overlapping layers with visible edges |
| India ink on paper | Thick, confident black borders (4-5px solid) |
| Pencil underdrawing | Light gray guidelines or subtle grid patterns |
| Aged newsprint | Warm parchment backgrounds with subtle brown spotting |
| Projection screen | Off-white background with radial gradient hotspot |
| Charcoal shading | Soft gray gradients for volume and depth |
| Rubber (limbs) | Curved CSS borders, smooth bezier animations, elastic easing |

---

## Sub-styles and Variations

### Classic Fleischer (1929-1939)

- Pure black and white, maximum contrast
- Betty Boop, Bimbo, Koko the Clown
- Jazz-age musical synchronization
- Urban, gritty New York settings
- Surreal, sometimes unsettling transformations
- Strong vaudeville and burlesque influence

### Stereoptical / Dimensional (1934-1940)

- 3D miniature backgrounds with 2D animated characters
- Enhanced depth and parallax effect
- More cinematic, atmospheric compositions
- Used in Superman and Popeye shorts
- Darker, more dramatic lighting

### Cuphead Revival (Modern Interpretation)

- Faithful recreation of 1930s aesthetic in interactive media
- Watercolor-style backgrounds with vivid, muted colors
- Hand-drawn frame-by-frame animation quality
- Combines Fleischer style with Disney and Ub Iwerks influences
- Demonstrates the style's viability for modern digital applications

### Bendy / Inkwell Horror (Modern Subgenre)

- Takes the darker undertones of Fleischer and amplifies them
- Ink as both medium and menace
- Sepia-tinted, decayed versions of the cheerful 1930s aesthetic
- Dripping, melting, corrupted cartoon forms

---

## Related Aesthetics

| Aesthetic | Relationship to Fleischer Style |
|-----------|--------------------------------|
| **Art Deco** | Contemporary design movement; shares geometric elegance and Jazz Age sensibility |
| **Electro Swing** | Modern music genre that revives the same jazz/swing energy in audio form |
| **Streamline Moderne** | Later evolution of the same era's design language; smoother, more aerodynamic |
| **Surrealism** | Shared interest in dream logic, irrational transformations, and subconscious imagery |
| **Vaudeville** | Performance tradition that directly influenced Fleischer gags, pacing, and character types |
| **Dieselpunk** | Retro-futuristic aesthetic drawing from the same 1920s-1940s industrial era |
| **Gothic** | Shares the dark, atmospheric qualities of Fleischer's moodier works |
| **Vintage Americana** | Overlapping cultural nostalgia for pre-war American pop culture |

---

## Quick-Start: Minimal Fleischer Style Page Template

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Fleischer Style Page</title>
  <link href="https://fonts.googleapis.com/css2?family=Bungee+Shade&family=Josefin+Sans:wght@300;400;600&family=Fredoka:wght@300;400;500&family=Special+Elite&display=swap" rel="stylesheet">
  <style>
    :root {
      --fleischer-ink: #1a1a1a;
      --fleischer-charcoal: #4a4a4a;
      --fleischer-parchment: #f5e6c8;
      --fleischer-cream: #f5f0e1;
      --fleischer-amber: #d4a54a;
      --fleischer-faded-red: #b84a3c;
      --fleischer-burnt-umber: #613323;
    }

    * { margin: 0; padding: 0; box-sizing: border-box; }

    body {
      background: var(--fleischer-parchment);
      color: var(--fleischer-ink);
      font-family: 'Fredoka', sans-serif;
      font-weight: 400;
      line-height: 1.7;
      letter-spacing: 0.02em;
      overflow-x: hidden;
    }

    /* Film grain overlay */
    body::after {
      content: '';
      position: fixed;
      inset: 0;
      pointer-events: none;
      z-index: 9999;
      opacity: 0.05;
      background-image: url("data:image/svg+xml,%3Csvg viewBox='0 0 256 256' xmlns='http://www.w3.org/2000/svg'%3E%3Cfilter id='n'%3E%3CfeTurbulence type='fractalNoise' baseFrequency='0.9' numOctaves='4' stitchTiles='stitch'/%3E%3C/filter%3E%3Crect width='100%25' height='100%25' filter='url(%23n)'/%3E%3C/svg%3E");
      mix-blend-mode: multiply;
    }

    /* Vignette */
    body::before {
      content: '';
      position: fixed;
      inset: 0;
      pointer-events: none;
      z-index: 9998;
      background: radial-gradient(ellipse at center, transparent 50%, rgba(26,26,26,0.35) 100%);
    }

    /* Title card hero */
    .hero {
      background: var(--fleischer-ink);
      color: var(--fleischer-parchment);
      text-align: center;
      padding: 5rem 2rem;
      border-bottom: 5px solid var(--fleischer-charcoal);
      position: relative;
    }

    .hero::before, .hero::after {
      content: '';
      position: absolute;
      width: 36px;
      height: 36px;
      border-color: var(--fleischer-parchment);
      border-style: solid;
    }
    .hero::before { top: 14px; left: 14px; border-width: 3px 0 0 3px; }
    .hero::after { bottom: 14px; right: 14px; border-width: 0 3px 3px 0; }

    .hero h1 {
      font-family: 'Bungee Shade', cursive;
      font-size: clamp(2.5rem, 7vw, 5.5rem);
      letter-spacing: 0.08em;
      text-shadow: 3px 3px 0 var(--fleischer-amber);
    }

    .hero p {
      font-family: 'Special Elite', cursive;
      font-size: 1.2rem;
      margin-top: 1rem;
      opacity: 0.85;
    }

    /* Headings */
    h1, h2, h3 {
      font-family: 'Josefin Sans', sans-serif;
      text-transform: uppercase;
      letter-spacing: 0.1em;
      font-weight: 600;
    }

    /* Wavy divider */
    .divider {
      width: 100%;
      height: 40px;
      background: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 800 40'%3E%3Cpath d='M0 20Q100 0 200 20Q300 40 400 20Q500 0 600 20Q700 40 800 20' fill='none' stroke='%231a1a1a' stroke-width='4' stroke-linecap='round'/%3E%3C/svg%3E") no-repeat center;
      background-size: 100% 100%;
      margin: 1.5rem auto;
    }

    /* Content sections */
    section {
      max-width: 850px;
      margin: 0 auto;
      padding: 3rem 2rem;
      text-align: center;
    }

    /* Cartoon panel card */
    .panel {
      background: var(--fleischer-cream);
      border: 4px solid var(--fleischer-ink);
      border-radius: 14px;
      padding: 2rem;
      margin: 1.5rem 0;
      box-shadow: 5px 5px 0 var(--fleischer-ink);
    }
  </style>
</head>
<body>
  <div class="hero">
    <h1>Title Here</h1>
    <p>A subtitle in that old-timey typewriter style</p>
  </div>
  <section>
    <div class="divider"></div>
    <h2>Section Heading</h2>
    <p>Content styled in the Fleischer tradition -- thick ink borders, aged paper tones, and a touch of jazz-age whimsy.</p>
    <div class="panel">
      <h3>A Cartoon Panel</h3>
      <p>Rounded corners and bold shadows, just like a frame from a 1930s animated short.</p>
    </div>
  </section>
</body>
</html>
```
