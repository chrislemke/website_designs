# Flat Design Reference

Flat Design is a minimalist user interface and visual design aesthetic characterized by the elimination of three-dimensional visual effects -- no gradients, drop shadows, bevels, or textures. It emphasizes clean, open space, crisp edges, bright colors, and two-dimensional illustrations. The style prioritizes usability, accessibility, and clarity, reducing visual noise to its absolute minimum so that content and interaction take center stage.

---

## Visual Characteristics

### Core Design Traits

- **Strictly two-dimensional** -- all elements are rendered flat with zero depth simulation; no gradients, no shadows, no bevels, no embossing
- **Bold, solid color fills** -- every surface is a single uniform color; textures and patterns are eliminated
- **Crisp, geometric shapes** -- UI elements are constructed from simple rectangles, circles, and rounded rectangles with clean edges
- **Generous whitespace** -- open, uncluttered layouts where breathing room is as important as content
- **Simple, easily decipherable icons** -- vector-based, minimal iconography that communicates instantly
- **Rounded corners** -- UI elements favor soft, rounded edges to reduce visual sharpness and improve approachability
- **High contrast** -- strong color differentiation between foreground and background for maximum legibility
- **Minimalist logos and branding** -- simplified, geometric marks stripped of ornamental detail
- **No decorative ornamentation** -- every visual element serves a functional purpose
- **Mobile-first sensibility** -- designed for small screens where clarity and tap-target accuracy are paramount

### Design Principles

- Reduce every element to its simplest possible form
- Use color, spacing, and typography (not depth effects) to create visual hierarchy
- Prioritize accessibility: high contrast, readable type, clear interactive affordances
- Maintain consistency across all components -- every button, card, and icon follows the same flat rules
- Favor vector-based graphics (SVG) for infinite scalability and sharp rendering at any resolution
- Embrace bold color as the primary means of visual interest and differentiation
- Design for scannability: users should understand the page structure at a glance
- White/negative space is a deliberate design tool, not empty filler

---

## Color Palette

### Flat UI Classic Palette (Designmodo)

The canonical Flat UI color palette, widely adopted across the web design community. These are the base (500-level) values; each color has lighter and darker variants.

| Color Name | Hex | Role / Usage |
|------------|-----|-------------|
| **Turquoise** | `#1ABC9C` | Primary accent, CTAs, success states |
| **Green Sea** | `#16A085` | Darker turquoise variant, hover states |
| **Emerald** | `#2ECC71` | Secondary accent, success indicators |
| **Nephritis** | `#27AE60` | Darker green variant, confirmed states |
| **Peter River** | `#3498DB` | Primary blue, links, interactive elements |
| **Belize Hole** | `#2980B9` | Darker blue, active/pressed states |
| **Amethyst** | `#9B59B6` | Accent purple, tags, badges |
| **Wisteria** | `#8E44AD` | Darker purple variant |
| **Wet Asphalt** | `#34495E` | Dark text, headers, navigation |
| **Midnight Blue** | `#2C3E50` | Darkest text, footer backgrounds |
| **Sun Flower** | `#F1C40F` | Warning accents, highlights, stars |
| **Orange** | `#F39C12` | Secondary warning, attention elements |
| **Carrot** | `#E67E22` | Warm accent, pricing highlights |
| **Pumpkin** | `#D35400` | Darker orange, hover on warm CTAs |
| **Alizarin** | `#E74C3C` | Error states, destructive actions, alerts |
| **Pomegranate** | `#C0392B` | Darker red, critical warnings |
| **Clouds** | `#ECF0F1` | Light backgrounds, card surfaces |
| **Silver** | `#BDC3C7` | Borders, disabled states, dividers |
| **Concrete** | `#95A5A6` | Placeholder text, muted labels |
| **Asbestos** | `#7F8C8D` | Secondary text, captions |

### Extended Tint Scale

Each base color expands into a 50-900 scale for nuanced usage:

| Level | Purpose | Example (Peter River) |
|-------|---------|----------------------|
| 50 | Tinted backgrounds | `#EBF5FB` |
| 100 | Hover backgrounds | `#D6EAF8` |
| 200 | Light borders, tags | `#AED6F1` |
| 300 | Accent backgrounds | `#85C1E9` |
| 400 | Button hover states | `#5DADE2` |
| **500** | **Base color** | **`#3498DB`** |
| 600 | Active/pressed states | `#2E86C1` |
| 700 | Dark variant | `#2874A6` |
| 800 | High-emphasis text on light | `#21618C` |
| 900 | Maximum contrast | `#1B4F72` |

### CSS Custom Properties

```css
:root {
  /* Primary palette */
  --flat-turquoise: #1abc9c;
  --flat-green-sea: #16a085;
  --flat-emerald: #2ecc71;
  --flat-nephritis: #27ae60;
  --flat-peter-river: #3498db;
  --flat-belize-hole: #2980b9;
  --flat-amethyst: #9b59b6;
  --flat-wisteria: #8e44ad;

  /* Neutral palette */
  --flat-wet-asphalt: #34495e;
  --flat-midnight-blue: #2c3e50;
  --flat-clouds: #ecf0f1;
  --flat-silver: #bdc3c7;
  --flat-concrete: #95a5a6;
  --flat-asbestos: #7f8c8d;

  /* Warm accents */
  --flat-sun-flower: #f1c40f;
  --flat-orange: #f39c12;
  --flat-carrot: #e67e22;
  --flat-pumpkin: #d35400;
  --flat-alizarin: #e74c3c;
  --flat-pomegranate: #c0392b;

  /* Backgrounds */
  --flat-bg-white: #ffffff;
  --flat-bg-light: #ecf0f1;
  --flat-bg-dark: #2c3e50;

  /* Text */
  --flat-text-dark: #2c3e50;
  --flat-text-medium: #7f8c8d;
  --flat-text-light: #ecf0f1;
}
```

### Color Usage Guidelines

- **Use 2-3 primary colors maximum** per page to maintain a clean, focused appearance
- **Blue + white** is the most common Flat Design combination -- it reads as clean, trustworthy, and professional
- Avoid earth tones -- Flat Design favors synthetic, digitally vibrant hues
- Use **low-to-medium saturation** across the board to reduce eye strain
- Reserve high-saturation colors for interactive elements (buttons, links, CTAs)
- Background colors should be very light (Clouds, white) or very dark (Midnight Blue, Wet Asphalt) -- avoid mid-tones for page backgrounds
- Never use gradients for fills; a solid flat color is always preferred
- Differentiate interactive states (hover, active, disabled) purely through color shifts, not shadow or depth effects

---

## Typography

### Typeface Characteristics

Flat Design typography is:

- **Clean geometric sans-serif** -- matching the mathematical precision of the visual style
- **Highly legible at all sizes** -- readability is a core accessibility requirement
- **Medium to bold weights for headings** -- establishing hierarchy through weight, not decoration
- **Regular weight for body text** -- clean and comfortable for extended reading
- **No serifs, no scripts, no decorative faces** -- these conflict with the reductive, geometric ethos
- **Generous line-height and letter-spacing** -- airy and open, matching the whitespace-heavy layouts

### Recommended Web Fonts (Google Fonts)

| Font | Style | Best For |
|------|-------|----------|
| **Open Sans** | Humanist sans-serif, clean and neutral | Body text, UI labels -- the workhorse of Flat Design era |
| **Roboto** | Neo-grotesque, geometric underpinnings | Body text, Material-adjacent flat layouts |
| **Lato** | Semi-rounded, warm geometric | Headlines and body, friendly flat interfaces |
| **Montserrat** | Geometric sans, strong uppercase | Headlines, navigation, display text |
| **Raleway** | Elegant thin-to-bold range | Headlines, hero text, elegant flat pages |
| **Source Sans Pro** | Adobe's clean UI sans | Body text, data-heavy flat dashboards |
| **Nunito** | Rounded terminals, soft geometry | Friendly interfaces, approachable flat UIs |
| **Poppins** | Pure geometric circles and shapes | Modern headlines, all-purpose flat layouts |
| **Inter** | Designed for screens, tall x-height | UI text, buttons, labels, small sizes |
| **Work Sans** | Optimized for screens, geometric | Body text, editorial flat layouts |

### Font Pairing Suggestions

| Heading Font | Body Font | Character |
|-------------|-----------|-----------|
| **Montserrat** (700) | **Open Sans** (400) | Classic Flat Design, professional |
| **Poppins** (600) | **Inter** (400) | Modern, geometric, tech-forward |
| **Raleway** (600) | **Lato** (400) | Elegant, refined flat style |
| **Nunito** (700) | **Nunito Sans** (400) | Friendly, approachable, rounded |
| **Work Sans** (600) | **Source Sans Pro** (400) | Editorial, content-focused |

### Typography CSS Example

```css
/* Import fonts */
@import url('https://fonts.googleapis.com/css2?family=Montserrat:wght@500;600;700&family=Open+Sans:wght@400;600&display=swap');

/* Headings */
h1, h2, h3, h4, h5, h6 {
  font-family: 'Montserrat', 'Poppins', sans-serif;
  font-weight: 600;
  color: var(--flat-text-dark);
  line-height: 1.2;
  letter-spacing: -0.01em;
}

/* Display / Hero text */
.flat-display {
  font-family: 'Montserrat', sans-serif;
  font-size: clamp(2.5rem, 5vw, 4.5rem);
  font-weight: 700;
  letter-spacing: -0.02em;
  line-height: 1.1;
}

/* Body text */
body {
  font-family: 'Open Sans', 'Lato', sans-serif;
  font-weight: 400;
  font-size: 1rem;
  line-height: 1.7;
  color: var(--flat-text-dark);
}

/* UI labels and buttons */
.flat-label {
  font-family: 'Montserrat', sans-serif;
  font-weight: 600;
  font-size: 0.875rem;
  letter-spacing: 0.04em;
  text-transform: uppercase;
}

/* Subtext / captions */
.flat-caption {
  font-family: 'Open Sans', sans-serif;
  font-weight: 400;
  font-size: 0.85rem;
  color: var(--flat-text-medium);
  line-height: 1.5;
}
```

---

## Layout Principles

### Grid and Structure

- **Centered, constrained containers** -- max-width of 1000-1200px keeps content focused and readable
- **Generous whitespace everywhere** -- sections separated by 60-100px of vertical space; padding within components is liberal
- **Simple grid systems** -- 12-column or CSS Grid with `auto-fit`/`auto-fill`; avoid complex nested grids
- **Card-based content organization** -- flat cards (no shadows) arranged in clean grids
- **Clear visual hierarchy** -- established through font size, weight, and color contrast alone, never through depth
- **Full-width color blocks** -- sections alternate between light and colored backgrounds to create visual rhythm without borders or dividers
- **Mobile-first responsive design** -- layouts designed for small screens first, then expanded for larger viewports
- **No decorative borders or dividers** -- separation achieved purely through spacing and background color changes

### Section Organization

- **Navigation**: Minimal top bar with logo and horizontal links; no backgrounds, no borders, no shadows
- **Hero**: Large bold headline + short supporting text + single CTA button; optional simple illustration
- **Features**: 3 or 4-column grid of icon + title + short description
- **Content rows**: Alternating text-left/image-right and image-left/text-right sections
- **Statistics / metrics**: Large numbers with short labels, arranged in a row
- **Testimonials**: Simple quote cards with minimal decoration
- **CTA section**: Bold colored background + centered text + prominent button
- **Footer**: Dark background, organized link columns, minimal

### Responsive Approach

- Stack columns vertically on mobile (single-column below 768px)
- Maintain generous padding even at smaller breakpoints -- never let content touch screen edges
- Typography scales fluidly using `clamp()` for smooth transitions between breakpoints
- Interactive elements maintain minimum 44px touch targets on mobile
- Images and icons scale proportionally

---

## CSS / Design Techniques

### Flat Card Component

```css
.flat-card {
  background: #ffffff;
  border-radius: 8px;
  padding: 32px;
  /* Absolutely no box-shadow -- this is flat design */
  /* Separation comes from background color contrast */
}

/* Card on a colored background section */
.flat-section--colored .flat-card {
  background: #ffffff;
  color: var(--flat-text-dark);
}

/* Card grid */
.flat-card-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
  gap: 24px;
}
```

### Flat Button

```css
.flat-button {
  display: inline-flex;
  align-items: center;
  justify-content: center;
  background: var(--flat-peter-river);
  color: #ffffff;
  border: none;
  border-radius: 4px;  /* subtle rounding, not pill-shaped */
  padding: 12px 32px;
  font-family: 'Montserrat', sans-serif;
  font-weight: 600;
  font-size: 0.95rem;
  cursor: pointer;
  transition: background 0.2s ease;
  /* No box-shadow -- strictly flat */
  text-decoration: none;
}

.flat-button:hover {
  background: var(--flat-belize-hole);
}

.flat-button:active {
  background: #21618c;
}

/* Success variant */
.flat-button--success {
  background: var(--flat-turquoise);
}

.flat-button--success:hover {
  background: var(--flat-green-sea);
}

/* Danger variant */
.flat-button--danger {
  background: var(--flat-alizarin);
}

.flat-button--danger:hover {
  background: var(--flat-pomegranate);
}

/* Ghost / outline variant */
.flat-button--ghost {
  background: transparent;
  color: var(--flat-peter-river);
  border: 2px solid var(--flat-peter-river);
}

.flat-button--ghost:hover {
  background: var(--flat-peter-river);
  color: #ffffff;
}

/* Disabled state */
.flat-button:disabled {
  background: var(--flat-silver);
  color: #ffffff;
  cursor: not-allowed;
}
```

### Navigation Bar

```css
.flat-nav {
  display: flex;
  align-items: center;
  justify-content: space-between;
  max-width: 1200px;
  margin: 0 auto;
  padding: 20px 40px;
  /* No background, no border, no shadow -- pure flat */
}

.flat-nav__logo {
  font-family: 'Montserrat', sans-serif;
  font-weight: 700;
  font-size: 1.4rem;
  color: var(--flat-text-dark);
  text-decoration: none;
}

.flat-nav__links {
  display: flex;
  gap: 32px;
  list-style: none;
  margin: 0;
  padding: 0;
}

.flat-nav__links a {
  font-family: 'Open Sans', sans-serif;
  font-weight: 600;
  font-size: 0.95rem;
  color: var(--flat-text-medium);
  text-decoration: none;
  transition: color 0.2s ease;
}

.flat-nav__links a:hover {
  color: var(--flat-peter-river);
}

.flat-nav__links a.active {
  color: var(--flat-peter-river);
}
```

### Hero Section

```css
.flat-hero {
  display: flex;
  align-items: center;
  justify-content: space-between;
  max-width: 1200px;
  margin: 0 auto;
  padding: 80px 40px;
  gap: 60px;
}

.flat-hero__content {
  flex: 1;
  max-width: 520px;
}

.flat-hero__content h1 {
  font-size: clamp(2.5rem, 5vw, 4rem);
  font-weight: 700;
  margin-bottom: 1rem;
  line-height: 1.15;
}

.flat-hero__content p {
  font-size: 1.15rem;
  color: var(--flat-text-medium);
  margin-bottom: 2rem;
  line-height: 1.7;
}

.flat-hero__visual {
  flex: 1;
  display: flex;
  justify-content: center;
  align-items: center;
}

.flat-hero__visual img,
.flat-hero__visual svg {
  width: 100%;
  max-width: 500px;
  height: auto;
}

@media (max-width: 768px) {
  .flat-hero {
    flex-direction: column-reverse;
    text-align: center;
    padding: 40px 20px;
    gap: 40px;
  }
}
```

### Feature Grid

```css
.flat-features {
  padding: 80px 0;
}

.flat-features__grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(260px, 1fr));
  gap: 40px;
  max-width: 1200px;
  margin: 0 auto;
  padding: 0 40px;
}

.flat-feature {
  text-align: center;
  padding: 24px;
}

.flat-feature__icon {
  width: 64px;
  height: 64px;
  border-radius: 8px;
  margin: 0 auto 20px;
  display: flex;
  align-items: center;
  justify-content: center;
  font-size: 1.75rem;
  /* Use flat color backgrounds for icon containers */
  background: var(--flat-clouds);
}

.flat-feature h3 {
  font-size: 1.2rem;
  margin-bottom: 0.75rem;
}

.flat-feature p {
  font-size: 0.95rem;
  color: var(--flat-text-medium);
  line-height: 1.6;
}
```

### Section Color Blocks

```css
.flat-section {
  padding: 80px 0;
}

.flat-section--white {
  background: #ffffff;
}

.flat-section--light {
  background: var(--flat-clouds);
}

.flat-section--blue {
  background: var(--flat-peter-river);
  color: #ffffff;
}

.flat-section--dark {
  background: var(--flat-midnight-blue);
  color: var(--flat-text-light);
}

.flat-section--turquoise {
  background: var(--flat-turquoise);
  color: #ffffff;
}

/* Invert text colors on dark/colored sections */
.flat-section--blue h1,
.flat-section--blue h2,
.flat-section--blue h3,
.flat-section--dark h1,
.flat-section--dark h2,
.flat-section--dark h3,
.flat-section--turquoise h1,
.flat-section--turquoise h2,
.flat-section--turquoise h3 {
  color: #ffffff;
}

.flat-section--blue p,
.flat-section--dark p,
.flat-section--turquoise p {
  color: rgba(255, 255, 255, 0.85);
}
```

### Alternating Content Rows

```css
.flat-row {
  display: flex;
  align-items: center;
  gap: 60px;
  max-width: 1200px;
  margin: 0 auto;
  padding: 80px 40px;
}

.flat-row:nth-child(even) {
  flex-direction: row-reverse;
}

.flat-row__text {
  flex: 1;
}

.flat-row__image {
  flex: 1;
}

.flat-row__image img,
.flat-row__image svg {
  width: 100%;
  max-width: 480px;
  height: auto;
}

@media (max-width: 768px) {
  .flat-row,
  .flat-row:nth-child(even) {
    flex-direction: column;
    gap: 30px;
    padding: 40px 20px;
  }
}
```

### Form Elements

```css
.flat-input {
  width: 100%;
  padding: 12px 16px;
  border: 2px solid var(--flat-silver);
  border-radius: 4px;
  font-family: 'Open Sans', sans-serif;
  font-size: 0.95rem;
  color: var(--flat-text-dark);
  background: #ffffff;
  transition: border-color 0.2s ease;
  /* No box-shadow, no inner shadow -- flat */
  outline: none;
}

.flat-input:focus {
  border-color: var(--flat-peter-river);
}

.flat-input::placeholder {
  color: var(--flat-concrete);
}

/* Toggle switch */
.flat-toggle {
  width: 48px;
  height: 26px;
  background: var(--flat-silver);
  border-radius: 13px;
  position: relative;
  cursor: pointer;
  transition: background 0.2s ease;
}

.flat-toggle.active {
  background: var(--flat-turquoise);
}

.flat-toggle::after {
  content: '';
  width: 22px;
  height: 22px;
  background: #ffffff;
  border-radius: 50%;
  position: absolute;
  top: 2px;
  left: 2px;
  transition: transform 0.2s ease;
}

.flat-toggle.active::after {
  transform: translateX(22px);
}
```

### Alert / Notification Components

```css
.flat-alert {
  padding: 16px 20px;
  border-radius: 4px;
  font-size: 0.95rem;
  font-weight: 600;
  /* No borders, no shadows -- color alone communicates */
}

.flat-alert--info {
  background: #d6eaf8;
  color: #21618c;
}

.flat-alert--success {
  background: #d5f5e3;
  color: #1e8449;
}

.flat-alert--warning {
  background: #fef9e7;
  color: #9a7d0a;
}

.flat-alert--danger {
  background: #fadbd8;
  color: #943126;
}
```

### Flat Icon Style (SVG)

```css
.flat-icon {
  /* Icons should be single-color, solid fills */
  fill: currentColor;
  width: 24px;
  height: 24px;
}

/* Icon in a colored circle container */
.flat-icon-circle {
  display: inline-flex;
  align-items: center;
  justify-content: center;
  width: 48px;
  height: 48px;
  border-radius: 50%;
  background: var(--flat-clouds);
}

.flat-icon-circle .flat-icon {
  fill: var(--flat-peter-river);
}
```

---

## Design Do's and Don'ts

### Do

- Use solid, flat color fills for every surface
- Create hierarchy through typography weight, size, and color contrast
- Maintain generous whitespace and padding throughout
- Design with accessibility as a primary concern (WCAG contrast ratios, readable type sizes)
- Use vector graphics (SVG) for icons and illustrations
- Keep interactions simple: color shifts for hover/active states
- Provide dark mode / high-contrast alternatives
- Use rounded corners on interactive elements (buttons, inputs, cards)
- Separate sections with background color changes and vertical spacing

### Don't

- Use drop shadows, box shadows, or text shadows
- Apply gradients to backgrounds, buttons, or any surface
- Use textures, patterns, or photographic backgrounds
- Add skeuomorphic details (stitching, leather, wood grain, etc.)
- Use 3D effects, perspective transforms, or depth simulation
- Add decorative borders or hairline dividers between sections
- Use earth tones as the primary palette
- Sacrifice legibility for aesthetic minimalism
- Over-animate -- transitions should be subtle and functional, not decorative

---

## Related Aesthetics

| Aesthetic | Relationship to Flat Design |
|-----------|----------------------------|
| **Corporate Memphis** | Direct subset/child; flat illustration systems with disproportionate human figures, adopted by major tech companies (2017-2023) |
| **Material Design** | Google's evolution of Flat Design; reintroduces deliberate shadow/elevation layers to add hierarchy while maintaining flat color fills |
| **Minimalism** | Broader parent philosophy; Flat Design applies minimalist principles specifically to digital interface design |
| **International Typographic Style (Swiss Style)** | Historical precursor; grid-based, sans-serif, reductive design philosophy from the 1950s that directly influenced Flat Design |
| **Bauhaus** | Foundational influence; form-follows-function philosophy, geometric shapes, primary colors |
| **Plakatstil** | Early 1900s poster art with flat color, bold shapes, minimal text -- a print-era ancestor |
| **Cyberminimalism** | Contemporary sibling; applies flat, minimal principles with a tech/digital identity focus |
| **Memphis Design** | 1980s Italian movement; shares geometric shapes and bold color but embraces pattern, texture, and ornament that Flat Design rejects |
| **Y2K Futurism** | Predecessor era aesthetic; glossy, gradient-heavy, and textured -- the opposite of flat |
| **Frutiger Aero** | Immediate predecessor (2004-2013); glossy, textured, skeuomorphic interfaces that Flat Design deliberately displaced |
| **Skeuomorphism** | Direct opposite; realistic textures, shadows, and physical-object metaphors that Flat Design was created to replace |
| **Glassmorphism** | Successor trend; reintroduces translucency, blur, and layered depth while retaining some flat simplicity |
| **Claymorphism** | Successor trend; adds puffy, inflated 3D depth to flat shapes, creating a soft, clay-like appearance |
| **Neumorphism** | Successor trend; uses subtle inner/outer shadows on same-colored surfaces to create soft, extruded interfaces |
| **Neubrutalism** | Reactionary counter-movement; embraces raw, unpolished, high-contrast aesthetics with visible borders and harsh shadows as an antidote to Flat Design's smoothness |
| **Vectorheart** | Related aesthetic that uses flat vector art with an emphasis on colorful, geometric character illustration |

---

## Quick-Start: Minimal Flat Design Page Template

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Flat Design Page</title>
  <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@500;600;700&family=Open+Sans:wght@400;600&display=swap" rel="stylesheet">
  <style>
    :root {
      --flat-turquoise: #1abc9c;
      --flat-peter-river: #3498db;
      --flat-belize-hole: #2980b9;
      --flat-wet-asphalt: #34495e;
      --flat-midnight-blue: #2c3e50;
      --flat-clouds: #ecf0f1;
      --flat-silver: #bdc3c7;
      --flat-concrete: #95a5a6;
      --flat-alizarin: #e74c3c;
      --flat-sun-flower: #f1c40f;
    }

    * { margin: 0; padding: 0; box-sizing: border-box; }

    body {
      background: #ffffff;
      color: var(--flat-midnight-blue);
      font-family: 'Open Sans', sans-serif;
      font-weight: 400;
      line-height: 1.7;
    }

    h1, h2, h3 {
      font-family: 'Montserrat', sans-serif;
      font-weight: 600;
      line-height: 1.2;
    }

    /* Navigation */
    nav {
      display: flex;
      align-items: center;
      justify-content: space-between;
      max-width: 1200px;
      margin: 0 auto;
      padding: 20px 40px;
    }

    nav a.logo {
      font-family: 'Montserrat', sans-serif;
      font-weight: 700;
      font-size: 1.3rem;
      color: var(--flat-midnight-blue);
      text-decoration: none;
    }

    nav ul {
      display: flex;
      gap: 28px;
      list-style: none;
    }

    nav ul a {
      color: var(--flat-concrete);
      text-decoration: none;
      font-weight: 600;
      font-size: 0.95rem;
      transition: color 0.2s;
    }

    nav ul a:hover { color: var(--flat-peter-river); }

    /* Hero */
    .hero {
      display: flex;
      align-items: center;
      justify-content: space-between;
      max-width: 1200px;
      margin: 0 auto;
      padding: 80px 40px;
      gap: 60px;
    }

    .hero-content { flex: 1; max-width: 520px; }

    .hero h1 {
      font-size: clamp(2.5rem, 5vw, 4rem);
      margin-bottom: 1rem;
    }

    .hero p {
      font-size: 1.15rem;
      color: var(--flat-concrete);
      margin-bottom: 2rem;
    }

    .hero-visual {
      flex: 1;
      display: flex;
      justify-content: center;
    }

    /* Flat button */
    .btn {
      display: inline-block;
      background: var(--flat-peter-river);
      color: #fff;
      border: none;
      border-radius: 4px;
      padding: 14px 36px;
      font-family: 'Montserrat', sans-serif;
      font-weight: 600;
      font-size: 1rem;
      cursor: pointer;
      text-decoration: none;
      transition: background 0.2s;
    }

    .btn:hover { background: var(--flat-belize-hole); }

    /* Feature section */
    .features {
      background: var(--flat-clouds);
      padding: 80px 0;
    }

    .features h2 {
      text-align: center;
      font-size: 2rem;
      margin-bottom: 48px;
    }

    .features-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
      gap: 32px;
      max-width: 1200px;
      margin: 0 auto;
      padding: 0 40px;
    }

    .feature {
      background: #ffffff;
      border-radius: 8px;
      padding: 32px;
      text-align: center;
    }

    .feature-icon {
      width: 56px;
      height: 56px;
      border-radius: 8px;
      margin: 0 auto 20px;
      display: flex;
      align-items: center;
      justify-content: center;
    }

    .feature h3 { margin-bottom: 0.5rem; font-size: 1.15rem; }
    .feature p { color: var(--flat-concrete); font-size: 0.95rem; }

    /* CTA section */
    .cta {
      background: var(--flat-peter-river);
      color: #ffffff;
      text-align: center;
      padding: 80px 40px;
    }

    .cta h2 {
      font-size: 2.25rem;
      margin-bottom: 1rem;
    }

    .cta p {
      font-size: 1.1rem;
      opacity: 0.9;
      margin-bottom: 2rem;
    }

    .cta .btn {
      background: #ffffff;
      color: var(--flat-peter-river);
    }

    .cta .btn:hover {
      background: var(--flat-clouds);
    }

    /* Footer */
    footer {
      background: var(--flat-midnight-blue);
      color: var(--flat-silver);
      text-align: center;
      padding: 40px;
      font-size: 0.9rem;
    }

    @media (max-width: 768px) {
      .hero {
        flex-direction: column-reverse;
        text-align: center;
        padding: 40px 20px;
      }
      nav { padding: 16px 20px; }
      nav ul { gap: 16px; }
    }
  </style>
</head>
<body>
  <nav>
    <a href="#" class="logo">FlatCo</a>
    <ul>
      <li><a href="#">Product</a></li>
      <li><a href="#">Features</a></li>
      <li><a href="#">Pricing</a></li>
      <li><a href="#">About</a></li>
    </ul>
  </nav>

  <section class="hero">
    <div class="hero-content">
      <h1>Simple tools for complex work</h1>
      <p>Clean, focused software that gets out of your way so you can focus on what matters most.</p>
      <a href="#" class="btn">Get Started</a>
    </div>
    <div class="hero-visual">
      <svg width="400" height="300" viewBox="0 0 400 300" fill="none" xmlns="http://www.w3.org/2000/svg">
        <!-- Monitor -->
        <rect x="80" y="30" width="240" height="160" rx="8" fill="#34495e"/>
        <rect x="92" y="42" width="216" height="136" rx="4" fill="#ffffff"/>
        <!-- Screen content: flat bars -->
        <rect x="108" y="60" width="60" height="8" rx="4" fill="#3498db"/>
        <rect x="108" y="78" width="184" height="6" rx="3" fill="#ecf0f1"/>
        <rect x="108" y="94" width="184" height="6" rx="3" fill="#ecf0f1"/>
        <rect x="108" y="110" width="120" height="6" rx="3" fill="#ecf0f1"/>
        <rect x="108" y="134" width="80" height="28" rx="4" fill="#1abc9c"/>
        <rect x="108" y="140" width="60" height="16" rx="2" fill="#1abc9c"/>
        <!-- Stand -->
        <rect x="175" y="190" width="50" height="20" rx="2" fill="#bdc3c7"/>
        <rect x="150" y="210" width="100" height="8" rx="4" fill="#bdc3c7"/>
        <!-- Decorative elements -->
        <circle cx="340" cy="60" r="24" fill="#f1c40f" opacity="0.3"/>
        <circle cx="60" cy="240" r="18" fill="#e74c3c" opacity="0.2"/>
        <rect x="320" y="220" width="40" height="40" rx="4" fill="#3498db" opacity="0.15"/>
        <circle cx="50" cy="80" r="12" fill="#1abc9c" opacity="0.25"/>
      </svg>
    </div>
  </section>

  <section class="features">
    <h2>Why teams choose us</h2>
    <div class="features-grid">
      <div class="feature">
        <div class="feature-icon" style="background: #d6eaf8;">
          <svg width="28" height="28" viewBox="0 0 28 28"><rect x="4" y="8" width="20" height="14" rx="3" fill="#3498db"/><rect x="8" y="12" width="12" height="2" rx="1" fill="#fff"/><rect x="8" y="16" width="8" height="2" rx="1" fill="#fff"/></svg>
        </div>
        <h3>Clean Interface</h3>
        <p>Every pixel has a purpose. No clutter, no distractions, just the tools you need.</p>
      </div>
      <div class="feature">
        <div class="feature-icon" style="background: #d5f5e3;">
          <svg width="28" height="28" viewBox="0 0 28 28"><circle cx="14" cy="14" r="10" fill="#1abc9c"/><path d="M9 14 L12 17 L19 10" stroke="#fff" stroke-width="2" fill="none" stroke-linecap="round" stroke-linejoin="round"/></svg>
        </div>
        <h3>Reliable Performance</h3>
        <p>Built for speed and stability. Your workflow stays smooth even under heavy load.</p>
      </div>
      <div class="feature">
        <div class="feature-icon" style="background: #fef9e7;">
          <svg width="28" height="28" viewBox="0 0 28 28"><circle cx="14" cy="14" r="10" fill="#f1c40f"/><rect x="11" y="10" width="6" height="8" rx="1" fill="#fff"/></svg>
        </div>
        <h3>Smart Insights</h3>
        <p>Clear analytics and reporting help you make better decisions faster.</p>
      </div>
    </div>
  </section>

  <section class="cta">
    <h2>Ready to simplify your workflow?</h2>
    <p>Join thousands of teams who have already made the switch.</p>
    <a href="#" class="btn">Start Free Trial</a>
  </section>

  <footer>
    <p>Built with Flat Design principles. Clean, simple, effective.</p>
  </footer>
</body>
</html>
```
