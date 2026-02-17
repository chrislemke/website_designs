# Pop Art

Mass-culture celebration: Ben-Day dots, comic-book bold outlines, saturated commercial imagery a la Warhol and Lichtenstein. Pop Art emerged in the 1950s-60s as a reaction against the elitism of abstract expressionism, elevating the imagery of advertising, comic strips, consumer products, and celebrity culture into fine art. In digital design, it translates to high-energy compositions with halftone dot patterns, thick black outlines, speech bubbles, and unapologetically bold, saturated color palettes drawn from commercial printing.

---

## Visual Characteristics

### Core Design Traits

- **Ben-Day dots / halftone patterns** -- the signature visual motif; colored dots arranged in regular grids simulate the printing process of mass-produced comics and advertisements
- **Thick black outlines** -- every shape, panel, and figure is enclosed in heavy black contour lines (3-6px), mimicking comic-book inking
- **Saturated, high-chroma colors** -- CMYK-inspired primaries and secondaries at maximum saturation; nothing is muted or subtle
- **Comic-book panel layouts** -- content organized in rectangular panels with gutters, reminiscent of comic strip grids
- **Speech bubbles and thought balloons** -- text containers shaped like dialogue balloons with pointer tails
- **Repetition and serialization** -- Warhol-style repeated images with color variations; a single motif iterated across a grid
- **Flat, screen-printed color fills** -- no gradients; color is applied in solid, uniform blocks
- **Pop typography** -- bold, condensed, uppercase display type with exaggerated impact; comic-book lettering with slight irregularity
- **Ironic commercial imagery** -- soup cans, dollar signs, lips, stars, product labels treated as graphic elements
- **High contrast** -- stark juxtapositions of complementary colors and black outlines for maximum visual punch

### Design Principles

- Embrace popular culture and commercial aesthetics without ironic distance
- Use bold, immediate visual language that communicates at a glance
- Favor maximum saturation and contrast over subtlety and nuance
- Treat every surface as a potential canvas for pattern and color
- Repetition transforms the mundane into the iconic
- Typography is as loud as the imagery; text shouts, it does not whisper
- The grid is borrowed from comics and commercial printing, not from Swiss design
- More is more: density, color, and energy fill every available space

---

## Color Palette

### Pop Art Core Palette

The Pop Art palette derives from CMYK process printing and the limited color separations of 1960s comic books.

| Color Name | Hex | Role / Usage |
|------------|-----|-------------|
| **Pop Red** | `#FF0033` | Primary accent, headlines, key interactive elements |
| **Pop Yellow** | `#FFD600` | Secondary accent, backgrounds, highlight areas |
| **Pop Blue** | `#0057E7` | Tertiary accent, links, panel backgrounds |
| **Pop Pink** | `#FF69B4` | Feature accent, speech bubbles, secondary buttons |
| **Pop Cyan** | `#00BFFF` | Ben-Day dot fill, secondary backgrounds |
| **Pop Orange** | `#FF6600` | Warm accent, badges, notification elements |
| **Pop Green** | `#00CC44` | Success states, secondary accent |
| **Pure Black** | `#000000` | Outlines, text, panel borders, structural lines |
| **Pure White** | `#FFFFFF` | Background, speech bubble fills, text on dark |
| **Halftone Gray** | `#E8E8E8` | Light background for dot patterns |
| **Deep Purple** | `#8B00FF` | Accent variation, Warhol-inspired alternate |
| **Cream** | `#FFF8E1` | Off-white backgrounds, vintage print feel |

### CSS Custom Properties

```css
:root {
  /* Primary pop colors */
  --pop-red: #ff0033;
  --pop-yellow: #ffd600;
  --pop-blue: #0057e7;
  --pop-pink: #ff69b4;
  --pop-cyan: #00bfff;
  --pop-orange: #ff6600;
  --pop-green: #00cc44;
  --pop-purple: #8b00ff;

  /* Neutrals */
  --pop-black: #000000;
  --pop-white: #ffffff;
  --pop-cream: #fff8e1;
  --pop-gray: #e8e8e8;

  /* Hover/active states */
  --pop-red-dark: #cc0029;
  --pop-blue-dark: #0044b8;
  --pop-yellow-dark: #ccaa00;

  /* Backgrounds */
  --pop-bg-white: #ffffff;
  --pop-bg-cream: #fff8e1;
  --pop-bg-dots: #e8e8e8;
}
```

### Color Usage Guidelines

- **Use 3-4 bold colors per section** -- Pop Art is not restrained; it is a celebration of chromatic excess
- Every section should have a different dominant color to create visual energy
- Complement saturated fills with thick black outlines for definition
- Yellow and cyan serve as Ben-Day dot fill colors over white or cream backgrounds
- Use complementary color pairings for maximum contrast (red/cyan, blue/orange, yellow/purple)
- Never desaturate; Pop Art lives at full chroma
- Black outlines are non-negotiable; without them, Pop Art loses its comic-book identity

---

## Typography

### Typeface Characteristics

Pop Art typography is:

- **Bold, condensed, and uppercase** -- display type screams from the page with maximum impact
- **Comic-book lettering** -- slightly irregular, hand-lettered feel for speech bubbles and callouts
- **High contrast between display and body** -- headlines are enormous and heavy; body text is simple and readable
- **Graphic, not elegant** -- type is a visual element, not a refined reading experience
- **Sometimes distorted** -- stretched, compressed, or italicized for dynamic emphasis

### Recommended Web Fonts (Google Fonts)

| Font | Style | Best For |
|------|-------|----------|
| **Bangers** | Comic-book display | Headlines, speech bubble text, display |
| **Bungee** | Ultra-bold display | Hero text, large statements |
| **Permanent Marker** | Hand-lettered marker | Informal callouts, labels |
| **Oswald** | Condensed gothic | Subheadings, navigation, body headings |
| **Anton** | Impact-style condensed | Oversized display, poster headings |
| **Archivo Black** | Bold grotesque | Secondary headings, buttons |
| **Luckiest Guy** | Rounded comic display | Fun headlines, badges |
| **Russo One** | Geometric bold | Modern pop display, tech-pop crossover |
| **Open Sans** | Clean sans-serif | Body text, readable contrast to display fonts |
| **Roboto** | Neutral sans-serif | Body text, UI elements |

### Font Pairing Suggestions

| Heading Font | Body Font | Character |
|-------------|-----------|-----------|
| **Bangers** (400) | **Open Sans** (400) | Classic comic-book Pop Art |
| **Bungee** (400) | **Roboto** (400) | Ultra-bold modern pop |
| **Anton** (400) | **Open Sans** (400) | Poster-style, high impact |
| **Luckiest Guy** (400) | **Roboto** (400) | Playful, energetic pop |
| **Oswald** (700) | **Open Sans** (400) | Condensed, editorial pop |

### Typography CSS Example

```css
/* Import fonts */
@import url('https://fonts.googleapis.com/css2?family=Bangers&family=Open+Sans:wght@400;600;700&display=swap');

/* Headings */
h1, h2, h3, h4, h5, h6 {
  font-family: 'Bangers', 'Impact', cursive;
  font-weight: 400;
  color: var(--pop-black);
  line-height: 1.1;
  letter-spacing: 0.04em;
  text-transform: uppercase;
}

/* Display / Hero text */
.pop-display {
  font-family: 'Bangers', cursive;
  font-size: clamp(3rem, 8vw, 7rem);
  letter-spacing: 0.06em;
  line-height: 0.95;
  text-transform: uppercase;
  -webkit-text-stroke: 3px var(--pop-black);
  paint-order: stroke fill;
}

/* Body text */
body {
  font-family: 'Open Sans', sans-serif;
  font-weight: 400;
  font-size: 1rem;
  line-height: 1.7;
  color: var(--pop-black);
}

/* Speech bubble text */
.pop-speech {
  font-family: 'Bangers', cursive;
  font-size: 1.2rem;
  letter-spacing: 0.03em;
  text-transform: uppercase;
  line-height: 1.4;
}

/* Caption / small text */
.pop-caption {
  font-family: 'Open Sans', sans-serif;
  font-weight: 700;
  font-size: 0.85rem;
  text-transform: uppercase;
  letter-spacing: 0.06em;
}
```

---

## Layout Principles

### Grid and Structure

- **Comic-panel grid** -- content organized into thick-bordered rectangular panels with consistent gutters (8-12px black gaps)
- **Irregular panel sizes** -- unlike Swiss grids, Pop Art panels vary in size to create hierarchy and dramatic pacing
- **Full-bleed color sections** -- entire sections filled with solid saturated colors, switching dramatically between sections
- **Layered elements** -- speech bubbles, starburst shapes, and callouts overlap panel boundaries for dynamic energy
- **Dense compositions** -- Pop Art fills space rather than leaving it; whitespace is replaced with dots, color, or pattern
- **Max-width 1200px** for structured content, but background patterns and colors extend full-width

### Section Organization

- **Navigation**: Bold colored bar with thick bottom border; logo in comic-book lettering; links in uppercase condensed type
- **Hero**: Massive headline with text-stroke outline, Ben-Day dot background, speech bubble with CTA
- **Features**: Comic-panel grid with each feature in its own bordered panel; each panel a different background color
- **Content rows**: Alternating bold color backgrounds with halftone dot patterns
- **Callout / CTA**: Starburst or explosion shape containing text and button
- **Footer**: Black background with colored accents, comic-style lettering

### Responsive Approach

- Panel grids collapse from multi-column to single-column on mobile
- Thick outlines and borders maintain their weight at all sizes
- Display typography scales aggressively using `clamp()`
- Ben-Day dot patterns scale with the container using relative units
- Speech bubbles stack vertically on small screens

---

## CSS / Design Techniques

### Ben-Day Dot Pattern (CSS Background)

```css
.pop-dots {
  background-image: radial-gradient(
    circle,
    var(--pop-cyan) 20%,
    transparent 20%
  );
  background-size: 12px 12px;
  background-color: var(--pop-white);
}

/* Larger dots */
.pop-dots--large {
  background-image: radial-gradient(
    circle,
    var(--pop-yellow) 25%,
    transparent 25%
  );
  background-size: 20px 20px;
  background-color: var(--pop-cream);
}

/* Pink dots on white */
.pop-dots--pink {
  background-image: radial-gradient(
    circle,
    var(--pop-pink) 18%,
    transparent 18%
  );
  background-size: 14px 14px;
  background-color: var(--pop-white);
}
```

### Pop Art Card / Panel

```css
.pop-card {
  background: var(--pop-white);
  border: 4px solid var(--pop-black);
  padding: 28px;
  position: relative;
}

/* Shadow offset for comic-book depth */
.pop-card::after {
  content: '';
  position: absolute;
  top: 6px;
  left: 6px;
  right: -6px;
  bottom: -6px;
  background: var(--pop-black);
  z-index: -1;
}

.pop-card-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
  gap: 24px;
}
```

### Pop Art Button

```css
.pop-button {
  display: inline-block;
  background: var(--pop-red);
  color: var(--pop-white);
  border: 4px solid var(--pop-black);
  border-radius: 0;
  padding: 14px 36px;
  font-family: 'Bangers', cursive;
  font-size: 1.2rem;
  letter-spacing: 0.06em;
  text-transform: uppercase;
  cursor: pointer;
  text-decoration: none;
  position: relative;
  transition: transform 0.1s ease;
}

.pop-button::after {
  content: '';
  position: absolute;
  top: 4px;
  left: 4px;
  right: -4px;
  bottom: -4px;
  background: var(--pop-black);
  z-index: -1;
  transition: all 0.1s ease;
}

.pop-button:hover {
  transform: translate(-2px, -2px);
}

.pop-button:hover::after {
  top: 6px;
  left: 6px;
}

.pop-button:active {
  transform: translate(2px, 2px);
}

.pop-button:active::after {
  top: 0;
  left: 0;
}

/* Color variants */
.pop-button--blue { background: var(--pop-blue); }
.pop-button--yellow { background: var(--pop-yellow); color: var(--pop-black); }
.pop-button--pink { background: var(--pop-pink); }
```

### Speech Bubble

```css
.pop-speech-bubble {
  background: var(--pop-white);
  border: 4px solid var(--pop-black);
  border-radius: 20px;
  padding: 24px 28px;
  position: relative;
  display: inline-block;
  max-width: 400px;
}

.pop-speech-bubble::after {
  content: '';
  position: absolute;
  bottom: -24px;
  left: 40px;
  width: 0;
  height: 0;
  border: 12px solid transparent;
  border-top-color: var(--pop-black);
}

.pop-speech-bubble::before {
  content: '';
  position: absolute;
  bottom: -16px;
  left: 44px;
  width: 0;
  height: 0;
  border: 8px solid transparent;
  border-top-color: var(--pop-white);
  z-index: 1;
}
```

### Navigation Bar

```css
.pop-nav {
  display: flex;
  align-items: center;
  justify-content: space-between;
  background: var(--pop-yellow);
  border-bottom: 5px solid var(--pop-black);
  padding: 16px 40px;
}

.pop-nav__logo {
  font-family: 'Bangers', cursive;
  font-size: 2rem;
  color: var(--pop-red);
  text-decoration: none;
  -webkit-text-stroke: 1px var(--pop-black);
  letter-spacing: 0.04em;
}

.pop-nav__links {
  display: flex;
  gap: 28px;
  list-style: none;
  margin: 0;
  padding: 0;
}

.pop-nav__links a {
  font-family: 'Bangers', cursive;
  font-size: 1.1rem;
  color: var(--pop-black);
  text-decoration: none;
  text-transform: uppercase;
  letter-spacing: 0.04em;
  transition: color 0.2s ease;
}

.pop-nav__links a:hover {
  color: var(--pop-red);
}
```

### Hero Section

```css
.pop-hero {
  position: relative;
  padding: 80px 40px;
  overflow: hidden;
  background-image: radial-gradient(
    circle,
    var(--pop-cyan) 18%,
    transparent 18%
  );
  background-size: 16px 16px;
  background-color: var(--pop-cream);
}

.pop-hero__content {
  max-width: 1200px;
  margin: 0 auto;
  position: relative;
  z-index: 1;
}

.pop-hero__content h1 {
  font-size: clamp(3rem, 8vw, 6rem);
  color: var(--pop-red);
  -webkit-text-stroke: 3px var(--pop-black);
  paint-order: stroke fill;
  margin-bottom: 1.5rem;
}

.pop-hero__content p {
  font-size: 1.2rem;
  max-width: 500px;
  margin-bottom: 2rem;
  line-height: 1.6;
}

@media (max-width: 768px) {
  .pop-hero { padding: 60px 24px; }
}
```

### Starburst / Explosion Shape

```css
.pop-starburst {
  position: relative;
  display: inline-flex;
  align-items: center;
  justify-content: center;
  width: 200px;
  height: 200px;
  background: var(--pop-yellow);
  clip-path: polygon(
    50% 0%, 61% 15%, 78% 5%, 75% 25%,
    95% 28%, 83% 42%, 100% 50%, 83% 58%,
    95% 72%, 75% 75%, 78% 95%, 61% 85%,
    50% 100%, 39% 85%, 22% 95%, 25% 75%,
    5% 72%, 17% 58%, 0% 50%, 17% 42%,
    5% 28%, 25% 25%, 22% 5%, 39% 15%
  );
  font-family: 'Bangers', cursive;
  font-size: 1.5rem;
  text-transform: uppercase;
  text-align: center;
}
```

---

## Design Do's and Don'ts

### Do

- Use Ben-Day dot patterns as backgrounds and texture fills
- Apply thick black outlines (3-6px) to every major element
- Use saturated, high-chroma colors at maximum intensity
- Create comic-panel grid layouts with visible borders
- Use comic-book display fonts for headlines and callouts
- Include speech bubbles and starburst shapes for emphasis
- Repeat visual motifs Warhol-style across grids
- Make every section visually distinct with its own color scheme

### Don't

- Use muted, pastel, or desaturated colors -- Pop Art demands full saturation
- Remove the black outlines; they are essential to the comic-book aesthetic
- Use elegant, thin, or serif typefaces for headings
- Leave large areas of empty whitespace -- fill space with dots, color, or pattern
- Apply gradients or smooth transitions between colors
- Use photographic imagery without halftone treatment or bold outline processing
- Create subtle, restrained hover effects -- interactions should be bold and immediate
- Mix Pop Art with minimalist or Swiss-style layouts; the philosophies conflict

---

## Related Aesthetics

| Aesthetic | Relationship to Pop Art |
|-----------|----------------------|
| **Memphis Design** | 1980s successor; shares bold color and geometric pattern but adds postmodern irony and squiggles |
| **Neubrutalism** | Contemporary relative; shares thick outlines and bold colors but with raw, unpolished intentional ugliness |
| **Flat Design** | Shares the solid color fills and absence of gradients but strips away the expressive energy and ornament |
| **Ligne Claire** | European comic-art sibling; shares uniform-weight outlines and flat color but with more refined, narrative-driven illustration |
| **Superflat Pop** | Japanese contemporary response; Takashi Murakami's fusion of Pop Art with anime and otaku culture |
| **Gen Z Maximalism** | Contemporary spiritual descendant; shares the more-is-more philosophy and saturated color palette |
| **Colorful Pop** | Direct digital adaptation of Pop Art principles for modern interfaces and branding |
| **Wacky Pomo** | Postmodern cousin; shares the irreverence and bold graphics but adds more chaos and deconstruction |
| **Corporate Memphis** | Shares flat illustration style but corporate-sanitized; Pop Art's rebellious energy drained for brand safety |
| **Graffiti Pop** | Street-art evolution; brings Pop Art's bold graphics into urban, spray-painted contexts |

---

## Quick-Start: Minimal Pop Art Page Template

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Pop Art Page</title>
  <link href="https://fonts.googleapis.com/css2?family=Bangers&family=Open+Sans:wght@400;600;700&display=swap" rel="stylesheet">
  <style>
    :root {
      --pop-red: #ff0033;
      --pop-yellow: #ffd600;
      --pop-blue: #0057e7;
      --pop-pink: #ff69b4;
      --pop-cyan: #00bfff;
      --pop-orange: #ff6600;
      --pop-black: #000000;
      --pop-white: #ffffff;
      --pop-cream: #fff8e1;
    }

    * { margin: 0; padding: 0; box-sizing: border-box; }

    body {
      background: var(--pop-white);
      color: var(--pop-black);
      font-family: 'Open Sans', sans-serif;
      font-weight: 400;
      line-height: 1.7;
    }

    h1, h2, h3 {
      font-family: 'Bangers', cursive;
      font-weight: 400;
      text-transform: uppercase;
      letter-spacing: 0.04em;
      line-height: 1.05;
    }

    /* Navigation */
    nav {
      display: flex;
      align-items: center;
      justify-content: space-between;
      background: var(--pop-yellow);
      border-bottom: 5px solid var(--pop-black);
      padding: 16px 40px;
    }

    nav a.logo {
      font-family: 'Bangers', cursive;
      font-size: 2rem;
      color: var(--pop-red);
      text-decoration: none;
      -webkit-text-stroke: 1px var(--pop-black);
    }

    nav ul {
      display: flex;
      gap: 24px;
      list-style: none;
    }

    nav ul a {
      font-family: 'Bangers', cursive;
      font-size: 1.1rem;
      color: var(--pop-black);
      text-decoration: none;
      text-transform: uppercase;
      transition: color 0.2s;
    }

    nav ul a:hover { color: var(--pop-red); }

    /* Hero with Ben-Day dots */
    .hero {
      padding: 80px 40px;
      background-image: radial-gradient(circle, var(--pop-cyan) 18%, transparent 18%);
      background-size: 14px 14px;
      background-color: var(--pop-cream);
      border-bottom: 5px solid var(--pop-black);
    }

    .hero-inner {
      max-width: 1200px;
      margin: 0 auto;
      display: flex;
      align-items: center;
      gap: 60px;
    }

    .hero-content { flex: 1; }

    .hero h1 {
      font-size: clamp(3rem, 8vw, 6rem);
      color: var(--pop-red);
      -webkit-text-stroke: 2px var(--pop-black);
      paint-order: stroke fill;
      margin-bottom: 1.5rem;
    }

    .hero p {
      font-size: 1.15rem;
      max-width: 460px;
      margin-bottom: 2rem;
    }

    .btn {
      display: inline-block;
      background: var(--pop-red);
      color: var(--pop-white);
      border: 4px solid var(--pop-black);
      padding: 14px 36px;
      font-family: 'Bangers', cursive;
      font-size: 1.3rem;
      text-transform: uppercase;
      letter-spacing: 0.04em;
      text-decoration: none;
      cursor: pointer;
      position: relative;
      transition: transform 0.1s;
    }

    .btn::after {
      content: '';
      position: absolute;
      top: 4px; left: 4px; right: -4px; bottom: -4px;
      background: var(--pop-black);
      z-index: -1;
    }

    .btn:hover { transform: translate(-2px, -2px); }

    .hero-visual { flex: 1; display: flex; justify-content: center; }

    /* Speech bubble */
    .speech-bubble {
      background: var(--pop-white);
      border: 4px solid var(--pop-black);
      border-radius: 24px;
      padding: 28px 32px;
      position: relative;
      max-width: 320px;
    }

    .speech-bubble::after {
      content: '';
      position: absolute;
      bottom: -20px; left: 40px;
      border: 10px solid transparent;
      border-top-color: var(--pop-black);
    }

    .speech-bubble::before {
      content: '';
      position: absolute;
      bottom: -12px; left: 44px;
      border: 6px solid transparent;
      border-top-color: var(--pop-white);
      z-index: 1;
    }

    .speech-bubble p {
      font-family: 'Bangers', cursive;
      font-size: 1.4rem;
      text-transform: uppercase;
      line-height: 1.3;
    }

    /* Features as comic panels */
    .features {
      background: var(--pop-white);
      padding: 80px 40px;
      border-bottom: 5px solid var(--pop-black);
    }

    .features h2 {
      text-align: center;
      font-size: 3rem;
      color: var(--pop-blue);
      -webkit-text-stroke: 1px var(--pop-black);
      margin-bottom: 48px;
    }

    .panel-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
      gap: 20px;
      max-width: 1200px;
      margin: 0 auto;
    }

    .panel {
      border: 4px solid var(--pop-black);
      padding: 28px;
      position: relative;
      text-align: center;
    }

    .panel::after {
      content: '';
      position: absolute;
      top: 5px; left: 5px; right: -5px; bottom: -5px;
      background: var(--pop-black);
      z-index: -1;
    }

    .panel:nth-child(1) { background: var(--pop-pink); }
    .panel:nth-child(2) { background: var(--pop-yellow); }
    .panel:nth-child(3) { background: var(--pop-cyan); }

    .panel h3 { font-size: 1.6rem; margin-bottom: 0.5rem; }
    .panel p { font-size: 0.95rem; }

    /* CTA section */
    .cta {
      background: var(--pop-red);
      border-bottom: 5px solid var(--pop-black);
      text-align: center;
      padding: 80px 40px;
    }

    .cta h2 {
      font-size: clamp(2rem, 5vw, 3.5rem);
      color: var(--pop-white);
      -webkit-text-stroke: 2px var(--pop-black);
      margin-bottom: 1rem;
    }

    .cta p {
      color: var(--pop-white);
      font-size: 1.15rem;
      margin-bottom: 2rem;
      max-width: 500px;
      margin-left: auto;
      margin-right: auto;
    }

    .cta .btn {
      background: var(--pop-yellow);
      color: var(--pop-black);
    }

    /* Footer */
    footer {
      background: var(--pop-black);
      color: var(--pop-white);
      text-align: center;
      padding: 40px;
      font-family: 'Bangers', cursive;
      font-size: 1.1rem;
      letter-spacing: 0.04em;
    }

    @media (max-width: 768px) {
      .hero-inner { flex-direction: column; }
      .hero { padding: 60px 24px; }
      nav { padding: 14px 20px; }
      nav ul { gap: 16px; }
    }
  </style>
</head>
<body>
  <nav>
    <a href="#" class="logo">POW!</a>
    <ul>
      <li><a href="#">Gallery</a></li>
      <li><a href="#">Artists</a></li>
      <li><a href="#">Shop</a></li>
      <li><a href="#">About</a></li>
    </ul>
  </nav>

  <section class="hero">
    <div class="hero-inner">
      <div class="hero-content">
        <h1>Art Is What You Can Get Away With</h1>
        <p>Bold colors. Thick outlines. Mass culture elevated to fine art. Welcome to the pop revolution.</p>
        <a href="#" class="btn">Explore Now!</a>
      </div>
      <div class="hero-visual">
        <div class="speech-bubble">
          <p>Wow! This design is incredible!</p>
        </div>
      </div>
    </div>
  </section>

  <section class="features">
    <h2>What We Do</h2>
    <div class="panel-grid">
      <div class="panel">
        <h3>Create</h3>
        <p>Bold visual experiences inspired by the pop masters. Every project pops off the screen.</p>
      </div>
      <div class="panel">
        <h3>Inspire</h3>
        <p>We turn everyday content into iconic visual moments. Commercial imagery becomes art.</p>
      </div>
      <div class="panel">
        <h3>Disrupt</h3>
        <p>Challenge the ordinary. Break the rules. Make people stop scrolling and start looking.</p>
      </div>
    </div>
  </section>

  <section class="cta">
    <h2>Ready To Make Some Noise?</h2>
    <p>Join the movement. Let your brand explode with color, energy, and unmistakable pop style.</p>
    <a href="#" class="btn">Get Started!</a>
  </section>

  <footer>
    <p>Built with Pop Art energy. Warhol would approve.</p>
  </footer>
</body>
</html>
```
