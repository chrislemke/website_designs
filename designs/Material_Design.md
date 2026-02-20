# Material Design

## Overview

Material Design is a comprehensive design system created by Google in 2014 (codenamed "Quantum Paper"), built on the metaphor of physical materials -- particularly paper and ink -- existing in a rational, three-dimensional space governed by consistent rules of light, surface, and motion. Unlike purely flat design, Material Design uses elevation, shadow, and layered surfaces to communicate hierarchy and interactive affordances, while retaining bold color, clean typography, and geometric simplicity. The system defines precise specifications for spacing (using an 8dp baseline grid), elevation (0-24dp), motion (easing curves and durations), and color roles, making it one of the most rigorously documented design languages in existence. It has evolved through three major versions -- Material Design 1 (2014), Material Design 2 (2018), and Material Design 3 / Material You (2021-present) -- each expanding personalization and theming capabilities while preserving the core physical metaphor. Material Design powers Android, Google's product suite, and thousands of third-party applications worldwide, making it one of the most widely deployed design systems in history.

---

## Visual Characteristics

### Core Design Traits

- **Layered surfaces with elevation**: UI elements exist on distinct planes in z-space, with shadow depth communicating their stacking order and interactive importance
- **Bold, intentional color**: A structured color system with primary, secondary, tertiary, and error roles, where vibrant hues draw attention to key actions and surfaces
- **8dp baseline grid**: All spacing, sizing, and layout measurements adhere to a strict 8-density-independent-pixel grid for mathematical consistency across devices
- **Responsive motion**: Purposeful animations with specific easing curves (standard, decelerate, accelerate) communicate spatial relationships and state changes
- **Rounded geometry**: Components favor rounded rectangles with consistent corner radii (small: 4dp, medium: 12dp, large: 16dp, extra-large: 28dp) creating a friendly, approachable interface
- **Typographic hierarchy via scale**: A defined type scale with specific sizes, weights, and letter-spacing values for display, headline, title, body, and label roles
- **Material metaphor**: Surfaces behave like physical sheets of paper -- they can be stacked, split, joined, and transformed, but never pass through each other or bend in impossible ways

### Design Principles

- **Material is the metaphor**: Inspired by the study of paper and ink, the design language treats UI surfaces as tangible objects with physical properties -- thickness, shadow, and response to touch
- **Bold, graphic, and intentional**: Foundational elements of print design (typography, grids, space, scale, color, imagery) guide visual treatments, with every choice serving a deliberate communicative purpose
- **Motion provides meaning**: Motion respects and reinforces the user as the prime mover; transitions are coherent, indicating spatial relationships between elements and guiding attention naturally
- **Adaptive and flexible**: The system adapts across screen sizes, input methods, and devices through responsive layout grids, flexible components, and dynamic color theming
- **Accessible by default**: Color contrast ratios, touch target sizes (minimum 48dp), and semantic structure are built into the system specifications rather than treated as afterthoughts

---

## Color Palette

Material Design 3 uses a tonal palette system where colors are generated from seed colors through hue and chroma adjustments. Below is the baseline Material Design 3 color scheme.

| Swatch | Hex | Role |
|--------|-----|------|
| **Primary** | `#6750A4` | Main brand color, prominent buttons, active states |
| **On Primary** | `#FFFFFF` | Text and icons on primary-colored surfaces |
| **Primary Container** | `#EADDFF` | Lighter primary for filled containers, chips, cards |
| **Secondary** | `#625B71` | Less prominent components, filters, selection controls |
| **Secondary Container** | `#E8DEF8` | Secondary container fills, tonal buttons |
| **Tertiary** | `#7D5260` | Accent for contrast and visual interest, balancing primary |
| **Tertiary Container** | `#FFD8E4` | Tertiary container fills, decorative accents |
| **Surface** | `#FFFBFE` | Default background for sheets, cards, and menus |
| **Surface Variant** | `#E7E0EC` | Alternate surface for visual differentiation |
| **Error** | `#B3261E` | Error states, destructive actions, validation failures |
| **Outline** | `#79747E` | Borders, dividers, and decorative outlines |
| **On Surface** | `#1C1B1F` | Primary text and icons on surface backgrounds |

### CSS Custom Properties

```css
:root {
  /* Primary */
  --md-primary: #6750A4;
  --md-on-primary: #FFFFFF;
  --md-primary-container: #EADDFF;
  --md-on-primary-container: #21005D;
  /* Secondary */
  --md-secondary: #625B71;
  --md-on-secondary: #FFFFFF;
  --md-secondary-container: #E8DEF8;
  --md-on-secondary-container: #1D192B;
  /* Tertiary */
  --md-tertiary: #7D5260;
  --md-on-tertiary: #FFFFFF;
  --md-tertiary-container: #FFD8E4;
  --md-on-tertiary-container: #31111D;
  /* Error */
  --md-error: #B3261E;
  --md-on-error: #FFFFFF;
  --md-error-container: #F9DEDC;
  --md-on-error-container: #410E0B;
  /* Surface */
  --md-surface: #FFFBFE;
  --md-on-surface: #1C1B1F;
  --md-surface-variant: #E7E0EC;
  --md-on-surface-variant: #49454F;
  /* Outline and inverse */
  --md-outline: #79747E;
  --md-outline-variant: #CAC4D0;
  --md-inverse-surface: #313033;
  --md-inverse-on-surface: #F4EFF4;
  --md-inverse-primary: #D0BCFF;
  /* Surface elevation tints */
  --md-surface-1: #F6F0FA;
  --md-surface-2: #F1EAFA;
  --md-surface-3: #ECE4F9;
}
```

---

## Typography

### Recommended Google Fonts

| Font | Weight(s) | Usage | Link |
|------|-----------|-------|------|
| **Roboto** | 300, 400, 500, 700 | Default Material typeface for body, labels, and UI text | [Google Fonts](https://fonts.google.com/specimen/Roboto) |
| **Roboto Flex** | Variable (100-1000) | Variable-weight alternative with optical sizing and grade axes | [Google Fonts](https://fonts.google.com/specimen/Roboto+Flex) |
| **Roboto Serif** | 400, 500, 700 | Serif companion for editorial content and long-form reading | [Google Fonts](https://fonts.google.com/specimen/Roboto+Serif) |
| **Inter** | 400, 500, 700 | Display and headline text (open-source alternative to Google Sans) | [Google Fonts](https://fonts.google.com/specimen/Inter) |
| **Noto Sans** | 300, 400, 500, 700 | Multi-script fallback covering all languages not handled by Roboto | [Google Fonts](https://fonts.google.com/noto/specimen/Noto+Sans) |

### Font Pairing Suggestions

| Heading | Body | Vibe |
|---------|------|------|
| **Inter** (700) | **Roboto** (400) | Clean, modern Material interface with display-weight headlines |
| **Roboto Serif** (700) | **Roboto** (400) | Editorial Material with warmth in headings, consistency in body |
| **Roboto Flex** (600) | **Noto Sans** (400) | Internationalized Material with variable headings and universal support |

### CSS Example

```css
@import url('https://fonts.googleapis.com/css2?family=Inter:wght@400;500;700&family=Roboto:wght@300;400;500;700&display=swap');

/* Display */
.md-display-large {
  font-family: 'Inter', 'Roboto', sans-serif;
  font-size: 3.5625rem;
  font-weight: 400;
  line-height: 4rem;
  letter-spacing: -0.015625rem;
}

/* Headline */
.md-headline-medium {
  font-family: 'Inter', 'Roboto', sans-serif;
  font-size: 1.75rem;
  font-weight: 400;
  line-height: 2.25rem;
}

/* Title */
.md-title-large {
  font-family: 'Roboto', sans-serif;
  font-size: 1.375rem;
  font-weight: 500;
  line-height: 1.75rem;
}

/* Body */
.md-body-large {
  font-family: 'Roboto', sans-serif;
  font-size: 1rem;
  font-weight: 400;
  line-height: 1.5rem;
  letter-spacing: 0.03125rem;
}

/* Label */
.md-label-large {
  font-family: 'Roboto', sans-serif;
  font-size: 0.875rem;
  font-weight: 500;
  line-height: 1.25rem;
  letter-spacing: 0.00625rem;
}
```

---

## Layout Principles

- **8dp baseline grid**: All dimensions (margins, padding, component sizes) are multiples of 8dp, with 4dp allowed for small adjustments like icon padding or text alignment
- **Responsive column grid**: Layouts use 4 columns on compact screens (< 600dp), 8 on medium (600-840dp), and 12 on expanded (> 840dp) with 16dp or 24dp gutters
- **Elevation hierarchy**: Elements at higher elevation cast larger, softer shadows and take visual precedence; resting states range from 0dp (flat on surface) to 8dp (FAB resting state)
- **Content regions**: Screens are organized into navigation rail/drawer, top app bar, body content, and optional bottom navigation, each with defined elevation and behavior
- **Contained width with edge-to-edge color**: Content areas are constrained (840-1240dp max-width) while surface colors and app bars extend to screen edges
- **Consistent component spacing**: Cards use 16dp internal padding, list items use 16dp horizontal padding, and interactive elements maintain 48dp minimum touch targets
- **Predictable breakpoints**: Compact (0-599dp), Medium (600-839dp), Expanded (840-1199dp), Large (1200-1599dp), and Extra-large (1600dp+)

---

## CSS / Design Techniques

### Card

```css
.md-card {
  background: var(--md-surface);
  border-radius: 12px;
  overflow: hidden;
  transition: box-shadow 0.2s cubic-bezier(0.4, 0, 0.2, 1);
}

.md-card--elevated {
  box-shadow: 0 1px 4px 0 rgba(0, 0, 0, 0.37);
}

.md-card--elevated:hover {
  box-shadow: 0 2px 2px 0 rgba(0, 0, 0, 0.2), 0 6px 10px 0 rgba(0, 0, 0, 0.3);
}

.md-card--filled {
  background: var(--md-surface-variant);
  box-shadow: none;
}

.md-card--outlined {
  box-shadow: none;
  border: 1px solid var(--md-outline-variant);
}

.md-card__content { padding: 16px; }

.md-card__title {
  font-family: 'Roboto', sans-serif;
  font-size: 1.375rem;
  font-weight: 500;
  color: var(--md-on-surface);
}

.md-card__actions {
  padding: 8px;
  display: flex;
  gap: 8px;
  justify-content: flex-end;
}
```

### Button

```css
.md-button {
  display: inline-flex;
  align-items: center;
  justify-content: center;
  gap: 8px;
  height: 40px;
  padding: 0 24px;
  border: none;
  border-radius: 20px;
  font-family: 'Roboto', sans-serif;
  font-size: 0.875rem;
  font-weight: 500;
  letter-spacing: 0.00625rem;
  cursor: pointer;
  position: relative;
  overflow: hidden;
  transition: box-shadow 0.2s cubic-bezier(0.4, 0, 0.2, 1);
  text-decoration: none;
}

.md-button--filled {
  background: var(--md-primary);
  color: var(--md-on-primary);
}

.md-button--filled:hover {
  box-shadow: 0 1px 4px 0 rgba(0, 0, 0, 0.37);
}

.md-button--tonal {
  background: var(--md-secondary-container);
  color: var(--md-on-secondary-container);
}

.md-button--outlined {
  background: transparent;
  color: var(--md-primary);
  border: 1px solid var(--md-outline);
}

.md-button--outlined:hover {
  background: rgba(103, 80, 164, 0.08);
}

/* Ripple state layer */
.md-button::after {
  content: '';
  position: absolute;
  inset: 0;
  background: currentColor;
  opacity: 0;
  transition: opacity 0.15s;
  border-radius: inherit;
}

.md-button:active::after { opacity: 0.12; }
```

### Navigation

```css
.md-top-bar {
  display: flex;
  align-items: center;
  height: 64px;
  padding: 0 16px;
  background: var(--md-surface-2);
  position: sticky;
  top: 0;
  z-index: 100;
}

.md-top-bar__title {
  flex: 1;
  font-family: 'Roboto', sans-serif;
  font-size: 1.375rem;
  font-weight: 500;
  margin-left: 4px;
  color: var(--md-on-surface);
}

.md-nav-rail {
  width: 80px;
  background: var(--md-surface);
  display: flex;
  flex-direction: column;
  align-items: center;
  padding: 12px 0;
  gap: 4px;
  position: fixed;
  top: 0;
  left: 0;
  height: 100vh;
}

.md-nav-rail__icon {
  width: 56px;
  height: 32px;
  display: flex;
  align-items: center;
  justify-content: center;
  border-radius: 16px;
  transition: background 0.2s cubic-bezier(0.4, 0, 0.2, 1);
}

.md-nav-rail__item--active .md-nav-rail__icon {
  background: var(--md-secondary-container);
  color: var(--md-on-secondary-container);
}
```

### Hero Section

```css
.md-hero {
  background: var(--md-primary);
  color: var(--md-on-primary);
  padding: 96px 24px 80px;
  text-align: center;
  position: relative;
  overflow: hidden;
}

.md-hero__title {
  font-family: 'Inter', 'Roboto', sans-serif;
  font-size: clamp(2.25rem, 5vw, 3.5625rem);
  font-weight: 400;
  line-height: 1.12;
  margin-bottom: 24px;
}

.md-hero__subtitle {
  font-size: 1.125rem;
  line-height: 1.75rem;
  opacity: 0.9;
  max-width: 600px;
  margin: 0 auto 40px;
}

/* Decorative surface shapes */
.md-hero::before {
  content: '';
  position: absolute;
  width: 400px;
  height: 400px;
  border-radius: 50%;
  background: rgba(255, 255, 255, 0.06);
  top: -120px;
  right: -80px;
}
```

### Floating Action Button

```css
.md-fab {
  display: inline-flex;
  align-items: center;
  justify-content: center;
  width: 56px;
  height: 56px;
  border-radius: 16px;
  border: none;
  cursor: pointer;
  background: var(--md-primary-container);
  color: var(--md-on-primary-container);
  font-size: 1.5rem;
  position: fixed;
  bottom: 24px;
  right: 24px;
  box-shadow: 0 11px 7px 0 rgba(0, 0, 0, 0.19), 0 13px 25px 0 rgba(0, 0, 0, 0.3);
  transition: box-shadow 0.2s cubic-bezier(0.4, 0, 0.2, 1);
  z-index: 50;
}

.md-fab:hover {
  box-shadow: 0 14px 12px 0 rgba(0, 0, 0, 0.17), 0 20px 40px 0 rgba(0, 0, 0, 0.3);
}

.md-fab--extended {
  width: auto;
  padding: 0 20px;
  gap: 12px;
  font-family: 'Roboto', sans-serif;
  font-size: 0.875rem;
  font-weight: 500;
}
```

### Chips and Snackbar

```css
.md-chip {
  display: inline-flex;
  align-items: center;
  gap: 8px;
  height: 32px;
  padding: 0 16px;
  border-radius: 8px;
  border: 1px solid var(--md-outline);
  background: transparent;
  color: var(--md-on-surface);
  font-family: 'Roboto', sans-serif;
  font-size: 0.875rem;
  font-weight: 500;
  cursor: pointer;
  transition: background 0.2s cubic-bezier(0.4, 0, 0.2, 1);
}

.md-chip--selected {
  background: var(--md-secondary-container);
  color: var(--md-on-secondary-container);
  border-color: transparent;
}

.md-snackbar {
  display: flex;
  align-items: center;
  gap: 8px;
  min-width: 288px;
  max-width: 560px;
  padding: 14px 16px;
  border-radius: 4px;
  background: var(--md-inverse-surface);
  color: var(--md-inverse-on-surface);
  font-family: 'Roboto', sans-serif;
  font-size: 0.875rem;
  box-shadow: 0 11px 7px 0 rgba(0, 0, 0, 0.19), 0 13px 25px 0 rgba(0, 0, 0, 0.3);
  position: fixed;
  bottom: 24px;
  left: 50%;
  transform: translateX(-50%);
}

.md-snackbar__action {
  background: none;
  border: none;
  color: var(--md-inverse-primary);
  font-family: 'Roboto', sans-serif;
  font-weight: 500;
  cursor: pointer;
}
```

---

## Design Do's and Don'ts

### Do's

- Use the 8dp grid consistently for all spacing, padding, and component sizing to maintain visual rhythm
- Apply elevation and shadow intentionally to communicate hierarchy -- higher elevation means greater importance
- Follow the Material type scale precisely, using the correct size, weight, line-height, and letter-spacing for each role
- Use the tonal color system with primary, secondary, and tertiary roles to create harmonious and accessible palettes
- Provide ripple or state-layer feedback on every interactive element to confirm user input
- Maintain minimum 48dp touch targets for all interactive elements, even when the visual element appears smaller
- Design for both light and dark themes from the start, using surface tints and tonal palettes that adapt to both

### Don'ts

- Do not use hard drop shadows with sharp edges -- Material shadows are always soft and multi-layered from a consistent light source
- Do not mix arbitrary colors outside the defined tonal palette roles; every color should map to a semantic role
- Do not place interactive elements closer than 8dp apart or use touch targets smaller than 48dp on mobile
- Do not use elevation above level 5 (24dp) or apply shadows inconsistently across the component hierarchy
- Do not ignore motion specifications; transitions need proper easing curves (standard: cubic-bezier(0.2, 0, 0, 1))
- Do not override the type scale with arbitrary font sizes or weights -- the scale is calibrated for readability
- Do not flatten all elements to zero elevation; the layered surface model distinguishes Material from pure Flat Design

---

## Related Aesthetics

| Aesthetic | Relationship |
|-----------|-------------|
| **Flat Design** | Direct predecessor; Material evolved from flat principles by reintroducing purposeful elevation while retaining bold color and simplicity |
| **Skeuomorphism** | Philosophical opposite that Material partially reconciles -- borrowing physical metaphor but abstracting it into a rationalized system |
| **Neumorphism** | Cousin aesthetic using subtle shadows for physicality, but with a monochromatic, extruded approach lacking Material's color vibrancy |
| **Glassmorphism** | Contemporary alternative using translucent, frosted-glass surfaces where Material uses opaque, tinted paper; both create depth differently |
| **Minimalism** | Broader parent philosophy -- clean layouts, purposeful whitespace, reduced decoration -- but Material adds systematic depth and motion |
| **Bauhaus** | Historical ancestor whose form-follows-function ethos and grid-based layouts directly informed Material's rational, systematic approach |

---

## Quick-Start HTML Template

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Material Design Page</title>
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;700&family=Roboto:wght@300;400;500;700&display=swap" rel="stylesheet">
  <style>
    :root {
      --md-primary: #6750A4; --md-on-primary: #FFFFFF;
      --md-primary-container: #EADDFF; --md-on-primary-container: #21005D;
      --md-secondary: #625B71; --md-on-secondary: #FFFFFF;
      --md-secondary-container: #E8DEF8; --md-on-secondary-container: #1D192B;
      --md-tertiary: #7D5260; --md-on-tertiary: #FFFFFF;
      --md-tertiary-container: #FFD8E4; --md-on-tertiary-container: #31111D;
      --md-error: #B3261E; --md-on-error: #FFFFFF;
      --md-surface: #FFFBFE; --md-on-surface: #1C1B1F;
      --md-surface-variant: #E7E0EC; --md-on-surface-variant: #49454F;
      --md-outline: #79747E; --md-outline-variant: #CAC4D0;
      --md-inverse-surface: #313033; --md-inverse-on-surface: #F4EFF4;
      --md-surface-1: #F6F0FA; --md-surface-2: #F1EAFA;
      --md-elevation-1: 0 1px 4px 0 rgba(0,0,0,0.37);
      --md-elevation-2: 0 2px 2px 0 rgba(0,0,0,0.2), 0 6px 10px 0 rgba(0,0,0,0.3);
      --md-elevation-3: 0 11px 7px 0 rgba(0,0,0,0.19), 0 13px 25px 0 rgba(0,0,0,0.3);
    }
    * { margin: 0; padding: 0; box-sizing: border-box; }
    body {
      background: var(--md-surface);
      color: var(--md-on-surface);
      font-family: 'Roboto', sans-serif;
      font-size: 0.875rem;
      line-height: 1.25rem;
    }

    /* Top App Bar */
    .top-bar {
      display: flex; align-items: center; height: 64px; padding: 0 16px;
      background: var(--md-surface-2); position: sticky; top: 0; z-index: 100;
    }
    .top-bar__icon {
      width: 48px; height: 48px; display: flex; align-items: center; justify-content: center;
      border: none; background: transparent; border-radius: 50%; cursor: pointer;
      color: var(--md-on-surface); font-size: 1.25rem; transition: background 0.2s;
    }
    .top-bar__icon:hover { background: rgba(28,27,31,0.08); }
    .top-bar__title {
      flex: 1; font-size: 1.375rem; font-weight: 500; margin-left: 4px;
    }

    /* Hero */
    .hero {
      background: var(--md-primary); color: var(--md-on-primary);
      padding: 80px 24px 72px; text-align: center;
      position: relative; overflow: hidden;
    }
    .hero::before {
      content: ''; position: absolute; width: 500px; height: 500px;
      border-radius: 50%; background: rgba(255,255,255,0.06); top: -200px; right: -100px;
    }
    .hero::after {
      content: ''; position: absolute; width: 350px; height: 350px;
      border-radius: 50%; background: rgba(255,255,255,0.04); bottom: -150px; left: -80px;
    }
    .hero__inner { max-width: 840px; margin: 0 auto; position: relative; z-index: 1; }
    .hero__eyebrow {
      font-size: 0.875rem; font-weight: 500; text-transform: uppercase;
      opacity: 0.85; margin-bottom: 16px; letter-spacing: 0.00625rem;
    }
    .hero__title {
      font-family: 'Inter', 'Roboto', sans-serif;
      font-size: clamp(2.25rem, 5vw, 3.5625rem); font-weight: 400;
      line-height: 1.12; margin-bottom: 24px;
    }
    .hero__subtitle {
      font-size: 1.125rem; line-height: 1.75rem; opacity: 0.9;
      max-width: 600px; margin: 0 auto 40px;
    }
    .hero__actions { display: flex; gap: 16px; justify-content: center; flex-wrap: wrap; }

    /* Buttons */
    .btn {
      display: inline-flex; align-items: center; justify-content: center; gap: 8px;
      height: 40px; padding: 0 24px; border: none; border-radius: 20px;
      font-family: 'Roboto', sans-serif; font-size: 0.875rem; font-weight: 500;
      letter-spacing: 0.00625rem; cursor: pointer; text-decoration: none;
      position: relative; overflow: hidden;
      transition: box-shadow 0.2s cubic-bezier(0.4,0,0.2,1);
    }
    .btn::after {
      content: ''; position: absolute; inset: 0; background: currentColor;
      opacity: 0; transition: opacity 0.15s; border-radius: inherit;
    }
    .btn:active::after { opacity: 0.12; }
    .btn--filled { background: var(--md-primary); color: var(--md-on-primary); }
    .btn--filled:hover { box-shadow: var(--md-elevation-1); }
    .btn--on-primary { background: var(--md-on-primary); color: var(--md-primary); }
    .btn--tonal { background: var(--md-secondary-container); color: var(--md-on-secondary-container); }
    .btn--outlined { background: transparent; color: var(--md-primary); border: 1px solid var(--md-outline); }
    .btn--outlined:hover { background: rgba(103,80,164,0.08); }
    .btn--text { background: transparent; color: var(--md-primary); padding: 0 12px; }
    .btn--hero-outline { color: rgba(255,255,255,0.9); border: 1px solid rgba(255,255,255,0.4); background: transparent; }

    /* Sections */
    .section { padding: 64px 24px; max-width: 1200px; margin: 0 auto; }
    .section__header { text-align: center; margin-bottom: 48px; }
    .section__title {
      font-family: 'Inter', 'Roboto', sans-serif; font-size: 1.75rem;
      font-weight: 400; margin-bottom: 8px;
    }
    .section__subtitle { font-size: 1rem; color: var(--md-on-surface-variant); max-width: 600px; margin: 0 auto; }

    /* Cards */
    .card-grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(280px, 1fr)); gap: 24px; }
    .card {
      background: var(--md-surface); border-radius: 12px; overflow: hidden;
      box-shadow: var(--md-elevation-1);
      transition: box-shadow 0.2s cubic-bezier(0.4,0,0.2,1);
    }
    .card:hover { box-shadow: var(--md-elevation-2); }
    .card__media {
      width: 100%; height: 180px; display: flex;
      align-items: center; justify-content: center; font-size: 3rem;
    }
    .card__content { padding: 16px; }
    .card__title { font-size: 1.375rem; font-weight: 500; margin-bottom: 4px; }
    .card__subtitle { font-size: 0.875rem; color: var(--md-on-surface-variant); margin-bottom: 12px; }
    .card__body { font-size: 0.875rem; line-height: 1.25rem; color: var(--md-on-surface-variant); }
    .card__actions { padding: 8px; display: flex; gap: 8px; justify-content: flex-end; }

    /* Chips */
    .chip-row { display: flex; gap: 8px; flex-wrap: wrap; justify-content: center; margin-bottom: 40px; }
    .chip {
      display: inline-flex; align-items: center; height: 32px; padding: 0 16px;
      border-radius: 8px; border: 1px solid var(--md-outline); background: transparent;
      color: var(--md-on-surface); font-family: 'Roboto', sans-serif;
      font-size: 0.875rem; font-weight: 500; cursor: pointer; transition: background 0.2s;
    }
    .chip:hover { background: rgba(28,27,31,0.08); }
    .chip--selected {
      background: var(--md-secondary-container); color: var(--md-on-secondary-container);
      border-color: transparent;
    }

    /* Stats */
    .stats { background: var(--md-surface-1); padding: 64px 24px; }
    .stats__grid {
      display: grid; grid-template-columns: repeat(auto-fit, minmax(180px, 1fr));
      gap: 32px; max-width: 1000px; margin: 0 auto; text-align: center;
    }
    .stat__number {
      font-family: 'Inter', 'Roboto', sans-serif; font-size: 2.8125rem;
      font-weight: 400; color: var(--md-primary); margin-bottom: 8px;
    }
    .stat__label { font-size: 0.875rem; font-weight: 500; color: var(--md-on-surface-variant); }

    /* CTA */
    .cta {
      background: var(--md-tertiary-container); color: var(--md-on-tertiary-container);
      text-align: center; padding: 80px 24px;
    }
    .cta__title {
      font-family: 'Inter', 'Roboto', sans-serif;
      font-size: clamp(1.75rem, 3vw, 2.25rem); font-weight: 400; margin-bottom: 16px;
    }
    .cta__subtitle { font-size: 1rem; opacity: 0.85; max-width: 500px; margin: 0 auto 32px; }
    .cta .btn--filled { background: var(--md-tertiary); color: var(--md-on-tertiary); }

    /* Footer */
    .footer { background: var(--md-inverse-surface); color: var(--md-inverse-on-surface); padding: 40px 24px; }
    .footer__inner {
      max-width: 1200px; margin: 0 auto; display: flex; justify-content: space-between;
      align-items: center; flex-wrap: wrap; gap: 16px;
    }
    .footer__brand { font-family: 'Inter', sans-serif; font-size: 1.25rem; font-weight: 700; }
    .footer__links { display: flex; gap: 24px; list-style: none; }
    .footer__links a { color: var(--md-inverse-on-surface); text-decoration: none; font-size: 0.875rem; opacity: 0.7; }
    .footer__links a:hover { opacity: 1; }
    .footer__copy { width: 100%; text-align: center; margin-top: 24px; font-size: 0.75rem; opacity: 0.5; }

    /* FAB */
    .fab {
      position: fixed; bottom: 24px; right: 24px; width: 56px; height: 56px;
      border-radius: 16px; border: none; background: var(--md-primary-container);
      color: var(--md-on-primary-container); font-size: 1.5rem; cursor: pointer;
      display: flex; align-items: center; justify-content: center;
      box-shadow: var(--md-elevation-3); z-index: 50;
      transition: box-shadow 0.2s cubic-bezier(0.4,0,0.2,1);
    }
    .fab:hover { box-shadow: 0 14px 12px 0 rgba(0,0,0,0.17), 0 20px 40px 0 rgba(0,0,0,0.3); }

    /* Responsive */
    @media (max-width: 600px) {
      .hero { padding: 56px 16px 48px; }
      .hero__title { font-size: 2rem; }
      .section { padding: 48px 16px; }
      .card-grid { grid-template-columns: 1fr; }
      .footer__inner { flex-direction: column; text-align: center; }
      .footer__links { flex-direction: column; gap: 12px; }
    }
  </style>
</head>
<body>
  <header class="top-bar">
    <button class="top-bar__icon" aria-label="Menu">&#9776;</button>
    <span class="top-bar__title">MaterialApp</span>
    <div style="display:flex;gap:4px;">
      <button class="top-bar__icon" aria-label="Search">&#128269;</button>
      <button class="top-bar__icon" aria-label="More">&#8942;</button>
    </div>
  </header>

  <section class="hero">
    <div class="hero__inner">
      <p class="hero__eyebrow">Material Design 3</p>
      <h1 class="hero__title">Build beautiful, usable products</h1>
      <p class="hero__subtitle">A design system combining purposeful color, meaningful motion, and layered surfaces for intuitive and accessible interfaces.</p>
      <div class="hero__actions">
        <a href="#cards" class="btn btn--on-primary">Get Started</a>
        <a href="#stats" class="btn btn--hero-outline">Learn More</a>
      </div>
    </div>
  </section>

  <section class="section">
    <div class="section__header">
      <h2 class="section__title">Explore Components</h2>
      <p class="section__subtitle">Adaptive, flexible components built for any platform.</p>
    </div>
    <div class="chip-row">
      <button class="chip chip--selected">All</button>
      <button class="chip">Buttons</button>
      <button class="chip">Cards</button>
      <button class="chip">Navigation</button>
      <button class="chip">Inputs</button>
    </div>
    <div class="card-grid" id="cards">
      <div class="card">
        <div class="card__media" style="background:var(--md-primary-container);">
          <svg width="72" height="72" viewBox="0 0 72 72" fill="none">
            <rect x="10" y="16" width="52" height="40" rx="8" fill="var(--md-primary)" opacity="0.2"/>
            <rect x="18" y="24" width="36" height="24" rx="4" fill="var(--md-primary)" opacity="0.4"/>
            <rect x="24" y="32" width="24" height="8" rx="4" fill="var(--md-primary)"/>
          </svg>
        </div>
        <div class="card__content">
          <h3 class="card__title">Elevation</h3>
          <p class="card__subtitle">Layered surfaces</p>
          <p class="card__body">Surfaces at different elevations cast shadows that communicate hierarchy and interactive depth.</p>
        </div>
        <div class="card__actions"><button class="btn btn--text">Learn More</button></div>
      </div>
      <div class="card">
        <div class="card__media" style="background:var(--md-secondary-container);">
          <svg width="72" height="72" viewBox="0 0 72 72" fill="none">
            <circle cx="26" cy="36" r="14" fill="var(--md-secondary)" opacity="0.3"/>
            <circle cx="46" cy="36" r="14" fill="var(--md-tertiary)" opacity="0.3"/>
            <circle cx="36" cy="24" r="14" fill="var(--md-primary)" opacity="0.3"/>
          </svg>
        </div>
        <div class="card__content">
          <h3 class="card__title">Color System</h3>
          <p class="card__subtitle">Dynamic theming</p>
          <p class="card__body">A tonal palette with semantic roles enables cohesive theming and automatic dark mode adaptation.</p>
        </div>
        <div class="card__actions"><button class="btn btn--text">Learn More</button></div>
      </div>
      <div class="card">
        <div class="card__media" style="background:var(--md-tertiary-container);">
          <svg width="72" height="72" viewBox="0 0 72 72" fill="none">
            <rect x="14" y="20" width="44" height="7" rx="3.5" fill="var(--md-tertiary)" opacity="0.3"/>
            <rect x="14" y="32" width="32" height="5" rx="2.5" fill="var(--md-tertiary)" opacity="0.5"/>
            <rect x="14" y="42" width="44" height="5" rx="2.5" fill="var(--md-tertiary)" opacity="0.2"/>
          </svg>
        </div>
        <div class="card__content">
          <h3 class="card__title">Typography</h3>
          <p class="card__subtitle">Type scale system</p>
          <p class="card__body">Defined text styles from display to label with precise size, weight, and spacing for clear hierarchy.</p>
        </div>
        <div class="card__actions"><button class="btn btn--text">Learn More</button></div>
      </div>
    </div>
  </section>

  <section class="stats" id="stats">
    <div class="stats__grid">
      <div><div class="stat__number">1000+</div><div class="stat__label">Components</div></div>
      <div><div class="stat__number">3B+</div><div class="stat__label">Devices Worldwide</div></div>
      <div><div class="stat__number">48dp</div><div class="stat__label">Min Touch Target</div></div>
      <div><div class="stat__number">8dp</div><div class="stat__label">Baseline Grid</div></div>
    </div>
  </section>

  <section class="section">
    <div class="section__header">
      <h2 class="section__title">Button Variants</h2>
      <p class="section__subtitle">Each button type serves a distinct role in the interface hierarchy.</p>
    </div>
    <div style="display:flex;gap:16px;justify-content:center;flex-wrap:wrap;">
      <button class="btn btn--filled">Filled</button>
      <button class="btn btn--tonal">Tonal</button>
      <button class="btn btn--outlined">Outlined</button>
      <button class="btn btn--text">Text</button>
    </div>
  </section>

  <section class="cta">
    <h2 class="cta__title">Ready to build with Material?</h2>
    <p class="cta__subtitle">Create accessible, beautiful, and consistent interfaces with the full design system.</p>
    <a href="#" class="btn btn--filled">Start Building</a>
  </section>

  <footer class="footer">
    <div class="footer__inner">
      <div class="footer__brand">MaterialApp</div>
      <ul class="footer__links">
        <li><a href="#">Documentation</a></li>
        <li><a href="#">Components</a></li>
        <li><a href="#">Design Tokens</a></li>
        <li><a href="#">GitHub</a></li>
      </ul>
      <p class="footer__copy">Built with Material Design 3 principles.</p>
    </div>
  </footer>

  <button class="fab" aria-label="Compose">&#10011;</button>
</body>
</html>
```

---

## Implementation Tips

- **Use CSS custom properties for the entire color system** so that switching between light and dark themes requires only reassigning variable values on a single selector (e.g., `[data-theme="dark"]`) rather than overriding individual component styles
- **Implement elevation with shadow custom properties** (e.g., `--md-elevation-1` through `--md-elevation-5`) and apply them semantically based on component role, not by manually writing box-shadow values on each element
- **Build the ripple/state-layer effect with a `::after` pseudo-element** using `background: currentColor` and varying opacity (0.08 hover, 0.12 pressed, 0.16 focus) for lightweight implementations without heavy JavaScript ripple libraries
- **Follow the 8dp grid by defining spacing utilities in multiples of 8** (e.g., `--space-1: 8px`, `--space-2: 16px`, `--space-3: 24px`) and reserve 4dp only for internal component fine-tuning like icon-to-text gaps
- **Use `cubic-bezier(0.2, 0, 0, 1)` as your standard easing curve** with durations of 200ms for simple state changes, 300ms for expansion/collapse, and 500ms for full-screen transitions
- **Leverage Google's Material Theme Builder** to generate a complete tonal palette from a single seed color, then export the CSS custom properties directly rather than manually calculating tonal values
