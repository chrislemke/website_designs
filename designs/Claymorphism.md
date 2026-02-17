# Claymorphism Design Reference

Claymorphism is a UI design trend coined by Michal Malewicz (Hype4 Academy) that gives interface elements a **soft, inflated, 3D clay-like appearance**. Elements look as if molded from Play-Doh or clay, floating above the background with puffy, tactile surfaces. Unlike Neumorphism (where elements extrude from the background), claymorphic elements **float on top of the background** using outer shadows for separation and inner shadows for the illusion of volume and inflation.

---

## Visual Characteristics

### Core Design Traits

- **Inflated geometry** -- objects resemble air-filled, softly sculpted forms with chunky, rounded shapes; no sharp edges anywhere
- **Discrete modeled surfaces** -- elements float above backgrounds rather than extruding from them
- **Dual inner shadows + outer shadow** -- the signature CSS technique creating the clay/puffy illusion
- **Strong, vivid color cues** -- bright pastels and vivid hues differentiate interactive elements, improving accessibility over monochromatic approaches
- **Minimal, clean typography** -- bold, rounded typefaces balance the whimsical 3D clay visuals
- **Friendly, tactile aesthetic** -- evokes stuffed toys, balloons, and Play-Doh forms
- **Blob-like formations** -- organic, rounded shapes throughout the UI

### Design Principles

- Every element should look like it could be physically picked up or squeezed
- Maintain clear visual hierarchy despite the 3D effect
- Keep backgrounds light and bright so drop shadows remain effective (dark backgrounds diminish the clay effect)
- Ensure adequate contrast between objects and the background surface
- Respect motion preferences to avoid overwhelming animations
- Use generous padding inside elements to reinforce the "inflated" feeling
- Limit the number of claymorphic layers to prevent visual clutter

---

## Color Palette

### Primary Scheme

Claymorphism demands **bright pastels and vivid colors**. Drop shadows become ineffective on darker variations, so foregrounds and backgrounds should stay in the lighter pastel range.

| Role | Colors | Hex (suggested) |
|------|--------|-----------------|
| **Background** | Soft white, light lavender, light mint | `#F5F5FA`, `#F0EEFF`, `#EEFBF5` |
| **Card surfaces** | White, soft pastels | `#FFFFFF`, `#FFF5F5`, `#F0F4FF` |
| **Primary accent** | Vivid coral / red | `#F76D6D`, `#FF6B6B` |
| **Secondary accent** | Bright sky blue | `#62CDFF`, `#6CB4EE` |
| **Tertiary accent** | Soft purple / lavender | `#D6A2FF`, `#AA3FFE` |
| **Success** | Pastel green | `#7AE582`, `#82D993` |
| **Warm accent** | Soft amber / peach | `#FFB347`, `#FFCBA4` |
| **Text (dark)** | Deep blue-gray | `#2D3557`, `#333652` |
| **Text (light)** | Off-white | `#F1F1F1`, `#FAFAFA` |

### Suggested CSS Custom Properties

```css
:root {
  /* Backgrounds */
  --clay-bg-primary: #f5f5fa;
  --clay-bg-secondary: #eee8ff;
  --clay-bg-tertiary: #eefbf5;

  /* Surface colors (cards, elements) */
  --clay-surface-white: #ffffff;
  --clay-surface-coral: #f76d6d;
  --clay-surface-blue: #62cdff;
  --clay-surface-purple: #d6a2ff;
  --clay-surface-green: #7ae582;
  --clay-surface-peach: #ffb347;
  --clay-surface-pink: #ff9eb5;
  --clay-surface-mint: #a8e6cf;

  /* Text */
  --clay-text-dark: #2d3557;
  --clay-text-medium: #555b7a;
  --clay-text-light: #f1f1f1;

  /* Shadows (base colors for rgba manipulation) */
  --clay-shadow-purple: rgba(170, 63, 254, 0.42);
  --clay-shadow-coral: rgba(247, 109, 109, 0.40);
  --clay-shadow-blue: rgba(98, 205, 255, 0.40);
}
```

### Color Guidelines

- **Always** keep the background lighter than the foreground elements
- Shadow colors should derive from the element's own background color (tinted darker)
- Inner highlight shadow should be a **lighter** tint of the element's color
- Inner depth shadow should be a **darker** shade of the element's color (with 60-70% opacity)
- Outer drop shadow should match the element's hue but with significant transparency (30-50%)

---

## Typography

### Typeface Characteristics

Claymorphism typography should be:

- **Rounded, soft, and friendly** -- matching the organic clay aesthetic
- **Bold weight for headings** -- reinforcing the chunky, inflated feel
- **Clean and legible** -- balancing the whimsical visual style with usability
- **Sans-serif** -- angular serifs clash with the rounded clay forms

### Recommended Web Fonts (Google Fonts)

| Font | Style | Usage |
|------|-------|-------|
| **Nunito** | Rounded sans-serif, soft terminals | Headlines, body text (ideal match for claymorphism) |
| **Nunito Sans** | Clean companion to Nunito | Body text, UI labels |
| **Quicksand** | Rounded geometric sans | Headlines, cards, buttons |
| **Comfortaa** | Rounded geometric, friendly | Display headings, logos |
| **Poppins** | Geometric sans, versatile weights | All-purpose: headings + body |
| **Varela Round** | Single-weight rounded sans | UI elements, labels |
| **DM Sans** | Clean geometric sans | Body text, smaller UI copy |

### Typography CSS Example

```css
/* Import fonts */
@import url('https://fonts.googleapis.com/css2?family=Nunito:wght@400;600;700;800&family=Quicksand:wght@500;600;700&display=swap');

/* Headlines */
h1, h2, h3 {
  font-family: 'Quicksand', 'Nunito', sans-serif;
  font-weight: 700;
  color: var(--clay-text-dark);
  line-height: 1.2;
}

/* Display / Hero text */
.clay-display {
  font-family: 'Quicksand', sans-serif;
  font-size: clamp(2.5rem, 6vw, 5rem);
  font-weight: 700;
  letter-spacing: -0.01em;
  line-height: 1.1;
}

/* Body text */
body {
  font-family: 'Nunito', sans-serif;
  font-weight: 400;
  font-size: 1rem;
  line-height: 1.6;
  color: var(--clay-text-dark);
}

/* Bold UI labels / buttons */
.clay-label {
  font-family: 'Nunito', sans-serif;
  font-weight: 700;
  font-size: 0.95rem;
  letter-spacing: 0.02em;
  text-transform: none; /* avoid uppercase -- it feels too rigid for clay */
}
```

---

## Layout Principles

### Grid and Structure

- **Generous spacing** -- ample padding inside elements (40-60px) and between them; clay elements need room to "breathe"
- **Centered, card-based layouts** -- floating card elements on a soft background
- **Flexible, asymmetric grids** -- avoid rigid formality; slight organic placement enhances the playful feel
- **Large border-radius everywhere** -- 30px to 50px on cards, 16px-24px on buttons, fully rounded (999px) on pills and avatars
- **Stacked vertical layouts** work well; horizontal arrangements should use generous gaps
- **Max-width containers** (900-1100px) prevent elements from stretching too wide

### Section Organization

- Use **soft color transitions** between sections rather than hard dividers
- Group related content in **clay cards** floating on the background
- Create hierarchy through **element size and shadow depth** -- more important items get deeper shadows
- Allow **generous whitespace** -- the clay effect needs visual breathing room
- Navigation and headers can use subtler clay treatment to avoid overwhelming the layout

---

## CSS/Design Techniques

### The Claymorphism Shadow Formula

The core visual effect relies on combining **two inset shadows** (one dark, one light) with **one outer shadow**:

```
box-shadow:
  [outer-x] [outer-y] [outer-blur] [outer-color],        /* depth/float */
  inset [dark-x] [dark-y] [dark-blur] [dark-color],       /* volume/concavity */
  inset [light-x] [light-y] [light-blur] [light-color];   /* highlight/inflation */
```

### Basic Claymorphic Card

```css
.clay-card {
  background: #ffffff;
  border-radius: 40px;
  padding: 48px;
  box-shadow:
    0 35px 68px 0 rgba(145, 112, 201, 0.25),
    inset 0 -8px 16px 0 rgba(145, 112, 201, 0.15),
    inset 0 12px 24px 0 rgba(255, 255, 255, 0.9);
}
```

### Colored Claymorphic Element

```css
.clay-coral {
  background: #f76d6d;
  border-radius: 40px;
  padding: 48px;
  color: #f1f1f1;
  box-shadow:
    12px 12px 24px rgba(200, 80, 80, 0.4),
    inset -8px -8px 16px rgba(180, 50, 50, 0.3),
    inset 8px 8px 16px rgba(255, 180, 180, 0.5);
}
```

### Blue Variation

```css
.clay-blue {
  background: #62cdff;
  border-radius: 40px;
  padding: 48px;
  box-shadow:
    12px 12px 24px rgba(60, 150, 200, 0.35),
    inset -8px -8px 16px rgba(40, 120, 180, 0.3),
    inset 8px 8px 16px rgba(180, 230, 255, 0.6);
}
```

### Purple Variation

```css
.clay-purple {
  background: #d6a2ff;
  border-radius: 48px;
  padding: 48px;
  box-shadow:
    0 35px 68px 0 rgba(170, 63, 254, 0.42),
    inset 0 -8px 16px 0 rgba(140, 40, 220, 0.3),
    inset 0 12px 24px 0 rgba(240, 210, 255, 0.6);
}
```

### Green Variation (HSL approach)

```css
.clay-green {
  background: hsl(120deg 35% 82%);
  border-radius: 50px;
  padding: 50px;
  color: hsl(120deg 5% 35%);
  box-shadow:
    34px 34px 68px hsl(120deg 10% 50%),
    inset -8px -8px 16px hsl(120deg 20% 50% / 0.7),
    inset 0 14px 28px hsl(120deg 20% 95%);
}
```

### Warm Brown Variation

```css
.clay-brown {
  background: rgba(165, 79, 29, 0.6);
  border-radius: 30px;
  padding: 40px;
  box-shadow:
    0.8em 0.8em 2em rgba(165, 79, 29, 0.6),
    inset -0.6em -0.6em 1em rgba(165, 79, 29, 0.6),
    inset 0.4em 0.4em 0.5em rgba(245, 230, 221, 0.6);
}
```

### Claymorphic Button

```css
.clay-button {
  background: var(--clay-surface-coral);
  color: var(--clay-text-light);
  border: none;
  border-radius: 20px;
  padding: 16px 36px;
  font-family: 'Nunito', sans-serif;
  font-weight: 700;
  font-size: 1rem;
  cursor: pointer;
  transition: transform 0.2s ease, box-shadow 0.2s ease;
  box-shadow:
    8px 8px 20px rgba(200, 80, 80, 0.35),
    inset -4px -4px 10px rgba(180, 50, 50, 0.25),
    inset 4px 4px 10px rgba(255, 180, 180, 0.45);
}

.clay-button:hover {
  transform: translateY(-2px);
  box-shadow:
    10px 12px 24px rgba(200, 80, 80, 0.45),
    inset -4px -4px 10px rgba(180, 50, 50, 0.25),
    inset 4px 4px 10px rgba(255, 180, 180, 0.5);
}

.clay-button:active {
  transform: translateY(1px);
  box-shadow:
    4px 4px 12px rgba(200, 80, 80, 0.3),
    inset -6px -6px 14px rgba(180, 50, 50, 0.35),
    inset 6px 6px 14px rgba(255, 180, 180, 0.35);
}
```

### Claymorphic Input Field

```css
.clay-input {
  background: #ffffff;
  border: none;
  border-radius: 20px;
  padding: 16px 24px;
  font-family: 'Nunito', sans-serif;
  font-size: 1rem;
  color: var(--clay-text-dark);
  outline: none;
  box-shadow:
    6px 6px 16px rgba(145, 112, 201, 0.15),
    inset -4px -4px 8px rgba(145, 112, 201, 0.08),
    inset 4px 4px 8px rgba(255, 255, 255, 0.8);
}

.clay-input:focus {
  box-shadow:
    8px 8px 20px rgba(145, 112, 201, 0.25),
    inset -4px -4px 10px rgba(145, 112, 201, 0.12),
    inset 4px 4px 10px rgba(255, 255, 255, 0.9);
}
```

### Claymorphism + Glassmorphism Hybrid

Combining clay shadows with glass transparency for a layered effect:

```css
.clay-glass {
  background: rgba(255, 255, 255, 0.4);
  backdrop-filter: blur(15px);
  -webkit-backdrop-filter: blur(15px);
  border-radius: 30px;
  padding: 48px;
  box-shadow:
    0 35px 68px 0 rgba(170, 63, 254, 0.42),
    inset 0 -8px 16px 0 #d6a2ff;
}
```

### Drop Shadow Alternative (for non-rectangular shapes)

```css
.clay-shape {
  filter: drop-shadow(34px 34px 34px hsl(120deg 10% 50%));
}
```

### Using clay.css Library

For rapid prototyping, the `clay.css` micro-library provides a single `.clay` class with CSS custom properties:

```html
<link rel="stylesheet" href="https://unpkg.com/claymorphism-css/dist/clay.css"/>

<div class="clay" style="
  --clay-background: #f76d6d;
  --clay-border-radius: 48px;
  padding: 48px;
  color: #f1f1f1;
">
  Content here
</div>
```

Available CSS variables:
- `--clay-background` -- element background color
- `--clay-border-radius` -- corner rounding
- `--clay-shadow-outset` -- outer shadow value
- `--clay-shadow-inset-primary` -- first inset shadow
- `--clay-shadow-inset-secondary` -- second inset shadow

### Tailwind CSS Configuration

```javascript
// tailwind.config.js
module.exports = {
  theme: {
    extend: {
      boxShadow: {
        'clay-card': `
          inset -10px -10px 20px hsl(302deg 25% 50% / 0.7),
          inset 0 16px 32px hsl(302deg 25% 95%)
        `,
        'clay-btn': `
          16px 16px 32px 0 hsl(277deg 50% 65% / 0.5),
          inset -16px -16px 32px 0 hsl(277deg 50% 65%),
          inset 8px 8px 16px 0 hsl(227deg 65% 75% / 0.45)
        `,
      },
      dropShadow: {
        'clay': '35px 35px 35px hsl(302deg 25% 50%)',
      },
      borderRadius: {
        'clay': '40px',
        'clay-lg': '50px',
      },
    },
  },
};
```

---

## Shadow Construction Guide

Building claymorphic shadows from any base color requires three shadow layers:

| Layer | Direction | Purpose | Color Derivation |
|-------|-----------|---------|-----------------|
| **Outer shadow** | Positive X/Y (e.g. `12px 12px`) | Creates floating/depth effect | Base color darkened, 30-45% opacity |
| **Inset dark** | Negative X/Y (e.g. `inset -8px -8px`) | Creates concavity/volume | Base color darkened 20-30%, 30-70% opacity |
| **Inset light** | Positive X/Y (e.g. `inset 8px 8px`) | Creates highlight/inflation | Base color lightened heavily, 50-90% opacity |

### Shadow Recipe for Any Color

```css
/* Given a base color, e.g. #62CDFF (blue): */
.clay-element {
  background: #62CDFF;                    /* base color */
  border-radius: 40px;                    /* generous rounding */
  box-shadow:
    12px 12px 24px rgba(50, 140, 200, 0.35),     /* outer: darker hue, ~35% opacity */
    inset -8px -8px 16px rgba(30, 110, 170, 0.3), /* inset dark: much darker, ~30% opacity */
    inset 8px 8px 16px rgba(180, 230, 255, 0.6);  /* inset light: very light tint, ~60% opacity */
}
```

---

## Related Aesthetics

| Aesthetic | Relationship to Claymorphism |
|-----------|------------------------------|
| **Neumorphism** | Predecessor; elements extrude from background vs. claymorphism where they float above it; neumorphism is monochromatic while claymorphism uses vivid colors |
| **Glassmorphism** | Contemporary; uses transparency and blur vs. claymorphism's opaque, inflated surfaces; they can be combined |
| **Skeuomorphism** | Ancestor; claymorphism borrows the tactile, physical-object metaphor but abstracts it into playful clay forms |
| **Corporate Memphis** | Shares the friendly, colorful, rounded illustration style; often paired with claymorphic UI elements |
| **Minimalism** | Claymorphism applies minimalist content principles with maximum surface treatment |

---

## Quick-Start: Minimal Claymorphism Page Template

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Claymorphism Page</title>
  <link href="https://fonts.googleapis.com/css2?family=Nunito:wght@400;600;700;800&family=Quicksand:wght@500;600;700&display=swap" rel="stylesheet">
  <style>
    :root {
      --clay-bg: #f0eeff;
      --clay-text: #2d3557;
      --clay-surface: #ffffff;
      --clay-coral: #f76d6d;
      --clay-blue: #62cdff;
      --clay-purple: #d6a2ff;
    }

    * { margin: 0; padding: 0; box-sizing: border-box; }

    body {
      background: var(--clay-bg);
      color: var(--clay-text);
      font-family: 'Nunito', sans-serif;
      font-weight: 400;
      line-height: 1.6;
      min-height: 100vh;
      display: flex;
      flex-direction: column;
      align-items: center;
      padding: 4rem 2rem;
      gap: 3rem;
    }

    h1, h2, h3 {
      font-family: 'Quicksand', sans-serif;
      font-weight: 700;
    }

    .hero {
      text-align: center;
      padding: 3rem;
    }

    .hero h1 {
      font-size: clamp(2.5rem, 6vw, 4.5rem);
      line-height: 1.1;
      margin-bottom: 1rem;
    }

    .clay-card {
      background: var(--clay-surface);
      border-radius: 40px;
      padding: 48px;
      max-width: 600px;
      width: 100%;
      box-shadow:
        0 30px 60px rgba(145, 112, 201, 0.2),
        inset 0 -6px 12px rgba(145, 112, 201, 0.1),
        inset 0 10px 20px rgba(255, 255, 255, 0.9);
    }

    .clay-card h2 {
      margin-bottom: 1rem;
    }

    .clay-button {
      display: inline-block;
      background: var(--clay-coral);
      color: #f1f1f1;
      border: none;
      border-radius: 20px;
      padding: 14px 32px;
      font-family: 'Nunito', sans-serif;
      font-weight: 700;
      font-size: 1rem;
      cursor: pointer;
      margin-top: 1.5rem;
      transition: transform 0.2s ease, box-shadow 0.2s ease;
      box-shadow:
        8px 8px 20px rgba(200, 80, 80, 0.35),
        inset -4px -4px 10px rgba(180, 50, 50, 0.25),
        inset 4px 4px 10px rgba(255, 180, 180, 0.45);
    }

    .clay-button:hover {
      transform: translateY(-2px);
    }
  </style>
</head>
<body>
  <div class="hero">
    <h1>Claymorphism</h1>
    <p>Soft, puffy, and delightfully tactile UI design</p>
  </div>
  <div class="clay-card">
    <h2>Hello, Clay World</h2>
    <p>This card demonstrates the core claymorphic effect: an outer shadow for floating depth, an inner dark shadow for volume, and an inner light shadow for the inflated highlight.</p>
    <button class="clay-button">Touch Me</button>
  </div>
</body>
</html>
```
