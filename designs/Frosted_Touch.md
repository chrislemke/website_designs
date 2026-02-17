# Frosted Touch -- Design Reference

Frosted Touch is the 2026 evolution of glassmorphism -- more refined, more subtle, with better performance and deeper layering. Where early glassmorphism relied on a single frosted panel over a colorful background, Frosted Touch builds entire interfaces from translucent layers at multiple depths, each revealing hints of color beneath. Frosted glass panels float over vibrant gradient backgrounds, connected by diffused shadows that create elegant depth without heaviness. Semi-transparent whites and soft blurs replace hard edges and solid fills. The result is an interface that feels like looking through layers of architectural glass: luminous, airy, and quietly sophisticated. Every surface breathes, every boundary is soft, and the vibrant world beneath the frost is always felt but never fully revealed.

---

## Visual Characteristics

- **Frosted glass panels** with `backdrop-filter: blur()` creating translucent surfaces that obscure but do not hide the layers beneath
- **Multiple depth layers** -- 3-4 z-levels of translucent panels, each with slightly different blur intensity and opacity, creating a convincing sense of spatial depth
- **Diffused box-shadows** -- large spread values (20-40px) with low opacity (0.05-0.15) replacing hard drop shadows, producing soft halos of depth rather than defined edges
- **Rounded edges everywhere** -- 16-24px border-radius on panels, cards, and containers, with smaller radii (8-12px) on buttons and inputs
- **Soft inner-glow borders** -- 1px semi-transparent white borders (`rgba(255,255,255,0.15-0.25)`) that catch light and define panel edges without hard contrast
- **Subtle gradients within glass** -- panels carry faint directional gradients (top-to-bottom or diagonal) to simulate light falling across frosted glass
- **Vibrant gradient backgrounds** -- rich, multi-stop gradients in deep blues, purples, and magentas provide the color energy that frosted panels partially reveal
- **Light refraction effects** at panel edges -- brighter border highlights on the side facing the virtual light source
- **Color bleed through frost** -- background colors shift and warm as they pass through translucent layers, creating organic chromatic variation
- **Saturation boost behind glass** -- `saturate(1.2-1.8)` applied with backdrop-filter to make colors beneath the frost richer, not duller
- **Floating composition** -- panels appear to hover in space, detached from any solid surface, supported only by light and shadow
- **Minimal visual noise** -- no textures, no patterns, no grain; the aesthetic derives all visual interest from transparency, blur, and light

---

## Color Palette

The Frosted Touch palette centers on semi-transparent whites layered over vibrant gradients. The frost itself is nearly colorless; all chromatic energy comes from the backgrounds and accents beneath:

- **Semi-transparent whites** -- the primary surface color, ranging from `rgba(255,255,255,0.08)` for deep background layers to `rgba(255,255,255,0.25)` for foreground panels
- **Vibrant gradient backgrounds** -- deep blue to purple to magenta, providing the luminous color field behind all frost layers
- **Frosted panel borders** -- thin white strokes at low opacity (`rgba(255,255,255,0.15-0.25)`) to catch and define edges
- **Accent blue** -- a clear, cool blue for interactive elements, links, and highlights
- **Accent purple** -- a soft violet for secondary accents, tags, and decorative elements
- **Warm white text** -- not pure white but a soft, slightly warm off-white for comfortable reading against translucent surfaces
- **Shadow tones** -- deep indigo and blue-black at very low opacity for diffused shadows
- **Success, warning, error states** -- kept soft and muted, rendered as tinted frosted panels rather than solid blocks of color

### Suggested Implementation Palette

| Role                  | Color                | Hex / Value                        |
|-----------------------|----------------------|------------------------------------|
| Background Gradient A | Deep Navy Blue       | `#1a1a4e`                          |
| Background Gradient B | Deep Purple          | `#4a1a6b`                          |
| Background Gradient C | Deep Magenta         | `#6b1a4a`                          |
| Frost Surface Deep    | Translucent White    | `rgba(255, 255, 255, 0.08)`        |
| Frost Surface Mid     | Translucent White    | `rgba(255, 255, 255, 0.12)`        |
| Frost Surface Light   | Translucent White    | `rgba(255, 255, 255, 0.18)`        |
| Frost Surface Raised  | Translucent White    | `rgba(255, 255, 255, 0.25)`        |
| Frost Border          | White Edge           | `rgba(255, 255, 255, 0.18)`        |
| Frost Border Bright   | White Edge Highlight | `rgba(255, 255, 255, 0.30)`        |
| Accent Blue           | Clear Sky Blue       | `#60A5FA`                          |
| Accent Purple         | Soft Violet          | `#A78BFA`                          |
| Accent Cyan           | Frost Cyan           | `#67E8F9`                          |
| Text Primary          | Warm White           | `#F8FAFC`                          |
| Text Secondary        | Muted Lavender       | `rgba(248, 250, 252, 0.70)`        |
| Text Muted            | Faded White          | `rgba(248, 250, 252, 0.45)`        |
| Shadow                | Deep Indigo          | `rgba(15, 10, 40, 0.25)`          |
| Shadow Diffused       | Blue-Black           | `rgba(10, 10, 50, 0.15)`          |
| Glow Accent           | Blue Glow            | `rgba(96, 165, 250, 0.20)`        |

### CSS Custom Properties

```css
:root {
  /* Background gradient stops */
  --frost-bg-a: #1a1a4e;
  --frost-bg-b: #4a1a6b;
  --frost-bg-c: #6b1a4a;

  /* Frost surface layers (ordered by depth, back to front) */
  --frost-surface-deep: rgba(255, 255, 255, 0.08);
  --frost-surface-mid: rgba(255, 255, 255, 0.12);
  --frost-surface-light: rgba(255, 255, 255, 0.18);
  --frost-surface-raised: rgba(255, 255, 255, 0.25);

  /* Borders */
  --frost-border: rgba(255, 255, 255, 0.18);
  --frost-border-bright: rgba(255, 255, 255, 0.30);
  --frost-border-subtle: rgba(255, 255, 255, 0.10);

  /* Text */
  --frost-text-primary: #F8FAFC;
  --frost-text-secondary: rgba(248, 250, 252, 0.70);
  --frost-text-muted: rgba(248, 250, 252, 0.45);
  --frost-text-heading: #FFFFFF;

  /* Accents */
  --frost-accent-blue: #60A5FA;
  --frost-accent-purple: #A78BFA;
  --frost-accent-cyan: #67E8F9;
  --frost-accent-pink: #F472B6;

  /* Shadows */
  --frost-shadow: rgba(15, 10, 40, 0.25);
  --frost-shadow-diffused: rgba(10, 10, 50, 0.15);
  --frost-shadow-glow: rgba(96, 165, 250, 0.12);

  /* Functional mappings */
  --frost-bg-primary: var(--frost-bg-a);
  --frost-bg-card: var(--frost-surface-light);
  --frost-bg-card-hover: var(--frost-surface-raised);
  --frost-text-body: var(--frost-text-primary);
  --frost-accent-primary: var(--frost-accent-blue);
  --frost-accent-secondary: var(--frost-accent-purple);

  /* Blur values */
  --frost-blur-sm: blur(8px);
  --frost-blur-md: blur(16px);
  --frost-blur-lg: blur(24px);
  --frost-blur-xl: blur(40px);

  /* Border radius */
  --frost-radius-sm: 8px;
  --frost-radius-md: 16px;
  --frost-radius-lg: 24px;
  --frost-radius-pill: 9999px;
}
```

---

## Typography

### Typeface Characteristics

Frosted Touch typography prioritizes clean legibility against translucent, shifting backgrounds:

- **Geometric sans-serifs** -- clean, open letterforms with even stroke widths that remain readable at any blur level beneath them
- **Medium weight bias** -- 400-500 weight range for body text; thinner weights disappear against frost, heavier weights feel too solid for the airy aesthetic
- **Generous letter-spacing** -- slightly open tracking (0.01-0.03em) improves readability on translucent surfaces where letter edges can blur into the background
- **High line-height** -- 1.6-1.8 for body text; the spaciousness of the typography matches the spaciousness of the frosted layout
- **Subtle text-shadow for legibility** -- a faint dark shadow (0 1px 2px with low opacity) behind text ensures characters remain readable even when the frost background shifts color
- **White and near-white text** -- all text lives in the white/cool-gray range; colored text is reserved exclusively for interactive elements and accents
- **Heading distinction through weight and size, not color** -- headings use 600-700 weight and larger size but remain white, preserving the monochromatic frost feeling

### Recommended Web Fonts

| Font | Style | Usage |
|------|-------|-------|
| **Inter** | Geometric sans-serif | Primary body and UI text -- excellent legibility, wide range of weights, variable font support |
| **Plus Jakarta Sans** | Modern geometric sans | Headings and display text -- slightly warmer and more characterful than Inter |
| **DM Sans** | Clean geometric sans | Alternative body text -- compact and clear with geometric proportions |
| **Outfit** | Geometric sans-serif | Headings -- geometric with slight softness, good for larger sizes |
| **Manrope** | Semi-rounded sans | Friendly alternative for body text -- open apertures aid readability on glass |
| **Space Grotesk** | Monospace-inspired sans | UI labels, data displays, technical text |
| **JetBrains Mono** | Monospace | Code snippets, status indicators, numerical data |

### Typography CSS Example

```css
@import url('https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700&family=Plus+Jakarta+Sans:wght@500;600;700;800&family=Space+Grotesk:wght@400;500;600&family=JetBrains+Mono:wght@400;500&display=swap');

/* Primary body text -- clean, readable against frost */
body {
  font-family: 'Inter', 'DM Sans', system-ui, -apple-system, sans-serif;
  font-size: 16px;
  line-height: 1.7;
  letter-spacing: 0.01em;
  color: var(--frost-text-primary);
  font-weight: 400;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}

/* Headings -- slightly heavier, geometric, white */
h1, h2, h3 {
  font-family: 'Plus Jakarta Sans', 'Inter', sans-serif;
  color: var(--frost-text-heading);
  font-weight: 700;
  letter-spacing: -0.01em;
  line-height: 1.3;
  text-shadow: 0 1px 3px rgba(0, 0, 0, 0.15);
}

h1 {
  font-size: clamp(2rem, 5vw, 3.5rem);
  font-weight: 800;
  letter-spacing: -0.02em;
}

h2 {
  font-size: clamp(1.4rem, 3vw, 2rem);
  font-weight: 700;
  color: var(--frost-text-primary);
}

h3 {
  font-size: clamp(1.1rem, 2vw, 1.4rem);
  font-weight: 600;
  color: var(--frost-text-secondary);
}

/* Paragraph text on glass surfaces */
.frost-body-text {
  font-family: 'Inter', sans-serif;
  font-size: 1rem;
  font-weight: 400;
  line-height: 1.7;
  color: var(--frost-text-secondary);
  text-shadow: 0 1px 2px rgba(0, 0, 0, 0.08);
}

/* Small UI labels */
.frost-label {
  font-family: 'Space Grotesk', 'Inter', sans-serif;
  font-size: 0.75rem;
  font-weight: 500;
  letter-spacing: 0.06em;
  text-transform: uppercase;
  color: var(--frost-text-muted);
}

/* Accent text for links and interactive elements */
.frost-link {
  color: var(--frost-accent-blue);
  text-decoration: none;
  font-weight: 500;
  transition: color 0.2s ease;
}

.frost-link:hover {
  color: var(--frost-accent-cyan);
}

/* Monospace for data and code */
.frost-mono {
  font-family: 'JetBrains Mono', 'Space Grotesk', monospace;
  font-size: 0.9rem;
  font-weight: 400;
  color: var(--frost-accent-cyan);
  letter-spacing: 0.02em;
}
```

---

## Key Design Elements and Motifs

### Frosted Glass Panel

The defining element of the aesthetic -- a translucent surface that partially reveals what lies behind:

- **Semi-transparent background** using rgba white values (0.08-0.25 alpha depending on depth)
- **Backdrop blur** via `backdrop-filter: blur(16-24px)` softening everything behind the panel
- **Saturation boost** via `backdrop-filter: saturate(1.2-1.8)` keeping colors vibrant through the frost
- **Thin luminous border** -- 1px solid with `rgba(255,255,255,0.15-0.25)` catching virtual light
- **Generous border-radius** -- 16-24px creating soft, rounded panel shapes
- **Inner glow gradient** -- a faint top-to-bottom gradient within the panel (lighter at top) simulating light hitting the glass surface
- **No hard shadows** -- only diffused, wide-spread box-shadows at low opacity

### Layered Depth System

Multiple translucent layers create a convincing 3D space:

- **Layer 0 (Background)** -- vibrant gradient mesh, no blur, full color saturation
- **Layer 1 (Deep frost)** -- lowest opacity (0.06-0.10), heaviest blur (32-40px), large ambient panels
- **Layer 2 (Mid frost)** -- medium opacity (0.12-0.18), medium blur (16-24px), content containers
- **Layer 3 (Surface frost)** -- higher opacity (0.18-0.25), lighter blur (8-16px), interactive cards and elements
- **Layer 4 (Raised)** -- highest opacity (0.25-0.35), minimal blur (4-8px), tooltips, dropdowns, modals
- Each layer casts a **wider, softer shadow** than the one above it

### Gradient Background

The energy source beneath all frost layers:

- **Multi-stop radial and linear gradients** using deep, saturated colors (navy, purple, magenta, deep teal)
- **Gradient mesh simulation** -- multiple overlapping radial gradients at different positions creating organic color fields
- **Slow animation** -- optional subtle gradient shift (15-30s cycle) keeping the background alive
- **No repeating patterns** -- backgrounds should feel like a single continuous color field, not tiled

### Diffused Shadows

Shadows in Frosted Touch are atmospheric, not structural:

- **Large spread, low opacity** -- `box-shadow: 0 8px 32px rgba(10, 10, 50, 0.12)` typical for cards
- **Multiple shadow layers** -- 2-3 box-shadows stacked at different spreads for realistic depth
- **No sharp offset shadows** -- shadows spread evenly or slightly downward, never with hard directional offset
- **Color-tinted shadows** -- shadows may carry a hint of the background gradient color (blue-purple tint)
- **Inner shadows avoided** -- frosted glass does not cast inward shadows; depth is conveyed by background blur

### Hover and Interaction States

Interactions feel like moving a panel closer to the viewer:

- **Opacity increase on hover** -- surface background shifts from 0.15 to 0.22, brightening the frost
- **Blur reduction on hover** -- optional slight blur decrease to make content beneath sharper, suggesting the panel moved closer
- **Border brightening** -- border alpha increases from 0.15 to 0.30 on hover
- **Shadow intensification** -- shadow spread and opacity increase subtly
- **Smooth transitions** -- all hover changes animate over 0.25-0.35s with ease-out timing
- **Glow effect on focus** -- focused elements gain a subtle colored glow (accent blue at 0.15-0.25 opacity)

### Dividers and Separators

- **1px lines** using `rgba(255,255,255,0.08-0.12)` -- barely visible, more felt than seen
- **Gradient dividers** -- horizontal rules that fade from transparent to white to transparent
- **Spacing over lines** -- generous padding and margin used more often than visible dividers

---

## Layout Principles

- **Floating panel composition** -- panels appear to hover in space over the gradient background, not anchored to edges or to each other
- **Generous whitespace** -- 24-48px gaps between panels; the gradient background is a first-class design element, not wasted space
- **Consistent border-radius** -- all rectangular elements share the same radius family (8, 16, 24px) creating visual cohesion
- **Asymmetric depth** -- not all panels sit at the same depth; vary opacity and blur to create a landscape of foreground and background elements
- **Full-bleed gradient background** -- the vibrant gradient extends edge to edge, with frosted panels floating in front
- **Content density is low** -- each frosted panel contains a focused amount of content; dense data is broken across multiple panels
- **Max-width containers** -- content areas limited to 1200-1400px to maintain comfortable reading widths behind frost
- **Stacking order matters** -- overlapping panels should have clearly different opacity/blur levels so the layering reads correctly
- **Subtle grid alignment** -- panels align to an invisible grid, but gaps and slight positional offsets prevent rigidity

### Modern Web Adaptation

- Use **CSS Grid or Flexbox** with generous gap values (24-40px) for panel layouts
- **Frosted panels as cards** -- each content section wrapped in a glass panel with consistent radius and border
- **Sticky frosted navigation** -- a top navbar with backdrop-filter, becoming more opaque on scroll
- **Modal dialogs as raised frost** -- modals use the highest frost opacity and minimal blur for foreground presence
- **Sidebar panels at a different depth** than main content, creating spatial hierarchy
- **Dark mode default** -- the aesthetic requires a dark, vibrant background; light mode fundamentally changes the character
- **Responsive adaptation** -- on smaller screens, reduce the number of visible depth layers and increase panel opacity for readability

---

## CSS/Design Techniques

### Core Frost Panel

```css
/* The fundamental frosted glass panel */
.frost-panel {
  background: var(--frost-surface-light);
  backdrop-filter: blur(16px) saturate(1.4);
  -webkit-backdrop-filter: blur(16px) saturate(1.4);
  border: 1px solid var(--frost-border);
  border-radius: var(--frost-radius-lg);
  box-shadow:
    0 8px 32px var(--frost-shadow-diffused),
    0 2px 8px rgba(0, 0, 0, 0.08);
  padding: 2rem;
}

/* Inner light gradient simulating light on glass */
.frost-panel::before {
  content: '';
  position: absolute;
  inset: 0;
  border-radius: inherit;
  background: linear-gradient(
    135deg,
    rgba(255, 255, 255, 0.08) 0%,
    rgba(255, 255, 255, 0.02) 50%,
    transparent 100%
  );
  pointer-events: none;
}
```

### Depth Layers

```css
/* Layer 1 -- deepest frost, ambient background panels */
.frost-layer-deep {
  background: var(--frost-surface-deep);
  backdrop-filter: blur(40px) saturate(1.2);
  -webkit-backdrop-filter: blur(40px) saturate(1.2);
  border: 1px solid rgba(255, 255, 255, 0.06);
  border-radius: var(--frost-radius-lg);
  box-shadow: 0 16px 64px rgba(10, 10, 50, 0.10);
}

/* Layer 2 -- mid-depth content containers */
.frost-layer-mid {
  background: var(--frost-surface-mid);
  backdrop-filter: blur(20px) saturate(1.4);
  -webkit-backdrop-filter: blur(20px) saturate(1.4);
  border: 1px solid rgba(255, 255, 255, 0.12);
  border-radius: var(--frost-radius-lg);
  box-shadow: 0 8px 32px rgba(10, 10, 50, 0.12);
}

/* Layer 3 -- surface-level interactive cards */
.frost-layer-surface {
  background: var(--frost-surface-light);
  backdrop-filter: blur(16px) saturate(1.6);
  -webkit-backdrop-filter: blur(16px) saturate(1.6);
  border: 1px solid var(--frost-border);
  border-radius: var(--frost-radius-md);
  box-shadow:
    0 4px 16px rgba(10, 10, 50, 0.15),
    0 1px 4px rgba(0, 0, 0, 0.08);
}

/* Layer 4 -- raised elements (tooltips, dropdowns, modals) */
.frost-layer-raised {
  background: var(--frost-surface-raised);
  backdrop-filter: blur(8px) saturate(1.8);
  -webkit-backdrop-filter: blur(8px) saturate(1.8);
  border: 1px solid var(--frost-border-bright);
  border-radius: var(--frost-radius-md);
  box-shadow:
    0 12px 40px rgba(10, 10, 50, 0.20),
    0 4px 12px rgba(0, 0, 0, 0.10);
}
```

### Gradient Background

```css
/* Vibrant gradient mesh background */
.frost-background {
  position: fixed;
  inset: 0;
  background: linear-gradient(
    135deg,
    var(--frost-bg-a) 0%,
    var(--frost-bg-b) 50%,
    var(--frost-bg-c) 100%
  );
  z-index: -2;
}

/* Overlay radial gradients for mesh effect */
.frost-background::before {
  content: '';
  position: absolute;
  inset: 0;
  background:
    radial-gradient(
      ellipse 80% 60% at 20% 30%,
      rgba(96, 165, 250, 0.25) 0%,
      transparent 70%
    ),
    radial-gradient(
      ellipse 60% 80% at 80% 70%,
      rgba(167, 139, 250, 0.20) 0%,
      transparent 70%
    ),
    radial-gradient(
      ellipse 70% 50% at 50% 90%,
      rgba(244, 114, 182, 0.15) 0%,
      transparent 70%
    );
  z-index: -1;
}

/* Optional slow gradient animation */
@keyframes frost-gradient-shift {
  0% { background-position: 0% 50%; }
  50% { background-position: 100% 50%; }
  100% { background-position: 0% 50%; }
}

.frost-background--animated {
  background-size: 200% 200%;
  animation: frost-gradient-shift 20s ease-in-out infinite;
}
```

### Frosted Navigation Bar

```css
/* Sticky frosted navigation */
.frost-nav {
  position: sticky;
  top: 0;
  z-index: 100;
  background: rgba(255, 255, 255, 0.08);
  backdrop-filter: blur(24px) saturate(1.6);
  -webkit-backdrop-filter: blur(24px) saturate(1.6);
  border-bottom: 1px solid var(--frost-border-subtle);
  padding: 0.75rem 2rem;
  display: flex;
  align-items: center;
  justify-content: space-between;
  transition: background 0.3s ease;
}

/* Increase opacity on scroll for readability */
.frost-nav--scrolled {
  background: rgba(255, 255, 255, 0.15);
  box-shadow: 0 4px 24px var(--frost-shadow-diffused);
}

.frost-nav a {
  color: var(--frost-text-secondary);
  text-decoration: none;
  font-family: 'Inter', sans-serif;
  font-weight: 500;
  font-size: 0.9rem;
  padding: 0.5rem 1rem;
  border-radius: var(--frost-radius-sm);
  transition: color 0.2s ease, background 0.2s ease;
}

.frost-nav a:hover {
  color: var(--frost-text-primary);
  background: rgba(255, 255, 255, 0.08);
}

.frost-nav a.active {
  color: var(--frost-accent-blue);
  background: rgba(96, 165, 250, 0.10);
}
```

### Frost Card with Hover

```css
/* Interactive frosted card with hover elevation */
.frost-card {
  position: relative;
  background: var(--frost-surface-light);
  backdrop-filter: blur(16px) saturate(1.4);
  -webkit-backdrop-filter: blur(16px) saturate(1.4);
  border: 1px solid var(--frost-border);
  border-radius: var(--frost-radius-lg);
  padding: 2rem;
  box-shadow:
    0 4px 16px var(--frost-shadow-diffused),
    0 1px 4px rgba(0, 0, 0, 0.06);
  transition:
    background 0.3s ease,
    border-color 0.3s ease,
    box-shadow 0.3s ease,
    transform 0.3s ease;
  overflow: hidden;
}

/* Light refraction gradient overlay */
.frost-card::before {
  content: '';
  position: absolute;
  inset: 0;
  border-radius: inherit;
  background: linear-gradient(
    135deg,
    rgba(255, 255, 255, 0.10) 0%,
    rgba(255, 255, 255, 0.03) 40%,
    transparent 70%
  );
  pointer-events: none;
  transition: opacity 0.3s ease;
}

/* Hover state -- panel moves closer to viewer */
.frost-card:hover {
  background: var(--frost-surface-raised);
  border-color: var(--frost-border-bright);
  box-shadow:
    0 8px 32px rgba(10, 10, 50, 0.20),
    0 2px 8px rgba(0, 0, 0, 0.10),
    0 0 0 1px rgba(255, 255, 255, 0.05);
  transform: translateY(-2px);
}

.frost-card:hover::before {
  opacity: 1.4;
}
```

### Frost Button

```css
/* Primary frosted button */
.frost-button {
  display: inline-flex;
  align-items: center;
  justify-content: center;
  gap: 0.5rem;
  padding: 0.65rem 1.6rem;
  background: rgba(96, 165, 250, 0.18);
  backdrop-filter: blur(12px) saturate(1.3);
  -webkit-backdrop-filter: blur(12px) saturate(1.3);
  border: 1px solid rgba(96, 165, 250, 0.30);
  border-radius: var(--frost-radius-sm);
  color: var(--frost-text-primary);
  font-family: 'Inter', sans-serif;
  font-size: 0.9rem;
  font-weight: 500;
  letter-spacing: 0.01em;
  cursor: pointer;
  transition:
    background 0.25s ease,
    border-color 0.25s ease,
    box-shadow 0.25s ease;
}

.frost-button:hover {
  background: rgba(96, 165, 250, 0.28);
  border-color: rgba(96, 165, 250, 0.45);
  box-shadow:
    0 4px 16px rgba(96, 165, 250, 0.15),
    0 0 0 1px rgba(96, 165, 250, 0.08);
}

.frost-button:active {
  background: rgba(96, 165, 250, 0.35);
  transform: scale(0.98);
  transition-duration: 0.1s;
}

/* Secondary / ghost button */
.frost-button--secondary {
  background: var(--frost-surface-mid);
  border-color: var(--frost-border);
  color: var(--frost-text-secondary);
}

.frost-button--secondary:hover {
  background: var(--frost-surface-light);
  border-color: var(--frost-border-bright);
  color: var(--frost-text-primary);
  box-shadow: 0 4px 16px var(--frost-shadow-diffused);
}
```

### Frost Input / Form Fields

```css
/* Frosted input field */
.frost-input {
  width: 100%;
  padding: 0.7rem 1rem;
  background: rgba(255, 255, 255, 0.06);
  backdrop-filter: blur(8px);
  -webkit-backdrop-filter: blur(8px);
  border: 1px solid rgba(255, 255, 255, 0.10);
  border-radius: var(--frost-radius-sm);
  color: var(--frost-text-primary);
  font-family: 'Inter', sans-serif;
  font-size: 0.95rem;
  outline: none;
  transition:
    border-color 0.25s ease,
    box-shadow 0.25s ease,
    background 0.25s ease;
}

.frost-input::placeholder {
  color: var(--frost-text-muted);
}

.frost-input:focus {
  border-color: rgba(96, 165, 250, 0.50);
  background: rgba(255, 255, 255, 0.10);
  box-shadow:
    0 0 0 3px rgba(96, 165, 250, 0.12),
    0 2px 8px rgba(10, 10, 50, 0.10);
}
```

### Frosted Divider

```css
/* Gradient divider that fades at edges */
.frost-divider {
  border: none;
  height: 1px;
  background: linear-gradient(
    to right,
    transparent 0%,
    rgba(255, 255, 255, 0.12) 20%,
    rgba(255, 255, 255, 0.12) 80%,
    transparent 100%
  );
  margin: 2rem 0;
}

/* Accented divider with glow */
.frost-divider--accent {
  height: 1px;
  background: linear-gradient(
    to right,
    transparent 0%,
    rgba(96, 165, 250, 0.30) 30%,
    rgba(167, 139, 250, 0.30) 70%,
    transparent 100%
  );
  box-shadow: 0 0 8px rgba(96, 165, 250, 0.08);
}
```

### Frosted Modal / Dialog

```css
/* Modal overlay with blur */
.frost-modal-overlay {
  position: fixed;
  inset: 0;
  background: rgba(10, 10, 30, 0.50);
  backdrop-filter: blur(6px);
  -webkit-backdrop-filter: blur(6px);
  display: flex;
  align-items: center;
  justify-content: center;
  z-index: 1000;
}

/* Modal panel -- raised frost */
.frost-modal {
  background: var(--frost-surface-raised);
  backdrop-filter: blur(24px) saturate(1.8);
  -webkit-backdrop-filter: blur(24px) saturate(1.8);
  border: 1px solid var(--frost-border-bright);
  border-radius: var(--frost-radius-lg);
  padding: 2.5rem;
  max-width: 520px;
  width: 90%;
  box-shadow:
    0 24px 80px rgba(10, 10, 40, 0.35),
    0 8px 24px rgba(0, 0, 0, 0.15),
    inset 0 1px 0 rgba(255, 255, 255, 0.10);
}
```

### Frosted Tag / Badge

```css
/* Small frosted tag / badge */
.frost-tag {
  display: inline-flex;
  align-items: center;
  padding: 0.25rem 0.75rem;
  background: rgba(167, 139, 250, 0.15);
  border: 1px solid rgba(167, 139, 250, 0.25);
  border-radius: var(--frost-radius-pill);
  font-family: 'Space Grotesk', 'Inter', sans-serif;
  font-size: 0.75rem;
  font-weight: 500;
  color: var(--frost-accent-purple);
  letter-spacing: 0.02em;
}

.frost-tag--blue {
  background: rgba(96, 165, 250, 0.15);
  border-color: rgba(96, 165, 250, 0.25);
  color: var(--frost-accent-blue);
}

.frost-tag--cyan {
  background: rgba(103, 232, 249, 0.12);
  border-color: rgba(103, 232, 249, 0.25);
  color: var(--frost-accent-cyan);
}
```

---

## Materials and Textures (Visual Metaphors for Web)

| Physical / Architectural Reference | Web Equivalent |
|------------------------------------|----------------|
| Frosted architectural glass panels | `backdrop-filter: blur(16-24px)` with semi-transparent rgba white background |
| Layered glass walls at different depths | Multiple overlapping elements with varying blur intensity and opacity |
| Light falling across a glass surface | `linear-gradient(135deg, rgba(255,255,255,0.08), transparent)` overlay on panels |
| Diffused light through frosted glass | `backdrop-filter: saturate(1.2-1.8)` boosting color vibrancy through the blur |
| Soft shadows cast by floating glass | Large-spread, low-opacity `box-shadow` (20-40px spread, 0.08-0.15 alpha) |
| Thin luminous edge of glass catching light | `border: 1px solid rgba(255,255,255,0.15-0.25)` |
| Gradient light refracting through glass edges | Border-top or border-left with slightly higher opacity than other borders |
| Vibrant colored wall behind glass partitions | Multi-stop CSS `linear-gradient` and `radial-gradient` backgrounds |
| Glass with varying thickness / frost density | Different `blur()` and background opacity values for panels at different depths |
| Rounded glass corners (no sharp edges) | `border-radius: 16-24px` on all panel elements |
| Anti-reflective glass coating | Smooth CSS transitions on hover (0.25-0.35s ease-out) preventing harsh visual jumps |
| Stacked glass shelves | `z-index` layering with decreasing blur and increasing opacity for closer layers |

---

## Imagery and Visual Content Guidelines

When creating or sourcing imagery for a Frosted Touch styled site:

- **Favor abstract gradient imagery** -- soft color fields, blurred light photography, and bokeh effects complement the frosted surfaces
- **Avoid busy, high-detail photographs** -- detailed images behind frost panels create visual noise; use images with large color blocks and soft gradients
- **Icon style should be outlined or semi-filled** -- thin-line icons at 1.5-2px stroke weight, using white or accent colors, matching the lightness of the frost borders
- **Illustrations should be minimal and geometric** -- simple shapes with translucent fills and soft gradients, not complex detailed drawings
- **Avatar images work well inside circular frost containers** -- circular crop with a frosted ring border creates a polished look
- **Charts and data visualizations** should use semi-transparent fills with visible stroke lines, matching the translucent panel language
- **Background images (when used)** should be heavily blurred (30-50px) and desaturated slightly before being placed behind frost layers
- **No hard-edged or pixel-art imagery** -- all visual content should match the soft, diffused quality of the frost panels
- **Hero sections** can use large, vibrant gradient images that become the color source for the entire page's frost layers
- **Maintain consistent translucency** -- any embedded media (images, video) should have slightly rounded corners and subtle frosted borders to integrate with the panel system

---

## Related Aesthetics

| Aesthetic | Relationship to Frosted Touch |
|-----------|-------------------------------|
| **Glassmorphism** | Direct predecessor; Frosted Touch refines and deepens glassmorphism with multi-layer depth, better performance patterns, and more sophisticated color handling |
| **Neumorphism** | Shares the soft-shadow philosophy but differs fundamentally -- neumorphism uses extruded surfaces on solid backgrounds while Frosted Touch uses translucent surfaces over vibrant backgrounds |
| **Aurora Gradient** | Shares vibrant gradient backgrounds; Aurora Gradient focuses on the gradient itself as the primary visual element, while Frosted Touch uses gradients as the foundation beneath frost layers |
| **Dark Mode Neon** | Both work on dark backgrounds, but Dark Mode Neon uses high-contrast glowing elements while Frosted Touch uses soft, diffused translucency |
| **Cyberminimalism** | Shares the minimal, clean approach to UI but Cyberminimalism uses flat surfaces and sharp type, lacking the frosted depth and warmth |
| **Claymorphism** | Both create soft, rounded, elevated surfaces, but Claymorphism simulates opaque clay/plastic while Frosted Touch simulates transparent glass |

---

## Implementation Notes

- **`backdrop-filter` browser support** is critical -- the entire aesthetic depends on it. As of 2026, support is strong across modern browsers, but always provide a solid-color fallback (`background: rgba(30, 30, 60, 0.85)`) for environments where `backdrop-filter` is unavailable or disabled. Use `@supports (backdrop-filter: blur(1px))` to detect support.
- **Performance matters** -- `backdrop-filter: blur()` is GPU-intensive, especially with large blur radii and multiple overlapping layers. Limit frosted panels to 3-4 visible at any time. Avoid animating blur values. Use `will-change: backdrop-filter` sparingly and only on elements that will transition.
- **Stacking context awareness** -- `backdrop-filter` creates a new stacking context. Nested frost panels may not blur content outside their stacking context parent. Test depth layering carefully.
- **Contrast and accessibility** -- translucent text backgrounds make WCAG contrast ratios harder to guarantee. Use `text-shadow` for legibility, increase panel opacity in critical reading areas, and test with varying background gradient positions to ensure text remains readable in all states.
- **The gradient background is not optional** -- frosted panels over a solid dark background look like faded gray boxes, not glass. The vibrant gradient is what gives the frost its visual purpose and beauty. Always provide a rich, colorful background.
- **Border subtlety is key** -- borders that are too bright (above 0.35 alpha) look like outlines, not light catching glass edges. Keep border opacity in the 0.12-0.25 range for authenticity.
- **Avoid combining with patterns or textures** -- the Frosted Touch aesthetic is anti-texture. Adding noise, grain, or repeating patterns to frost panels undermines the clean, glassy quality. All visual richness comes from transparency, blur, and color alone.
- **Responsive considerations** -- on low-resolution or mobile screens, reduce blur values and increase background opacity slightly to maintain readability. A panel that looks elegantly translucent on a retina desktop display may look muddy on a low-density mobile screen.
- **Dark mode only** -- Frosted Touch is inherently a dark-mode aesthetic. Attempting to adapt it to a light background fundamentally changes the visual language into something closer to standard glassmorphism. If a light mode is required, significantly increase panel border contrast and use colored tints instead of white transparency.

---

## Quick-Start: Minimal Frosted Touch Page Template

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Frosted Touch Page</title>
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700&family=Plus+Jakarta+Sans:wght@500;600;700;800&family=Space+Grotesk:wght@400;500&family=JetBrains+Mono:wght@400&display=swap" rel="stylesheet">
  <style>
    :root {
      /* Background gradient */
      --frost-bg-a: #1a1a4e;
      --frost-bg-b: #4a1a6b;
      --frost-bg-c: #6b1a4a;

      /* Frost surfaces */
      --frost-surface-deep: rgba(255, 255, 255, 0.08);
      --frost-surface-mid: rgba(255, 255, 255, 0.12);
      --frost-surface-light: rgba(255, 255, 255, 0.18);
      --frost-surface-raised: rgba(255, 255, 255, 0.25);

      /* Borders */
      --frost-border: rgba(255, 255, 255, 0.18);
      --frost-border-bright: rgba(255, 255, 255, 0.30);
      --frost-border-subtle: rgba(255, 255, 255, 0.10);

      /* Text */
      --frost-text-primary: #F8FAFC;
      --frost-text-secondary: rgba(248, 250, 252, 0.70);
      --frost-text-muted: rgba(248, 250, 252, 0.45);

      /* Accents */
      --frost-accent-blue: #60A5FA;
      --frost-accent-purple: #A78BFA;
      --frost-accent-cyan: #67E8F9;
      --frost-accent-pink: #F472B6;

      /* Shadows */
      --frost-shadow: rgba(15, 10, 40, 0.25);
      --frost-shadow-diffused: rgba(10, 10, 50, 0.15);

      /* Radius */
      --frost-radius-sm: 8px;
      --frost-radius-md: 16px;
      --frost-radius-lg: 24px;
      --frost-radius-pill: 9999px;
    }

    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body {
      font-family: 'Inter', system-ui, -apple-system, sans-serif;
      font-size: 16px;
      line-height: 1.7;
      color: var(--frost-text-primary);
      min-height: 100vh;
      overflow-x: hidden;
      -webkit-font-smoothing: antialiased;
      -moz-osx-font-smoothing: grayscale;
    }

    /* ---- Gradient Background ---- */
    .frost-bg {
      position: fixed;
      inset: 0;
      background: linear-gradient(
        135deg,
        var(--frost-bg-a) 0%,
        var(--frost-bg-b) 50%,
        var(--frost-bg-c) 100%
      );
      z-index: -2;
    }

    .frost-bg::before {
      content: '';
      position: absolute;
      inset: 0;
      background:
        radial-gradient(
          ellipse 80% 50% at 15% 25%,
          rgba(96, 165, 250, 0.22) 0%,
          transparent 70%
        ),
        radial-gradient(
          ellipse 60% 70% at 85% 65%,
          rgba(167, 139, 250, 0.18) 0%,
          transparent 70%
        ),
        radial-gradient(
          ellipse 70% 40% at 50% 95%,
          rgba(244, 114, 182, 0.14) 0%,
          transparent 60%
        );
    }

    /* ---- Navigation ---- */
    .frost-nav {
      position: sticky;
      top: 0;
      z-index: 100;
      background: rgba(255, 255, 255, 0.07);
      backdrop-filter: blur(24px) saturate(1.5);
      -webkit-backdrop-filter: blur(24px) saturate(1.5);
      border-bottom: 1px solid var(--frost-border-subtle);
      padding: 0.8rem 2rem;
      display: flex;
      align-items: center;
      justify-content: space-between;
    }

    .frost-nav-brand {
      font-family: 'Plus Jakarta Sans', sans-serif;
      font-weight: 700;
      font-size: 1.2rem;
      color: var(--frost-text-primary);
      text-decoration: none;
    }

    .frost-nav-links {
      display: flex;
      gap: 0.25rem;
      list-style: none;
    }

    .frost-nav-links a {
      color: var(--frost-text-secondary);
      text-decoration: none;
      font-weight: 500;
      font-size: 0.9rem;
      padding: 0.4rem 0.9rem;
      border-radius: var(--frost-radius-sm);
      transition: color 0.2s ease, background 0.2s ease;
    }

    .frost-nav-links a:hover {
      color: var(--frost-text-primary);
      background: rgba(255, 255, 255, 0.08);
    }

    /* ---- Page Container ---- */
    .frost-page {
      max-width: 1200px;
      margin: 0 auto;
      padding: 3rem 2rem 4rem;
    }

    /* ---- Hero Section (Deep Layer) ---- */
    .frost-hero {
      position: relative;
      background: var(--frost-surface-deep);
      backdrop-filter: blur(40px) saturate(1.2);
      -webkit-backdrop-filter: blur(40px) saturate(1.2);
      border: 1px solid rgba(255, 255, 255, 0.06);
      border-radius: var(--frost-radius-lg);
      padding: 4rem 3rem;
      margin-bottom: 2.5rem;
      box-shadow: 0 16px 64px rgba(10, 10, 50, 0.12);
      text-align: center;
      overflow: hidden;
    }

    .frost-hero::before {
      content: '';
      position: absolute;
      inset: 0;
      border-radius: inherit;
      background: linear-gradient(
        135deg,
        rgba(255, 255, 255, 0.06) 0%,
        transparent 50%
      );
      pointer-events: none;
    }

    .frost-hero > * {
      position: relative;
      z-index: 1;
    }

    .frost-hero h1 {
      font-family: 'Plus Jakarta Sans', sans-serif;
      font-size: clamp(2rem, 5vw, 3.5rem);
      font-weight: 800;
      color: #FFFFFF;
      letter-spacing: -0.02em;
      line-height: 1.2;
      margin-bottom: 1rem;
      text-shadow: 0 2px 4px rgba(0, 0, 0, 0.12);
    }

    .frost-hero p {
      font-size: 1.15rem;
      color: var(--frost-text-secondary);
      max-width: 600px;
      margin: 0 auto 2rem;
      line-height: 1.7;
    }

    .frost-hero-tags {
      display: flex;
      gap: 0.5rem;
      justify-content: center;
      flex-wrap: wrap;
    }

    /* ---- Tags ---- */
    .frost-tag {
      display: inline-flex;
      align-items: center;
      padding: 0.3rem 0.85rem;
      background: rgba(167, 139, 250, 0.14);
      border: 1px solid rgba(167, 139, 250, 0.25);
      border-radius: var(--frost-radius-pill);
      font-family: 'Space Grotesk', sans-serif;
      font-size: 0.78rem;
      font-weight: 500;
      color: var(--frost-accent-purple);
      letter-spacing: 0.02em;
    }

    .frost-tag--blue {
      background: rgba(96, 165, 250, 0.14);
      border-color: rgba(96, 165, 250, 0.25);
      color: var(--frost-accent-blue);
    }

    .frost-tag--cyan {
      background: rgba(103, 232, 249, 0.10);
      border-color: rgba(103, 232, 249, 0.22);
      color: var(--frost-accent-cyan);
    }

    /* ---- Card Grid ---- */
    .frost-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(320px, 1fr));
      gap: 1.5rem;
      margin-bottom: 2.5rem;
    }

    /* ---- Cards (Surface Layer) ---- */
    .frost-card {
      position: relative;
      background: var(--frost-surface-light);
      backdrop-filter: blur(16px) saturate(1.5);
      -webkit-backdrop-filter: blur(16px) saturate(1.5);
      border: 1px solid var(--frost-border);
      border-radius: var(--frost-radius-lg);
      padding: 2rem;
      box-shadow:
        0 4px 16px var(--frost-shadow-diffused),
        0 1px 4px rgba(0, 0, 0, 0.06);
      transition:
        background 0.3s ease,
        border-color 0.3s ease,
        box-shadow 0.3s ease,
        transform 0.3s ease;
      overflow: hidden;
    }

    .frost-card::before {
      content: '';
      position: absolute;
      inset: 0;
      border-radius: inherit;
      background: linear-gradient(
        135deg,
        rgba(255, 255, 255, 0.08) 0%,
        rgba(255, 255, 255, 0.02) 40%,
        transparent 70%
      );
      pointer-events: none;
      transition: opacity 0.3s ease;
    }

    .frost-card:hover {
      background: var(--frost-surface-raised);
      border-color: var(--frost-border-bright);
      box-shadow:
        0 8px 32px rgba(10, 10, 50, 0.20),
        0 2px 8px rgba(0, 0, 0, 0.10);
      transform: translateY(-2px);
    }

    .frost-card > * {
      position: relative;
      z-index: 1;
    }

    .frost-card h2 {
      font-family: 'Plus Jakarta Sans', sans-serif;
      font-size: 1.3rem;
      font-weight: 700;
      color: var(--frost-text-primary);
      margin-bottom: 0.75rem;
      letter-spacing: -0.01em;
    }

    .frost-card p {
      color: var(--frost-text-secondary);
      font-size: 0.95rem;
      line-height: 1.7;
      margin-bottom: 1rem;
    }

    .frost-card .frost-mono {
      font-family: 'JetBrains Mono', monospace;
      font-size: 0.82rem;
      color: var(--frost-accent-cyan);
      letter-spacing: 0.02em;
    }

    /* ---- Content Panel (Mid Layer) ---- */
    .frost-content-panel {
      position: relative;
      background: var(--frost-surface-mid);
      backdrop-filter: blur(20px) saturate(1.4);
      -webkit-backdrop-filter: blur(20px) saturate(1.4);
      border: 1px solid rgba(255, 255, 255, 0.12);
      border-radius: var(--frost-radius-lg);
      padding: 2.5rem;
      box-shadow: 0 8px 32px rgba(10, 10, 50, 0.12);
      margin-bottom: 2.5rem;
      overflow: hidden;
    }

    .frost-content-panel::before {
      content: '';
      position: absolute;
      inset: 0;
      border-radius: inherit;
      background: linear-gradient(
        180deg,
        rgba(255, 255, 255, 0.05) 0%,
        transparent 40%
      );
      pointer-events: none;
    }

    .frost-content-panel > * {
      position: relative;
      z-index: 1;
    }

    .frost-content-panel h2 {
      font-family: 'Plus Jakarta Sans', sans-serif;
      font-size: 1.5rem;
      font-weight: 700;
      color: var(--frost-text-primary);
      margin-bottom: 1rem;
    }

    .frost-content-panel p {
      color: var(--frost-text-secondary);
      margin-bottom: 1rem;
    }

    /* ---- Buttons ---- */
    .frost-button {
      display: inline-flex;
      align-items: center;
      gap: 0.5rem;
      padding: 0.65rem 1.5rem;
      background: rgba(96, 165, 250, 0.18);
      backdrop-filter: blur(12px);
      -webkit-backdrop-filter: blur(12px);
      border: 1px solid rgba(96, 165, 250, 0.30);
      border-radius: var(--frost-radius-sm);
      color: var(--frost-text-primary);
      font-family: 'Inter', sans-serif;
      font-size: 0.9rem;
      font-weight: 500;
      cursor: pointer;
      text-decoration: none;
      transition:
        background 0.25s ease,
        border-color 0.25s ease,
        box-shadow 0.25s ease;
    }

    .frost-button:hover {
      background: rgba(96, 165, 250, 0.28);
      border-color: rgba(96, 165, 250, 0.45);
      box-shadow: 0 4px 16px rgba(96, 165, 250, 0.15);
    }

    .frost-button--secondary {
      background: var(--frost-surface-mid);
      border-color: var(--frost-border);
      color: var(--frost-text-secondary);
    }

    .frost-button--secondary:hover {
      background: var(--frost-surface-light);
      border-color: var(--frost-border-bright);
      color: var(--frost-text-primary);
    }

    /* ---- Divider ---- */
    .frost-divider {
      border: none;
      height: 1px;
      background: linear-gradient(
        to right,
        transparent 0%,
        rgba(255, 255, 255, 0.10) 20%,
        rgba(255, 255, 255, 0.10) 80%,
        transparent 100%
      );
      margin: 2rem 0;
    }

    /* ---- Stats Row ---- */
    .frost-stats {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(160px, 1fr));
      gap: 1rem;
      margin-bottom: 2.5rem;
    }

    .frost-stat {
      position: relative;
      background: var(--frost-surface-mid);
      backdrop-filter: blur(20px) saturate(1.3);
      -webkit-backdrop-filter: blur(20px) saturate(1.3);
      border: 1px solid rgba(255, 255, 255, 0.10);
      border-radius: var(--frost-radius-md);
      padding: 1.5rem;
      text-align: center;
      overflow: hidden;
    }

    .frost-stat::before {
      content: '';
      position: absolute;
      inset: 0;
      border-radius: inherit;
      background: linear-gradient(
        180deg,
        rgba(255, 255, 255, 0.04) 0%,
        transparent 50%
      );
      pointer-events: none;
    }

    .frost-stat > * {
      position: relative;
      z-index: 1;
    }

    .frost-stat-value {
      font-family: 'Plus Jakarta Sans', sans-serif;
      font-size: 2rem;
      font-weight: 800;
      color: var(--frost-text-primary);
      line-height: 1.2;
      margin-bottom: 0.25rem;
    }

    .frost-stat-label {
      font-family: 'Space Grotesk', sans-serif;
      font-size: 0.75rem;
      font-weight: 500;
      color: var(--frost-text-muted);
      text-transform: uppercase;
      letter-spacing: 0.08em;
    }

    /* ---- Footer ---- */
    .frost-footer {
      text-align: center;
      padding: 2rem;
      color: var(--frost-text-muted);
      font-size: 0.85rem;
    }

    /* ---- Utility ---- */
    .text-accent-blue { color: var(--frost-accent-blue); }
    .text-accent-purple { color: var(--frost-accent-purple); }
    .text-accent-cyan { color: var(--frost-accent-cyan); }

    /* ---- Responsive ---- */
    @media (max-width: 768px) {
      .frost-page {
        padding: 1.5rem 1rem 3rem;
      }

      .frost-hero {
        padding: 2.5rem 1.5rem;
      }

      .frost-grid {
        grid-template-columns: 1fr;
      }

      .frost-nav {
        padding: 0.7rem 1rem;
      }

      .frost-nav-links {
        gap: 0;
      }

      .frost-nav-links a {
        padding: 0.4rem 0.6rem;
        font-size: 0.82rem;
      }

      .frost-content-panel {
        padding: 1.5rem;
      }
    }

    /* ---- Fallback for browsers without backdrop-filter ---- */
    @supports not (backdrop-filter: blur(1px)) {
      .frost-hero,
      .frost-card,
      .frost-content-panel,
      .frost-nav,
      .frost-stat {
        background: rgba(30, 25, 60, 0.88);
      }
    }
  </style>
</head>
<body>
  <!-- Gradient background -->
  <div class="frost-bg"></div>

  <!-- Navigation -->
  <nav class="frost-nav">
    <a href="#" class="frost-nav-brand">Frosted Touch</a>
    <ul class="frost-nav-links">
      <li><a href="#">Overview</a></li>
      <li><a href="#">Features</a></li>
      <li><a href="#">Layers</a></li>
      <li><a href="#">About</a></li>
    </ul>
  </nav>

  <div class="frost-page">
    <!-- Hero (Deep Layer) -->
    <section class="frost-hero">
      <h1>Through the Frost</h1>
      <p>Translucent layers reveal the color beneath. Every surface breathes, every boundary is soft, and depth emerges from light and glass alone.</p>
      <div class="frost-hero-tags">
        <span class="frost-tag frost-tag--blue">backdrop-filter</span>
        <span class="frost-tag">translucent layers</span>
        <span class="frost-tag frost-tag--cyan">diffused shadows</span>
      </div>
    </section>

    <!-- Stats Row (Mid Layer) -->
    <div class="frost-stats">
      <div class="frost-stat">
        <div class="frost-stat-value text-accent-blue">4</div>
        <div class="frost-stat-label">Depth Layers</div>
      </div>
      <div class="frost-stat">
        <div class="frost-stat-value text-accent-purple">24px</div>
        <div class="frost-stat-label">Border Radius</div>
      </div>
      <div class="frost-stat">
        <div class="frost-stat-value text-accent-cyan">16px</div>
        <div class="frost-stat-label">Blur Radius</div>
      </div>
      <div class="frost-stat">
        <div class="frost-stat-value text-accent-blue">0.18</div>
        <div class="frost-stat-label">Surface Alpha</div>
      </div>
    </div>

    <!-- Card Grid (Surface Layer) -->
    <div class="frost-grid">
      <div class="frost-card">
        <h2>Frosted Panels</h2>
        <p>Semi-transparent surfaces blur the vibrant world beneath them. Each layer reveals color while softening detail, creating depth without weight.</p>
        <span class="frost-mono">backdrop-filter: blur(16px) saturate(1.4)</span>
      </div>
      <div class="frost-card">
        <h2>Diffused Shadows</h2>
        <p>Large spread, low opacity. Shadows are atmospheric halos, not hard edges. They suggest floating glass rather than solid objects.</p>
        <span class="frost-mono">box-shadow: 0 8px 32px rgba(10,10,50,0.12)</span>
      </div>
      <div class="frost-card">
        <h2>Luminous Borders</h2>
        <p>Thin white borders at low opacity catch the light like glass edges. They define without constraining, glowing faintly against the frosted surface.</p>
        <span class="frost-mono">border: 1px solid rgba(255,255,255,0.18)</span>
      </div>
    </div>

    <!-- Content Panel (Mid Layer) -->
    <section class="frost-content-panel">
      <h2>Layered Depth</h2>
      <p>Frosted Touch builds interfaces from translucent layers at multiple depths. The deepest panels carry the heaviest blur and lowest opacity, while surface elements are crisper and brighter. The result is a spatial composition where every element has a clear position in z-space.</p>
      <hr class="frost-divider">
      <p>The vibrant gradient background is never hidden -- it is the color source for the entire composition, felt through every frosted layer. Without it, the frost panels are just gray boxes. With it, they become glass.</p>
      <div style="margin-top: 1.5rem; display: flex; gap: 0.75rem; flex-wrap: wrap;">
        <a href="#" class="frost-button">Primary Action</a>
        <a href="#" class="frost-button frost-button--secondary">Secondary</a>
      </div>
    </section>

    <!-- Footer -->
    <footer class="frost-footer">
      <p>Frosted Touch -- refined glassmorphism for 2026 and beyond</p>
    </footer>
  </div>
</body>
</html>
```
