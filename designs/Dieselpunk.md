# Dieselpunk Design Reference

Dieselpunk is a retrofuturistic aesthetic rooted in the interwar period (1920s-1950s), where diesel-powered machinery, Art Deco grandeur, and wartime industrial might converge into an alternative history of raw mechanical power and streamlined glamour. The genre sits chronologically between Steampunk (Victorian, steam-powered) and Cyberpunk (neon, digital), drawing from the era of zeppelins, propeller aircraft, riveted steel tanks, propaganda poster art, Streamline Moderne architecture, and the muscular optimism of heavy industry. Visually it blends the geometric elegance of Art Deco with the grit of diesel exhaust, oil-stained machinery, and military utilitarian design. In web and UI design, Dieselpunk translates to dark steel and olive-drab color palettes punctuated by brass and amber metallics, heavy geometric sans-serif typography inspired by 1930s poster lettering, riveted panel borders, gear-and-piston motifs, and an overall atmosphere that feels like a command bridge on an armored dreadnought cruising through an alternate 1942.

---

## Visual Characteristics

### Core Design Traits

- **Riveted steel and iron surfaces** -- UI panels and cards appear to be stamped from heavy-gauge sheet metal, fastened with visible rivets at corners and seams
- **Art Deco geometric ornamentation** -- chevrons, sunbursts, stepped forms, and radiating fan patterns used as borders, dividers, and decorative accents
- **Diesel-era machinery motifs** -- exposed gears, pistons, pressure gauges, propellers, and exhaust pipes referenced as visual metaphors and decorative elements
- **Military utilitarian styling** -- stenciled labels, olive-drab and khaki surfaces, dog-tag shapes, ammunition-crate textures, and command-panel layouts
- **Propaganda poster influence** -- bold, directive typography, high-contrast color blocking, heroic compositions, and direct calls-to-action styled as wartime recruitment posters
- **Warm industrial metallics** -- brass fittings, brushed steel highlights, oxidized copper accents, and oil-slicked dark surfaces
- **Streamline Moderne curves** -- aerodynamic rounded edges on certain elements, referencing the fluid design language of 1930s locomotives and automobiles
- **Dark, smoky atmospherics** -- vignette shadows, subtle noise textures, and muted warm lighting suggesting factory floors and dimly-lit war rooms
- **Analog instrument interfaces** -- toggle switches, rotary dials, analog meters, and backlit indicator panels as UI metaphors
- **Sepia and desaturated tones** -- an overall color treatment that suggests aged photographs, period newsreels, and oil-on-canvas propaganda art

### Design Principles

- Every surface should suggest a physical industrial material: steel, brass, leather, riveted iron, or oiled wood
- Balance Art Deco elegance with industrial grit -- the aesthetic is glamorous machinery, not polished luxury
- Typography should feel stamped, stenciled, or cast in metal -- never delicate or handwritten
- Color palettes lean dark and warm, dominated by charcoal, rust, olive, and amber -- bright colors are reserved for warning indicators and propaganda-style accents
- Layouts should feel structured and authoritative, like a military command dashboard or an engineer's control panel
- Ornamentation serves the machine aesthetic: gears, chevrons, and radiating lines -- never floral or organic
- Light sources are artificial and warm: incandescent bulbs, instrument panel backlighting, and furnace glow
- The mood oscillates between muscular optimism (the power of industry) and noir tension (the shadow of conflict)

---

## Color Palette

### Industrial Command Palette

| Color Name | Hex | Role / Usage |
|------------|-----|-------------|
| **Furnace Black** | `#1A1A1A` | Primary dark background, deepest layer |
| **Gunmetal** | `#2C2F33` | Card backgrounds, elevated panels, nav surfaces |
| **Battleship Gray** | `#6B7280` | Secondary text, muted labels, disabled states |
| **Riveted Steel** | `#8A8D93` | Borders, dividers, structural accents |
| **Polished Brass** | `#C9A84C` | Primary accent, headings, key interactive elements |
| **Dark Brass** | `#9A7B2F` | Hover states, active borders, metallic depth |
| **Amber Warning** | `#D4890E` | Warnings, highlight accents, call-to-action glow |
| **Rust Red** | `#8B3A1A` | Danger states, critical alerts, propaganda accents |
| **Propaganda Red** | `#B8221E` | Bold accent for banners, badges, and heroic CTAs |
| **Olive Drab** | `#4B5320` | Military accent, secondary backgrounds, subtle tones |
| **Army Khaki** | `#8F7E4F` | Tertiary accent, canvas textures, warm mid-tones |
| **Diesel Smoke** | `#3B3B3B` | Subtle dark variation, card borders, shadows |
| **Parchment Cream** | `#F0E6D0` | Light text on dark backgrounds, aged paper surfaces |
| **Cockpit White** | `#E8E4DA` | Primary text on dark backgrounds, instrument labels |
| **Oil Slick** | `#1E1E24` | Darkest accent, footer backgrounds, deep overlays |

### CSS Custom Properties

```css
:root {
  /* Backgrounds */
  --diesel-bg-dark: #1a1a1a;
  --diesel-bg-panel: #2c2f33;
  --diesel-bg-smoke: #3b3b3b;
  --diesel-bg-oil: #1e1e24;

  /* Metallics */
  --diesel-brass: #c9a84c;
  --diesel-brass-dark: #9a7b2f;
  --diesel-steel: #8a8d93;
  --diesel-gunmetal: #6b7280;

  /* Accents */
  --diesel-amber: #d4890e;
  --diesel-rust: #8b3a1a;
  --diesel-red: #b8221e;
  --diesel-olive: #4b5320;
  --diesel-khaki: #8f7e4f;

  /* Text */
  --diesel-text-light: #e8e4da;
  --diesel-text-parchment: #f0e6d0;
  --diesel-text-muted: #6b7280;
  --diesel-text-dark: #1a1a1a;

  /* Surfaces (gradients simulating materials) */
  --diesel-brass-surface: linear-gradient(145deg, #d4a843 0%, #c9a84c 40%, #9a7b2f 80%);
  --diesel-steel-surface: linear-gradient(145deg, #8a8d93 0%, #6b7280 50%, #8a8d93 100%);
  --diesel-panel: linear-gradient(180deg, #2c2f33 0%, #1e1e24 100%);

  /* Borders */
  --diesel-border-steel: #6b7280;
  --diesel-border-brass: #9a7b2f;

  /* Shadows */
  --diesel-shadow: 0 4px 12px rgba(0, 0, 0, 0.4);
  --diesel-shadow-inset: inset 0 2px 4px rgba(0, 0, 0, 0.3);
}
```

---

## Typography

### Typeface Characteristics

Dieselpunk typography is:

- **Heavy, geometric sans-serifs** -- typefaces that feel stamped from metal or stenciled onto crates, referencing 1930s-40s industrial signage
- **Art Deco display faces** -- angular, decorative letterforms with strong vertical emphasis and geometric construction
- **Stencil and military typefaces** -- utilitarian, no-nonsense lettering suggesting military markings and factory labels
- **Uppercase-dominant for headings** -- all-caps settings with wide letter-spacing evoke propaganda posters and brass nameplates
- **Condensed weights for data** -- tall, narrow letterforms used for instrument readouts and dashboard labels
- **Medium to heavy weights** -- bold presence that suggests stamped or embossed metal, never thin or wispy

### Recommended Google Fonts

| Font | Style | Best For |
|------|-------|----------|
| **Bebas Neue** | Condensed geometric sans | Headlines, propaganda-style display, posters |
| **Oswald** | Condensed neo-grotesque | Headings, navigation, strong labels |
| **Archivo Black** | Heavy geometric sans | Hero text, bold display, impactful titles |
| **Fjalla One** | Condensed, strong | Subheadings, section titles, UI labels |
| **Marcellus** | Classic Roman inscriptional | Art Deco-flavored headings, elegant accents |
| **Stencil** (system) | Military stencil | Labels, badges, military-style markings |
| **Source Sans 3** | Utilitarian sans-serif | Body text, readable long-form content |
| **IBM Plex Sans** | Industrial, clean | Body text, data labels, UI elements |
| **Special Elite** | Typewriter | Dispatches, field reports, atmospheric text |
| **Roboto Condensed** | Condensed, modern | Dashboard labels, navigation, secondary text |

### Font Pairing Suggestions

| Heading Font | Body Font | Character |
|-------------|-----------|-----------|
| **Bebas Neue** (400) | **Source Sans 3** (400) | Classic propaganda poster meets readable utility |
| **Archivo Black** (400) | **IBM Plex Sans** (400) | Heavy industrial impact with clean body text |
| **Oswald** (700) | **Source Sans 3** (400) | Condensed authority with comfortable reading |
| **Fjalla One** (400) | **Roboto Condensed** (400) | Military briefing, data-dense layouts |
| **Marcellus** (400) | **IBM Plex Sans** (400) | Art Deco elegance grounded by industrial clarity |

### Typography CSS Example

```css
/* Import fonts */
@import url('https://fonts.googleapis.com/css2?family=Bebas+Neue&family=Oswald:wght@500;700&family=Source+Sans+3:ital,wght@0,400;0,600;1,400&display=swap');

/* Headings */
h1, h2, h3, h4, h5, h6 {
  font-family: 'Bebas Neue', 'Oswald', 'Arial Narrow', sans-serif;
  font-weight: 400;
  color: var(--diesel-text-parchment);
  text-transform: uppercase;
  letter-spacing: 0.06em;
  line-height: 1.1;
}

/* Display / Hero text */
.diesel-display {
  font-family: 'Bebas Neue', sans-serif;
  font-size: clamp(3rem, 7vw, 6rem);
  letter-spacing: 0.08em;
  text-transform: uppercase;
  color: var(--diesel-brass);
  text-shadow: 2px 2px 0 rgba(0, 0, 0, 0.4), 0 0 20px rgba(201, 168, 76, 0.15);
}

/* Body text */
body {
  font-family: 'Source Sans 3', 'IBM Plex Sans', sans-serif;
  font-weight: 400;
  font-size: 1rem;
  line-height: 1.7;
  color: var(--diesel-text-light);
}

/* Military label */
.diesel-label {
  font-family: 'Oswald', sans-serif;
  font-weight: 500;
  font-size: 0.7rem;
  letter-spacing: 0.14em;
  text-transform: uppercase;
  color: var(--diesel-text-muted);
}

/* Stencil text */
.diesel-stencil {
  font-family: 'Stencil', 'Oswald', sans-serif;
  font-weight: 700;
  letter-spacing: 0.1em;
  text-transform: uppercase;
  color: var(--diesel-olive);
}

/* Typewriter / dispatch text */
.diesel-dispatch {
  font-family: 'Special Elite', 'Courier New', monospace;
  font-size: 0.95rem;
  color: var(--diesel-text-parchment);
  line-height: 1.6;
}
```

---

## Layout Principles

### Grid and Structure

- **Dark, industrial full-bleed backgrounds** -- the viewport is a dark steel canvas; light colors appear only as instrument panel readouts and text labels
- **Rigid, panel-based layouts** -- content organized in bolted-down steel panels with visible borders, rivets, and structural framing
- **Symmetrical and authoritative compositions** -- centered headings, evenly-spaced grid columns, and bilateral balance referencing military command interfaces
- **Horizontal banding** -- alternating sections of dark steel, brass-accented dividers, and olive or khaki mid-sections
- **Art Deco decorative borders** -- chevron patterns, stepped forms, and sunburst motifs used as section dividers and frame accents
- **Dense but organized information** -- dashboard-style layouts with multiple panels, gauges, and data readouts

### Section Organization

- **Navigation**: Dark gunmetal bar with brass-accented logo, stenciled links, and riveted bottom border
- **Hero**: Full-width dark background with massive condensed headline, propaganda-style subheading, and prominent CTA button
- **Features**: Grid of riveted steel cards with brass-accented headings and gear/propeller icon accents
- **Content rows**: Alternating dark and olive-tinted sections with Art Deco dividers between them
- **Propaganda banner**: Full-width bold color section (red or amber) with large stenciled text and directive messaging
- **Data dashboard**: Multi-panel layout with analog gauge components and instrument-style data readouts
- **Footer**: Darkest background with brass top-border, organized columns, and military-style identification text

### Responsive Approach

- Maintain dark color temperatures across all breakpoints -- never introduce light backgrounds on mobile
- Simplify rivet decorations on smaller screens but preserve the steel-panel border structure
- Stack card grids into single columns on mobile; maintain riveted card styling
- Reduce Art Deco ornamental complexity on small screens for clarity
- Typography remains condensed sans-serif at all sizes; increase line-height on mobile for readability
- Gear and propeller decorative elements can be hidden on mobile for performance

---

## CSS / Design Techniques

### Dieselpunk Card Component

```css
.diesel-card {
  background: var(--diesel-panel);
  border: 2px solid var(--diesel-border-steel);
  padding: 32px;
  position: relative;
  box-shadow: var(--diesel-shadow), var(--diesel-shadow-inset);
}

/* Corner rivets using pseudo-elements and box-shadows for all four corners */
.diesel-card::before,
.diesel-card::after {
  content: '';
  position: absolute;
  width: 10px;
  height: 10px;
  border-radius: 50%;
  background: radial-gradient(circle at 35% 35%, #a0a0a8 0%, #6b7280 50%, #4a4a52 100%);
  box-shadow:
    inset 0 1px 1px rgba(255, 255, 255, 0.3),
    0 1px 2px rgba(0, 0, 0, 0.5);
}

.diesel-card::before { top: 10px; left: 10px; }
.diesel-card::after { top: 10px; right: 10px; }

/* Additional bottom rivets via a wrapper */
.diesel-card-rivet-bottom::before { bottom: 10px; left: 10px; top: auto; }
.diesel-card-rivet-bottom::after { bottom: 10px; right: 10px; top: auto; }

/* Card heading */
.diesel-card h3 {
  font-family: 'Oswald', sans-serif;
  font-weight: 700;
  font-size: 1.1rem;
  text-transform: uppercase;
  letter-spacing: 0.06em;
  color: var(--diesel-brass);
  margin-bottom: 12px;
  padding-bottom: 8px;
  border-bottom: 1px solid var(--diesel-border-steel);
}

/* Card grid */
.diesel-card-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
  gap: 24px;
}
```

### Dieselpunk Button

```css
.diesel-button {
  display: inline-flex;
  align-items: center;
  justify-content: center;
  gap: 8px;
  background: var(--diesel-brass-surface);
  color: var(--diesel-bg-dark);
  border: 2px solid var(--diesel-brass-dark);
  padding: 14px 36px;
  font-family: 'Bebas Neue', 'Oswald', sans-serif;
  font-size: 1rem;
  letter-spacing: 0.1em;
  text-transform: uppercase;
  cursor: pointer;
  text-decoration: none;
  box-shadow: 0 3px 6px rgba(0, 0, 0, 0.3), inset 0 1px 0 rgba(255, 255, 255, 0.15);
  transition: all 0.2s ease;
  position: relative;
}

.diesel-button:hover {
  background: linear-gradient(145deg, #ddb860 0%, #c9a84c 50%, #b08830 100%);
  box-shadow: 0 4px 10px rgba(0, 0, 0, 0.4), inset 0 1px 0 rgba(255, 255, 255, 0.25);
  transform: translateY(-1px);
}

.diesel-button:active {
  box-shadow: inset 0 2px 6px rgba(0, 0, 0, 0.4);
  transform: translateY(1px);
}

/* Steel variant */
.diesel-button--steel {
  background: var(--diesel-steel-surface);
  color: var(--diesel-text-light);
  border-color: var(--diesel-gunmetal);
}

.diesel-button--steel:hover {
  background: linear-gradient(145deg, #9a9da3 0%, #8a8d93 50%, #7a7d83 100%);
}

/* Danger / Red variant */
.diesel-button--danger {
  background: linear-gradient(145deg, #c82820 0%, #b8221e 50%, #981a16 100%);
  color: var(--diesel-text-parchment);
  border-color: #8b1a16;
}

.diesel-button--danger:hover {
  background: linear-gradient(145deg, #d83030 0%, #c82820 50%, #a81e1a 100%);
}

/* Outline variant */
.diesel-button--outline {
  background: transparent;
  color: var(--diesel-brass);
  border: 2px solid var(--diesel-brass);
  box-shadow: none;
}

.diesel-button--outline:hover {
  background: rgba(201, 168, 76, 0.1);
  box-shadow: 0 0 12px rgba(201, 168, 76, 0.15);
}
```

### Navigation Bar

```css
.diesel-nav {
  display: flex;
  align-items: center;
  justify-content: space-between;
  max-width: 1200px;
  margin: 0 auto;
  padding: 0 40px;
  height: 64px;
  background: var(--diesel-panel);
  border-bottom: 3px solid var(--diesel-brass-dark);
  box-shadow: 0 2px 8px rgba(0, 0, 0, 0.4);
  position: relative;
}

/* Decorative rivet strip along the bottom border */
.diesel-nav::after {
  content: '';
  position: absolute;
  bottom: -3px;
  left: 0;
  right: 0;
  height: 3px;
  background: repeating-linear-gradient(
    90deg,
    var(--diesel-brass-dark) 0px,
    var(--diesel-brass-dark) 6px,
    var(--diesel-brass) 6px,
    var(--diesel-brass) 8px,
    var(--diesel-brass-dark) 8px,
    var(--diesel-brass-dark) 40px
  );
}

.diesel-nav__logo {
  font-family: 'Bebas Neue', sans-serif;
  font-size: 1.5rem;
  color: var(--diesel-brass);
  text-decoration: none;
  text-transform: uppercase;
  letter-spacing: 0.12em;
  text-shadow: 1px 1px 2px rgba(0, 0, 0, 0.5);
}

.diesel-nav__links {
  display: flex;
  gap: 32px;
  list-style: none;
  margin: 0;
  padding: 0;
}

.diesel-nav__links a {
  font-family: 'Oswald', sans-serif;
  font-weight: 500;
  font-size: 0.85rem;
  color: var(--diesel-text-muted);
  text-decoration: none;
  text-transform: uppercase;
  letter-spacing: 0.08em;
  transition: color 0.2s ease;
  position: relative;
}

.diesel-nav__links a:hover,
.diesel-nav__links a.active {
  color: var(--diesel-brass);
}

.diesel-nav__links a.active::after {
  content: '';
  position: absolute;
  bottom: -20px;
  left: 0;
  right: 0;
  height: 2px;
  background: var(--diesel-brass);
}
```

### Hero Section

```css
.diesel-hero {
  position: relative;
  display: flex;
  align-items: center;
  justify-content: center;
  text-align: center;
  min-height: 80vh;
  padding: 100px 40px;
  background: var(--diesel-bg-dark);
  overflow: hidden;
}

/* Subtle noise/grain texture overlay */
.diesel-hero::before {
  content: '';
  position: absolute;
  inset: 0;
  background-image: url("data:image/svg+xml,%3Csvg viewBox='0 0 256 256' xmlns='http://www.w3.org/2000/svg'%3E%3Cfilter id='n'%3E%3CfeTurbulence type='fractalNoise' baseFrequency='0.85' numOctaves='4' stitchTiles='stitch'/%3E%3C/filter%3E%3Crect width='100%25' height='100%25' filter='url(%23n)' opacity='0.04'/%3E%3C/svg%3E");
  pointer-events: none;
  z-index: 1;
}

/* Art Deco sunburst background pattern */
.diesel-hero::after {
  content: '';
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  width: 800px;
  height: 800px;
  background: repeating-conic-gradient(
    from 0deg,
    rgba(201, 168, 76, 0.03) 0deg 5deg,
    transparent 5deg 10deg
  );
  border-radius: 50%;
  pointer-events: none;
  z-index: 1;
}

.diesel-hero__content {
  position: relative;
  z-index: 2;
  max-width: 800px;
}

.diesel-hero__content h1 {
  font-family: 'Bebas Neue', sans-serif;
  font-size: clamp(3rem, 8vw, 6rem);
  color: var(--diesel-brass);
  text-shadow: 2px 2px 0 rgba(0, 0, 0, 0.5), 0 0 30px rgba(201, 168, 76, 0.1);
  letter-spacing: 0.1em;
  margin-bottom: 1rem;
}

.diesel-hero__content p {
  font-size: 1.15rem;
  color: var(--diesel-text-muted);
  max-width: 600px;
  margin: 0 auto 2.5rem;
  line-height: 1.8;
}

@media (max-width: 768px) {
  .diesel-hero {
    min-height: auto;
    padding: 60px 20px;
  }
}
```

### Rivet Border Strip

```css
/* A decorative horizontal rivet border that can be placed between sections */
.diesel-rivet-border {
  width: 100%;
  height: 20px;
  background: var(--diesel-bg-smoke);
  border-top: 2px solid var(--diesel-border-steel);
  border-bottom: 2px solid var(--diesel-border-steel);
  position: relative;
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 40px;
}

.diesel-rivet-border::before,
.diesel-rivet-border::after {
  content: '';
  width: 8px;
  height: 8px;
  border-radius: 50%;
  background: radial-gradient(circle at 35% 35%, #a0a0a8, #5a5a62);
  box-shadow: inset 0 1px 1px rgba(255, 255, 255, 0.2), 0 1px 2px rgba(0, 0, 0, 0.4);
}

/* Repeating rivets via background-image */
.diesel-rivet-strip {
  width: 100%;
  height: 12px;
  background:
    radial-gradient(circle, #8a8d93 3px, transparent 3px) 20px center / 40px 12px repeat-x,
    linear-gradient(180deg, #3b3b3b 0%, #2c2f33 100%);
  border-top: 1px solid #555;
  border-bottom: 1px solid #555;
}
```

### Art Deco Chevron Divider

```css
.diesel-deco-divider {
  display: flex;
  align-items: center;
  justify-content: center;
  padding: 32px 0;
  gap: 16px;
}

.diesel-deco-divider::before,
.diesel-deco-divider::after {
  content: '';
  flex: 1;
  max-width: 200px;
  height: 2px;
  background: linear-gradient(
    90deg,
    transparent,
    var(--diesel-brass-dark),
    var(--diesel-brass),
    var(--diesel-brass-dark),
    transparent
  );
}

/* The central chevron ornament */
.diesel-deco-divider__chevron {
  width: 30px;
  height: 30px;
  position: relative;
  display: flex;
  align-items: center;
  justify-content: center;
}

.diesel-deco-divider__chevron::before {
  content: '';
  width: 16px;
  height: 16px;
  border-right: 3px solid var(--diesel-brass);
  border-bottom: 3px solid var(--diesel-brass);
  transform: rotate(-45deg);
}
```

### Propaganda Banner

```css
.diesel-propaganda {
  background: linear-gradient(135deg, #b8221e 0%, #981a16 50%, #b8221e 100%);
  padding: 48px 40px;
  text-align: center;
  position: relative;
  border-top: 4px solid var(--diesel-brass-dark);
  border-bottom: 4px solid var(--diesel-brass-dark);
  overflow: hidden;
}

/* Diagonal stripe overlay */
.diesel-propaganda::before {
  content: '';
  position: absolute;
  inset: 0;
  background: repeating-linear-gradient(
    -45deg,
    transparent,
    transparent 20px,
    rgba(0, 0, 0, 0.06) 20px,
    rgba(0, 0, 0, 0.06) 22px
  );
  pointer-events: none;
}

.diesel-propaganda h2 {
  font-family: 'Bebas Neue', sans-serif;
  font-size: clamp(2rem, 5vw, 3.5rem);
  color: var(--diesel-text-parchment);
  text-transform: uppercase;
  letter-spacing: 0.12em;
  text-shadow: 2px 2px 0 rgba(0, 0, 0, 0.3);
  position: relative;
  z-index: 1;
  margin-bottom: 0.5rem;
}

.diesel-propaganda p {
  font-family: 'Oswald', sans-serif;
  font-weight: 500;
  font-size: 1.1rem;
  color: rgba(240, 230, 208, 0.85);
  text-transform: uppercase;
  letter-spacing: 0.06em;
  position: relative;
  z-index: 1;
  margin-bottom: 1.5rem;
}
```

### Analog Gauge Component

```css
.diesel-gauge {
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 8px;
  width: 120px;
}

.diesel-gauge__dial {
  width: 100px;
  height: 50px;
  border: 3px solid var(--diesel-steel);
  border-radius: 100px 100px 0 0;
  background: radial-gradient(ellipse at bottom, #2c2f33, #1a1a1a);
  position: relative;
  overflow: hidden;
  box-shadow: inset 0 -2px 6px rgba(0, 0, 0, 0.4);
}

/* Gauge fill */
.diesel-gauge__fill {
  position: absolute;
  bottom: 0;
  left: 0;
  width: 100%;
  background: linear-gradient(0deg, var(--diesel-rust), var(--diesel-amber), var(--diesel-brass));
  transition: height 0.6s ease;
}

/* Gauge tick marks */
.diesel-gauge__dial::after {
  content: '';
  position: absolute;
  top: 4px;
  left: 50%;
  transform: translateX(-50%);
  width: 80%;
  height: 1px;
  background: repeating-linear-gradient(
    90deg,
    var(--diesel-steel) 0px,
    var(--diesel-steel) 1px,
    transparent 1px,
    transparent 10px
  );
}

.diesel-gauge__label {
  font-family: 'Oswald', sans-serif;
  font-weight: 500;
  font-size: 0.65rem;
  text-transform: uppercase;
  letter-spacing: 0.12em;
  color: var(--diesel-text-muted);
}

.diesel-gauge__value {
  font-family: 'Bebas Neue', sans-serif;
  font-size: 1.2rem;
  color: var(--diesel-brass);
}
```

### Art Deco Frame

```css
.diesel-deco-frame {
  position: relative;
  border: 2px solid var(--diesel-brass-dark);
  padding: 40px;
  margin: 24px;
}

/* Inner border for double-frame effect */
.diesel-deco-frame::before {
  content: '';
  position: absolute;
  inset: 6px;
  border: 1px solid var(--diesel-brass-dark);
  pointer-events: none;
}

/* Corner ornaments */
.diesel-deco-frame::after {
  content: '';
  position: absolute;
  top: -6px;
  left: -6px;
  right: -6px;
  bottom: -6px;
  border: none;
  background:
    /* Top-left corner */
    linear-gradient(var(--diesel-brass) 0%, var(--diesel-brass) 100%) 0 0 / 20px 3px no-repeat,
    linear-gradient(var(--diesel-brass) 0%, var(--diesel-brass) 100%) 0 0 / 3px 20px no-repeat,
    /* Top-right corner */
    linear-gradient(var(--diesel-brass) 0%, var(--diesel-brass) 100%) 100% 0 / 20px 3px no-repeat,
    linear-gradient(var(--diesel-brass) 0%, var(--diesel-brass) 100%) 100% 0 / 3px 20px no-repeat,
    /* Bottom-left corner */
    linear-gradient(var(--diesel-brass) 0%, var(--diesel-brass) 100%) 0 100% / 20px 3px no-repeat,
    linear-gradient(var(--diesel-brass) 0%, var(--diesel-brass) 100%) 0 100% / 3px 20px no-repeat,
    /* Bottom-right corner */
    linear-gradient(var(--diesel-brass) 0%, var(--diesel-brass) 100%) 100% 100% / 20px 3px no-repeat,
    linear-gradient(var(--diesel-brass) 0%, var(--diesel-brass) 100%) 100% 100% / 3px 20px no-repeat;
  pointer-events: none;
}
```

---

## Design Do's and Don'ts

### Do

- Use dark, industrial backgrounds (charcoal, gunmetal, oil-black) as the primary canvas throughout
- Apply visible rivet decorations to card corners and panel seams for tactile authenticity
- Choose heavy, condensed sans-serif typefaces (Bebas Neue, Oswald) that feel stamped or stenciled
- Include Art Deco ornamental patterns: chevrons, sunbursts, and stepped forms as section dividers
- Use brass and amber metallics for primary accent colors, interactive elements, and headings
- Add subtle noise or grain textures to backgrounds to simulate aged, industrial surfaces
- Reference propaganda poster design for bold CTAs: large text, high contrast, directive language
- Make buttons feel like heavy mechanical switches -- substantial, metallic, and satisfying to press
- Use analog instrument metaphors (gauges, dials, meters) for data visualization
- Maintain a warm, incandescent lighting feel -- amber glows and vignette shadows

### Don't

- Use bright, saturated colors as primary palette elements -- color should be muted, smoky, and warm
- Apply thin, delicate typefaces -- nothing should feel lightweight or fragile in Dieselpunk
- Use organic, flowing curves (Art Nouveau vines, botanical motifs) -- all ornamentation is geometric and mechanical
- Make layouts too sparse or minimalist -- Dieselpunk panels should feel full, structured, and information-rich
- Mix in modern flat design patterns (pill buttons, pastel gradients, rounded cards) that break the period illusion
- Use pure white backgrounds -- the lightest surface should be aged parchment or cream
- Forget the material quality -- every surface should suggest steel, brass, leather, or oiled wood
- Overuse the propaganda red -- it should be a powerful accent, not the dominant color
- Apply neon or electric glow effects -- light sources are incandescent, not digital
- Neglect the rivet and bolt details -- these small touches are essential to the industrial authenticity

---

## Related Aesthetics

| Aesthetic | Relationship to Dieselpunk |
|-----------|---------------------------|
| **Steampunk** | Direct sibling and predecessor; both are retrofuturistic "-punk" aesthetics, but Steampunk is Victorian/steam-powered while Dieselpunk advances to the interwar diesel era with Art Deco replacing Victorian ornament |
| **Cyberpunk** | Fellow "-punk" genre set in the future; Dieselpunk looks backward to analog industrial might while Cyberpunk looks forward to digital corporate dystopia -- both share themes of power and conflict |
| **Art Deco** | Primary decorative influence; Dieselpunk borrows Art Deco's geometric patterns, metallic color palettes, and Streamline Moderne curves, then roughens them with industrial grit |
| **Constructivism** | Shares the propaganda poster aesthetic, bold typography, and angular compositions; Constructivism is Soviet revolutionary, Dieselpunk is broader interwar industrial |
| **Atomic Age** | Chronological successor; as Dieselpunk's interwar period ends, Atomic Age picks up with jet-powered, nuclear-era optimism and Space Age streamlining |
| **Solarpunk** | Philosophical opposite; where Dieselpunk glorifies fossil-fuel industrial might, Solarpunk imagines a sustainable, green-powered future |
| **Heroic Realism** | Shares the muscular, propagandistic visual language and glorification of human labor and industrial power |
| **Industrial Gothic** | Overlaps in dark, heavy, metallic aesthetics; Industrial Gothic is more subcultural and brooding, Dieselpunk is more adventurous and militaristic |
| **Bauhaus** | Contemporary movement of the diesel era; shares the geometric, functional ethos but Bauhaus is stripped-down modernist while Dieselpunk embraces decorative industrial excess |

---

## Quick-Start HTML Template

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Dieselpunk Page</title>
  <link href="https://fonts.googleapis.com/css2?family=Bebas+Neue&family=Oswald:wght@500;700&family=Source+Sans+3:ital,wght@0,400;0,600;1,400&display=swap" rel="stylesheet">
  <style>
    :root {
      --diesel-bg-dark: #1a1a1a;
      --diesel-bg-panel: #2c2f33;
      --diesel-bg-smoke: #3b3b3b;
      --diesel-bg-oil: #1e1e24;
      --diesel-brass: #c9a84c;
      --diesel-brass-dark: #9a7b2f;
      --diesel-steel: #8a8d93;
      --diesel-gunmetal: #6b7280;
      --diesel-amber: #d4890e;
      --diesel-rust: #8b3a1a;
      --diesel-red: #b8221e;
      --diesel-olive: #4b5320;
      --diesel-khaki: #8f7e4f;
      --diesel-text-light: #e8e4da;
      --diesel-text-parchment: #f0e6d0;
      --diesel-text-muted: #6b7280;
    }

    * { margin: 0; padding: 0; box-sizing: border-box; }

    body {
      background: var(--diesel-bg-dark);
      color: var(--diesel-text-light);
      font-family: 'Source Sans 3', sans-serif;
      font-size: 1rem;
      line-height: 1.7;
    }

    h1, h2, h3 {
      font-family: 'Bebas Neue', sans-serif;
      font-weight: 400;
      text-transform: uppercase;
      letter-spacing: 0.06em;
      line-height: 1.1;
    }

    /* ---- Navigation ---- */
    nav {
      display: flex;
      align-items: center;
      justify-content: space-between;
      max-width: 1200px;
      margin: 0 auto;
      padding: 0 40px;
      height: 60px;
      background: linear-gradient(180deg, #2c2f33, #1e1e24);
      border-bottom: 3px solid var(--diesel-brass-dark);
      position: relative;
    }

    nav::after {
      content: '';
      position: absolute;
      bottom: -3px;
      left: 0;
      right: 0;
      height: 3px;
      background: repeating-linear-gradient(
        90deg,
        var(--diesel-brass-dark) 0px,
        var(--diesel-brass-dark) 6px,
        var(--diesel-brass) 6px,
        var(--diesel-brass) 8px,
        var(--diesel-brass-dark) 8px,
        var(--diesel-brass-dark) 40px
      );
    }

    nav a.logo {
      font-family: 'Bebas Neue', sans-serif;
      font-size: 1.5rem;
      color: var(--diesel-brass);
      text-decoration: none;
      text-transform: uppercase;
      letter-spacing: 0.12em;
      text-shadow: 1px 1px 2px rgba(0, 0, 0, 0.5);
    }

    nav ul { display: flex; gap: 28px; list-style: none; }

    nav ul a {
      font-family: 'Oswald', sans-serif;
      font-weight: 500;
      font-size: 0.85rem;
      color: var(--diesel-text-muted);
      text-decoration: none;
      text-transform: uppercase;
      letter-spacing: 0.08em;
      transition: color 0.2s;
    }

    nav ul a:hover { color: var(--diesel-brass); }

    /* ---- Hero ---- */
    .hero {
      position: relative;
      display: flex;
      align-items: center;
      justify-content: center;
      text-align: center;
      min-height: 80vh;
      padding: 100px 40px;
      overflow: hidden;
    }

    /* Art Deco sunburst */
    .hero::after {
      content: '';
      position: absolute;
      top: 50%;
      left: 50%;
      transform: translate(-50%, -50%);
      width: 700px;
      height: 700px;
      background: repeating-conic-gradient(
        from 0deg,
        rgba(201, 168, 76, 0.03) 0deg 5deg,
        transparent 5deg 10deg
      );
      border-radius: 50%;
      pointer-events: none;
    }

    .hero-content {
      position: relative;
      z-index: 2;
      max-width: 750px;
    }

    .hero h1 {
      font-size: clamp(3rem, 8vw, 6rem);
      color: var(--diesel-brass);
      text-shadow: 2px 2px 0 rgba(0, 0, 0, 0.5), 0 0 30px rgba(201, 168, 76, 0.1);
      letter-spacing: 0.1em;
      margin-bottom: 1rem;
    }

    .hero p {
      font-size: 1.15rem;
      color: var(--diesel-text-muted);
      max-width: 580px;
      margin: 0 auto 2.5rem;
    }

    .btn {
      display: inline-block;
      background: linear-gradient(145deg, #d4a843, #c9a84c, #9a7b2f);
      color: var(--diesel-bg-dark);
      border: 2px solid var(--diesel-brass-dark);
      padding: 14px 40px;
      font-family: 'Bebas Neue', sans-serif;
      font-size: 1.1rem;
      letter-spacing: 0.1em;
      text-transform: uppercase;
      text-decoration: none;
      cursor: pointer;
      box-shadow: 0 3px 6px rgba(0, 0, 0, 0.3), inset 0 1px 0 rgba(255, 255, 255, 0.15);
      transition: all 0.2s;
    }

    .btn:hover {
      background: linear-gradient(145deg, #ddb860, #c9a84c, #b08830);
      box-shadow: 0 4px 10px rgba(0, 0, 0, 0.4), inset 0 1px 0 rgba(255, 255, 255, 0.25);
      transform: translateY(-1px);
    }

    /* ---- Rivet Strip Divider ---- */
    .rivet-strip {
      width: 100%;
      height: 12px;
      background:
        radial-gradient(circle, #8a8d93 3px, transparent 3px) 20px center / 40px 12px repeat-x,
        linear-gradient(180deg, #3b3b3b, #2c2f33);
      border-top: 1px solid #555;
      border-bottom: 1px solid #555;
    }

    /* ---- Features Section ---- */
    .features {
      padding: 72px 0;
      background: linear-gradient(180deg, var(--diesel-bg-panel), var(--diesel-bg-dark));
    }

    .features h2 {
      text-align: center;
      font-size: clamp(1.8rem, 4vw, 2.5rem);
      color: var(--diesel-text-parchment);
      margin-bottom: 12px;
    }

    .features .subtitle {
      text-align: center;
      font-family: 'Oswald', sans-serif;
      font-weight: 500;
      font-size: 0.8rem;
      color: var(--diesel-text-muted);
      text-transform: uppercase;
      letter-spacing: 0.14em;
      margin-bottom: 48px;
    }

    .features-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
      gap: 24px;
      max-width: 1100px;
      margin: 0 auto;
      padding: 0 40px;
    }

    .feature {
      background: linear-gradient(180deg, #2c2f33, #1e1e24);
      border: 2px solid var(--diesel-gunmetal);
      padding: 28px 28px 28px 28px;
      position: relative;
      box-shadow: 0 4px 12px rgba(0, 0, 0, 0.3), inset 0 1px 0 rgba(255, 255, 255, 0.03);
    }

    /* Corner rivets */
    .feature::before,
    .feature::after {
      content: '';
      position: absolute;
      width: 8px;
      height: 8px;
      border-radius: 50%;
      background: radial-gradient(circle at 35% 35%, #a0a0a8, #5a5a62);
      box-shadow: inset 0 1px 1px rgba(255, 255, 255, 0.2), 0 1px 2px rgba(0, 0, 0, 0.5);
    }

    .feature::before { top: 10px; left: 10px; }
    .feature::after { top: 10px; right: 10px; }

    .feature-icon {
      font-size: 1.6rem;
      margin-bottom: 12px;
    }

    .feature h3 {
      font-family: 'Oswald', sans-serif;
      font-weight: 700;
      font-size: 1.05rem;
      color: var(--diesel-brass);
      margin-bottom: 8px;
      padding-bottom: 8px;
      border-bottom: 1px solid var(--diesel-gunmetal);
    }

    .feature p {
      font-size: 0.95rem;
      color: var(--diesel-text-muted);
    }

    /* ---- Art Deco Chevron Divider ---- */
    .deco-divider {
      display: flex;
      align-items: center;
      justify-content: center;
      padding: 24px 0;
      gap: 12px;
    }

    .deco-divider::before,
    .deco-divider::after {
      content: '';
      flex: 1;
      max-width: 180px;
      height: 2px;
      background: linear-gradient(90deg, transparent, var(--diesel-brass-dark), var(--diesel-brass), var(--diesel-brass-dark), transparent);
    }

    .deco-divider span {
      width: 14px;
      height: 14px;
      border-right: 2px solid var(--diesel-brass);
      border-bottom: 2px solid var(--diesel-brass);
      transform: rotate(-45deg);
    }

    /* ---- Propaganda Banner ---- */
    .propaganda {
      background: linear-gradient(135deg, #b8221e, #981a16, #b8221e);
      padding: 48px 40px;
      text-align: center;
      position: relative;
      border-top: 4px solid var(--diesel-brass-dark);
      border-bottom: 4px solid var(--diesel-brass-dark);
      overflow: hidden;
    }

    .propaganda::before {
      content: '';
      position: absolute;
      inset: 0;
      background: repeating-linear-gradient(
        -45deg,
        transparent,
        transparent 20px,
        rgba(0, 0, 0, 0.06) 20px,
        rgba(0, 0, 0, 0.06) 22px
      );
      pointer-events: none;
    }

    .propaganda h2 {
      font-size: clamp(1.8rem, 5vw, 3rem);
      color: var(--diesel-text-parchment);
      letter-spacing: 0.12em;
      text-shadow: 2px 2px 0 rgba(0, 0, 0, 0.3);
      position: relative;
      z-index: 1;
      margin-bottom: 0.5rem;
    }

    .propaganda p {
      font-family: 'Oswald', sans-serif;
      font-weight: 500;
      font-size: 1rem;
      color: rgba(240, 230, 208, 0.8);
      text-transform: uppercase;
      letter-spacing: 0.06em;
      position: relative;
      z-index: 1;
      margin-bottom: 1.5rem;
    }

    .propaganda .btn {
      background: transparent;
      color: var(--diesel-text-parchment);
      border: 2px solid var(--diesel-text-parchment);
      box-shadow: none;
      position: relative;
      z-index: 1;
    }

    .propaganda .btn:hover {
      background: rgba(240, 230, 208, 0.12);
      box-shadow: 0 0 12px rgba(240, 230, 208, 0.15);
    }

    /* ---- Data Dashboard Section ---- */
    .dashboard {
      padding: 60px 40px;
      background: var(--diesel-bg-dark);
    }

    .dashboard h2 {
      text-align: center;
      font-size: 2rem;
      color: var(--diesel-text-parchment);
      margin-bottom: 40px;
    }

    .gauges {
      display: flex;
      justify-content: center;
      gap: 48px;
      flex-wrap: wrap;
    }

    .gauge {
      display: flex;
      flex-direction: column;
      align-items: center;
      gap: 6px;
    }

    .gauge-dial {
      width: 100px;
      height: 50px;
      border: 3px solid var(--diesel-steel);
      border-radius: 100px 100px 0 0;
      background: radial-gradient(ellipse at bottom, #2c2f33, #1a1a1a);
      position: relative;
      overflow: hidden;
      box-shadow: inset 0 -2px 6px rgba(0, 0, 0, 0.4);
    }

    .gauge-fill {
      position: absolute;
      bottom: 0;
      left: 0;
      width: 100%;
      background: linear-gradient(0deg, var(--diesel-rust), var(--diesel-amber), var(--diesel-brass));
      transition: height 0.6s ease;
    }

    .gauge-label {
      font-family: 'Oswald', sans-serif;
      font-weight: 500;
      font-size: 0.6rem;
      text-transform: uppercase;
      letter-spacing: 0.12em;
      color: var(--diesel-text-muted);
    }

    .gauge-value {
      font-family: 'Bebas Neue', sans-serif;
      font-size: 1.3rem;
      color: var(--diesel-brass);
    }

    /* ---- Footer ---- */
    footer {
      background: var(--diesel-bg-oil);
      text-align: center;
      padding: 28px 40px;
      border-top: 3px solid var(--diesel-brass-dark);
    }

    footer p {
      font-family: 'Oswald', sans-serif;
      font-weight: 500;
      font-size: 0.8rem;
      color: var(--diesel-text-muted);
      text-transform: uppercase;
      letter-spacing: 0.08em;
    }

    /* ---- Responsive ---- */
    @media (max-width: 768px) {
      nav { padding: 0 20px; height: 52px; }
      nav ul { gap: 16px; }
      .hero { min-height: auto; padding: 60px 20px; }
      .features { padding: 48px 0; }
      .features-grid { padding: 0 20px; }
      .propaganda { padding: 36px 20px; }
      .dashboard { padding: 40px 20px; }
      .gauges { gap: 24px; }
    }
  </style>
</head>
<body>
  <nav>
    <a href="#" class="logo">Iron Vanguard</a>
    <ul>
      <li><a href="#">Hangar</a></li>
      <li><a href="#">Arsenal</a></li>
      <li><a href="#">Command</a></li>
      <li><a href="#">Dispatch</a></li>
    </ul>
  </nav>

  <section class="hero">
    <div class="hero-content">
      <h1>Forge the Future</h1>
      <p>Heavy diesel engineering for the modern frontier. Riveted steel, precision gears, and the thunder of turbocharged power -- built to endure.</p>
      <a href="#" class="btn">Enter the Foundry</a>
    </div>
  </section>

  <div class="rivet-strip"></div>

  <section class="features">
    <h2>Divisions & Operations</h2>
    <p class="subtitle">Strategic capabilities across all theaters</p>
    <div class="features-grid">
      <div class="feature">
        <div class="feature-icon">&#9881;</div>
        <h3>Armored Division</h3>
        <p>Heavy diesel-powered ground vehicles with reinforced plating and dual-turret configurations. Built for sustained forward operations.</p>
      </div>
      <div class="feature">
        <div class="feature-icon">&#9992;</div>
        <h3>Aerial Corps</h3>
        <p>Twin-engine propeller aircraft and rigid airships for reconnaissance and strategic bombardment across contested airspace.</p>
      </div>
      <div class="feature">
        <div class="feature-icon">&#9878;</div>
        <h3>Naval Dreadnoughts</h3>
        <p>Armored warships with steam-turbine propulsion and heavy-caliber gun batteries. Command the seas with overwhelming firepower.</p>
      </div>
    </div>
  </section>

  <div class="deco-divider"><span></span></div>

  <section class="propaganda">
    <h2>The Iron Will Prevails</h2>
    <p>Your industry builds the future. Report to the foundry.</p>
    <a href="#" class="btn">Enlist Now</a>
  </section>

  <section class="dashboard">
    <h2>Operational Readiness</h2>
    <div class="gauges">
      <div class="gauge">
        <div class="gauge-dial"><div class="gauge-fill" style="height: 75%;"></div></div>
        <div class="gauge-label">Engine Output</div>
        <div class="gauge-value">75%</div>
      </div>
      <div class="gauge">
        <div class="gauge-dial"><div class="gauge-fill" style="height: 90%;"></div></div>
        <div class="gauge-label">Fuel Reserve</div>
        <div class="gauge-value">90%</div>
      </div>
      <div class="gauge">
        <div class="gauge-dial"><div class="gauge-fill" style="height: 60%;"></div></div>
        <div class="gauge-label">Armor Integrity</div>
        <div class="gauge-value">60%</div>
      </div>
      <div class="gauge">
        <div class="gauge-dial"><div class="gauge-fill" style="height: 45%;"></div></div>
        <div class="gauge-label">Munitions</div>
        <div class="gauge-value">45%</div>
      </div>
    </div>
  </section>

  <div class="rivet-strip"></div>

  <footer>
    <p>Iron Vanguard Industrial Co. -- Est. 1932 -- Forged in Steel, Driven by Diesel</p>
  </footer>
</body>
</html>
```
