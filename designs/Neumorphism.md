# Neumorphism

## Overview

Neumorphism (also called Soft UI or Neo-skeuomorphism) is a UI design aesthetic that creates the illusion of elements extruding from or recessing into the background surface, as if molded from a single sheet of soft material. The effect is achieved through carefully paired light and dark shadows on elements that share the same color as their parent background, producing a subtle, tactile dimensionality that sits between flat design and full skeuomorphism. Coined by designer Jason Kelley and popularized by Alexander Plyuto's Dribbble explorations in late 2019, the style evokes extruded plastic, embossed paper, or molded rubber -- surfaces that feel physically continuous rather than layered.

## Visual Characteristics

- **Extruded from the surface**: UI elements appear to push outward from the background rather than floating above it; element and background are visually part of the same continuous material
- **Dual directional shadows**: Every raised element uses two box-shadows -- a dark shadow on one side (typically bottom-right) and a light shadow on the opposite side (typically top-left) -- simulating a single consistent light source
- **Monochromatic color scheme**: Elements share the same (or nearly the same) background color as their parent container; color differentiation is minimal, with depth conveyed through shadow alone
- **Low contrast**: The entire interface operates at deliberately low contrast ratios; visual hierarchy comes from shadow depth rather than color variation
- **Soft, rounded corners**: Generous border-radius values are essential; sharp edges are nearly absent, reinforcing the soft, molded material metaphor
- **No borders or outlines**: Element boundaries are defined exclusively through shadow and light; traditional borders, outlines, and hard edges are eliminated
- **Inset shadows for active states**: Interactive elements use inset (concave) shadows to communicate pressed or active states, creating a dented-into-the-surface effect
- **Minimal ornamentation**: The style is reductive and clean; decorative elements, textures, and patterns are avoided in favor of pure form and shadow
- **Single light source**: All shadows across the interface must originate from one consistent direction to maintain the physical illusion; mixed light directions break the effect
- **Subtle surface gradients**: Optional convex/concave gradients on element surfaces can enhance the 3D illusion -- lighter toward the light source, darker away from it

### Design Principles

- The background color is the foundation; every element derives its color from the background
- Shadow is the only tool for creating depth and hierarchy -- never rely on color contrast alone
- Maintain a single, consistent light source direction across the entire interface (top-left is most common)
- Raised elements use outset shadows; pressed/active elements use inset shadows
- Keep the number of depth levels limited (raised, flat, recessed) to avoid visual confusion
- Use accent colors sparingly and only for interactive highlights (toggles, active indicators, progress bars)
- Generous padding and spacing are critical; cramped layouts undermine the soft, breathable aesthetic

---

## Color Palette

### Light Theme (Primary)

Neumorphism is inherently monochromatic. The entire palette derives from a single background hue with shadows computed as darker and lighter variants of that base.

| Role | Hex | Description |
|------|-----|-------------|
| Background base | `#e0e5ec` | The canonical neumorphic background; a cool, slightly blue-tinted light gray |
| Dark shadow | `#a3b1c6` | Shadow cast away from light source (~15-20% darker than base) |
| Light shadow | `#ffffff` | Highlight shadow toward light source (pure white or near-white) |
| Text primary | `#2d3436` | Dark charcoal for primary text; sufficient contrast on light gray |
| Text secondary | `#636e72` | Medium gray for secondary text and labels |
| Text muted | `#b2bec3` | Light gray for placeholders and disabled text |

### Alternative Light Bases

| Name | Hex | Shadow Dark | Shadow Light | Vibe |
|------|-----|-------------|--------------|------|
| Warm gray | `#e8e0d8` | `#c4bdb6` | `#ffffff` | Warmer, organic feel |
| Cool lavender | `#e6e7ee` | `#b8b9bf` | `#ffffff` | The Themesberg Neumorphism UI default |
| Neutral gray | `#e0e0e0` | `#bebebe` | `#ffffff` | Pure neutral, no color cast |
| Soft mint | `#dce8e0` | `#b5c2b8` | `#ffffff` | Subtle green undertone |
| Pale blue | `#dde4f0` | `#b0b8c6` | `#ffffff` | Slightly more saturated cool tone |

### Dark Theme

| Role | Hex | Description |
|------|-----|-------------|
| Background base | `#2d2d2d` | Deep neutral dark gray |
| Dark shadow | `#252525` | ~10% darker than base |
| Light shadow | `#353535` | ~10% lighter than base |
| Alt background | `#303030` | Slightly lighter variant for layering |
| Text primary | `#e0e0e0` | Light text for dark surfaces |
| Text secondary | `#a0a0a0` | Muted light text |

### Accent Colors

Used sparingly for interactive states, toggles, progress indicators, and focus rings:

| Role | Hex | Description |
|------|-----|-------------|
| Primary accent | `#4d7cff` | Soft blue for active states and links |
| Success | `#55efc4` | Muted mint green |
| Warning | `#ffeaa7` | Soft warm yellow |
| Danger | `#ff7675` | Soft coral red |
| Info | `#74b9ff` | Light sky blue |
| Active toggle | `#6c5ce7` | Muted purple for on-state indicators |

### CSS Custom Properties

```css
:root {
  /* Base surface */
  --neu-bg: #e0e5ec;
  --neu-shadow-dark: #a3b1c6;
  --neu-shadow-light: #ffffff;

  /* Text */
  --neu-text-primary: #2d3436;
  --neu-text-secondary: #636e72;
  --neu-text-muted: #b2bec3;

  /* Accent */
  --neu-accent: #4d7cff;
  --neu-accent-soft: rgba(77, 124, 255, 0.15);
  --neu-success: #55efc4;
  --neu-warning: #ffeaa7;
  --neu-danger: #ff7675;

  /* Shadow distances */
  --neu-distance: 8px;
  --neu-blur: 15px;
  --neu-distance-sm: 4px;
  --neu-blur-sm: 8px;
  --neu-distance-lg: 12px;
  --neu-blur-lg: 24px;
}
```

### Shadow Color Derivation Rule

For any base background color, compute shadows as follows:
- **Dark shadow**: Decrease lightness by 15-20% from the base color, apply at 50-80% opacity
- **Light shadow**: Increase lightness by 15-20% (or use pure white), apply at 60-80% opacity
- Both shadows use the same offset distance but in opposite directions

---

## Typography

### Typeface Characteristics

Neumorphism typography should be:

- **Clean, rounded sans-serif** -- matching the soft, molded surfaces of the UI
- **Highly legible** -- critical because the low-contrast environment already challenges readability
- **Medium to semi-bold weights** -- thin weights disappear against the soft gray backgrounds; bold weights for headings provide necessary contrast
- **No serifs, no decorative faces** -- angular or ornate type clashes with the rounded, minimal aesthetic
- **Generous sizing** -- body text should be at least 16px to remain comfortable against low-contrast surfaces

### Recommended Web Fonts (Google Fonts)

| Font | Weight(s) | Usage | Link |
|------|-----------|-------|------|
| **Nunito Sans** | 400, 600, 700 | Primary UI font; the default for the Neumorphism UI framework | [Nunito Sans](https://fonts.google.com/specimen/Nunito+Sans) |
| **Nunito** | 400, 600, 700 | Rounded terminals; ideal match for soft neumorphic surfaces | [Nunito](https://fonts.google.com/specimen/Nunito) |
| **Inter** | 400, 500, 600 | Excellent screen legibility at small sizes; tall x-height | [Inter](https://fonts.google.com/specimen/Inter) |
| **Poppins** | 300, 400, 500, 600 | Geometric and modern; works well for headings | [Poppins](https://fonts.google.com/specimen/Poppins) |
| **Quicksand** | 400, 500, 700 | Rounded geometric; reinforces the soft material metaphor | [Quicksand](https://fonts.google.com/specimen/Quicksand) |
| **Varela Round** | 400 | Single-weight rounded sans; clean and friendly | [Varela Round](https://fonts.google.com/specimen/Varela+Round) |
| **DM Sans** | 400, 500, 700 | Clean geometric sans-serif; good body text alternative | [DM Sans](https://fonts.google.com/specimen/DM+Sans) |

### Font Pairing Suggestions

| Heading Font | Body Font | Character |
|-------------|-----------|-----------|
| **Poppins** (600) | **Nunito Sans** (400) | Modern, geometric, polished |
| **Quicksand** (700) | **Nunito** (400) | Soft, rounded, cohesive |
| **Nunito** (700) | **Inter** (400) | Friendly headings, legible body |
| **DM Sans** (700) | **Nunito Sans** (400) | Clean and minimal |

### Typography CSS Example

```css
@import url('https://fonts.googleapis.com/css2?family=Nunito+Sans:wght@400;600;700&family=Poppins:wght@400;500;600&display=swap');

body {
  font-family: 'Nunito Sans', -apple-system, BlinkMacSystemFont, sans-serif;
  font-weight: 400;
  font-size: 1rem;
  line-height: 1.6;
  color: var(--neu-text-primary);
  -webkit-font-smoothing: antialiased;
}

h1, h2, h3, h4, h5, h6 {
  font-family: 'Poppins', 'Nunito Sans', sans-serif;
  font-weight: 600;
  color: var(--neu-text-primary);
  line-height: 1.2;
  letter-spacing: -0.01em;
}

.neu-display {
  font-family: 'Poppins', sans-serif;
  font-size: clamp(2.5rem, 5vw, 4rem);
  font-weight: 600;
  letter-spacing: -0.02em;
  line-height: 1.1;
}

.neu-label {
  font-family: 'Nunito Sans', sans-serif;
  font-weight: 700;
  font-size: 0.85rem;
  letter-spacing: 0.05em;
  text-transform: uppercase;
  color: var(--neu-text-secondary);
}
```

---

## Layout Principles

### Grid and Structure

- **Single background color foundation**: The entire page shares one background color; sections are not distinguished by background changes but by shadow-defined containers
- **Centered, constrained containers**: Max-width of 900-1100px to keep the soft shadow effects at a comfortable viewing scale
- **Generous spacing**: Ample padding inside elements (32-48px) and between them (24-40px gaps); the extruded illusion requires visual breathing room
- **Card-based organization**: Content is grouped into neumorphic cards that extrude from the surface
- **Rounded everything**: All containers, buttons, inputs, and cards use generous border-radius (12-25px for cards, 8-16px for smaller elements, 999px for pill shapes)
- **Flat visual hierarchy**: Since color contrast is minimal, use shadow depth (small vs. large shadows) and element size to establish hierarchy
- **Avoid dense layouts**: Too many extruded elements in close proximity creates visual noise; leave generous gaps between neumorphic surfaces

### Section Organization

- **Navigation**: Neumorphic bar or set of pill-shaped links raised from the background; active state uses inset shadow
- **Hero**: Large display text with a prominent neumorphic card or circular element; accent color used sparingly for CTA
- **Content cards**: Raised neumorphic panels arranged in a grid or vertical stack with generous gaps
- **Interactive elements**: Buttons raised from the surface; inputs recessed into it; toggles switch between raised and inset states
- **Metrics / stats**: Large numbers displayed in individual neumorphic circles or rounded squares
- **Footer**: Subtle, recessed treatment or minimal flat text; avoid heavy shadow at the bottom of the page

### Responsive Approach

- Reduce shadow distances at smaller viewports (use `--neu-distance-sm` below 768px)
- Stack card grids to single column on mobile
- Maintain generous padding even at small sizes -- never let neumorphic elements touch or overlap
- Scale border-radius proportionally; 20px on desktop can become 14px on mobile

---

## CSS Code Snippets

### Raised (Convex) Element

The fundamental neumorphic effect -- element appears to push out from the background:

```css
.neu-raised {
  background: var(--neu-bg);
  border-radius: 20px;
  padding: 32px;
  box-shadow:
    8px 8px 15px var(--neu-shadow-dark),
    -8px -8px 15px var(--neu-shadow-light);
}
```

### Pressed (Concave) Element

Element appears dented into the surface -- used for active states and input fields:

```css
.neu-pressed {
  background: var(--neu-bg);
  border-radius: 20px;
  padding: 32px;
  box-shadow:
    inset 5px 5px 10px var(--neu-shadow-dark),
    inset -5px -5px 10px var(--neu-shadow-light);
}
```

### Flat Element (No Shadow)

Resting state with no elevation -- useful for transitional states:

```css
.neu-flat {
  background: var(--neu-bg);
  border-radius: 20px;
  padding: 32px;
  box-shadow: none;
}
```

### Neumorphic Card

```css
.neu-card {
  background: var(--neu-bg);
  border-radius: 20px;
  padding: 40px;
  box-shadow:
    8px 8px 15px rgba(163, 177, 198, 0.5),
    -8px -8px 15px rgba(255, 255, 255, 0.6);
}
```

### Neumorphic Button

```css
.neu-button {
  background: var(--neu-bg);
  color: var(--neu-text-primary);
  border: none;
  border-radius: 12px;
  padding: 14px 32px;
  font-family: 'Nunito Sans', sans-serif;
  font-weight: 600;
  font-size: 1rem;
  cursor: pointer;
  transition: box-shadow 0.2s ease;
  box-shadow:
    5px 5px 10px rgba(163, 177, 198, 0.5),
    -5px -5px 10px rgba(255, 255, 255, 0.6);
}

.neu-button:hover {
  box-shadow:
    3px 3px 6px rgba(163, 177, 198, 0.5),
    -3px -3px 6px rgba(255, 255, 255, 0.6);
}

.neu-button:active {
  box-shadow:
    inset 3px 3px 6px rgba(163, 177, 198, 0.5),
    inset -3px -3px 6px rgba(255, 255, 255, 0.8);
}
```

### Accent Button (with color highlight)

```css
.neu-button-accent {
  background: var(--neu-accent);
  color: #ffffff;
  border: none;
  border-radius: 12px;
  padding: 14px 32px;
  font-family: 'Nunito Sans', sans-serif;
  font-weight: 600;
  font-size: 1rem;
  cursor: pointer;
  transition: box-shadow 0.2s ease, transform 0.15s ease;
  box-shadow:
    5px 5px 10px rgba(163, 177, 198, 0.5),
    -5px -5px 10px rgba(255, 255, 255, 0.6);
}

.neu-button-accent:hover {
  transform: translateY(-1px);
  box-shadow:
    6px 6px 12px rgba(163, 177, 198, 0.6),
    -6px -6px 12px rgba(255, 255, 255, 0.7);
}

.neu-button-accent:active {
  transform: translateY(0);
  box-shadow:
    inset 3px 3px 6px rgba(50, 80, 180, 0.3),
    inset -3px -3px 6px rgba(120, 170, 255, 0.4);
}
```

### Neumorphic Input Field

```css
.neu-input {
  background: var(--neu-bg);
  border: none;
  border-radius: 10px;
  padding: 14px 20px;
  font-family: 'Nunito Sans', sans-serif;
  font-size: 1rem;
  color: var(--neu-text-primary);
  outline: none;
  box-shadow:
    inset 5px 5px 10px rgba(163, 177, 198, 0.5),
    inset -5px -5px 12px rgba(255, 255, 255, 0.8);
}

.neu-input::placeholder {
  color: var(--neu-text-muted);
}

.neu-input:focus {
  box-shadow:
    inset 5px 5px 10px rgba(163, 177, 198, 0.5),
    inset -5px -5px 12px rgba(255, 255, 255, 0.8),
    0 0 0 3px var(--neu-accent-soft);
}
```

### Neumorphic Toggle Switch

```css
.neu-toggle {
  width: 56px;
  height: 30px;
  background: var(--neu-bg);
  border-radius: 999px;
  position: relative;
  cursor: pointer;
  box-shadow:
    inset 4px 4px 8px rgba(163, 177, 198, 0.5),
    inset -4px -4px 8px rgba(255, 255, 255, 0.7);
  transition: background 0.3s ease;
}

.neu-toggle::after {
  content: '';
  width: 24px;
  height: 24px;
  background: var(--neu-bg);
  border-radius: 50%;
  position: absolute;
  top: 3px;
  left: 3px;
  transition: transform 0.3s ease, box-shadow 0.3s ease;
  box-shadow:
    3px 3px 6px rgba(163, 177, 198, 0.5),
    -3px -3px 6px rgba(255, 255, 255, 0.6);
}

.neu-toggle.active {
  background: var(--neu-accent);
}

.neu-toggle.active::after {
  transform: translateX(26px);
  box-shadow:
    3px 3px 6px rgba(50, 80, 180, 0.3),
    -3px -3px 6px rgba(120, 170, 255, 0.4);
}
```

### Neumorphic Circular Element

```css
.neu-circle {
  width: 100px;
  height: 100px;
  background: var(--neu-bg);
  border-radius: 50%;
  display: flex;
  align-items: center;
  justify-content: center;
  box-shadow:
    8px 8px 15px rgba(163, 177, 198, 0.5),
    -8px -8px 15px rgba(255, 255, 255, 0.6);
}
```

### Neumorphic Progress Bar

```css
.neu-progress-track {
  background: var(--neu-bg);
  border-radius: 999px;
  height: 14px;
  box-shadow:
    inset 3px 3px 6px rgba(163, 177, 198, 0.5),
    inset -3px -3px 6px rgba(255, 255, 255, 0.7);
  overflow: hidden;
  padding: 3px;
}

.neu-progress-fill {
  background: var(--neu-accent);
  height: 100%;
  border-radius: 999px;
  box-shadow:
    2px 2px 4px rgba(50, 80, 180, 0.3),
    -2px -2px 4px rgba(120, 170, 255, 0.3);
  transition: width 0.4s ease;
}
```

### Convex Surface Gradient (Optional Enhancement)

Adding a subtle gradient to the element surface enhances the 3D illusion:

```css
.neu-raised-convex {
  background: linear-gradient(145deg, #e6ebf2, #ccd1d8);
  border-radius: 20px;
  padding: 32px;
  box-shadow:
    8px 8px 15px #a3b1c6,
    -8px -8px 15px #ffffff;
}

.neu-pressed-concave {
  background: linear-gradient(145deg, #ccd1d8, #e6ebf2);
  border-radius: 20px;
  padding: 32px;
  box-shadow:
    inset 5px 5px 10px #a3b1c6,
    inset -5px -5px 10px #ffffff;
}
```

### Neumorphic Divider

```css
.neu-divider {
  height: 2px;
  background: var(--neu-bg);
  border: none;
  margin: 24px 0;
  box-shadow:
    0px 1px 2px rgba(163, 177, 198, 0.5),
    0px -1px 1px rgba(255, 255, 255, 0.6);
}
```

### Full Background Setup

```css
html, body {
  background: var(--neu-bg);
  min-height: 100vh;
}
```

---

## Full Page Starter Template

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Neumorphism Layout</title>
  <link href="https://fonts.googleapis.com/css2?family=Nunito+Sans:wght@400;600;700&family=Poppins:wght@400;600&display=swap" rel="stylesheet">
  <style>
    :root {
      --neu-bg: #e0e5ec;
      --neu-shadow-dark: rgba(163, 177, 198, 0.6);
      --neu-shadow-light: rgba(255, 255, 255, 0.7);
      --neu-text-primary: #2d3436;
      --neu-text-secondary: #636e72;
      --neu-text-muted: #b2bec3;
      --neu-accent: #4d7cff;
    }

    *, *::before, *::after { margin: 0; padding: 0; box-sizing: border-box; }

    body {
      font-family: 'Nunito Sans', sans-serif;
      font-weight: 400;
      font-size: 1rem;
      line-height: 1.6;
      color: var(--neu-text-primary);
      background: var(--neu-bg);
      min-height: 100vh;
      display: flex;
      flex-direction: column;
      align-items: center;
      padding: 3rem 1.5rem;
      gap: 2.5rem;
      -webkit-font-smoothing: antialiased;
    }

    h1, h2, h3 {
      font-family: 'Poppins', sans-serif;
      font-weight: 600;
      line-height: 1.2;
    }

    /* Navigation */
    nav {
      display: flex;
      align-items: center;
      justify-content: space-between;
      width: 100%;
      max-width: 900px;
      background: var(--neu-bg);
      border-radius: 16px;
      padding: 16px 28px;
      box-shadow:
        6px 6px 12px var(--neu-shadow-dark),
        -6px -6px 12px var(--neu-shadow-light);
    }

    nav a.logo {
      font-family: 'Poppins', sans-serif;
      font-weight: 700;
      font-size: 1.2rem;
      color: var(--neu-text-primary);
      text-decoration: none;
    }

    nav ul {
      display: flex;
      gap: 24px;
      list-style: none;
    }

    nav ul a {
      color: var(--neu-text-secondary);
      text-decoration: none;
      font-weight: 600;
      font-size: 0.9rem;
      padding: 8px 16px;
      border-radius: 10px;
      transition: box-shadow 0.2s ease;
    }

    nav ul a:hover {
      box-shadow:
        inset 3px 3px 6px var(--neu-shadow-dark),
        inset -3px -3px 6px var(--neu-shadow-light);
    }

    /* Hero */
    .hero {
      text-align: center;
      max-width: 600px;
      padding: 2rem 0;
    }

    .hero h1 {
      font-size: clamp(2rem, 5vw, 3.5rem);
      margin-bottom: 1rem;
      letter-spacing: -0.02em;
    }

    .hero p {
      color: var(--neu-text-secondary);
      font-size: 1.1rem;
      margin-bottom: 2rem;
    }

    /* Cards grid */
    .card-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(260px, 1fr));
      gap: 28px;
      max-width: 900px;
      width: 100%;
    }

    .neu-card {
      background: var(--neu-bg);
      border-radius: 20px;
      padding: 36px;
      box-shadow:
        8px 8px 15px var(--neu-shadow-dark),
        -8px -8px 15px var(--neu-shadow-light);
    }

    .neu-card h3 {
      margin-bottom: 0.75rem;
      font-size: 1.15rem;
    }

    .neu-card p {
      color: var(--neu-text-secondary);
      font-size: 0.95rem;
      line-height: 1.6;
    }

    /* Icon circle */
    .icon-circle {
      width: 56px;
      height: 56px;
      background: var(--neu-bg);
      border-radius: 50%;
      display: flex;
      align-items: center;
      justify-content: center;
      margin-bottom: 1.25rem;
      font-size: 1.5rem;
      box-shadow:
        4px 4px 8px var(--neu-shadow-dark),
        -4px -4px 8px var(--neu-shadow-light);
    }

    /* Button */
    .btn {
      display: inline-block;
      background: var(--neu-accent);
      color: #ffffff;
      border: none;
      border-radius: 12px;
      padding: 14px 36px;
      font-family: 'Nunito Sans', sans-serif;
      font-weight: 700;
      font-size: 1rem;
      cursor: pointer;
      text-decoration: none;
      box-shadow:
        5px 5px 10px var(--neu-shadow-dark),
        -5px -5px 10px var(--neu-shadow-light);
      transition: box-shadow 0.2s ease, transform 0.15s ease;
    }

    .btn:hover {
      transform: translateY(-1px);
    }

    .btn:active {
      transform: translateY(0);
      box-shadow:
        inset 3px 3px 6px rgba(50, 80, 180, 0.3),
        inset -3px -3px 6px rgba(120, 170, 255, 0.4);
    }

    /* Footer */
    footer {
      color: var(--neu-text-muted);
      font-size: 0.85rem;
      padding: 2rem 0;
      text-align: center;
    }

    @media (max-width: 768px) {
      body { padding: 2rem 1rem; }
      nav { flex-direction: column; gap: 12px; }
      nav ul { gap: 12px; }
    }
  </style>
</head>
<body>
  <nav>
    <a href="#" class="logo">SoftUI</a>
    <ul>
      <li><a href="#">Features</a></li>
      <li><a href="#">Pricing</a></li>
      <li><a href="#">About</a></li>
    </ul>
  </nav>

  <div class="hero">
    <h1>Design that feels real</h1>
    <p>Soft shadows and subtle depth create interfaces that look like they are molded from a single surface.</p>
    <a href="#" class="btn">Get Started</a>
  </div>

  <div class="card-grid">
    <div class="neu-card">
      <div class="icon-circle">
        <svg width="24" height="24" viewBox="0 0 24 24" fill="none"><circle cx="12" cy="12" r="9" stroke="#4d7cff" stroke-width="2"/><path d="M12 7v5l3 3" stroke="#4d7cff" stroke-width="2" stroke-linecap="round"/></svg>
      </div>
      <h3>Subtle Depth</h3>
      <p>Dual shadows create a tactile illusion of elements rising from the background surface.</p>
    </div>
    <div class="neu-card">
      <div class="icon-circle">
        <svg width="24" height="24" viewBox="0 0 24 24" fill="none"><rect x="4" y="4" width="16" height="16" rx="4" stroke="#4d7cff" stroke-width="2"/><path d="M9 12l2 2 4-4" stroke="#4d7cff" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/></svg>
      </div>
      <h3>Soft Interaction</h3>
      <p>Pressed states invert the shadow direction, giving buttons a satisfying physical response.</p>
    </div>
    <div class="neu-card">
      <div class="icon-circle">
        <svg width="24" height="24" viewBox="0 0 24 24" fill="none"><circle cx="12" cy="12" r="4" fill="#4d7cff"/><circle cx="12" cy="12" r="9" stroke="#4d7cff" stroke-width="2" stroke-dasharray="4 3"/></svg>
      </div>
      <h3>Monochrome Calm</h3>
      <p>A restrained palette keeps the focus on form and shadow rather than color competition.</p>
    </div>
  </div>

  <footer>
    <p>Molded from a single surface. Neumorphism in action.</p>
  </footer>
</body>
</html>
```

## Implementation Tips

- **Background color is everything**: The element and its parent must share the same (or very similar) background color. If they differ, the extrusion illusion breaks immediately.
- **Always pair shadows**: A neumorphic element without both a dark and light shadow looks like a plain drop shadow, not a neumorphic surface. Both are mandatory.
- **Consistent light direction**: Pick one light source (top-left is conventional) and use it across the entire page. Mixed light directions destroy the physical coherence.
- **Inset for interaction**: Swap outset shadows to inset shadows for active/pressed states. This is the primary way to communicate interaction in a neumorphic UI.
- **Avoid pure white or pure black backgrounds**: The effect works best on muted, mid-light tones (lightness 80-90% in HSL) where both dark and light shadows are clearly visible.
- **Shadow distance and blur**: Keep shadow offsets proportional to the element size. Small elements (buttons, toggles) use 3-6px offsets; medium elements (cards) use 6-10px; large elements (panels) use 10-15px. Blur should be 1.5-2x the offset distance.
- **Accent color sparingly**: In a monochromatic system, even a small splash of color draws heavy attention. Reserve accent colors for primary CTAs, active toggles, and focus indicators.
- **Accessibility caveat**: Neumorphism's low contrast is its biggest limitation. Always ensure text meets WCAG AA contrast ratios (4.5:1 for body text). Consider offering a high-contrast mode or using stronger text colors than the surrounding surfaces.
- **Dark mode adjustments**: In dark mode, the light shadow becomes a slightly lighter shade of the dark background (not white), and the dark shadow becomes slightly darker. The contrast range between shadows shrinks significantly.
- **Performance**: `box-shadow` with multiple values is well-optimized in modern browsers, but avoid animating shadow blur values directly; transition `box-shadow` as a whole property instead.

---

## Related Aesthetics

| Aesthetic | Relationship to Neumorphism |
|-----------|----------------------------|
| **Flat Design** | Direct predecessor; neumorphism reintroduces depth that flat design deliberately eliminated, but retains the minimal, clean sensibility |
| **Skeuomorphism** | Historical ancestor; neumorphism inherits the physical-object metaphor but strips away realistic textures, reflections, and glossy surfaces in favor of pure shadow |
| **Claymorphism** | Successor; elements float above the background (vs. extruding from it) and use vivid colors instead of monochrome; shares the soft, rounded, tactile quality |
| **Glassmorphism** | Contemporary sibling; uses transparency and blur for depth rather than shadow and extrusion; colorful and layered vs. monochromatic and continuous |
| **Material Design** | Google's elevation system shares the concept of shadow-based depth, but uses distinct surface colors and sharper shadow hierarchies; more structured and less organic |
| **Minimalism** | Parent philosophy; neumorphism applies minimalist reduction to interface decoration while adding controlled physical depth |
| **Cyberminimalism** | Shares the clean, reduced approach but relies on stark contrast and flat surfaces rather than soft shadows |
