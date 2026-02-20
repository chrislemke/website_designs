# Metro Design

## Overview

Metro Design is Microsoft's influential design language, originally developed for Windows Phone 7 and later expanded to Windows 8, Xbox, and the broader Microsoft ecosystem. Rooted in the principles of Swiss graphic design (International Typographic Style), Metro emphasizes bold typography, flat colored tiles, clean grid-based layouts, and a radical "content before chrome" philosophy that strips away decorative elements in favor of information density and clarity. The aesthetic draws direct inspiration from public transit signage systems — especially the clean wayfinding graphics of European metro stations — prioritizing instant legibility and purposeful use of whitespace. Metro was considered revolutionary upon its 2010 debut for rejecting the skeuomorphic trends dominant at the time, instead championing a purely digital visual identity built on geometric shapes, vivid accent colors against neutral backgrounds, and kinetic typography. Its influence extends far beyond Microsoft products, helping catalyze the broader industry shift toward flat design that defined the mid-2010s web and mobile landscape.

## Visual Characteristics

### Core Design Traits

- **Flat Colored Tiles**: Rectangular tiles in bold, saturated accent colors serve as the primary interactive and navigational elements, replacing traditional icons and buttons with information-rich surfaces
- **Typography-Driven Hierarchy**: Oversized, lightweight sans-serif headings (originally Segoe UI) create dramatic visual hierarchy, with text itself functioning as the primary design element rather than imagery or ornamentation
- **Content Before Chrome**: UI decorations, borders, gradients, and textures are eliminated in favor of letting actual content — text, images, data — serve as the interface itself
- **Bold Accent Colors**: A carefully curated palette of vivid accent colors is used sparingly against predominantly dark or white backgrounds, creating high-contrast focal points and brand identity
- **Grid-Based Layout**: A strict underlying grid (originally based on 20px units with 5px subunits) governs all element placement, ensuring mathematical precision and visual harmony across the interface
- **Panoramic Canvas**: Horizontally scrolling layouts extend beyond the viewport, encouraging lateral exploration and creating an expansive sense of space within the interface
- **Motion and Transitions**: Purposeful animations — tiles flipping, content sliding, elements scaling — communicate state changes and spatial relationships, giving the flat interface a sense of depth through movement rather than visual decoration

### Design Principles

- **Pride in Craftsmanship**: Every pixel and typographic detail is intentional; the design celebrates precision, alignment, and the beauty of well-set type on a clean canvas
- **Be Fast and Fluid**: Responsive interactions and smooth transitions create a sense of immediacy; the interface should feel alive and reactive to user input at all times
- **Authentically Digital**: Rather than mimicking physical materials, Metro embraces its digital nature with purely screen-native elements — flat color fields, scalable vector shapes, and resolution-independent typography
- **Do More With Less**: Ruthless reduction of visual noise ensures that every element on screen earns its place; negative space is treated as an active design component, not empty filler
- **Win As One**: Consistency across the entire ecosystem means shared grid systems, color palettes, typography, and interaction patterns so users feel at home whether on phone, tablet, desktop, or console

## Color Palette

The Metro palette features vibrant, saturated accent colors designed for maximum contrast against dark (#1d1d1d) or light (#ffffff) backgrounds. Each color is intended for use as a tile background, accent highlight, or status indicator.

| Swatch | Hex | Role |
|--------|-----|------|
| ![#2d89ef](https://via.placeholder.com/20/2d89ef/2d89ef.png) | `#2d89ef` | Primary Blue — default accent, links, active states |
| ![#1d1d1d](https://via.placeholder.com/20/1d1d1d/1d1d1d.png) | `#1d1d1d` | Dark Background — primary dark theme base |
| ![#ffffff](https://via.placeholder.com/20/ffffff/ffffff.png) | `#ffffff` | Light Background — primary light theme base |
| ![#00aba9](https://via.placeholder.com/20/00aba9/00aba9.png) | `#00aba9` | Teal — secondary accent, highlights |
| ![#e51400](https://via.placeholder.com/20/e51400/e51400.png) | `#e51400` | Red — alerts, errors, destructive actions |
| ![#ff0097](https://via.placeholder.com/20/ff0097/ff0097.png) | `#ff0097` | Magenta — accent tiles, branding |
| ![#00a300](https://via.placeholder.com/20/00a300/00a300.png) | `#00a300` | Green — success states, confirmation |
| ![#9f00a7](https://via.placeholder.com/20/9f00a7/9f00a7.png) | `#9f00a7` | Purple — featured content, highlights |
| ![#ffc40d](https://via.placeholder.com/20/ffc40d/ffc40d.png) | `#ffc40d` | Yellow — warnings, attention |
| ![#da532c](https://via.placeholder.com/20/da532c/da532c.png) | `#da532c` | Orange — secondary alerts, categories |
| ![#2b5797](https://via.placeholder.com/20/2b5797/2b5797.png) | `#2b5797` | Dark Blue — navigation, headers |
| ![#603cba](https://via.placeholder.com/20/603cba/603cba.png) | `#603cba` | Dark Purple — accent variation, tags |

### CSS Custom Properties

```css
:root {
  --metro-blue: #2d89ef;
  --metro-dark: #1d1d1d;
  --metro-white: #ffffff;
  --metro-teal: #00aba9;
  --metro-red: #e51400;
  --metro-magenta: #ff0097;
  --metro-green: #00a300;
  --metro-purple: #9f00a7;
  --metro-yellow: #ffc40d;
  --metro-orange: #da532c;
  --metro-dark-blue: #2b5797;
  --metro-dark-purple: #603cba;
  --metro-gray-100: #f5f5f5;
  --metro-gray-200: #e0e0e0;
  --metro-gray-300: #b3b3b3;
  --metro-gray-500: #7a7a7a;
  --metro-gray-700: #3a3a3a;
  --metro-gray-900: #1d1d1d;
  --metro-accent: var(--metro-blue);
  --metro-unit: 20px;
  --metro-subunit: 5px;
  --metro-gutter: 10px;
  --metro-tile-gap: 10px;
}
```

## Typography

Metro Design's typographic approach is its most distinctive feature. Text is used at dramatically large sizes with light font weights, creating hierarchy through scale rather than decoration. The original system used Segoe UI, but several excellent Google Fonts alternatives capture the same clean, humanist sans-serif character.

### Recommended Google Fonts

| Font | Weight(s) | Usage | Link |
|------|-----------|-------|------|
| Open Sans | 300, 400, 600, 700 | Primary UI text, body copy — closest free match to Segoe UI | [Google Fonts](https://fonts.google.com/specimen/Open+Sans) |
| Roboto | 100, 300, 400, 500, 700 | Alternative primary — clean geometric sans-serif | [Google Fonts](https://fonts.google.com/specimen/Roboto) |
| Raleway | 100, 200, 300, 400, 600 | Display headings — ultralight weights for oversized thin type | [Google Fonts](https://fonts.google.com/specimen/Raleway) |
| Source Sans 3 | 200, 300, 400, 600, 700 | Body text and UI labels — designed for digital interfaces | [Google Fonts](https://fonts.google.com/specimen/Source+Sans+3) |
| Noto Sans | 300, 400, 500, 700 | Multilingual support — Metro consistency across all scripts | [Google Fonts](https://fonts.google.com/specimen/Noto+Sans) |

### Font Pairing Suggestions

| Heading | Body | Vibe |
|---------|------|------|
| Raleway (200) | Open Sans (300, 400) | Classic Metro — ultralight display headings with readable body text, closest to original Windows 8 aesthetic |
| Roboto (100, 300) | Roboto (400) | Unified System — single-family approach mirrors how Segoe UI was used across all weight ranges |
| Raleway (100) | Source Sans 3 (300, 400) | Editorial Metro — dramatic thin headlines paired with structured body for content-heavy layouts |

### CSS Example

```css
@import url('https://fonts.googleapis.com/css2?family=Open+Sans:wght@300;400;600;700&family=Raleway:wght@100;200;300;400;600&display=swap');

body {
  font-family: 'Open Sans', 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
  font-weight: 300;
  font-size: 15px;
  line-height: 1.6;
  color: var(--metro-dark);
  -webkit-font-smoothing: antialiased;
}

h1 {
  font-family: 'Raleway', 'Segoe UI Light', sans-serif;
  font-weight: 100;
  font-size: 3.5rem;
  line-height: 1.1;
  letter-spacing: -0.02em;
  text-transform: lowercase;
}

h2 {
  font-family: 'Raleway', 'Segoe UI Light', sans-serif;
  font-weight: 200;
  font-size: 2.25rem;
  line-height: 1.2;
}

h3 {
  font-family: 'Open Sans', 'Segoe UI', sans-serif;
  font-weight: 300;
  font-size: 1.5rem;
  line-height: 1.3;
}

h4 {
  font-family: 'Open Sans', 'Segoe UI', sans-serif;
  font-weight: 600;
  font-size: 0.85rem;
  text-transform: uppercase;
  letter-spacing: 0.1em;
}

p {
  font-weight: 300;
  line-height: 1.7;
  max-width: 65ch;
}

.caption {
  font-size: 0.8rem;
  font-weight: 400;
  color: var(--metro-gray-500);
  text-transform: uppercase;
  letter-spacing: 0.05em;
}
```

## Layout Principles

- **Strict Grid Alignment**: All elements snap to a base grid of 20px units (with 5px subunits for fine-tuning), ensuring mathematical consistency across tiles, margins, gutters, and content positioning
- **Edge-to-Edge Tiles**: Tiles extend fully to their container boundaries with minimal gaps (typically 10px), creating a dense mosaic of color and information that maximizes screen real estate
- **Asymmetric Hierarchy**: Layout uses deliberate asymmetry — oversized headlines aligned left, varying tile sizes in a single row — to create visual interest and guide the eye through content priority
- **Horizontal Scrolling Panoramas**: Content extends beyond the right edge of the viewport, inviting lateral exploration; section headers remain visible as landmarks while content panels scroll beneath them
- **Generous Left Margin**: A consistent, wide left margin (40-80px) anchors content and provides breathing room, echoing Swiss design posters and transit signage
- **Responsive Tile Reflow**: Tile grids collapse from multi-column to single columns fluidly, with tiles maintaining their aspect ratios and relative size relationships across breakpoints
- **Flat Depth Through Layering**: Without shadows or gradients, depth is communicated through z-ordering, scale changes on interaction, and overlapping panels that slide in from screen edges

## CSS / Design Techniques

### Tile Grid

The fundamental Metro layout pattern: a responsive grid of uniformly-spaced, flat-colored tiles in various sizes.

```css
.tile-grid {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(150px, 1fr));
  gap: var(--metro-tile-gap);
  padding: var(--metro-gutter);
}

.tile {
  aspect-ratio: 1 / 1;
  background-color: var(--metro-blue);
  color: #fff;
  padding: 15px;
  display: flex;
  flex-direction: column;
  justify-content: flex-end;
  cursor: pointer;
  overflow: hidden;
  transition: opacity 0.15s ease;
}

.tile:hover { opacity: 0.85; }
.tile:active { transform: scale(0.97); }
.tile--wide { grid-column: span 2; aspect-ratio: 2 / 1; }
.tile--large { grid-column: span 2; grid-row: span 2; }

.tile__icon { font-size: 2.5rem; margin-bottom: auto; }
.tile__label { font-weight: 300; font-size: 0.9rem; }
.tile__count { font-family: 'Raleway', sans-serif; font-weight: 200; font-size: 2.5rem; line-height: 1; }
```

### Live Tile Animation

Metro's distinctive tile-flip animation that reveals updating content, mimicking the Windows Phone/8 live tile behavior.

```css
.live-tile {
  perspective: 800px;
}

.live-tile__inner {
  width: 100%; height: 100%;
  transform-style: preserve-3d;
  animation: tileFlip 8s ease-in-out infinite;
}

.live-tile__front,
.live-tile__back {
  position: absolute;
  inset: 0;
  backface-visibility: hidden;
  display: flex;
  flex-direction: column;
  justify-content: flex-end;
  padding: 15px;
}

.live-tile__back { transform: rotateX(180deg); }

@keyframes tileFlip {
  0%, 40%  { transform: rotateX(0deg); }
  50%, 90% { transform: rotateX(180deg); }
  100%     { transform: rotateX(360deg); }
}

/* Slide-up variant */
.live-tile--slide .live-tile__inner {
  animation: tileSlideUp 6s ease-in-out infinite;
}

@keyframes tileSlideUp {
  0%, 35%  { transform: translateY(0); }
  45%, 85% { transform: translateY(-100%); }
  95%, 100%{ transform: translateY(0); }
}
```

### Card

Metro cards are flatter and more minimal than typical card patterns — no shadows, no rounded corners, just a left accent border with typographic content.

```css
.metro-card {
  background-color: var(--metro-white);
  border-left: 4px solid var(--metro-accent);
  padding: 25px 20px;
  margin-bottom: var(--metro-gutter);
  transition: border-color 0.2s ease;
}

.metro-card:hover { border-left-color: var(--metro-teal); }

.metro-card__category {
  font-size: 0.75rem; font-weight: 600;
  text-transform: uppercase; letter-spacing: 0.1em;
  color: var(--metro-gray-500); margin-bottom: 8px;
}

.metro-card__title {
  font-family: 'Raleway', sans-serif; font-weight: 200;
  font-size: 1.5rem; line-height: 1.3; margin-bottom: 10px;
}

.metro-card__body {
  font-weight: 300; font-size: 0.95rem;
  line-height: 1.6; color: var(--metro-gray-500);
}

.metro-card--dark {
  background-color: var(--metro-gray-700);
  border-left-color: var(--metro-magenta);
}
.metro-card--dark .metro-card__title { color: #fff; }
.metro-card--dark .metro-card__body { color: var(--metro-gray-300); }
```

### Button

Metro buttons are flat rectangles with no border-radius. Interaction states rely on opacity and color shifts rather than shadows.

```css
.metro-btn {
  display: inline-flex;
  align-items: center; justify-content: center;
  gap: 8px; padding: 10px 24px;
  border: 2px solid var(--metro-accent);
  background: transparent;
  color: var(--metro-accent);
  font-family: 'Open Sans', 'Segoe UI', sans-serif;
  font-weight: 400; font-size: 0.9rem;
  cursor: pointer; border-radius: 0;
  transition: background-color 0.15s ease, color 0.15s ease;
}

.metro-btn:hover { background-color: var(--metro-accent); color: #fff; }
.metro-btn:active { opacity: 0.8; }

.metro-btn--filled { background-color: var(--metro-accent); color: #fff; border-color: var(--metro-accent); }
.metro-btn--filled:hover { opacity: 0.85; }
.metro-btn--large { padding: 14px 36px; font-size: 1.05rem; font-weight: 300; }
.metro-btn--dark { border-color: #fff; color: #fff; }
.metro-btn--dark:hover { background-color: #fff; color: var(--metro-dark); }
```

### Navigation

Metro navigation uses flat, text-based tabs. No background fills on items — only an accent-colored bottom border for the active state.

```css
.metro-nav {
  display: flex; align-items: center;
  padding: 0 40px; height: 48px;
  background-color: var(--metro-dark);
}

.metro-nav__brand {
  font-family: 'Raleway', sans-serif; font-weight: 200;
  font-size: 1.2rem; color: #fff;
  margin-right: 40px; text-transform: lowercase;
}

.metro-nav__links {
  display: flex; list-style: none;
  margin: 0; padding: 0; height: 100%;
}

.metro-nav__link {
  display: flex; align-items: center; height: 100%;
  padding: 0 20px; color: var(--metro-gray-300);
  text-decoration: none; font-size: 0.85rem;
  text-transform: uppercase; letter-spacing: 0.05em;
  border-bottom: 2px solid transparent;
  transition: color 0.2s, border-color 0.2s;
}

.metro-nav__link:hover { color: #fff; }
.metro-nav__link--active { color: #fff; border-bottom-color: var(--metro-accent); }
```

### Hero Section

A bold, typographic hero that uses Metro's oversized lightweight text and a strong accent color field.

```css
.metro-hero {
  background-color: var(--metro-dark);
  color: #fff;
  padding: 80px 40px 60px;
  position: relative; overflow: hidden;
}

.metro-hero__accent-bar {
  position: absolute; top: 0; left: 0;
  width: 100%; height: 4px;
  background-color: var(--metro-accent);
}

.metro-hero__category {
  font-size: 0.75rem; font-weight: 600;
  text-transform: uppercase; letter-spacing: 0.15em;
  color: var(--metro-accent); margin-bottom: 20px;
}

.metro-hero__title {
  font-family: 'Raleway', sans-serif; font-weight: 100;
  font-size: clamp(2.5rem, 6vw, 5rem);
  line-height: 1.05; letter-spacing: -0.03em;
  max-width: 800px; margin-bottom: 24px;
  text-transform: lowercase;
}

.metro-hero__subtitle {
  font-weight: 300; font-size: 1.15rem; line-height: 1.6;
  max-width: 550px; color: var(--metro-gray-300); margin-bottom: 36px;
}

.metro-hero__block {
  position: absolute; right: -60px; bottom: -60px;
  width: 300px; height: 300px;
  background-color: var(--metro-accent);
  opacity: 0.08; transform: rotate(15deg);
}
```

### App Bar

The Metro app bar is a bottom-anchored command bar with circular icon buttons — a distinctive pattern from Windows Phone and Windows 8 apps.

```css
.metro-appbar {
  position: fixed; bottom: 0; left: 0; right: 0;
  height: 72px;
  background-color: var(--metro-dark);
  display: flex; align-items: center; justify-content: center;
  gap: 24px; padding: 0 20px;
  z-index: 1000;
  border-top: 1px solid var(--metro-gray-700);
  transform: translateY(100%);
  transition: transform 0.3s ease;
}

.metro-appbar--visible { transform: translateY(0); }

.metro-appbar__btn {
  display: flex; flex-direction: column; align-items: center;
  gap: 4px; background: none; border: none;
  color: #fff; cursor: pointer;
}

.metro-appbar__icon {
  width: 40px; height: 40px;
  border: 2px solid #fff; border-radius: 50%;
  display: flex; align-items: center; justify-content: center;
  font-size: 1.1rem;
}

.metro-appbar__label {
  font-size: 0.65rem; text-transform: lowercase;
}
```

## Design Do's and Don'ts

### Do's

- **Do use oversized, lightweight typography** as the primary visual element — let headings at 100-200 weight dominate the visual hierarchy and set the Metro tone
- **Do embrace generous whitespace** around text and tiles; negative space is an essential compositional element that gives content room to breathe
- **Do maintain strict grid alignment** for all elements; every tile, margin, and gutter should snap to the base grid for mathematical precision
- **Do use a single accent color consistently** throughout a section, changing it only to signal different contexts or user-selected personalization
- **Do keep animations purposeful and swift** — slide transitions, tile flips, and scale changes should communicate state changes, never merely decorate
- **Do design for touch-first interaction** with generously sized tap targets (minimum 44px), adequate spacing, and clear pressed/active states
- **Do use flat, solid-color backgrounds** for tiles and UI surfaces; the power of Metro comes from bold color blocks, crisp typography, and open space

### Don'ts

- **Don't add drop shadows, gradients, or textures** — these directly contradict Metro's "authentically digital" principle and reintroduce skeuomorphic decoration
- **Don't use rounded corners on primary elements** — Metro tiles, buttons, and cards are sharp rectangles; border-radius undermines the geometric precision
- **Don't overcrowd the layout with content** — Metro's power comes from restraint; if every space is filled, the hierarchy collapses into visual noise
- **Don't rely on icons alone without text labels** — Metro prioritizes typographic clarity; icons should supplement text, not replace it
- **Don't use more than two or three accent colors** in a single view — the palette is vibrant but should be deployed with discipline to maintain focus
- **Don't center-align body text or headings** — Metro's typographic system is rooted in left-aligned, flush-left composition drawn from Swiss design traditions
- **Don't add decorative borders or dividers** between sections — use whitespace, color changes, and typographic scale shifts to separate content areas

## Related Aesthetics

| Aesthetic | Relationship |
|-----------|-------------|
| [Flat Design](Flat_Design.md) | Metro was one of the earliest and most influential implementations of flat design, directly inspiring the broader movement from 2012 onward |
| [International Typographic Style](International_Typographic_Style.md) | Metro's direct ancestor — Swiss grid systems, sans-serif emphasis, and content-first philosophy are inherited from mid-century Swiss graphic design |
| [Minimalism](Minimalism.md) | Shares Metro's commitment to reduction, though Metro is more color-forward and tile-structured than pure minimalism's neutral austerity |
| [Bauhaus](Bauhaus.md) | Metro echoes Bauhaus principles of form following function, geometric purity, and integrated design across media |
| [Neubrutalism](Neubrutalism.md) | Both reject decoration in favor of raw, honest interface elements — Neubrutalism is Metro's bolder, more irreverent cousin |
| [Bento Grid](Bento_Grid.md) | Metro's tile-based grid layout directly anticipates the Bento Grid trend with modular, varied-size rectangular containers |

## Quick-Start HTML Template

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Metro Design</title>
  <link href="https://fonts.googleapis.com/css2?family=Open+Sans:wght@300;400;600;700&family=Raleway:wght@100;200;300;400;600&display=swap" rel="stylesheet">
  <style>
    *, *::before, *::after { margin: 0; padding: 0; box-sizing: border-box; }

    :root {
      --metro-blue: #2d89ef; --metro-dark: #1d1d1d; --metro-white: #ffffff;
      --metro-teal: #00aba9; --metro-red: #e51400; --metro-magenta: #ff0097;
      --metro-green: #00a300; --metro-purple: #9f00a7; --metro-yellow: #ffc40d;
      --metro-orange: #da532c; --metro-dark-blue: #2b5797; --metro-dark-purple: #603cba;
      --metro-gray-100: #f5f5f5; --metro-gray-300: #b3b3b3;
      --metro-gray-500: #7a7a7a; --metro-gray-700: #3a3a3a;
      --metro-accent: var(--metro-blue); --metro-gutter: 10px;
    }

    html { scroll-behavior: smooth; }
    body {
      font-family: 'Open Sans', 'Segoe UI', sans-serif;
      font-weight: 300; font-size: 15px; line-height: 1.6;
      color: var(--metro-dark); background: var(--metro-gray-100);
      -webkit-font-smoothing: antialiased;
    }

    /* --- Navigation --- */
    .nav {
      display: flex; align-items: center; padding: 0 40px; height: 48px;
      background: var(--metro-dark); position: sticky; top: 0; z-index: 100;
    }
    .nav__brand {
      font-family: 'Raleway', sans-serif; font-weight: 200; font-size: 1.2rem;
      color: #fff; text-decoration: none; margin-right: 40px; text-transform: lowercase;
    }
    .nav__links { display: flex; list-style: none; height: 100%; }
    .nav__link {
      display: flex; align-items: center; height: 48px; padding: 0 20px;
      color: var(--metro-gray-300); text-decoration: none; font-size: 0.8rem;
      font-weight: 400; text-transform: uppercase; letter-spacing: 0.06em;
      border-bottom: 2px solid transparent; transition: color 0.2s, border-color 0.2s;
    }
    .nav__link:hover, .nav__link--active {
      color: #fff; border-bottom-color: var(--metro-accent);
    }

    /* --- Hero --- */
    .hero {
      background: var(--metro-dark); color: #fff;
      padding: 80px 40px 70px; position: relative; overflow: hidden;
    }
    .hero__bar { position: absolute; top: 0; left: 0; width: 100%; height: 4px; background: var(--metro-accent); }
    .hero__category {
      font-size: 0.72rem; font-weight: 600; text-transform: uppercase;
      letter-spacing: 0.15em; color: var(--metro-accent); margin-bottom: 20px;
    }
    .hero__title {
      font-family: 'Raleway', sans-serif; font-weight: 100;
      font-size: clamp(2.5rem, 6vw, 4.8rem); line-height: 1.05;
      letter-spacing: -0.03em; text-transform: lowercase; max-width: 750px; margin-bottom: 20px;
    }
    .hero__sub {
      font-weight: 300; font-size: 1.1rem; line-height: 1.65;
      color: var(--metro-gray-300); max-width: 520px; margin-bottom: 36px;
    }
    .hero__actions { display: flex; gap: 12px; flex-wrap: wrap; }
    .hero__block {
      position: absolute; right: -80px; bottom: -80px;
      width: 340px; height: 340px; background: var(--metro-accent);
      opacity: 0.07; transform: rotate(15deg);
    }

    /* --- Buttons --- */
    .btn {
      display: inline-flex; align-items: center; padding: 10px 26px;
      border: 2px solid #fff; background: transparent; color: #fff;
      font-family: 'Open Sans', sans-serif; font-weight: 400; font-size: 0.88rem;
      cursor: pointer; border-radius: 0; text-decoration: none;
      transition: background 0.15s, color 0.15s;
    }
    .btn:hover { background: #fff; color: var(--metro-dark); }
    .btn--filled { background: var(--metro-accent); border-color: var(--metro-accent); }
    .btn--filled:hover { opacity: 0.85; color: #fff; background: var(--metro-accent); }
    .btn--large { padding: 13px 34px; font-size: 1rem; font-weight: 300; }

    /* --- Sections --- */
    .section { padding: 60px 40px; }
    .section--dark { background: var(--metro-dark); color: #fff; }
    .section__cat {
      font-size: 0.72rem; font-weight: 600; text-transform: uppercase;
      letter-spacing: 0.15em; color: var(--metro-accent); margin-bottom: 10px;
    }
    .section__title {
      font-family: 'Raleway', sans-serif; font-weight: 200;
      font-size: 2.25rem; line-height: 1.2; margin-bottom: 12px;
    }
    .section__sub {
      font-weight: 300; color: var(--metro-gray-500); max-width: 550px; margin-bottom: 40px;
    }
    .section--dark .section__sub { color: var(--metro-gray-300); }

    /* --- Tile Grid --- */
    .tiles { display: grid; grid-template-columns: repeat(auto-fill, minmax(150px, 1fr)); gap: var(--metro-gutter); }
    .tile {
      aspect-ratio: 1/1; color: #fff; padding: 16px;
      display: flex; flex-direction: column; justify-content: flex-end;
      cursor: pointer; overflow: hidden; transition: opacity 0.15s; text-decoration: none;
    }
    .tile:hover { opacity: 0.85; }
    .tile--wide { grid-column: span 2; aspect-ratio: 2/1; }
    .tile--large { grid-column: span 2; grid-row: span 2; }
    .tile__icon { font-size: 2rem; margin-bottom: auto; }
    .tile__count { font-family: 'Raleway', sans-serif; font-weight: 200; font-size: 2.5rem; line-height: 1; }
    .tile__label { font-weight: 300; font-size: 0.85rem; margin-top: 4px; }

    /* Live tile flip */
    .live-tile { perspective: 800px; }
    .live-tile__inner {
      width: 100%; height: 100%; transform-style: preserve-3d;
      animation: flip 8s ease-in-out infinite;
    }
    .live-tile__front, .live-tile__back {
      position: absolute; inset: 0; backface-visibility: hidden;
      display: flex; flex-direction: column; justify-content: flex-end; padding: 16px;
    }
    .live-tile__back { transform: rotateX(180deg); }
    @keyframes flip {
      0%,40% { transform: rotateX(0); }
      50%,90% { transform: rotateX(180deg); }
      100% { transform: rotateX(360deg); }
    }

    /* --- Cards --- */
    .cards { display: grid; grid-template-columns: repeat(auto-fill, minmax(280px, 1fr)); gap: var(--metro-gutter); }
    .card {
      background: #fff; border-left: 4px solid var(--metro-accent);
      padding: 28px 22px; transition: border-color 0.2s;
    }
    .card:hover { border-left-color: var(--metro-teal); }
    .card__cat {
      font-size: 0.7rem; font-weight: 600; text-transform: uppercase;
      letter-spacing: 0.1em; color: var(--metro-gray-500); margin-bottom: 8px;
    }
    .card__title {
      font-family: 'Raleway', sans-serif; font-weight: 200;
      font-size: 1.4rem; line-height: 1.3; margin-bottom: 10px;
    }
    .card__body {
      font-weight: 300; font-size: 0.92rem; line-height: 1.65;
      color: var(--metro-gray-500); margin-bottom: 18px;
    }
    .card__link {
      font-size: 0.82rem; font-weight: 600; color: var(--metro-accent);
      text-decoration: none; text-transform: uppercase; letter-spacing: 0.05em;
    }
    .card__link:hover { text-decoration: underline; }

    /* --- Features --- */
    .features { display: grid; grid-template-columns: repeat(auto-fit, minmax(220px, 1fr)); gap: 30px; }
    .feature { padding-top: 16px; border-top: 3px solid var(--metro-accent); }
    .feature__title { font-weight: 600; font-size: 0.95rem; margin-bottom: 8px; }
    .feature__text { font-weight: 300; font-size: 0.9rem; line-height: 1.6; color: var(--metro-gray-500); }

    /* --- Footer --- */
    .footer {
      background: var(--metro-dark); color: var(--metro-gray-300); padding: 40px;
      display: flex; justify-content: space-between; flex-wrap: wrap; gap: 30px;
    }
    .footer__brand {
      font-family: 'Raleway', sans-serif; font-weight: 200;
      font-size: 1.3rem; color: #fff; margin-bottom: 8px; text-transform: lowercase;
    }
    .footer__copy { font-size: 0.78rem; color: var(--metro-gray-500); }
    .footer__links { display: flex; gap: 24px; list-style: none; }
    .footer__link {
      color: var(--metro-gray-300); text-decoration: none;
      font-size: 0.82rem; transition: color 0.2s;
    }
    .footer__link:hover { color: #fff; }

    /* --- Responsive --- */
    @media (max-width: 768px) {
      .nav { padding: 0 20px; }
      .hero { padding: 50px 20px 40px; }
      .section { padding: 40px 20px; }
      .footer { padding: 30px 20px; }
      .tiles { grid-template-columns: repeat(2, 1fr); }
      .tile--large { grid-row: span 1; aspect-ratio: 2/1; }
      .nav__links { display: none; }
    }
  </style>
</head>
<body>

  <nav class="nav">
    <a href="#" class="nav__brand">metro app</a>
    <ul class="nav__links">
      <li><a href="#" class="nav__link nav__link--active">Start</a></li>
      <li><a href="#tiles" class="nav__link">Tiles</a></li>
      <li><a href="#features" class="nav__link">Features</a></li>
      <li><a href="#cards" class="nav__link">Cards</a></li>
    </ul>
  </nav>

  <header class="hero">
    <div class="hero__bar"></div>
    <p class="hero__category">Microsoft Design Language</p>
    <h1 class="hero__title">content before chrome</h1>
    <p class="hero__sub">
      A design language built on typography, flat color, and grid precision.
      Strip away the decoration. Let the content speak.
    </p>
    <div class="hero__actions">
      <a href="#tiles" class="btn btn--filled btn--large">Explore tiles</a>
      <a href="#features" class="btn btn--large">Learn more</a>
    </div>
    <div class="hero__block"></div>
  </header>

  <section class="section" id="tiles">
    <p class="section__cat">Start Screen</p>
    <h2 class="section__title">live tiles</h2>
    <p class="section__sub">Information at a glance. Each tile is a window into content, data, and actions.</p>
    <div class="tiles">
      <div class="tile tile--large live-tile" style="background:var(--metro-dark-blue)">
        <div class="live-tile__inner">
          <div class="live-tile__front">
            <span class="tile__icon">&#9993;</span>
            <span class="tile__count">12</span>
            <span class="tile__label">Mail</span>
          </div>
          <div class="live-tile__back">
            <span class="tile__label" style="margin-bottom:auto;font-size:0.8rem;opacity:0.8">Latest from J. Smith</span>
            <span class="tile__label">Project update ready for review...</span>
          </div>
        </div>
      </div>
      <a href="#" class="tile" style="background:var(--metro-teal)">
        <span class="tile__icon">&#9742;</span><span class="tile__label">Phone</span>
      </a>
      <a href="#" class="tile" style="background:var(--metro-green)">
        <span class="tile__icon">&#9881;</span><span class="tile__label">Settings</span>
      </a>
      <a href="#" class="tile tile--wide" style="background:var(--metro-magenta)">
        <span class="tile__icon">&#9835;</span>
        <span class="tile__count">Now Playing</span><span class="tile__label">Music</span>
      </a>
      <a href="#" class="tile" style="background:var(--metro-orange)">
        <span class="tile__icon">&#9733;</span><span class="tile__label">Store</span>
      </a>
      <a href="#" class="tile" style="background:var(--metro-purple)">
        <span class="tile__icon">&#9992;</span><span class="tile__label">Travel</span>
      </a>
      <a href="#" class="tile" style="background:var(--metro-yellow);color:var(--metro-dark)">
        <span class="tile__icon">&#9728;</span><span class="tile__label">Weather</span>
      </a>
      <a href="#" class="tile" style="background:var(--metro-red)">
        <span class="tile__icon">&#9829;</span><span class="tile__label">Health</span>
      </a>
      <a href="#" class="tile tile--wide" style="background:var(--metro-dark-purple)">
        <span class="tile__icon">&#128247;</span>
        <span class="tile__count">847</span><span class="tile__label">Photos</span>
      </a>
    </div>
  </section>

  <section class="section section--dark" id="features">
    <p class="section__cat">Design Principles</p>
    <h2 class="section__title">built on purpose</h2>
    <p class="section__sub">Every pixel serves a function. Every decision is deliberate.</p>
    <div class="features">
      <div class="feature" style="border-top-color:var(--metro-blue)">
        <h3 class="feature__title">Authentically Digital</h3>
        <p class="feature__text">No imitation of physical materials. The interface embraces its screen-native nature.</p>
      </div>
      <div class="feature" style="border-top-color:var(--metro-teal)">
        <h3 class="feature__title">Fast and Fluid</h3>
        <p class="feature__text">Interactions respond instantly. Transitions communicate spatial relationships.</p>
      </div>
      <div class="feature" style="border-top-color:var(--metro-magenta)">
        <h3 class="feature__title">Do More With Less</h3>
        <p class="feature__text">Reduce to essentials. Every element earns its place on screen.</p>
      </div>
      <div class="feature" style="border-top-color:var(--metro-green)">
        <h3 class="feature__title">Pride in Craftsmanship</h3>
        <p class="feature__text">Precision in typography, alignment, and spacing. The details are the design.</p>
      </div>
    </div>
  </section>

  <section class="section" id="cards">
    <p class="section__cat">Content</p>
    <h2 class="section__title">latest updates</h2>
    <p class="section__sub">Clean, typographic cards let information take center stage.</p>
    <div class="cards">
      <article class="card">
        <p class="card__cat">Typography</p>
        <h3 class="card__title">Type as the hero element</h3>
        <p class="card__body">Oversized lightweight headings create hierarchy through scale alone, eliminating the need for decorative elements.</p>
        <a href="#" class="card__link">Read more &rarr;</a>
      </article>
      <article class="card">
        <p class="card__cat">Layout</p>
        <h3 class="card__title">The precision of the grid</h3>
        <p class="card__body">Built on a strict 20px base unit, Metro layouts achieve mathematical harmony across every element.</p>
        <a href="#" class="card__link">Read more &rarr;</a>
      </article>
      <article class="card">
        <p class="card__cat">Color</p>
        <h3 class="card__title">Bold accents, restrained palette</h3>
        <p class="card__body">A single accent color per context provides identity and focus against neutral backgrounds.</p>
        <a href="#" class="card__link">Read more &rarr;</a>
      </article>
    </div>
  </section>

  <footer class="footer">
    <div>
      <p class="footer__brand">metro design</p>
      <p class="footer__copy">A design language for the digital age.</p>
    </div>
    <ul class="footer__links">
      <li><a href="#" class="footer__link">Start</a></li>
      <li><a href="#tiles" class="footer__link">Tiles</a></li>
      <li><a href="#features" class="footer__link">Features</a></li>
      <li><a href="#cards" class="footer__link">Cards</a></li>
    </ul>
  </footer>

</body>
</html>
```

## Implementation Tips

- **Use `border-radius: 0` globally on interactive elements** — Metro's sharp-cornered rectangles are fundamental; reset any framework defaults that add border-radius to buttons, cards, or inputs
- **Set up CSS custom properties for accent color theming** — by defining a single `--metro-accent` variable referenced throughout your stylesheet, users can switch the entire color scheme by changing one value
- **Leverage CSS Grid's `auto-fill` and `span` for tile layouts** — `repeat(auto-fill, minmax(150px, 1fr))` combined with `grid-column: span 2` on wide tiles naturally produces the responsive tile mosaic
- **Use `font-weight: 100` or `200` for hero text only if the font supports it** — test at target sizes and consider 300 if text appears too fragile on non-Retina displays or Windows ClearType
- **Implement live tile animations with CSS `@keyframes` and `backface-visibility`** — flip and slide-up effects work purely in CSS; use `animation-delay` to stagger multiple tiles
- **Prefer `opacity` transitions over color transitions for hover states** — applying `opacity: 0.85` on hover maintains tile identity color while signaling interactivity consistently across all accent colors
