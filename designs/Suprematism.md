# Suprematism

## Overview

Suprematism is a geometric abstract art movement founded by Kazimir Malevich in 1915, reducing visual expression to its purest forms: squares, circles, crosses, and rectangles floating on infinite white fields. It rejects representational imagery entirely, seeking to convey "the supremacy of pure artistic feeling" through color, shape, and spatial relationships alone. In digital design, Suprematism translates into radically minimal compositions built from bold geometric primitives, stark primary-plus-black palettes, dynamic diagonal axes, and vast white space that functions as infinite depth rather than emptiness.

## Visual Characteristics

### Core Design Traits

- **Pure geometric primitives**: Squares, rectangles, circles, triangles, and crosses used as the sole compositional vocabulary with no illustrative or representational elements
- **Floating on white fields**: Elements appear suspended in a depthless white void, creating a sense of weightlessness and cosmic space
- **Dynamic diagonal axes**: Compositions tilted along diagonal lines create energy and movement within static geometry
- **Bold, flat color fills**: Shapes rendered in solid, unmodulated color with no gradients, textures, or shadows
- **Asymmetric balance**: Elements arranged through dynamic equilibrium rather than symmetrical mirroring, creating tension and motion
- **Scale contrast**: Dramatic differences between large and small elements establish visual hierarchy purely through size
- **No ornamentation**: Total absence of borders, decorative elements, patterns, or embellishment of any kind

### Design Principles

- Reduce every visual element to its most essential geometric form
- Use white space as an active compositional element, not passive emptiness
- Create hierarchy through size, color weight, and position rather than detail or decoration
- Embrace diagonal composition for energy; orthogonal placement for stability
- Limit the palette to a small number of strongly contrasting hues
- Every element must justify its existence; if it can be removed without loss, remove it

## Color Palette

| Swatch | Hex | Role |
|--------|-----|------|
| Suprematist Black | `#1A1A1A` | Primary element color, text, dominant shapes |
| White Field | `#FFFFFF` | Background, infinite space, negative area |
| Malevich Red | `#D42B2B` | Primary accent, dynamic rectangles |
| Primary Yellow | `#F2C41D` | Secondary accent, circles and bars |
| Constructive Blue | `#2456A4` | Tertiary accent, supporting geometry |
| Warm Grey | `#E8E5E0` | Subtle background variation, muted surfaces |
| Deep Green | `#1B6B3A` | Occasional fourth accent (use sparingly) |
| Raw Ochre | `#C8933C` | Earth-tone geometric accent |
| Off-White | `#F8F6F2` | Warm white alternative background |
| Steel Grey | `#4A4A4A` | Secondary text, lighter geometric elements |

### CSS Custom Properties

```css
:root {
  --sup-black: #1A1A1A;
  --sup-white: #FFFFFF;
  --sup-red: #D42B2B;
  --sup-yellow: #F2C41D;
  --sup-blue: #2456A4;
  --sup-warm-grey: #E8E5E0;
  --sup-green: #1B6B3A;
  --sup-ochre: #C8933C;
  --sup-off-white: #F8F6F2;
  --sup-steel: #4A4A4A;
}
```

## Typography

### Recommended Google Fonts

| Font | Weight(s) | Usage | Link |
|------|-----------|-------|------|
| **Inter** | 300, 400, 700, 900 | Primary text; clean, geometric, highly legible | [Inter](https://fonts.google.com/specimen/Inter) |
| **Oswald** | 400, 500, 700 | Condensed headings; vertical emphasis and bold presence | [Oswald](https://fonts.google.com/specimen/Oswald) |
| **Roboto** | 300, 400, 700 | Neutral body text that recedes behind geometric elements | [Roboto](https://fonts.google.com/specimen/Roboto) |
| **Bebas Neue** | 400 | Display headlines; ultra-condensed, architectural | [Bebas Neue](https://fonts.google.com/specimen/Bebas+Neue) |
| **Space Grotesk** | 400, 500, 700 | Geometric sans-serif that echoes the forms of the shapes | [Space Grotesk](https://fonts.google.com/specimen/Space+Grotesk) |

### Font Pairing Suggestions

| Heading | Body | Mood |
|---------|------|------|
| Bebas Neue 400 | Inter 400 | Architectural poster, bold simplicity |
| Oswald 700 | Roboto 300 | Constructivist editorial, structured |
| Space Grotesk 700 | Inter 300 | Geometric harmony, modern gallery |

### CSS Example

```css
@import url('https://fonts.googleapis.com/css2?family=Bebas+Neue&family=Inter:wght@300;400;700;900&display=swap');

body {
  font-family: 'Inter', -apple-system, sans-serif;
  font-size: 1rem;
  line-height: 1.6;
  color: var(--sup-black);
  -webkit-font-smoothing: antialiased;
}

h1, h2, h3 {
  font-family: 'Bebas Neue', 'Oswald', sans-serif;
  font-weight: 400;
  letter-spacing: 0.08em;
  text-transform: uppercase;
  color: var(--sup-black);
}
```

## Layout Principles

- **White as infinite plane**: The white background is not empty space but an active, infinite field on which geometric elements float; it should dominate the composition
- **Diagonal axis composition**: Arrange key elements along a diagonal line from corner to corner to create dynamic tension and visual movement
- **Extreme asymmetry**: Avoid centering and symmetry; position elements at unexpected coordinates to create tension and balance through counterweight
- **Grid as invisible scaffold**: Use a strict underlying grid but allow elements to break and overlap it, creating the appearance of floating freedom within hidden structure
- **Scale as hierarchy**: The largest shape is the most important; use dramatic size differences (4x-10x) between primary and secondary elements
- **Responsive approach**: On mobile, simplify to fewer geometric elements while preserving the dominance of white space and the power of single bold shapes

## CSS / Design Techniques

### Geometric Card

```css
.sup-card {
  background: var(--sup-white);
  border: 2px solid var(--sup-black);
  padding: 40px;
  position: relative;
}

.sup-card::before {
  content: '';
  position: absolute;
  top: -8px;
  left: 16px;
  width: 40px;
  height: 40px;
  background: var(--sup-red);
}
```

### Suprematist Button

```css
.sup-button {
  background: var(--sup-black);
  color: var(--sup-white);
  border: none;
  padding: 16px 40px;
  font-family: 'Bebas Neue', sans-serif;
  font-size: 1.1rem;
  letter-spacing: 0.15em;
  text-transform: uppercase;
  cursor: pointer;
  position: relative;
  transition: background 0.2s ease;
}

.sup-button:hover {
  background: var(--sup-red);
}

.sup-button::after {
  content: '';
  position: absolute;
  bottom: -4px;
  right: -4px;
  width: 100%;
  height: 100%;
  border: 2px solid var(--sup-black);
  z-index: -1;
}
```

### Constructive Navigation

```css
.sup-nav {
  background: var(--sup-white);
  border-bottom: 3px solid var(--sup-black);
  padding: 20px 40px;
  display: flex;
  align-items: center;
  justify-content: space-between;
}

.sup-nav .logo {
  font-family: 'Bebas Neue', sans-serif;
  font-size: 1.5rem;
  letter-spacing: 0.2em;
  text-transform: uppercase;
  color: var(--sup-black);
  text-decoration: none;
  display: flex;
  align-items: center;
  gap: 12px;
}

.sup-nav .logo::before {
  content: '';
  display: inline-block;
  width: 16px;
  height: 16px;
  background: var(--sup-red);
}

.sup-nav a {
  font-family: 'Inter', sans-serif;
  font-size: 0.8rem;
  font-weight: 700;
  letter-spacing: 0.12em;
  text-transform: uppercase;
  color: var(--sup-black);
  text-decoration: none;
  transition: color 0.2s ease;
}

.sup-nav a:hover {
  color: var(--sup-red);
}
```

### Geometric Hero

```css
.sup-hero {
  background: var(--sup-white);
  min-height: 80vh;
  display: flex;
  align-items: center;
  justify-content: center;
  position: relative;
  overflow: hidden;
}

.sup-hero .shape-red {
  position: absolute;
  width: 200px;
  height: 200px;
  background: var(--sup-red);
  top: 10%;
  right: 15%;
  transform: rotate(15deg);
}

.sup-hero .shape-black {
  position: absolute;
  width: 120px;
  height: 120px;
  background: var(--sup-black);
  border-radius: 50%;
  bottom: 20%;
  left: 10%;
}

.sup-hero .shape-yellow {
  position: absolute;
  width: 60px;
  height: 300px;
  background: var(--sup-yellow);
  top: 30%;
  left: 35%;
  transform: rotate(-20deg);
}

.sup-hero .content {
  position: relative;
  z-index: 1;
  text-align: left;
  max-width: 500px;
}

.sup-hero h1 {
  font-family: 'Bebas Neue', sans-serif;
  font-size: 5rem;
  line-height: 0.9;
  letter-spacing: 0.06em;
  text-transform: uppercase;
  color: var(--sup-black);
}
```

### Geometric Divider

```css
.sup-divider {
  display: flex;
  align-items: center;
  gap: 16px;
  margin: 60px 0;
}

.sup-divider::before {
  content: '';
  flex: 1;
  height: 3px;
  background: var(--sup-black);
}

.sup-divider span {
  width: 12px;
  height: 12px;
  background: var(--sup-red);
}

.sup-divider::after {
  content: '';
  flex: 1;
  height: 3px;
  background: var(--sup-black);
}
```

### Cross Element

```css
.sup-cross {
  position: relative;
  width: 60px;
  height: 60px;
}

.sup-cross::before,
.sup-cross::after {
  content: '';
  position: absolute;
  background: var(--sup-black);
}

.sup-cross::before {
  top: 0;
  left: 50%;
  transform: translateX(-50%);
  width: 16px;
  height: 100%;
}

.sup-cross::after {
  top: 50%;
  left: 0;
  transform: translateY(-50%);
  width: 100%;
  height: 16px;
}
```

## Design Do's and Don'ts

### Do

- Use only pure geometric forms: squares, rectangles, circles, triangles, crosses
- Let white space dominate the composition as an active, infinite field
- Create hierarchy exclusively through size, position, and color contrast
- Use diagonal axes and rotation to create dynamic energy
- Limit your palette to 3-4 strongly contrasting colors plus black and white
- Make every element essential; remove anything that does not serve the composition
- Reference Malevich, El Lissitzky, and Constructivist design principles

### Don't

- Add gradients, textures, shadows, or any surface embellishment to geometric shapes
- Use decorative typefaces, script fonts, or ornamental borders
- Fill the white space with content; the void is the canvas
- Apply rounded corners to rectangles (use sharp 90-degree angles)
- Mix representational imagery (photos, illustrations, icons) with abstract geometry
- Create symmetrical, balanced layouts; asymmetric tension is fundamental
- Use more than 4-5 colors; chromatic restraint creates power

## Related Aesthetics

| Aesthetic | Relationship |
|-----------|-------------|
| **Constructivism** | Direct descendant; Constructivism applies Suprematist geometry to functional design, propaganda, and architecture |
| **De Stijl** | Parallel movement using geometric abstraction; De Stijl restricts to right angles and primary colors (Mondrian) |
| **Bauhaus** | Shares geometric purity and functional clarity; Bauhaus synthesizes Suprematism with industrial design and craft |
| **Swiss/International Style** | Inherits the grid discipline and geometric clarity; adds typographic hierarchy and photographic content |
| **Minimalism** | Shares reductive philosophy; Minimalism tends toward monochrome subtlety while Suprematism uses bold color contrast |
| **Brutalism (web)** | Both reject decoration; Brutalism is aggressive and raw while Suprematism is composed and intentional |

## Quick-Start HTML Template

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Suprematism Layout</title>
  <link href="https://fonts.googleapis.com/css2?family=Bebas+Neue&family=Inter:wght@300;400;700&display=swap" rel="stylesheet">
  <style>
    *, *::before, *::after { margin: 0; padding: 0; box-sizing: border-box; }

    body {
      font-family: 'Inter', sans-serif;
      font-size: 1rem;
      line-height: 1.6;
      color: #1A1A1A;
      background: #FFFFFF;
      min-height: 100vh;
    }

    .nav {
      background: #FFFFFF;
      border-bottom: 3px solid #1A1A1A;
      padding: 20px 40px;
      display: flex;
      align-items: center;
      justify-content: space-between;
    }

    .nav .logo {
      font-family: 'Bebas Neue', sans-serif;
      font-size: 1.5rem;
      letter-spacing: 0.2em;
      text-transform: uppercase;
      text-decoration: none;
      color: #1A1A1A;
      display: flex;
      align-items: center;
      gap: 12px;
    }

    .nav .logo::before {
      content: '';
      display: inline-block;
      width: 16px;
      height: 16px;
      background: #D42B2B;
    }

    .nav a {
      font-size: 0.8rem;
      font-weight: 700;
      letter-spacing: 0.12em;
      text-transform: uppercase;
      color: #1A1A1A;
      text-decoration: none;
    }

    .hero {
      background: #FFFFFF;
      min-height: 80vh;
      display: flex;
      align-items: center;
      justify-content: center;
      position: relative;
      overflow: hidden;
    }

    .shape-red {
      position: absolute;
      width: 200px;
      height: 200px;
      background: #D42B2B;
      top: 10%;
      right: 15%;
      transform: rotate(15deg);
    }

    .shape-circle {
      position: absolute;
      width: 120px;
      height: 120px;
      background: #1A1A1A;
      border-radius: 50%;
      bottom: 20%;
      left: 10%;
    }

    .shape-bar {
      position: absolute;
      width: 50px;
      height: 280px;
      background: #F2C41D;
      top: 25%;
      left: 35%;
      transform: rotate(-20deg);
    }

    .shape-blue {
      position: absolute;
      width: 80px;
      height: 80px;
      background: #2456A4;
      bottom: 15%;
      right: 30%;
      transform: rotate(35deg);
    }

    .hero-content {
      position: relative;
      z-index: 1;
      max-width: 480px;
    }

    .hero-content h1 {
      font-family: 'Bebas Neue', sans-serif;
      font-size: 5rem;
      line-height: 0.9;
      letter-spacing: 0.06em;
      text-transform: uppercase;
    }

    .hero-content p {
      font-weight: 300;
      font-size: 1.05rem;
      color: #4A4A4A;
      margin-top: 20px;
      max-width: 360px;
    }

    .content {
      max-width: 960px;
      margin: 80px auto;
      padding: 0 40px;
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 40px;
    }

    .card {
      background: #FFFFFF;
      border: 2px solid #1A1A1A;
      padding: 36px;
      position: relative;
    }

    .card::before {
      content: '';
      position: absolute;
      top: -8px;
      left: 16px;
      width: 32px;
      height: 32px;
      background: #D42B2B;
    }

    .card h2 {
      font-family: 'Bebas Neue', sans-serif;
      font-size: 1.8rem;
      letter-spacing: 0.1em;
      text-transform: uppercase;
      margin-bottom: 12px;
    }

    .card p {
      font-weight: 300;
      color: #4A4A4A;
    }

    .button {
      display: inline-block;
      margin-top: 20px;
      background: #1A1A1A;
      color: #FFFFFF;
      padding: 14px 36px;
      font-family: 'Bebas Neue', sans-serif;
      font-size: 1rem;
      letter-spacing: 0.15em;
      text-transform: uppercase;
      text-decoration: none;
      position: relative;
    }

    .button::after {
      content: '';
      position: absolute;
      bottom: -4px;
      right: -4px;
      width: 100%;
      height: 100%;
      border: 2px solid #1A1A1A;
      z-index: -1;
    }
  </style>
</head>
<body>
  <nav class="nav">
    <a href="#" class="logo">Suprematism</a>
    <div>
      <a href="#">Forms</a>
      <a href="#" style="margin-left:24px;">Space</a>
      <a href="#" style="margin-left:24px;">Color</a>
    </div>
  </nav>
  <header class="hero">
    <div class="shape-red"></div>
    <div class="shape-circle"></div>
    <div class="shape-bar"></div>
    <div class="shape-blue"></div>
    <div class="hero-content">
      <h1>Pure Form</h1>
      <p>Circles, squares, and crosses floating on white fields.
         The supremacy of pure artistic feeling over representation.</p>
    </div>
  </header>
  <main class="content">
    <div class="card">
      <h2>Black Square</h2>
      <p>The zero point of painting. A form reduced to its absolute
         essence, the foundation upon which all composition rests.</p>
      <a href="#" class="button">Explore</a>
    </div>
    <div class="card">
      <h2>Red Rectangle</h2>
      <p>Dynamic tension through color and angle. A tilted plane
         that defies gravity and asserts pure visual energy.</p>
      <a href="#" class="button">Explore</a>
    </div>
  </main>
</body>
</html>
```
