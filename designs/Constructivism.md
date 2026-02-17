# Constructivism

Soviet-era angular propaganda: diagonal compositions, bold red-and-black typography, photomontage. Constructivism emerged in post-revolutionary Russia (1913-1930s) as an art movement that rejected autonomous art in favor of design serving social and political purposes. Its visual language -- dominated by dramatic diagonal compositions, wedge-shaped forms, bold sans-serif type, and a restricted red-black-white palette -- was forged to communicate revolutionary ideals to the masses through posters, publications, and architecture. In digital design, it translates to high-energy, angular layouts with aggressive typography, stark color contrasts, and an unmistakable sense of dynamism and urgency.

---

## Visual Characteristics

### Core Design Traits

- **Dominant diagonal compositions** -- elements are rotated, tilted, and arranged at sharp angles to create dynamic tension and forward momentum
- **Red and black as the primary palette** -- the revolutionary colors dominate, with white providing contrast and negative space
- **Bold, oversized typography** -- text is a primary visual element, often larger than imagery; words shout with urgency
- **Wedge and angular shapes** -- triangles, parallelograms, and sharp-angled geometric forms pierce through the composition
- **Photomontage** -- cut-and-assembled photographic fragments combined with geometric shapes and typography
- **Stark contrast** -- extreme black-and-white juxtapositions with red as the single chromatic accent
- **Industrial / mechanical references** -- gears, beams, scaffolding, and structural forms evoking factory and construction imagery
- **Asymmetric, off-balance layouts** -- compositions that feel like they are in motion, never static
- **Propagandistic directness** -- visual communication is immediate, forceful, and unambiguous
- **Collage and layering** -- overlapping elements create depth through compositional collision rather than shadow or perspective

### Design Principles

- Art must serve society; design is a tool for communication, not self-expression
- Diagonal energy is superior to static horizontal/vertical arrangements
- Typography is architecture: words are built, not written
- Red is not decoration; it is the color of revolution, urgency, and action
- Compositions should feel like they are exploding outward from a central point of tension
- Photographic imagery gains power through fragmentation and recombination
- Every element should convey force, direction, and purpose
- Negative space is carved by the angular elements, not planned around them

---

## Color Palette

### Constructivist Core Palette

The Constructivist palette is deliberately restricted to maximize impact: red for revolution, black for power, white for contrast.

| Color Name | Hex | Role / Usage |
|------------|-----|-------------|
| **Revolutionary Red** | `#CC0000` | Primary accent, headlines, key elements, action states |
| **Deep Red** | `#990000` | Hover/active states, secondary red emphasis |
| **Pure Black** | `#000000` | Text, backgrounds, structural elements, outlines |
| **Off-Black** | `#1A1A1A` | Dark backgrounds, card surfaces |
| **Dark Charcoal** | `#2D2D2D` | Secondary dark surfaces, footer backgrounds |
| **Pure White** | `#FFFFFF` | Text on dark, negative space, contrast areas |
| **Off-White** | `#F2F0EB` | Warm background, paper-like surfaces |
| **Cream** | `#E8E0D0` | Aged paper effect, vintage poster feel |
| **Steel Gray** | `#6B6B6B` | Secondary text, muted elements |
| **Rust Orange** | `#C45522` | Optional secondary warm accent, aged poster palette |

### CSS Custom Properties

```css
:root {
  /* Primary palette */
  --con-red: #cc0000;
  --con-red-dark: #990000;
  --con-rust: #c45522;

  /* Neutrals */
  --con-black: #000000;
  --con-off-black: #1a1a1a;
  --con-charcoal: #2d2d2d;
  --con-steel: #6b6b6b;
  --con-white: #ffffff;
  --con-off-white: #f2f0eb;
  --con-cream: #e8e0d0;

  /* Functional */
  --con-bg-light: #f2f0eb;
  --con-bg-dark: #1a1a1a;
  --con-text-light: #ffffff;
  --con-text-dark: #000000;
  --con-text-muted: #6b6b6b;

  /* Angles */
  --con-skew: -5deg;
  --con-skew-strong: -12deg;
}
```

### Color Usage Guidelines

- **Red and black dominate** -- these two colors should account for 80% or more of the chromatic content
- White serves as contrast and breathing room, not as the primary background
- Use red sparingly for maximum impact; it should feel urgent and deliberate
- Dark backgrounds (black, off-black) are preferred over light for a dramatic, poster-like feel
- Cream and off-white evoke the aged paper of original Soviet posters
- Rust orange is an optional secondary accent for variety but should not compete with red
- Never use soft or pastel colors; the palette is harsh and confrontational by design
- Gray serves only for muted secondary text; it should not occupy large areas

---

## Typography

### Typeface Characteristics

Constructivist typography is:

- **Bold, condensed, and aggressive** -- letterforms carry the weight and urgency of proclamation
- **Mixed sizes for dramatic hierarchy** -- a single word may be 10x the size of surrounding text
- **Rotated and angled** -- text blocks are tilted at diagonals to reinforce the angular composition
- **Sans-serif and geometric** -- clean, industrial letterforms stripped of calligraphic heritage
- **Uppercase dominant** -- capitalization conveys authority and command
- **Stacked and fragmented** -- words broken across lines, stacked vertically, or split across compositional zones

### Recommended Web Fonts (Google Fonts)

| Font | Style | Best For |
|------|-------|----------|
| **Oswald** | Condensed gothic | Primary display, headlines, navigation |
| **Bebas Neue** | Ultra-condensed uppercase | Maximum-impact display text, poster headings |
| **Anton** | Impact-style condensed | Oversized single-word statements |
| **Archivo Black** | Bold grotesque | Secondary headings, buttons |
| **Russo One** | Geometric bold with Cyrillic feel | Display text with Soviet character |
| **Passion One** | Thick condensed display | Hero text, extreme emphasis |
| **Barlow Condensed** | Condensed geometric | Body headings, navigation, labels |
| **Roboto Condensed** | Condensed humanist | Body text on dark backgrounds |
| **Inter** | Screen-optimized sans | Body text, readable secondary content |
| **Source Sans Pro** | Clean UI sans | Body text, data-heavy layouts |

### Font Pairing Suggestions

| Heading Font | Body Font | Character |
|-------------|-----------|-----------|
| **Bebas Neue** (400) | **Roboto Condensed** (400) | Classic propaganda poster feel |
| **Oswald** (700) | **Inter** (400) | Bold, modern constructivism |
| **Anton** (400) | **Source Sans Pro** (400) | Maximum impact, readable body |
| **Russo One** (400) | **Roboto Condensed** (400) | Soviet-inspired, geometric |
| **Passion One** (700) | **Barlow Condensed** (400) | Ultra-bold, condensed throughout |

### Typography CSS Example

```css
/* Import fonts */
@import url('https://fonts.googleapis.com/css2?family=Bebas+Neue&family=Roboto+Condensed:wght@400;700&display=swap');

/* Headings */
h1, h2, h3, h4, h5, h6 {
  font-family: 'Bebas Neue', 'Impact', sans-serif;
  font-weight: 400;
  color: var(--con-white);
  line-height: 0.9;
  letter-spacing: 0.04em;
  text-transform: uppercase;
}

/* Display / Hero text */
.con-display {
  font-family: 'Bebas Neue', sans-serif;
  font-size: clamp(4rem, 12vw, 10rem);
  letter-spacing: 0.06em;
  line-height: 0.85;
  text-transform: uppercase;
  color: var(--con-red);
}

/* Body text */
body {
  font-family: 'Roboto Condensed', sans-serif;
  font-weight: 400;
  font-size: 1rem;
  line-height: 1.7;
  color: var(--con-text-dark);
}

/* Angled label */
.con-label {
  font-family: 'Bebas Neue', sans-serif;
  font-size: 1rem;
  letter-spacing: 0.12em;
  text-transform: uppercase;
  color: var(--con-red);
  transform: rotate(var(--con-skew));
  display: inline-block;
}

/* Caption */
.con-caption {
  font-family: 'Roboto Condensed', sans-serif;
  font-weight: 400;
  font-size: 0.85rem;
  color: var(--con-steel);
  line-height: 1.5;
}
```

---

## Layout Principles

### Grid and Structure

- **Diagonal axis** -- the primary compositional axis is diagonal, not horizontal; elements follow tilted implied lines across the page
- **Angular section dividers** -- sections are separated by skewed, angled edges rather than straight horizontal rules
- **Overlapping layers** -- elements collide and overlap; text crosses over shapes, shapes cross over images
- **Full-bleed dark backgrounds** -- compositions typically sit on dark (black or near-black) backgrounds for maximum drama
- **Off-center focal points** -- the visual center of gravity is deliberately displaced from the geometric center
- **Wedge shapes as structural elements** -- triangular and wedge-shaped containers guide the eye along diagonal paths
- **Max-width 1200px** for structured content, but angular backgrounds extend full-width

### Section Organization

- **Navigation**: Dark bar with angular red accent; bold condensed uppercase links; no rounded elements
- **Hero**: Massive diagonal headline (rotated 5-15 degrees), red accent wedge, stark black-and-white contrast
- **Features**: Cards or blocks at slight angles; each anchored by a red geometric accent (triangle, wedge, bar)
- **Content rows**: Diagonal dividers between sections; alternating dark and off-white backgrounds
- **Manifesto / Statement**: Full-width red background with enormous white text, tilted for urgency
- **Footer**: Black background, red accent bar, angular geometric elements

### Responsive Approach

- Angular compositions maintain their skew on mobile, scaled proportionally
- Diagonal section dividers use CSS `clip-path` or `transform: skewY()` for responsive scaling
- Display typography scales aggressively using `clamp()`; hero text should dominate even on small screens
- Dark backgrounds provide natural contrast for readability on any screen
- Touch targets remain accessible (44px minimum) despite the angular visual treatment

---

## CSS / Design Techniques

### Angular Section Divider

```css
.con-section {
  position: relative;
  padding: 80px 40px;
}

.con-section--dark {
  background: var(--con-off-black);
  color: var(--con-white);
}

.con-section--light {
  background: var(--con-off-white);
  color: var(--con-black);
}

/* Angled top edge */
.con-section--angled::before {
  content: '';
  position: absolute;
  top: -40px;
  left: 0;
  right: 0;
  height: 80px;
  background: inherit;
  transform: skewY(-3deg);
  z-index: -1;
}
```

### Constructivist Card Component

```css
.con-card {
  background: var(--con-charcoal);
  color: var(--con-white);
  padding: 32px;
  position: relative;
  border-left: 6px solid var(--con-red);
  transform: rotate(-1deg);
  transition: transform 0.2s ease;
}

.con-card:hover {
  transform: rotate(0deg);
}

/* Red wedge accent */
.con-card::before {
  content: '';
  position: absolute;
  top: 0;
  right: 0;
  width: 0;
  height: 0;
  border-top: 40px solid var(--con-red);
  border-left: 40px solid transparent;
}

.con-card-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
  gap: 28px;
  max-width: 1200px;
  margin: 0 auto;
}
```

### Constructivist Button

```css
.con-button {
  display: inline-block;
  background: var(--con-red);
  color: var(--con-white);
  border: none;
  border-radius: 0;
  padding: 14px 40px;
  font-family: 'Bebas Neue', sans-serif;
  font-size: 1.2rem;
  letter-spacing: 0.1em;
  text-transform: uppercase;
  cursor: pointer;
  text-decoration: none;
  transform: skewX(-5deg);
  transition: background 0.2s ease, transform 0.2s ease;
  position: relative;
}

.con-button:hover {
  background: var(--con-red-dark);
  transform: skewX(-5deg) translateY(-2px);
}

.con-button span {
  display: inline-block;
  transform: skewX(5deg);
}

/* Black variant */
.con-button--black {
  background: var(--con-black);
  border: 2px solid var(--con-white);
}

.con-button--black:hover {
  background: var(--con-red);
  border-color: var(--con-red);
}

/* Outline variant */
.con-button--outline {
  background: transparent;
  border: 3px solid var(--con-red);
  color: var(--con-red);
}

.con-button--outline:hover {
  background: var(--con-red);
  color: var(--con-white);
}
```

### Navigation Bar

```css
.con-nav {
  display: flex;
  align-items: center;
  justify-content: space-between;
  background: var(--con-black);
  padding: 0 40px;
  position: relative;
}

/* Red angular accent */
.con-nav::after {
  content: '';
  position: absolute;
  bottom: 0;
  left: 0;
  width: 200px;
  height: 4px;
  background: var(--con-red);
  transform: skewX(-20deg);
  transform-origin: bottom left;
}

.con-nav__logo {
  font-family: 'Bebas Neue', sans-serif;
  font-size: 1.8rem;
  color: var(--con-red);
  text-decoration: none;
  letter-spacing: 0.08em;
  padding: 20px 0;
}

.con-nav__links {
  display: flex;
  gap: 32px;
  list-style: none;
  margin: 0;
  padding: 0;
}

.con-nav__links a {
  font-family: 'Bebas Neue', sans-serif;
  font-size: 1.05rem;
  color: var(--con-white);
  text-decoration: none;
  letter-spacing: 0.08em;
  text-transform: uppercase;
  padding: 20px 0;
  transition: color 0.2s ease;
  position: relative;
}

.con-nav__links a:hover {
  color: var(--con-red);
}

.con-nav__links a::after {
  content: '';
  position: absolute;
  bottom: 16px;
  left: 0;
  width: 0;
  height: 2px;
  background: var(--con-red);
  transition: width 0.3s ease;
}

.con-nav__links a:hover::after {
  width: 100%;
}
```

### Hero Section

```css
.con-hero {
  background: var(--con-off-black);
  color: var(--con-white);
  padding: 100px 40px 120px;
  position: relative;
  overflow: hidden;
}

/* Diagonal red wedge */
.con-hero::before {
  content: '';
  position: absolute;
  top: 0;
  right: -100px;
  width: 500px;
  height: 100%;
  background: var(--con-red);
  transform: skewX(-12deg);
  opacity: 0.15;
}

.con-hero__content {
  max-width: 1200px;
  margin: 0 auto;
  position: relative;
  z-index: 1;
}

.con-hero__content h1 {
  font-size: clamp(4rem, 10vw, 8rem);
  color: var(--con-white);
  line-height: 0.85;
  margin-bottom: 1.5rem;
  transform: rotate(-3deg);
  transform-origin: left center;
}

.con-hero__content h1 .red {
  color: var(--con-red);
}

.con-hero__content p {
  font-size: 1.15rem;
  color: var(--con-steel);
  max-width: 500px;
  margin-bottom: 2.5rem;
  line-height: 1.7;
}

@media (max-width: 768px) {
  .con-hero {
    padding: 60px 24px 80px;
  }
}
```

### Feature Grid

```css
.con-features {
  background: var(--con-off-white);
  padding: 80px 40px;
  position: relative;
}

.con-features__header {
  max-width: 1200px;
  margin: 0 auto 60px;
}

.con-features__header h2 {
  font-size: 3rem;
  color: var(--con-black);
  position: relative;
  display: inline-block;
}

/* Red underline accent */
.con-features__header h2::after {
  content: '';
  position: absolute;
  bottom: -8px;
  left: 0;
  width: 60px;
  height: 6px;
  background: var(--con-red);
  transform: skewX(-15deg);
}

.con-features__grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
  gap: 28px;
  max-width: 1200px;
  margin: 0 auto;
}

.con-feature {
  background: var(--con-white);
  padding: 32px;
  border-left: 5px solid var(--con-red);
  position: relative;
}

.con-feature__number {
  font-family: 'Bebas Neue', sans-serif;
  font-size: 3.5rem;
  color: var(--con-cream);
  line-height: 1;
  margin-bottom: 0.5rem;
}

.con-feature h3 {
  font-size: 1.3rem;
  color: var(--con-black);
  margin-bottom: 0.75rem;
}

.con-feature p {
  font-size: 0.95rem;
  color: var(--con-steel);
  line-height: 1.6;
}
```

### Diagonal Stripe Accent

```css
.con-stripe {
  height: 60px;
  background: repeating-linear-gradient(
    -45deg,
    var(--con-red),
    var(--con-red) 20px,
    var(--con-black) 20px,
    var(--con-black) 40px
  );
}
```

### Manifesto Block

```css
.con-manifesto {
  background: var(--con-red);
  color: var(--con-white);
  padding: 80px 40px;
  text-align: center;
  position: relative;
  clip-path: polygon(0 8%, 100% 0, 100% 92%, 0 100%);
}

.con-manifesto h2 {
  font-size: clamp(2.5rem, 6vw, 4.5rem);
  margin-bottom: 1.5rem;
  transform: rotate(-2deg);
}

.con-manifesto p {
  font-size: 1.15rem;
  max-width: 550px;
  margin: 0 auto 2rem;
  opacity: 0.9;
}
```

---

## Design Do's and Don'ts

### Do

- Use diagonal compositions as the primary structural device
- Restrict the palette to red, black, and white with occasional rust/orange accents
- Make typography the dominant visual element; words should shout
- Use bold, condensed, uppercase sans-serif typefaces
- Create angular section dividers with CSS `clip-path` or `transform: skewY()`
- Apply wedge and triangle shapes as directional accents
- Design with urgency and directness; every element should feel purposeful
- Use dark backgrounds for dramatic, poster-like compositions
- Tilt and rotate text blocks for dynamic energy

### Don't

- Use soft, pastel, or muted colors -- the palette is harsh and confrontational
- Create static, symmetrical layouts -- Constructivism is about dynamic tension
- Use rounded corners, circles, or organic shapes as primary elements
- Apply subtle, elegant, or refined typographic treatment
- Use gradients or smooth color transitions
- Include decorative ornament or non-functional visual elements
- Design with generous whitespace or breathing room -- density conveys urgency
- Use serif, script, or decorative typefaces
- Forget the angular and diagonal foundation; horizontal/vertical compositions lose the Constructivist identity

---

## Related Aesthetics

| Aesthetic | Relationship to Constructivism |
|-----------|-------------------------------|
| **Bauhaus** | Contemporary sibling; shared the integration of art and industrial production but with German academic formality |
| **De Stijl** | Parallel reductionist movement; shared geometric abstraction but restricted to horizontals and verticals |
| **Heroic Realism** | Soviet successor; transitioned from abstract Constructivism to figurative propaganda while retaining bold compositional energy |
| **Suprematism** | Russian predecessor; Malevich's pure geometric abstraction laid the groundwork for Constructivist visual language |
| **International Typographic Style** | Descendant; formalized Constructivist typography and grid principles into a systematic design methodology |
| **Plakatstil** | Poster-art relative; shared bold, flat graphics and impactful typography for mass communication |
| **Neubrutalism** | Contemporary echo; shares the raw, bold graphic presence and rejection of polish |
| **Flat Design** | Distant descendant; shares flat color and absence of depth but lacks Constructivism's angular dynamism |
| **DIY Punk** | Spiritual heir; shares the collage aesthetic, anti-establishment energy, and raw, unpolished visual aggression |
| **New Wave** | Postmodern descendant; deconstructed Constructivist grid principles with layering and typographic experimentation |

---

## Quick-Start: Minimal Constructivism Page Template

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Constructivism Page</title>
  <link href="https://fonts.googleapis.com/css2?family=Bebas+Neue&family=Roboto+Condensed:wght@400;700&display=swap" rel="stylesheet">
  <style>
    :root {
      --con-red: #cc0000;
      --con-red-dark: #990000;
      --con-black: #000000;
      --con-off-black: #1a1a1a;
      --con-charcoal: #2d2d2d;
      --con-white: #ffffff;
      --con-off-white: #f2f0eb;
      --con-cream: #e8e0d0;
      --con-steel: #6b6b6b;
    }

    * { margin: 0; padding: 0; box-sizing: border-box; }

    body {
      background: var(--con-off-black);
      color: var(--con-white);
      font-family: 'Roboto Condensed', sans-serif;
      font-weight: 400;
      line-height: 1.7;
    }

    h1, h2, h3 {
      font-family: 'Bebas Neue', sans-serif;
      font-weight: 400;
      text-transform: uppercase;
      letter-spacing: 0.04em;
      line-height: 0.9;
    }

    /* Navigation */
    nav {
      display: flex;
      align-items: center;
      justify-content: space-between;
      background: var(--con-black);
      padding: 0 40px;
      position: relative;
    }

    nav::after {
      content: '';
      position: absolute;
      bottom: 0;
      left: 0;
      width: 180px;
      height: 4px;
      background: var(--con-red);
      transform: skewX(-20deg);
      transform-origin: bottom left;
    }

    nav a.logo {
      font-family: 'Bebas Neue', sans-serif;
      font-size: 1.8rem;
      color: var(--con-red);
      text-decoration: none;
      letter-spacing: 0.1em;
      padding: 20px 0;
    }

    nav ul {
      display: flex;
      gap: 28px;
      list-style: none;
    }

    nav ul a {
      font-family: 'Bebas Neue', sans-serif;
      font-size: 1rem;
      color: var(--con-white);
      text-decoration: none;
      letter-spacing: 0.08em;
      text-transform: uppercase;
      padding: 20px 0;
      transition: color 0.2s;
    }

    nav ul a:hover { color: var(--con-red); }

    /* Hero */
    .hero {
      padding: 100px 40px 120px;
      position: relative;
      overflow: hidden;
    }

    .hero::before {
      content: '';
      position: absolute;
      top: 0;
      right: -80px;
      width: 450px;
      height: 100%;
      background: var(--con-red);
      transform: skewX(-12deg);
      opacity: 0.12;
    }

    .hero-inner {
      max-width: 1200px;
      margin: 0 auto;
      position: relative;
      z-index: 1;
    }

    .hero h1 {
      font-size: clamp(4rem, 10vw, 8rem);
      line-height: 0.85;
      margin-bottom: 1.5rem;
      transform: rotate(-3deg);
      transform-origin: left center;
    }

    .hero h1 .red { color: var(--con-red); }

    .hero p {
      font-size: 1.1rem;
      color: var(--con-steel);
      max-width: 480px;
      margin-bottom: 2.5rem;
    }

    .btn {
      display: inline-block;
      background: var(--con-red);
      color: var(--con-white);
      padding: 14px 40px;
      font-family: 'Bebas Neue', sans-serif;
      font-size: 1.2rem;
      letter-spacing: 0.1em;
      text-transform: uppercase;
      text-decoration: none;
      transform: skewX(-5deg);
      transition: background 0.2s, transform 0.2s;
    }

    .btn span {
      display: inline-block;
      transform: skewX(5deg);
    }

    .btn:hover {
      background: var(--con-red-dark);
      transform: skewX(-5deg) translateY(-2px);
    }

    /* Diagonal stripe divider */
    .stripe {
      height: 50px;
      background: repeating-linear-gradient(
        -45deg,
        var(--con-red),
        var(--con-red) 15px,
        var(--con-black) 15px,
        var(--con-black) 30px
      );
    }

    /* Features */
    .features {
      background: var(--con-off-white);
      color: var(--con-black);
      padding: 80px 40px;
    }

    .features h2 {
      font-size: 3rem;
      color: var(--con-black);
      max-width: 1200px;
      margin: 0 auto 60px;
      position: relative;
      display: inline-block;
    }

    .features h2::after {
      content: '';
      position: absolute;
      bottom: -8px;
      left: 0;
      width: 50px;
      height: 5px;
      background: var(--con-red);
      transform: skewX(-15deg);
    }

    .features-header {
      max-width: 1200px;
      margin: 0 auto;
    }

    .features-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
      gap: 24px;
      max-width: 1200px;
      margin: 0 auto;
    }

    .feature {
      background: var(--con-white);
      padding: 32px;
      border-left: 5px solid var(--con-red);
    }

    .feature-num {
      font-family: 'Bebas Neue', sans-serif;
      font-size: 3rem;
      color: var(--con-cream);
      line-height: 1;
      margin-bottom: 0.5rem;
    }

    .feature h3 {
      font-size: 1.3rem;
      color: var(--con-black);
      margin-bottom: 0.75rem;
    }

    .feature p {
      color: var(--con-steel);
      font-size: 0.95rem;
    }

    /* Manifesto / CTA */
    .manifesto {
      background: var(--con-red);
      color: var(--con-white);
      padding: 100px 40px;
      text-align: center;
      clip-path: polygon(0 6%, 100% 0, 100% 94%, 0 100%);
    }

    .manifesto h2 {
      font-size: clamp(2.5rem, 6vw, 4.5rem);
      margin-bottom: 1.5rem;
      transform: rotate(-2deg);
    }

    .manifesto p {
      font-size: 1.15rem;
      max-width: 520px;
      margin: 0 auto 2rem;
      opacity: 0.9;
    }

    .manifesto .btn {
      background: var(--con-white);
      color: var(--con-red);
    }

    .manifesto .btn:hover {
      background: var(--con-black);
      color: var(--con-white);
    }

    /* Footer */
    footer {
      background: var(--con-black);
      color: var(--con-steel);
      text-align: center;
      padding: 40px;
      font-size: 0.85rem;
      position: relative;
    }

    footer::before {
      content: '';
      position: absolute;
      top: 0;
      left: 0;
      width: 100px;
      height: 4px;
      background: var(--con-red);
    }

    @media (max-width: 768px) {
      .hero { padding: 60px 24px 80px; }
      nav { padding: 0 20px; }
      nav ul { gap: 16px; }
      .features { padding: 60px 24px; }
      .manifesto { padding: 80px 24px; clip-path: polygon(0 3%, 100% 0, 100% 97%, 0 100%); }
    }
  </style>
</head>
<body>
  <nav>
    <a href="#" class="logo">Construct</a>
    <ul>
      <li><a href="#">Manifesto</a></li>
      <li><a href="#">Works</a></li>
      <li><a href="#">Archive</a></li>
      <li><a href="#">Join</a></li>
    </ul>
  </nav>

  <section class="hero">
    <div class="hero-inner">
      <h1><span class="red">Build</span> The<br>New World</h1>
      <p>Art in the service of revolution. Design as construction. Every angle, every line, every word forged with purpose and directed toward the future.</p>
      <a href="#" class="btn"><span>Forward</span></a>
    </div>
  </section>

  <div class="stripe"></div>

  <section class="features">
    <div class="features-header">
      <h2>Principles</h2>
    </div>
    <div class="features-grid">
      <div class="feature">
        <div class="feature-num">01</div>
        <h3>Purpose</h3>
        <p>Art is not decoration. It is a tool for communication, for construction, for transforming society through visual force.</p>
      </div>
      <div class="feature">
        <div class="feature-num">02</div>
        <h3>Dynamism</h3>
        <p>Diagonal energy drives every composition forward. Nothing is static. Every element carries momentum and direction.</p>
      </div>
      <div class="feature">
        <div class="feature-num">03</div>
        <h3>Collective</h3>
        <p>Design serves the many, not the few. Visual clarity ensures the message reaches every eye, every mind.</p>
      </div>
    </div>
  </section>

  <section class="manifesto">
    <h2>Art Into Life</h2>
    <p>The artist is a constructor. The canvas is the street. The medium is the message. Build forward.</p>
    <a href="#" class="btn"><span>Read Manifesto</span></a>
  </section>

  <footer>
    <p>Built on Constructivist principles. Moscow 1921.</p>
  </footer>
</body>
</html>
```
