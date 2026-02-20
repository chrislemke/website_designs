# Isometric Design

## Overview

Isometric Design is a visual aesthetic that creates the illusion of three-dimensional depth within a two-dimensional plane using isometric projection -- a method where all three spatial axes are equally foreshortened and lines remain parallel rather than converging toward a vanishing point. Popularized across tech landing pages, SaaS product sites, and startup marketing, this style occupies a deliberate middle ground between the simplicity of flat design and the realism of full 3D rendering. Objects are typically rendered at a 30-degree angle from the horizontal, producing a distinctive tilted top-down perspective that makes complex systems, workflows, and architectures feel approachable and legible. The aesthetic relies on clean geometric shapes, vivid color stepping, and carefully constructed shadow systems to give flat illustrations a tangible, toy-like dimensionality. Isometric Design excels at explaining abstract concepts visually -- server infrastructure, data flows, city maps, and product ecosystems all become immediately comprehensible when arranged on an isometric grid.

---

## Visual Characteristics

### Core Design Traits

- **30-degree angular projection**: All surfaces are rendered at consistent 30-degree angles from the horizontal axis, creating the signature isometric perspective where no lines converge toward vanishing points
- **Parallel line discipline**: Unlike true perspective drawing, parallel edges in the real world remain parallel in the illustration -- this uniformity produces the clean, schematic quality that defines the style
- **Flat 3D volumes**: Objects are built from simple extruded geometric primitives (cubes, cylinders, prisms) with flat-filled faces rather than photorealistic textures or complex lighting
- **Consistent scale across depth**: Objects in the background are the same size as objects in the foreground, eliminating size-based depth cues and reinforcing the diagrammatic clarity of the composition
- **Face-based color stepping**: Each visible face of an isometric object uses a distinct tonal value (light top, medium side, dark side) to simulate directional lighting without actual 3D rendering
- **Generous negative space**: Compositions float on clean white or subtly tinted backgrounds, allowing each isometric element to read clearly without visual clutter
- **Shadow and elevation systems**: Soft drop shadows beneath isometric objects anchor them to a ground plane, while elevation differences communicate hierarchy and layering

### Design Principles

- **Clarity over realism**: The goal is to explain, not to simulate -- every object should be immediately identifiable and every spatial relationship instantly readable
- **Systematic consistency**: All objects in a scene must share the same projection angle, light direction, scale ratio, and color logic to maintain the illusion of a unified isometric world
- **Hierarchical color coding**: Different functional categories (data, users, infrastructure, processes) receive distinct color families so viewers can parse complex scenes at a glance
- **Progressive disclosure through layers**: Isometric scenes can stack vertically to show system layers, with higher elements representing more abstract or user-facing concepts
- **Purposeful simplification**: Strip away unnecessary detail from each object until only the essential identifying features remain -- the style rewards geometric reduction

---

## Color Palette

Isometric Design palettes combine a vibrant primary with cool blues and purples, warm accent tones for highlights, and carefully stepped neutral grays for surfaces and shadows. The face-shading convention (light top, medium left, dark right) is fundamental.

| Swatch | Hex | Role |
|--------|-----|------|
| ![#6C5CE7](https://via.placeholder.com/20/6C5CE7/6C5CE7.png) | `#6C5CE7` | Primary purple -- hero elements, key objects |
| ![#A29BFE](https://via.placeholder.com/20/A29BFE/A29BFE.png) | `#A29BFE` | Light purple -- top faces, highlights |
| ![#0984E3](https://via.placeholder.com/20/0984E3/0984E3.png) | `#0984E3` | Primary blue -- secondary objects, links |
| ![#74B9FF](https://via.placeholder.com/20/74B9FF/74B9FF.png) | `#74B9FF` | Light blue -- top faces, hover states |
| ![#00CEC9](https://via.placeholder.com/20/00CEC9/00CEC9.png) | `#00CEC9` | Teal accent -- success states, data flows |
| ![#FDCB6E](https://via.placeholder.com/20/FDCB6E/FDCB6E.png) | `#FDCB6E` | Warm yellow -- attention, highlights, badges |
| ![#E17055](https://via.placeholder.com/20/E17055/E17055.png) | `#E17055` | Coral accent -- warnings, hot CTAs |
| ![#FF7675](https://via.placeholder.com/20/FF7675/FF7675.png) | `#FF7675` | Soft red -- error states, alerts |
| ![#DFE6E9](https://via.placeholder.com/20/DFE6E9/DFE6E9.png) | `#DFE6E9` | Light gray -- backgrounds, ground planes |
| ![#B2BEC3](https://via.placeholder.com/20/B2BEC3/B2BEC3.png) | `#B2BEC3` | Medium gray -- shadow faces, borders |
| ![#636E72](https://via.placeholder.com/20/636E72/636E72.png) | `#636E72` | Dark gray -- body text, dark side faces |
| ![#2D3436](https://via.placeholder.com/20/2D3436/2D3436.png) | `#2D3436` | Near-black -- headings, deep shadows |

### CSS Custom Properties

```css
:root {
  --iso-primary: #6C5CE7;
  --iso-primary-light: #A29BFE;
  --iso-primary-dark: #4B3FBF;
  --iso-secondary: #0984E3;
  --iso-secondary-light: #74B9FF;
  --iso-secondary-dark: #065FA3;
  --iso-teal: #00CEC9;
  --iso-teal-light: #81ECEC;
  --iso-yellow: #FDCB6E;
  --iso-yellow-light: #FFEAA7;
  --iso-coral: #E17055;
  --iso-coral-light: #FAB1A0;
  --iso-red: #FF7675;
  --iso-white: #FFFFFF;
  --iso-gray-100: #F5F6FA;
  --iso-gray-200: #DFE6E9;
  --iso-gray-300: #B2BEC3;
  --iso-gray-400: #636E72;
  --iso-gray-900: #2D3436;
  --iso-shadow: rgba(45, 52, 54, 0.15);
  --iso-shadow-deep: rgba(45, 52, 54, 0.25);
  --iso-gradient-primary: linear-gradient(135deg, #6C5CE7, #A29BFE);
  --iso-gradient-blue: linear-gradient(135deg, #0984E3, #74B9FF);
  --iso-gradient-warm: linear-gradient(135deg, #E17055, #FDCB6E);
}
```

---

## Typography

Isometric Design pairs geometric sans-serif headings with clean, highly legible body fonts. The typography should feel modern, technical, and approachable -- mirroring the clarity of the illustrations themselves.

### Recommended Google Fonts

| Font | Weight(s) | Usage | Link |
|------|-----------|-------|------|
| **Inter** | 400, 500, 600, 700 | Body text, UI labels, descriptions | [Google Fonts](https://fonts.google.com/specimen/Inter) |
| **Space Grotesk** | 500, 600, 700 | Headings, hero text, feature titles | [Google Fonts](https://fonts.google.com/specimen/Space+Grotesk) |
| **Poppins** | 400, 500, 600, 700 | Alternative headings, navigation | [Google Fonts](https://fonts.google.com/specimen/Poppins) |
| **IBM Plex Sans** | 400, 500, 600 | Technical copy, code-adjacent text | [Google Fonts](https://fonts.google.com/specimen/IBM+Plex+Sans) |
| **DM Sans** | 400, 500, 700 | Compact UI, cards, metadata | [Google Fonts](https://fonts.google.com/specimen/DM+Sans) |

### Font Pairing Suggestions

| Heading | Body | Vibe |
|---------|------|------|
| **Space Grotesk** (700) | **Inter** (400) | Modern tech -- geometric precision meets everyday readability |
| **Poppins** (600) | **DM Sans** (400) | Friendly SaaS -- rounded warmth with compact efficiency |
| **Space Grotesk** (600) | **IBM Plex Sans** (400) | Developer-focused -- structured clarity with technical credibility |

### CSS Example

```css
@import url('https://fonts.googleapis.com/css2?family=Space+Grotesk:wght@500;600;700&family=Inter:wght@400;500;600;700&display=swap');

body {
  font-family: 'Inter', -apple-system, BlinkMacSystemFont, 'Segoe UI', sans-serif;
  font-size: 16px;
  line-height: 1.7;
  color: var(--iso-gray-900);
  -webkit-font-smoothing: antialiased;
}

h1, h2, h3, h4, h5, h6 {
  font-family: 'Space Grotesk', sans-serif;
  font-weight: 700;
  line-height: 1.2;
  letter-spacing: -0.02em;
}

h1 { font-size: clamp(2.5rem, 5vw, 4rem); }
h2 { font-size: clamp(2rem, 4vw, 3rem); }
h3 { font-size: clamp(1.5rem, 3vw, 2rem); }

.label {
  font-size: 0.75rem;
  font-weight: 600;
  text-transform: uppercase;
  letter-spacing: 0.1em;
  color: var(--iso-primary);
}
```

---

## Layout Principles

- **Grid-based composition**: Use a 12-column grid with generous gutters (24-32px) to align both page content and isometric illustration placement; isometric scenes work best when they snap to grid intersections
- **Asymmetric hero splits**: Hero sections typically divide into a text-heavy left column (5-6 columns) and an isometric illustration right column (6-7 columns), allowing the 3D scene to breathe
- **Vertical rhythm through elevation**: Stack content sections at different conceptual heights -- use subtle background color shifts or shadow intensities to suggest layered depth as the user scrolls
- **Generous section spacing**: Maintain 80-120px vertical padding between major sections; isometric illustrations need breathing room to prevent angular edges from colliding with adjacent content
- **Card grids with isometric accents**: Feature cards in 3-column (desktop) or 2-column (tablet) grids, where each card contains a small isometric icon or illustration as its visual anchor
- **Floating illustration anchors**: Position isometric scenes so they slightly overflow their container or overlap section dividers, creating depth that extends beyond the column structure
- **Mobile-first stacking**: On narrow screens, isometric illustrations scale down and stack above their text blocks; maintain aspect ratios to prevent distortion of the angular perspective

---

## CSS / Design Techniques

### Card

```css
.iso-card {
  background: var(--iso-white);
  border-radius: 16px;
  padding: 2rem;
  box-shadow: 0 4px 6px var(--iso-shadow), 0 10px 30px var(--iso-shadow);
  transition: transform 0.3s ease, box-shadow 0.3s ease;
  position: relative;
  overflow: hidden;
}

.iso-card::before {
  content: '';
  position: absolute;
  top: 0; left: 0; right: 0;
  height: 4px;
  background: var(--iso-gradient-primary);
}

.iso-card:hover {
  transform: translateY(-8px) rotateX(2deg);
  box-shadow: 0 8px 12px var(--iso-shadow), 0 20px 60px var(--iso-shadow-deep);
}
```

### Button

```css
.iso-btn {
  display: inline-flex;
  align-items: center;
  gap: 0.5rem;
  padding: 0.875rem 2rem;
  font-family: 'Inter', sans-serif;
  font-size: 1rem;
  font-weight: 600;
  border: none;
  border-radius: 12px;
  cursor: pointer;
  transition: all 0.25s ease;
  text-decoration: none;
}

.iso-btn--primary {
  background: var(--iso-gradient-primary);
  color: var(--iso-white);
  box-shadow: 0 4px 15px rgba(108, 92, 231, 0.4);
}

.iso-btn--primary:hover {
  transform: translateY(-3px);
  box-shadow: 0 8px 25px rgba(108, 92, 231, 0.5);
}

.iso-btn--secondary {
  background: var(--iso-white);
  color: var(--iso-primary);
  border: 2px solid var(--iso-primary);
}

.iso-btn--secondary:hover {
  background: var(--iso-primary);
  color: var(--iso-white);
  transform: translateY(-3px);
}
```

### Navigation

```css
.iso-nav {
  position: fixed;
  top: 0; left: 0; right: 0;
  z-index: 1000;
  padding: 1rem 2rem;
  background: rgba(255, 255, 255, 0.92);
  backdrop-filter: blur(12px);
  -webkit-backdrop-filter: blur(12px);
  border-bottom: 1px solid var(--iso-gray-200);
}

.iso-nav__inner {
  max-width: 1200px;
  margin: 0 auto;
  display: flex;
  align-items: center;
  justify-content: space-between;
}

.iso-nav__links a {
  font-size: 0.9375rem;
  font-weight: 500;
  color: var(--iso-gray-400);
  text-decoration: none;
  transition: color 0.2s ease;
}

.iso-nav__links a:hover { color: var(--iso-primary); }
```

### Hero Section

```css
.iso-hero {
  min-height: 90vh;
  display: flex;
  align-items: center;
  padding: 8rem 2rem 4rem;
  background: var(--iso-gray-100);
  position: relative;
  overflow: hidden;
}

.iso-hero::before {
  content: '';
  position: absolute;
  inset: 0;
  background-image:
    linear-gradient(var(--iso-gray-200) 1px, transparent 1px),
    linear-gradient(90deg, var(--iso-gray-200) 1px, transparent 1px);
  background-size: 40px 40px;
  opacity: 0.5;
  pointer-events: none;
}

.iso-hero__inner {
  max-width: 1200px;
  margin: 0 auto;
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 4rem;
  align-items: center;
}

@media (max-width: 768px) {
  .iso-hero__inner { grid-template-columns: 1fr; text-align: center; }
}
```

### CSS Isometric Box

```css
.iso-cube {
  width: 100px;
  height: 100px;
  position: relative;
  transform-style: preserve-3d;
  transform: rotateX(60deg) rotateZ(-45deg);
}

.iso-cube__face {
  position: absolute;
  width: 100px;
  height: 100px;
}

.iso-cube__face--top {
  background: var(--iso-primary-light);
  transform: translateZ(50px);
}

.iso-cube__face--front {
  background: var(--iso-primary);
  transform: rotateX(-90deg) translateZ(50px);
  transform-origin: bottom;
}

.iso-cube__face--right {
  background: var(--iso-primary-dark);
  transform: rotateY(90deg) translateZ(50px);
  transform-origin: right;
}

.iso-cube--animated { animation: iso-float 4s ease-in-out infinite; }

@keyframes iso-float {
  0%, 100% { transform: rotateX(60deg) rotateZ(-45deg) translateZ(0); }
  50% { transform: rotateX(60deg) rotateZ(-45deg) translateZ(20px); }
}
```

### Isometric Grid Layout

```css
.iso-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
  gap: 2rem;
  padding: 4rem 2rem;
  transform: rotateX(55deg) rotateZ(-45deg);
  transform-style: preserve-3d;
}

.iso-grid__item {
  background: var(--iso-white);
  border-radius: 12px;
  padding: 1.5rem;
  box-shadow: 0 20px 40px var(--iso-shadow-deep);
  transition: transform 0.3s ease;
  transform: translateZ(0);
}

.iso-grid__item:hover {
  transform: translateZ(30px);
  box-shadow: 0 30px 60px var(--iso-shadow-deep);
}
```

---

## Design Do's and Don'ts

### Do's

- **Do maintain a single, consistent light source** across all isometric elements -- top-left illumination is the most common convention, producing a light top face, medium left face, and dark right face
- **Do use a strict isometric grid** (30-degree angles) as the foundation for all illustrations; freehand angles will break the mathematical precision that makes isometric design convincing
- **Do apply color stepping to faces** -- each visible face of an object should be a distinct tonal value of the same hue to reinforce the three-dimensional illusion
- **Do pair isometric illustrations with generous white space** to let the angular complexity of the artwork breathe and avoid overwhelming the viewer
- **Do create reusable isometric component libraries** (buildings, devices, people, icons) built on the same grid so they can be freely combined into new scenes
- **Do add subtle animations** like floating, rotating, or assembly sequences to bring isometric scenes to life without detracting from clarity
- **Do test at multiple viewport sizes** -- isometric angles can break down or become illegible when scaled too small, so provide simplified fallback illustrations for mobile

### Don'ts

- **Don't mix isometric projection with true perspective** in the same scene -- converging lines next to parallel lines will look like a rendering error, not a stylistic choice
- **Don't over-detail individual objects** at the expense of scene readability; isometric design rewards geometric simplification over photorealistic complexity
- **Don't use drop shadows that contradict the light direction** implied by the face shading -- shadow placement must be consistent with the simulated light source
- **Don't place too many objects in a single scene** without establishing clear visual hierarchy; complexity should be managed through color grouping, spacing, and layering
- **Don't ignore accessibility** -- ensure that information conveyed through isometric illustrations is also available as text; decorative 3D scenes should have appropriate ARIA labels
- **Don't use isometric grids for body text layout** -- the tilted perspective is for illustration and decorative elements only; content must remain in standard readable orientation
- **Don't neglect performance** -- complex isometric CSS transforms with many nested elements can trigger expensive repaints; use `will-change: transform` judiciously and test on lower-powered devices

---

## Related Aesthetics

| Aesthetic | Relationship |
|-----------|-------------|
| **Flat Design** | Isometric Design is the direct evolution of flat design, adding controlled dimensionality while preserving the clean, vector-based visual language |
| **Claymorphism** | Both create friendly 3D-like interfaces, but claymorphism uses soft inflated forms and inner shadows while isometric uses rigid geometric projection |
| **Bento Grid** | Bento grid layouts provide an excellent structural framework for arranging isometric illustration panels alongside conventional content cards |
| **Corporate Memphis** | Shares the tech/SaaS context and simplified illustration style, but corporate Memphis uses flat characters while isometric uses spatial environments |
| **Glassmorphism** | Frosted glass panels of glassmorphism can overlay isometric scenes, combining depth-through-projection with depth-through-transparency |
| **Neumorphism** | Both simulate depth on flat screens using distinct strategies -- neumorphism through soft extruded surfaces, isometric through angular geometric projection |

---

## Quick-Start HTML Template

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Isometric Design -- Quick-Start Template</title>
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Space+Grotesk:wght@500;600;700&family=Inter:wght@400;500;600;700&display=swap" rel="stylesheet">
  <style>
    :root {
      --iso-primary: #6C5CE7; --iso-primary-light: #A29BFE; --iso-primary-dark: #4B3FBF;
      --iso-secondary: #0984E3; --iso-secondary-light: #74B9FF;
      --iso-teal: #00CEC9; --iso-teal-light: #81ECEC;
      --iso-yellow: #FDCB6E; --iso-coral: #E17055;
      --iso-white: #FFFFFF; --iso-gray-100: #F5F6FA; --iso-gray-200: #DFE6E9;
      --iso-gray-300: #B2BEC3; --iso-gray-400: #636E72; --iso-gray-900: #2D3436;
      --iso-shadow: rgba(45, 52, 54, 0.12); --iso-shadow-deep: rgba(45, 52, 54, 0.22);
      --iso-gradient-primary: linear-gradient(135deg, #6C5CE7, #A29BFE);
    }

    *, *::before, *::after { margin: 0; padding: 0; box-sizing: border-box; }

    body {
      font-family: 'Inter', -apple-system, BlinkMacSystemFont, sans-serif;
      font-size: 16px; line-height: 1.7; color: var(--iso-gray-900);
      background: var(--iso-white);
      -webkit-font-smoothing: antialiased;
    }

    h1, h2, h3 {
      font-family: 'Space Grotesk', sans-serif;
      font-weight: 700; line-height: 1.2; letter-spacing: -0.02em;
    }

    /* -- Navigation -- */
    .nav {
      position: fixed; top: 0; left: 0; right: 0; z-index: 1000;
      padding: 1rem 2rem;
      background: rgba(255, 255, 255, 0.92);
      backdrop-filter: blur(12px); -webkit-backdrop-filter: blur(12px);
      border-bottom: 1px solid var(--iso-gray-200);
    }
    .nav__inner {
      max-width: 1200px; margin: 0 auto;
      display: flex; align-items: center; justify-content: space-between;
    }
    .nav__logo {
      font-family: 'Space Grotesk', sans-serif;
      font-size: 1.5rem; font-weight: 700; color: var(--iso-primary); text-decoration: none;
    }
    .nav__logo span { color: var(--iso-gray-900); }
    .nav__links { display: flex; gap: 2rem; list-style: none; }
    .nav__links a {
      font-size: 0.9375rem; font-weight: 500; color: var(--iso-gray-400);
      text-decoration: none; transition: color 0.2s ease;
    }
    .nav__links a:hover { color: var(--iso-primary); }
    .nav__cta {
      padding: 0.625rem 1.5rem; background: var(--iso-gradient-primary);
      color: var(--iso-white) !important; border-radius: 10px; font-weight: 600 !important;
      box-shadow: 0 2px 10px rgba(108, 92, 231, 0.3);
    }

    /* -- Hero -- */
    .hero {
      min-height: 100vh; display: flex; align-items: center;
      padding: 8rem 2rem 4rem; background: var(--iso-gray-100);
      position: relative; overflow: hidden;
    }
    .hero::before {
      content: ''; position: absolute; inset: 0;
      background-image:
        linear-gradient(var(--iso-gray-200) 1px, transparent 1px),
        linear-gradient(90deg, var(--iso-gray-200) 1px, transparent 1px);
      background-size: 40px 40px; opacity: 0.5; pointer-events: none;
    }
    .hero__inner {
      max-width: 1200px; margin: 0 auto; position: relative; z-index: 1;
      display: grid; grid-template-columns: 1fr 1fr; gap: 4rem; align-items: center;
    }
    .hero__label {
      font-size: 0.75rem; font-weight: 600; text-transform: uppercase;
      letter-spacing: 0.15em; color: var(--iso-primary); margin-bottom: 1rem;
    }
    .hero__title {
      font-size: clamp(2.5rem, 5vw, 3.75rem); margin-bottom: 1.5rem;
    }
    .hero__title .highlight {
      background: var(--iso-gradient-primary);
      -webkit-background-clip: text; -webkit-text-fill-color: transparent; background-clip: text;
    }
    .hero__subtitle {
      font-size: 1.2rem; color: var(--iso-gray-400);
      line-height: 1.7; margin-bottom: 2.5rem; max-width: 50ch;
    }
    .hero__actions { display: flex; gap: 1rem; flex-wrap: wrap; }

    /* -- Isometric Scene -- */
    .hero__scene { display: flex; align-items: center; justify-content: center; }
    .iso-scene {
      transform-style: preserve-3d; transform: rotateX(60deg) rotateZ(-45deg);
      position: relative; width: 260px; height: 260px;
    }
    .iso-block {
      position: absolute; width: 100px; height: 100px;
      transform-style: preserve-3d; animation: iso-float 4s ease-in-out infinite;
    }
    .iso-block:nth-child(1) { bottom: 0; left: 0; }
    .iso-block:nth-child(2) { bottom: 0; right: 20px; animation-delay: -1s; }
    .iso-block:nth-child(3) { bottom: 80px; left: 70px; animation-delay: -2s; }
    .iso-face { position: absolute; }
    .iso-face--top { width: 100%; height: 100%; transform: translateZ(60px); }
    .iso-face--front {
      width: 100%; height: 60px; bottom: 0;
      transform: rotateX(-90deg) translateZ(0); transform-origin: bottom;
    }
    .iso-face--right {
      width: 60px; height: 100%; right: 0;
      transform: rotateY(90deg) translateZ(0); transform-origin: right;
    }
    .iso-block--purple .iso-face--top { background: var(--iso-primary-light); }
    .iso-block--purple .iso-face--front { background: var(--iso-primary); }
    .iso-block--purple .iso-face--right { background: var(--iso-primary-dark); }
    .iso-block--blue .iso-face--top { background: var(--iso-secondary-light); }
    .iso-block--blue .iso-face--front { background: var(--iso-secondary); }
    .iso-block--blue .iso-face--right { background: #065FA3; }
    .iso-block--teal .iso-face--top { background: var(--iso-teal-light); }
    .iso-block--teal .iso-face--front { background: var(--iso-teal); }
    .iso-block--teal .iso-face--right { background: #00A8A3; }
    @keyframes iso-float {
      0%, 100% { transform: translateZ(0); }
      50% { transform: translateZ(16px); }
    }

    /* -- Buttons -- */
    .btn {
      display: inline-flex; align-items: center; gap: 0.5rem;
      padding: 0.875rem 2rem; font-family: 'Inter', sans-serif;
      font-size: 1rem; font-weight: 600; border: none; border-radius: 12px;
      cursor: pointer; text-decoration: none; transition: all 0.25s ease;
    }
    .btn--primary {
      background: var(--iso-gradient-primary); color: var(--iso-white);
      box-shadow: 0 4px 15px rgba(108, 92, 231, 0.4);
    }
    .btn--primary:hover { transform: translateY(-3px); box-shadow: 0 8px 25px rgba(108, 92, 231, 0.5); }
    .btn--secondary { background: var(--iso-white); color: var(--iso-primary); border: 2px solid var(--iso-primary); }
    .btn--secondary:hover { background: var(--iso-primary); color: var(--iso-white); transform: translateY(-3px); }

    /* -- Features -- */
    .features { padding: 6rem 2rem; background: var(--iso-white); }
    .section-header { text-align: center; max-width: 640px; margin: 0 auto 4rem; }
    .section-header__label {
      font-size: 0.75rem; font-weight: 600; text-transform: uppercase;
      letter-spacing: 0.15em; color: var(--iso-primary); margin-bottom: 0.75rem;
    }
    .section-header__title { font-size: clamp(2rem, 4vw, 2.75rem); margin-bottom: 1rem; }
    .section-header__text { font-size: 1.125rem; color: var(--iso-gray-400); line-height: 1.7; }
    .features__grid {
      display: grid; grid-template-columns: repeat(3, 1fr);
      gap: 2rem; max-width: 1200px; margin: 0 auto;
    }
    .feature-card {
      background: var(--iso-white); border-radius: 16px; padding: 2rem;
      border: 1px solid var(--iso-gray-200); transition: all 0.3s ease;
      position: relative; overflow: hidden;
    }
    .feature-card::before {
      content: ''; position: absolute; top: 0; left: 0; right: 0; height: 4px;
      background: var(--iso-gradient-primary); opacity: 0; transition: opacity 0.3s ease;
    }
    .feature-card:hover {
      transform: translateY(-6px); box-shadow: 0 12px 40px var(--iso-shadow-deep);
      border-color: var(--iso-primary-light);
    }
    .feature-card:hover::before { opacity: 1; }
    .feature-card__icon {
      width: 56px; height: 56px; border-radius: 14px;
      display: flex; align-items: center; justify-content: center;
      margin-bottom: 1.25rem; font-size: 1.5rem;
    }
    .feature-card__icon--purple { background: rgba(108, 92, 231, 0.12); color: var(--iso-primary); }
    .feature-card__icon--blue { background: rgba(9, 132, 227, 0.12); color: var(--iso-secondary); }
    .feature-card__icon--teal { background: rgba(0, 206, 201, 0.12); color: var(--iso-teal); }
    .feature-card__title { font-size: 1.25rem; margin-bottom: 0.5rem; }
    .feature-card__text { color: var(--iso-gray-400); font-size: 0.9375rem; line-height: 1.65; }

    /* -- CTA -- */
    .cta { padding: 6rem 2rem; background: var(--iso-gray-100); position: relative; overflow: hidden; }
    .cta::before {
      content: ''; position: absolute; inset: 0;
      background-image:
        linear-gradient(var(--iso-gray-200) 1px, transparent 1px),
        linear-gradient(90deg, var(--iso-gray-200) 1px, transparent 1px);
      background-size: 40px 40px; opacity: 0.4; pointer-events: none;
    }
    .cta__inner {
      max-width: 800px; margin: 0 auto; text-align: center; position: relative; z-index: 1;
      background: var(--iso-white); border-radius: 24px; padding: 4rem 3rem;
      box-shadow: 0 10px 40px var(--iso-shadow); border: 1px solid var(--iso-gray-200);
    }
    .cta__title { font-size: clamp(1.75rem, 3.5vw, 2.5rem); margin-bottom: 1rem; }
    .cta__text { font-size: 1.125rem; color: var(--iso-gray-400); margin-bottom: 2rem; }
    .cta__actions { display: flex; gap: 1rem; justify-content: center; flex-wrap: wrap; }

    /* -- Footer -- */
    .footer { padding: 3rem 2rem; background: var(--iso-gray-900); text-align: center; }
    .footer__logo {
      font-family: 'Space Grotesk', sans-serif;
      font-size: 1.25rem; font-weight: 700; color: var(--iso-white); margin-bottom: 0.5rem;
    }
    .footer__text { font-size: 0.875rem; color: var(--iso-gray-300); }

    /* -- Responsive -- */
    @media (max-width: 768px) {
      .hero__inner { grid-template-columns: 1fr; text-align: center; }
      .hero__actions { justify-content: center; }
      .hero__scene { order: -1; margin-bottom: 2rem; }
      .iso-scene { width: 200px; height: 200px; }
      .iso-block { width: 70px; height: 70px; }
      .features__grid { grid-template-columns: 1fr; }
      .nav__links { display: none; }
    }
    @media (max-width: 1024px) and (min-width: 769px) {
      .features__grid { grid-template-columns: repeat(2, 1fr); }
    }
  </style>
</head>
<body>

  <nav class="nav">
    <div class="nav__inner">
      <a href="#" class="nav__logo">Iso<span>Stack</span></a>
      <ul class="nav__links">
        <li><a href="#features">Features</a></li>
        <li><a href="#about">About</a></li>
        <li><a href="#" class="nav__cta">Get Started</a></li>
      </ul>
    </div>
  </nav>

  <section class="hero">
    <div class="hero__inner">
      <div class="hero__content">
        <div class="hero__label">Modern Isometric Platform</div>
        <h1 class="hero__title">Build in <span class="highlight">Three Dimensions</span></h1>
        <p class="hero__subtitle">
          A design system that brings depth, clarity, and spatial awareness
          to your web projects through the precision of isometric projection.
        </p>
        <div class="hero__actions">
          <a href="#" class="btn btn--primary">Start Building</a>
          <a href="#" class="btn btn--secondary">View Docs</a>
        </div>
      </div>
      <div class="hero__scene">
        <div class="iso-scene">
          <div class="iso-block iso-block--purple">
            <div class="iso-face iso-face--top"></div>
            <div class="iso-face iso-face--front"></div>
            <div class="iso-face iso-face--right"></div>
          </div>
          <div class="iso-block iso-block--blue">
            <div class="iso-face iso-face--top"></div>
            <div class="iso-face iso-face--front"></div>
            <div class="iso-face iso-face--right"></div>
          </div>
          <div class="iso-block iso-block--teal">
            <div class="iso-face iso-face--top"></div>
            <div class="iso-face iso-face--front"></div>
            <div class="iso-face iso-face--right"></div>
          </div>
        </div>
      </div>
    </div>
  </section>

  <section class="features" id="features">
    <div class="section-header">
      <div class="section-header__label">Features</div>
      <h2 class="section-header__title">Everything You Need</h2>
      <p class="section-header__text">
        Build spatial interfaces with a complete toolkit designed for clarity,
        consistency, and dimensional depth.
      </p>
    </div>
    <div class="features__grid">
      <div class="feature-card">
        <div class="feature-card__icon feature-card__icon--purple">&#9635;</div>
        <h3 class="feature-card__title">Isometric Grid System</h3>
        <p class="feature-card__text">
          A 30-degree angular grid foundation that ensures every element
          aligns with mathematical precision across your entire layout.
        </p>
      </div>
      <div class="feature-card">
        <div class="feature-card__icon feature-card__icon--blue">&#9670;</div>
        <h3 class="feature-card__title">3D Component Library</h3>
        <p class="feature-card__text">
          Pre-built isometric blocks, devices, and icons that snap together
          to create complex dimensional scenes.
        </p>
      </div>
      <div class="feature-card">
        <div class="feature-card__icon feature-card__icon--teal">&#9651;</div>
        <h3 class="feature-card__title">Smart Depth Mapping</h3>
        <p class="feature-card__text">
          Automatic shadow and face-shading calculations that maintain
          consistent lighting direction across all elements.
        </p>
      </div>
    </div>
  </section>

  <section class="cta">
    <div class="cta__inner">
      <h2 class="cta__title">Ready to Add a New Dimension?</h2>
      <p class="cta__text">
        Start building spatial interfaces today with our complete
        isometric design toolkit. No 3D software required.
      </p>
      <div class="cta__actions">
        <a href="#" class="btn btn--primary">Get Started Free</a>
        <a href="#" class="btn btn--secondary">See Examples</a>
      </div>
    </div>
  </section>

  <footer class="footer">
    <div class="footer__inner">
      <div class="footer__logo">IsoStack</div>
      <p class="footer__text">Isometric Design System. Built with precision.</p>
    </div>
  </footer>

</body>
</html>
```

---

## Implementation Tips

- **Use CSS `transform: rotateX(60deg) rotateZ(-45deg)` as your isometric foundation**: This combination of rotations applied to a container produces the standard isometric projection angle; child elements positioned with normal CSS layout will automatically appear in isometric space
- **Simulate face shading with HSL color manipulation**: For any given hue, use three lightness values -- `hsl(H, S, 65%)` for the top face, `hsl(H, S, 50%)` for the left face, and `hsl(H, S, 35%)` for the right face -- to create consistent directional lighting without manual color picking
- **Set `transform-style: preserve-3d` on all isometric containers**: Without this property, nested 3D transforms collapse into flat 2D rendering, breaking the depth illusion; apply it to every element in the transform chain
- **Optimize paint performance with `will-change: transform`**: Isometric layouts with animated elements can trigger expensive browser repaints; apply `will-change` to animated elements only and remove it after animations complete to free GPU memory
- **Build complex isometric illustrations as SVG**: While CSS transforms work well for simple cubes and grids, production-quality isometric scenes should be authored in vector tools (Figma, Illustrator, Affinity Designer) and exported as optimized SVG
- **Provide flat fallbacks for reduced-motion preferences**: Wrap isometric animations in `@media (prefers-reduced-motion: no-preference)` queries, and consider offering a completely flat alternative layout for users who experience motion sensitivity
