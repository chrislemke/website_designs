# Bento Grid Reference

Bento Grid is a modular UI layout aesthetic inspired by the compartmentalized structure of Japanese bento lunch boxes. It arranges content into asymmetric, rounded-rectangle tiles of varying sizes that interlock like a carefully packed meal. The style emphasizes visual balance through intentional imbalance, using generous padding, soft corners, and subtle depth to create interfaces that feel organized yet dynamic -- every compartment purposeful, every gap deliberate.

---

## Visual Characteristics

### Core Design Traits

- **Asymmetric grid compartments** -- tiles of different widths and heights arranged in a non-uniform grid that still feels balanced and intentional
- **Generous rounded corners** -- radii of 16-24px on every tile, creating a soft, approachable feel reminiscent of physical bento containers
- **Consistent inter-tile gaps** -- uniform spacing (12-20px) between all compartments, like the dividers in a bento box
- **Contained content blocks** -- each tile is a self-contained unit with its own background, padding, and visual identity
- **Soft, muted color palette** -- warm neutrals with selective accent colors; nothing garish or competing for attention
- **Subtle depth cues** -- very light shadows or slight background tint differences to separate tiles from the canvas
- **Dense yet breathable** -- maximum information density without visual clutter; padding within tiles is generous
- **Mixed content types** -- tiles freely combine icons, charts, text blocks, images, and interactive elements
- **Responsive reflow** -- tiles rearrange and resize gracefully across breakpoints while maintaining the bento feel
- **Clean internal hierarchy** -- within each tile, content follows a simple top-down flow with clear type hierarchy

### Design Principles

- Treat each tile as an independent module that communicates one idea or data point
- Use tile size to signal importance: larger tiles draw more attention
- Maintain uniform gap spacing across the entire grid for visual cohesion
- Let rounded corners and padding do the work of visual separation -- minimize borders
- Keep the overall canvas neutral so individual tile content stands out
- Design tiles to be rearrangeable without breaking the layout logic
- Balance visual weight across the grid: distribute colors, images, and dense content evenly
- Favor clarity over decoration -- the structure itself is the aesthetic

---

## Color Palette

### Bento Grid Core Palette

The palette draws from Japanese design sensibility: muted, sophisticated, with restrained warmth and selective bold accents.

| Color Name | Hex | Role / Usage |
|------------|-----|-------------|
| **Snow** | `#F8F7F4` | Page canvas background |
| **Rice** | `#FFFFFF` | Primary tile background |
| **Sesame** | `#F0EEEB` | Secondary tile background, alternating tiles |
| **Nori** | `#1A1A2E` | Primary text, headings |
| **Soy** | `#3D3D56` | Secondary text, descriptions |
| **Ginger** | `#6B6B80` | Tertiary text, captions, labels |
| **Wasabi** | `#4CAF82` | Success states, positive metrics, primary accent |
| **Umami** | `#FF6B35` | Call-to-action, attention-grabbing accent |
| **Sakura** | `#F472B6` | Highlight accent, badges, decorative elements |
| **Matcha** | `#86EFAC` | Light accent backgrounds, tags |
| **Tamago** | `#FCD34D` | Warning, star ratings, warm highlights |
| **Miso** | `#D4A574` | Warm neutral accent, earthy tone |
| **Ume** | `#A78BFA` | Purple accent, secondary interactive elements |
| **Tsuyu** | `#38BDF8` | Info states, links, cool accent |
| **Kombu** | `#374151` | Dark tile backgrounds, footer |
| **Tofu** | `#E8E6E3` | Borders, dividers, disabled states |

### CSS Custom Properties

```css
:root {
  /* Canvas */
  --bento-canvas: #f8f7f4;
  --bento-tile-primary: #ffffff;
  --bento-tile-secondary: #f0eeeb;

  /* Text */
  --bento-text-primary: #1a1a2e;
  --bento-text-secondary: #3d3d56;
  --bento-text-tertiary: #6b6b80;

  /* Accents */
  --bento-accent-green: #4caf82;
  --bento-accent-orange: #ff6b35;
  --bento-accent-pink: #f472b6;
  --bento-accent-yellow: #fcd34d;
  --bento-accent-purple: #a78bfa;
  --bento-accent-blue: #38bdf8;

  /* Neutrals */
  --bento-warm-neutral: #d4a574;
  --bento-border: #e8e6e3;
  --bento-dark: #374151;

  /* Layout tokens */
  --bento-gap: 16px;
  --bento-radius: 20px;
  --bento-tile-padding: 28px;
}
```

---

## Typography

### Typeface Characteristics

Bento Grid typography is:

- **Clean and modern sans-serif** -- matching the refined, modular aesthetic
- **Compact and efficient** -- text must work within confined tile spaces
- **Strong weight contrast** -- bold headings against light body text for in-tile hierarchy
- **Slightly rounded or humanist** -- complementing the soft rounded corners of tiles
- **Excellent at small sizes** -- labels, captions, and metrics must remain legible in compact tiles

### Recommended Web Fonts (Google Fonts)

| Font | Style | Best For |
|------|-------|----------|
| **Inter** | Screen-optimized, tall x-height | Body text, labels, metrics -- the ideal bento workhorse |
| **Plus Jakarta Sans** | Geometric, slightly rounded | Headlines, tile titles, modern feel |
| **DM Sans** | Clean geometric with personality | Headlines and body, balanced warmth |
| **Outfit** | Geometric, variable weight | Display numbers, metrics, tile headings |
| **Nunito** | Rounded terminals | Friendly interfaces, approachable tiles |
| **Satoshi** | Contemporary geometric | Headlines, navigation, modern bento layouts |
| **Manrope** | Semi-condensed, efficient | Body text in tight tile spaces |
| **Space Grotesk** | Monospace-inspired proportional | Code tiles, technical metrics, dashboards |

### Font Pairing Suggestions

| Heading Font | Body Font | Character |
|-------------|-----------|-----------|
| **Plus Jakarta Sans** (700) | **Inter** (400) | Modern, clean, professional bento |
| **DM Sans** (700) | **DM Sans** (400) | Unified, warm, approachable |
| **Outfit** (600) | **Inter** (400) | Contemporary, data-forward |
| **Nunito** (700) | **Manrope** (400) | Soft, friendly, compact |
| **Space Grotesk** (600) | **Inter** (400) | Technical, dashboard-oriented |

### Typography CSS Example

```css
@import url('https://fonts.googleapis.com/css2?family=Plus+Jakarta+Sans:wght@500;600;700;800&family=Inter:wght@400;500;600&display=swap');

h1, h2, h3, h4, h5, h6 {
  font-family: 'Plus Jakarta Sans', sans-serif;
  font-weight: 700;
  color: var(--bento-text-primary);
  line-height: 1.2;
  letter-spacing: -0.02em;
}

.bento-display {
  font-family: 'Plus Jakarta Sans', sans-serif;
  font-size: clamp(2rem, 4vw, 3.5rem);
  font-weight: 800;
  letter-spacing: -0.03em;
  line-height: 1.1;
}

body {
  font-family: 'Inter', sans-serif;
  font-weight: 400;
  font-size: 0.95rem;
  line-height: 1.6;
  color: var(--bento-text-secondary);
}

.bento-metric {
  font-family: 'Plus Jakarta Sans', sans-serif;
  font-weight: 800;
  font-size: 2.5rem;
  letter-spacing: -0.03em;
  line-height: 1;
}

.bento-label {
  font-family: 'Inter', sans-serif;
  font-weight: 500;
  font-size: 0.8rem;
  letter-spacing: 0.03em;
  text-transform: uppercase;
  color: var(--bento-text-tertiary);
}

.bento-caption {
  font-family: 'Inter', sans-serif;
  font-weight: 400;
  font-size: 0.85rem;
  color: var(--bento-text-tertiary);
}
```

---

## Layout Principles

### Grid and Structure

- **CSS Grid with explicit placement** -- tiles are placed with `grid-column` and `grid-row` spanning for the asymmetric bento pattern
- **Base grid of 4-6 columns** -- tiles span 1-3 columns and 1-2 rows to create visual variety
- **Uniform gap throughout** -- 16px gap is the standard; it acts as the bento box divider
- **Generous tile padding** -- 24-32px internal padding keeps content from feeling cramped
- **No tile-to-edge bleeding** -- every tile is inset from the page edges with consistent outer padding
- **Canvas background visible through gaps** -- the gap color (canvas) unifies the composition

### Section Organization

- **Navigation**: Minimal top bar outside the bento grid, or integrated as a narrow spanning tile
- **Hero**: Large tile spanning 2-3 columns, containing headline and CTA; paired with smaller accent tiles
- **Metrics row**: Equal-sized tiles each showcasing one key number with label
- **Feature tiles**: Mixed-size tiles with icon, title, and short description
- **Showcase tile**: Extra-large tile spanning full width or 3 columns for imagery or key content
- **CTA tile**: Accent-colored tile with centered text and button
- **Footer**: Full-width tile or row of small tiles with links and info

### Responsive Approach

- Desktop: 4-column grid with mixed spanning (the full bento experience)
- Tablet: 2-column grid; large tiles span full width, others stack in pairs
- Mobile: Single-column; all tiles become full-width cards stacked vertically
- Maintain rounded corners and padding at all breakpoints
- Gap can reduce slightly on mobile (12px) but never disappear

---

## CSS / Design Techniques

### Bento Grid Container

```css
.bento-grid {
  display: grid;
  grid-template-columns: repeat(4, 1fr);
  gap: var(--bento-gap);
  max-width: 1200px;
  margin: 0 auto;
  padding: var(--bento-gap);
}

/* Tile spanning utilities */
.bento-tile--wide { grid-column: span 2; }
.bento-tile--tall { grid-row: span 2; }
.bento-tile--large { grid-column: span 2; grid-row: span 2; }
.bento-tile--full { grid-column: 1 / -1; }

@media (max-width: 1024px) {
  .bento-grid { grid-template-columns: repeat(2, 1fr); }
  .bento-tile--large { grid-column: span 2; grid-row: span 1; }
}

@media (max-width: 640px) {
  .bento-grid { grid-template-columns: 1fr; gap: 12px; padding: 12px; }
  .bento-tile--wide,
  .bento-tile--tall,
  .bento-tile--large,
  .bento-tile--full { grid-column: span 1; grid-row: span 1; }
}
```

### Bento Tile Base

```css
.bento-tile {
  background: var(--bento-tile-primary);
  border-radius: var(--bento-radius);
  padding: var(--bento-tile-padding);
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  overflow: hidden;
  transition: transform 0.2s ease, box-shadow 0.2s ease;
}

.bento-tile:hover {
  transform: translateY(-2px);
  box-shadow: 0 8px 30px rgba(0, 0, 0, 0.06);
}

.bento-tile--muted {
  background: var(--bento-tile-secondary);
}

.bento-tile--dark {
  background: var(--bento-dark);
  color: #ffffff;
}

.bento-tile--accent-green {
  background: var(--bento-accent-green);
  color: #ffffff;
}

.bento-tile--accent-orange {
  background: var(--bento-accent-orange);
  color: #ffffff;
}
```

### Bento Button

```css
.bento-button {
  display: inline-flex;
  align-items: center;
  justify-content: center;
  gap: 8px;
  background: var(--bento-text-primary);
  color: #ffffff;
  border: none;
  border-radius: 12px;
  padding: 12px 28px;
  font-family: 'Inter', sans-serif;
  font-weight: 600;
  font-size: 0.9rem;
  cursor: pointer;
  transition: background 0.2s ease, transform 0.15s ease;
  text-decoration: none;
}

.bento-button:hover {
  background: var(--bento-text-secondary);
  transform: translateY(-1px);
}

.bento-button--accent {
  background: var(--bento-accent-orange);
}

.bento-button--accent:hover {
  background: #e55a25;
}

.bento-button--ghost {
  background: transparent;
  color: var(--bento-text-primary);
  border: 2px solid var(--bento-border);
}

.bento-button--ghost:hover {
  background: var(--bento-tile-secondary);
}
```

### Navigation Bar

```css
.bento-nav {
  display: flex;
  align-items: center;
  justify-content: space-between;
  max-width: 1200px;
  margin: 0 auto;
  padding: 20px 24px;
}

.bento-nav__logo {
  font-family: 'Plus Jakarta Sans', sans-serif;
  font-weight: 800;
  font-size: 1.3rem;
  color: var(--bento-text-primary);
  text-decoration: none;
}

.bento-nav__links {
  display: flex;
  gap: 28px;
  list-style: none;
  margin: 0;
  padding: 0;
}

.bento-nav__links a {
  font-family: 'Inter', sans-serif;
  font-weight: 500;
  font-size: 0.9rem;
  color: var(--bento-text-tertiary);
  text-decoration: none;
  transition: color 0.2s ease;
}

.bento-nav__links a:hover {
  color: var(--bento-text-primary);
}
```

### Metric Tile

```css
.bento-metric-tile {
  display: flex;
  flex-direction: column;
  gap: 8px;
}

.bento-metric-tile__value {
  font-family: 'Plus Jakarta Sans', sans-serif;
  font-weight: 800;
  font-size: 2.5rem;
  letter-spacing: -0.03em;
  line-height: 1;
  color: var(--bento-text-primary);
}

.bento-metric-tile__label {
  font-family: 'Inter', sans-serif;
  font-weight: 500;
  font-size: 0.85rem;
  color: var(--bento-text-tertiary);
}

.bento-metric-tile__trend {
  font-family: 'Inter', sans-serif;
  font-weight: 600;
  font-size: 0.8rem;
  color: var(--bento-accent-green);
}
```

### Feature Tile

```css
.bento-feature-tile__icon {
  width: 48px;
  height: 48px;
  border-radius: 14px;
  display: flex;
  align-items: center;
  justify-content: center;
  font-size: 1.5rem;
  margin-bottom: 16px;
  background: var(--bento-tile-secondary);
}

.bento-feature-tile h3 {
  font-size: 1.1rem;
  margin-bottom: 8px;
}

.bento-feature-tile p {
  font-size: 0.9rem;
  color: var(--bento-text-tertiary);
  line-height: 1.5;
}
```

---

## Design Do's and Don'ts

### Do

- Maintain uniform gap spacing across the entire grid
- Use generous rounded corners (16-24px) on every tile
- Vary tile sizes intentionally to create visual hierarchy
- Keep internal tile padding consistent (24-32px)
- Use the canvas background color to unify the composition
- Design each tile as a self-contained, modular unit
- Balance visual weight across the grid by distributing color and imagery evenly
- Use subtle hover effects (slight lift, soft shadow) for interactive tiles

### Don't

- Make all tiles the same size -- that defeats the bento purpose
- Use sharp corners or zero-radius tiles
- Remove the gaps between tiles -- the spacing is essential to the aesthetic
- Pack too much content into small tiles -- let them breathe
- Use heavy borders or outlines to define tiles
- Mix wildly different border-radius values across tiles
- Ignore responsive behavior -- the grid must reflow gracefully
- Add excessive shadows or depth that overwhelms the soft, modular feel

---

## Related Aesthetics

| Aesthetic | Relationship to Bento Grid |
|-----------|---------------------------|
| **Flat Design** | Shares minimalist philosophy; Bento Grid adds structural complexity through asymmetric tile arrangements |
| **Glassmorphism** | Can be layered into bento tiles with frosted-glass backgrounds for a premium, translucent variant |
| **Neumorphism** | Soft depth approach that can complement bento tiles when applied subtly to tile surfaces |
| **Neubrutalism** | Contrasting aesthetic; shares card-based layouts but uses harsh borders and raw edges instead of soft rounding |
| **Corporate Memphis** | Often used for illustrations within bento tiles; the modular layout pairs well with flat character art |
| **Japandi** | Shares Japanese design DNA; the same restraint, natural warmth, and intentional minimalism |
| **Material Design** | Google's card-based system is a predecessor; bento grids push further into asymmetric, non-uniform sizing |
| **Claymorphism** | Puffy 3D tiles can fill the bento structure for a more playful, tactile variant |
| **Cyberminimalism** | Shares clean digital minimalism; bento grids add warmth and modularity to the stark cyber approach |
| **Mid-Century Modern** | Geometric precision and balanced asymmetry echo the same design philosophy in physical space |

---

## Quick-Start: Minimal Bento Grid Page Template

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Bento Grid Page</title>
  <link href="https://fonts.googleapis.com/css2?family=Plus+Jakarta+Sans:wght@500;600;700;800&family=Inter:wght@400;500;600&display=swap" rel="stylesheet">
  <style>
    :root {
      --bento-canvas: #f8f7f4;
      --bento-tile-primary: #ffffff;
      --bento-tile-secondary: #f0eeeb;
      --bento-text-primary: #1a1a2e;
      --bento-text-secondary: #3d3d56;
      --bento-text-tertiary: #6b6b80;
      --bento-accent-green: #4caf82;
      --bento-accent-orange: #ff6b35;
      --bento-accent-pink: #f472b6;
      --bento-accent-yellow: #fcd34d;
      --bento-accent-purple: #a78bfa;
      --bento-accent-blue: #38bdf8;
      --bento-border: #e8e6e3;
      --bento-dark: #374151;
      --bento-gap: 16px;
      --bento-radius: 20px;
      --bento-tile-padding: 28px;
    }

    * { margin: 0; padding: 0; box-sizing: border-box; }

    body {
      background: var(--bento-canvas);
      color: var(--bento-text-secondary);
      font-family: 'Inter', sans-serif;
      font-weight: 400;
      line-height: 1.6;
    }

    h1, h2, h3 {
      font-family: 'Plus Jakarta Sans', sans-serif;
      font-weight: 700;
      color: var(--bento-text-primary);
      line-height: 1.2;
      letter-spacing: -0.02em;
    }

    /* Navigation */
    nav {
      display: flex;
      align-items: center;
      justify-content: space-between;
      max-width: 1200px;
      margin: 0 auto;
      padding: 20px 24px;
    }

    nav a.logo {
      font-family: 'Plus Jakarta Sans', sans-serif;
      font-weight: 800;
      font-size: 1.3rem;
      color: var(--bento-text-primary);
      text-decoration: none;
    }

    nav ul {
      display: flex;
      gap: 28px;
      list-style: none;
    }

    nav ul a {
      color: var(--bento-text-tertiary);
      text-decoration: none;
      font-weight: 500;
      font-size: 0.9rem;
      transition: color 0.2s;
    }

    nav ul a:hover { color: var(--bento-text-primary); }

    /* Bento Grid */
    .bento {
      display: grid;
      grid-template-columns: repeat(4, 1fr);
      gap: var(--bento-gap);
      max-width: 1200px;
      margin: 0 auto;
      padding: 0 var(--bento-gap) var(--bento-gap);
    }

    .tile {
      background: var(--bento-tile-primary);
      border-radius: var(--bento-radius);
      padding: var(--bento-tile-padding);
      display: flex;
      flex-direction: column;
      justify-content: space-between;
      overflow: hidden;
      transition: transform 0.2s ease, box-shadow 0.2s ease;
    }

    .tile:hover {
      transform: translateY(-2px);
      box-shadow: 0 8px 30px rgba(0, 0, 0, 0.06);
    }

    /* Spanning */
    .tile--hero { grid-column: span 2; grid-row: span 2; }
    .tile--wide { grid-column: span 2; }
    .tile--tall { grid-row: span 2; }
    .tile--full { grid-column: 1 / -1; }

    /* Color variants */
    .tile--muted { background: var(--bento-tile-secondary); }
    .tile--dark { background: var(--bento-dark); color: #fff; }
    .tile--dark h3 { color: #fff; }
    .tile--accent { background: var(--bento-accent-orange); color: #fff; }
    .tile--accent h3 { color: #fff; }

    /* Hero tile */
    .tile--hero h1 {
      font-size: clamp(2rem, 4vw, 3rem);
      font-weight: 800;
      margin-bottom: 1rem;
      letter-spacing: -0.03em;
    }

    .tile--hero p {
      font-size: 1.05rem;
      color: var(--bento-text-tertiary);
      margin-bottom: 1.5rem;
      max-width: 400px;
    }

    /* Metric */
    .metric { font-family: 'Plus Jakarta Sans', sans-serif; font-weight: 800; font-size: 2.5rem; letter-spacing: -0.03em; line-height: 1; }
    .metric-label { font-size: 0.85rem; color: var(--bento-text-tertiary); margin-top: 8px; }
    .metric-trend { font-weight: 600; font-size: 0.8rem; color: var(--bento-accent-green); margin-top: 4px; }

    /* Icon container */
    .tile-icon {
      width: 48px;
      height: 48px;
      border-radius: 14px;
      display: flex;
      align-items: center;
      justify-content: center;
      font-size: 1.4rem;
      margin-bottom: 16px;
    }

    .tile h3 { font-size: 1.1rem; margin-bottom: 8px; }
    .tile p { font-size: 0.9rem; color: var(--bento-text-tertiary); line-height: 1.5; }

    /* Button */
    .btn {
      display: inline-flex;
      align-items: center;
      gap: 8px;
      background: var(--bento-text-primary);
      color: #fff;
      border: none;
      border-radius: 12px;
      padding: 12px 28px;
      font-family: 'Inter', sans-serif;
      font-weight: 600;
      font-size: 0.9rem;
      cursor: pointer;
      text-decoration: none;
      transition: background 0.2s;
    }

    .btn:hover { background: var(--bento-text-secondary); }

    /* Footer tile */
    .tile--footer {
      background: var(--bento-dark);
      color: var(--bento-text-tertiary);
      text-align: center;
      font-size: 0.85rem;
    }

    @media (max-width: 1024px) {
      .bento { grid-template-columns: repeat(2, 1fr); }
      .tile--hero { grid-column: span 2; grid-row: span 1; }
    }

    @media (max-width: 640px) {
      .bento { grid-template-columns: 1fr; gap: 12px; padding: 0 12px 12px; }
      .tile--hero, .tile--wide, .tile--tall, .tile--full { grid-column: span 1; grid-row: span 1; }
      nav { padding: 16px; }
      nav ul { gap: 16px; }
    }
  </style>
</head>
<body>
  <nav>
    <a href="#" class="logo">BentoApp</a>
    <ul>
      <li><a href="#">Dashboard</a></li>
      <li><a href="#">Features</a></li>
      <li><a href="#">Pricing</a></li>
      <li><a href="#">About</a></li>
    </ul>
  </nav>

  <div class="bento">
    <!-- Hero tile -->
    <div class="tile tile--hero">
      <div>
        <h1>Everything you need, neatly organized</h1>
        <p>A modular workspace that adapts to how you think. Every piece in its place.</p>
        <a href="#" class="btn">Get Started</a>
      </div>
      <svg width="100%" height="80" viewBox="0 0 500 80" fill="none" style="margin-top:auto;">
        <rect x="0" y="0" width="120" height="80" rx="12" fill="#f0eeeb"/>
        <rect x="136" y="0" width="80" height="80" rx="12" fill="#fcd34d" opacity="0.3"/>
        <rect x="232" y="0" width="160" height="36" rx="12" fill="#f0eeeb"/>
        <rect x="232" y="44" width="76" height="36" rx="12" fill="#4caf82" opacity="0.2"/>
        <rect x="316" y="44" width="76" height="36" rx="12" fill="#f0eeeb"/>
        <rect x="408" y="0" width="80" height="80" rx="12" fill="#a78bfa" opacity="0.2"/>
      </svg>
    </div>

    <!-- Metric tiles -->
    <div class="tile">
      <div class="tile-icon" style="background:#e8f5e9;">
        <svg width="24" height="24" viewBox="0 0 24 24"><path d="M16 6l2.29 2.29-4.88 4.88-4-4L2 16.59 3.41 18l6-6 4 4 6.3-6.29L22 12V6z" fill="#4caf82"/></svg>
      </div>
      <div>
        <div class="metric">98.7%</div>
        <div class="metric-label">Uptime this month</div>
        <div class="metric-trend">+0.3% vs last month</div>
      </div>
    </div>

    <div class="tile tile--muted">
      <div class="tile-icon" style="background:#fff3e0;">
        <svg width="24" height="24" viewBox="0 0 24 24"><path d="M12 2C6.48 2 2 6.48 2 12s4.48 10 10 10 10-4.48 10-10S17.52 2 12 2zm-2 15l-5-5 1.41-1.41L10 14.17l7.59-7.59L19 8l-9 9z" fill="#ff6b35"/></svg>
      </div>
      <div>
        <div class="metric">2,847</div>
        <div class="metric-label">Tasks completed</div>
        <div class="metric-trend">+12% this week</div>
      </div>
    </div>

    <!-- Feature tiles -->
    <div class="tile tile--wide">
      <div class="tile-icon" style="background:#ede9fe;">
        <svg width="24" height="24" viewBox="0 0 24 24"><rect x="3" y="3" width="7" height="7" rx="2" fill="#a78bfa"/><rect x="14" y="3" width="7" height="7" rx="2" fill="#a78bfa"/><rect x="3" y="14" width="7" height="7" rx="2" fill="#a78bfa"/><rect x="14" y="14" width="7" height="7" rx="2" fill="#a78bfa"/></svg>
      </div>
      <div>
        <h3>Modular Workflows</h3>
        <p>Build custom workflows by combining modular components. Drag, drop, and connect pieces to match how your team actually works.</p>
      </div>
    </div>

    <div class="tile tile--dark">
      <div class="tile-icon" style="background:rgba(255,255,255,0.1);">
        <svg width="24" height="24" viewBox="0 0 24 24"><path d="M12 1L3 5v6c0 5.55 3.84 10.74 9 12 5.16-1.26 9-6.45 9-12V5l-9-4z" fill="#38bdf8"/></svg>
      </div>
      <div>
        <h3>Enterprise Security</h3>
        <p>Bank-grade encryption with SOC 2 compliance built in from day one.</p>
      </div>
    </div>

    <div class="tile">
      <div class="tile-icon" style="background:#fce7f3;">
        <svg width="24" height="24" viewBox="0 0 24 24"><path d="M19 3H5c-1.1 0-2 .9-2 2v14c0 1.1.9 2 2 2h14c1.1 0 2-.9 2-2V5c0-1.1-.9-2-2-2zm-5 14H7v-2h7v2zm3-4H7v-2h10v2zm0-4H7V7h10v2z" fill="#f472b6"/></svg>
      </div>
      <div>
        <h3>Smart Reports</h3>
        <p>Auto-generated insights that surface what matters most.</p>
      </div>
    </div>

    <!-- CTA tile -->
    <div class="tile tile--accent tile--wide" style="text-align:center; align-items:center;">
      <h3 style="font-size:1.5rem; margin-bottom:12px;">Ready to organize your workflow?</h3>
      <p style="color:rgba(255,255,255,0.9); margin-bottom:20px;">Join 10,000+ teams using BentoApp to stay organized.</p>
      <a href="#" class="btn" style="background:#fff; color:var(--bento-accent-orange);">Start Free Trial</a>
    </div>

    <!-- Footer tile -->
    <div class="tile tile--footer tile--full">
      <p>Built with the Bento Grid aesthetic. Modular, organized, beautiful.</p>
    </div>
  </div>
</body>
</html>
```
