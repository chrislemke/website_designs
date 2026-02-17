# Neubrutalism Design Reference

Neubrutalism (also spelled Neobrutalism or Neo-Brutalism) is a UI and visual design aesthetic that deliberately breaks conventional design rules with raw, unpolished, high-contrast elements. It evolved from traditional web brutalism but adds modern usability, bold color palettes, and a sense of intentional imperfection. The style is defined by thick black borders, hard-offset solid shadows with zero blur, oversized UI components, deliberately clashing vibrant colors, and unusual grotesque typography. It functions as a direct counter-movement to the polished smoothness of Flat Design, Corporate Memphis, and Glassmorphism -- prioritizing function over form while embracing visual confrontation and accessibility through oversized, high-contrast elements.

---

## Visual Characteristics

### Core Design Traits

- **Thick black outlines** -- every element (cards, buttons, inputs, images) is framed by bold, solid black borders, typically 2-3px wide
- **Hard-offset solid shadows** -- drop shadows use both X and Y offset with zero blur and full-opacity black, creating a stark pseudo-3D effect as if elements are cut-out and floating (e.g., `box-shadow: 4px 4px 0px 0px #000000`)
- **No gradients, no blur** -- surfaces are strictly flat, solid-color fills; the only depth comes from hard shadows and borders, never from smooth transitions
- **Oversized UI components** -- buttons, inputs, and interactive elements are deliberately larger than conventional design norms, improving accessibility and visual impact
- **Deliberately clashing color palettes** -- bold, saturated, often contrasting or off-putting color combinations that reject harmony in favor of visual energy
- **Raw, unpolished aesthetic** -- intentional roughness and imperfection; elements feel hand-placed rather than pixel-perfect
- **Pseudo-3D rendering** -- hard 45-degree-angle shadows create the illusion of flat objects stacked on top of each other
- **Geometric blocks and shapes** -- raw, unrefined rectangles, circles, stars, and polygons, often with visible strokes
- **Zig-zag lines and jagged edges** -- decorative elements embrace irregularity and sharp angular patterns
- **1930s-style cartoon characters and outline illustrations** -- when illustrations are used, they tend toward Fleischer-era rubber-hose cartoons or simple realistic outlines (empty/unshaded)
- **Graph paper grids and visible structure** -- layouts may expose their underlying grid or use ruled-paper backgrounds as decorative elements
- **Computer window / tab aesthetics** -- retro UI references such as Windows 98-style title bars, monospace system fonts, and old browser chrome

### Design Principles

- Prioritize usability and accessibility over visual elegance -- large touch targets, high contrast, readable type
- Break traditional design conventions deliberately but maintain functional clarity
- Use borders, shadows, and color (never gradients or blur) to create visual hierarchy
- Embrace imperfection: asymmetric layouts, irregular spacing, and misaligned elements are features, not bugs
- Every element should feel bold and confrontational -- nothing recedes into the background
- Typography is a primary decorative element, not just a vehicle for content
- Function over form: the design should feel utilitarian and direct, never precious or delicate
- Strategic whitespace prevents the bold elements from becoming overwhelming

---

## Color Palette

### Primary Scheme

Neubrutalism uses **bold, saturated, often clashing colors** alongside pure black and white. There are no gradients, no tones, no smooth transitions. Colors are flat, solid, and high-contrast. The palette deliberately avoids the desaturated, harmonious pastels of modern design trends.

| Role | Colors | Hex (suggested) |
|------|--------|-----------------|
| **Black (primary)** | Pure black for borders, shadows, text | `#000000` |
| **White** | Clean white for backgrounds, card surfaces | `#FFFFFF` |
| **Off-white / Cream** | Warm alternative backgrounds | `#F5F1EB`, `#FDF6EC` |
| **Electric Blue** | Primary accent, links, interactive elements | `#38DBFF`, `#3B82F6` |
| **Hot Yellow** | Highlight accent, attention-grabber | `#FFF503`, `#FFDD00` |
| **Warm Orange** | Secondary accent, CTAs, warnings | `#FFB443`, `#FF8A00` |
| **Coral Red** | Alert accent, destructive actions | `#FF5D5D`, `#FF3B30` |
| **Neon Green** | Success states, positive indicators | `#00FF75`, `#4ADE80` |
| **Vivid Purple** | Feature highlights, tags, badges | `#DD7DFF`, `#A855F7` |
| **Bubblegum Pink** | Playful accent, decorative fills | `#FF6B8A`, `#F472B6` |
| **Deep Navy** | Dark mode backgrounds, heavy text | `#1A1A2E`, `#0F172A` |

### CSS Custom Properties

```css
:root {
  /* Core */
  --nb-black: #000000;
  --nb-white: #ffffff;
  --nb-off-white: #f5f1eb;
  --nb-cream: #fdf6ec;

  /* Accent palette */
  --nb-blue: #38dbff;
  --nb-yellow: #fff503;
  --nb-orange: #ffb443;
  --nb-red: #ff5d5d;
  --nb-green: #00ff75;
  --nb-purple: #dd7dff;
  --nb-pink: #ff6b8a;

  /* Deeper variants for backgrounds */
  --nb-blue-bg: #d0f4ff;
  --nb-yellow-bg: #fffbd0;
  --nb-orange-bg: #ffe8c8;
  --nb-red-bg: #ffd6d6;
  --nb-green-bg: #ccffe4;
  --nb-purple-bg: #f3d6ff;
  --nb-pink-bg: #ffd6e2;

  /* Text */
  --nb-text-dark: #000000;
  --nb-text-body: #1a1a1a;
  --nb-text-light: #ffffff;

  /* Shadows & borders */
  --nb-shadow: 4px 4px 0px 0px #000000;
  --nb-shadow-lg: 8px 8px 0px 0px #000000;
  --nb-shadow-hover: 2px 2px 0px 0px #000000;
  --nb-border: 2px solid #000000;
  --nb-border-thick: 3px solid #000000;
}
```

### Color Usage Guidelines

- **Use 2-3 bold colors maximum** per section; pair them with black and white for structure
- **Pure black** is the defining structural color -- used for all borders, shadows, and primary text
- **No gradients ever** -- every fill is a single solid color
- Colors may deliberately clash (red + green, blue + orange) -- this is intentional, not a mistake
- Backgrounds can be white, cream, or any bold accent color; avoid mid-tone grays
- Different sections can use entirely different accent colors, creating a patchwork effect
- Reserve the most saturated colors for interactive elements and key content areas
- Dark mode inverts the base (dark background, light text) but keeps the same bold accents and black borders

---

## Typography

### Typeface Characteristics

Neubrutalism typography is:

- **Bold, chunky, and impactful** -- headlines demand attention through sheer weight and size
- **Unusual and grotesque** -- quirky, eccentric typefaces are embraced; stretched, condensed, and irregular letterforms are welcome
- **Uppercase-heavy** -- headings often use all-caps for maximum visual punch
- **Sans-serif dominant** -- clean geometric or neo-grotesque sans-serifs for body text; display faces can break this rule
- **Raw and unrefined** -- typography should feel direct and confrontational, never elegant or delicate
- **Strong geometric shapes** -- letterforms built from bold strokes and clear geometric construction
- **Large size contrasts** -- headlines should be dramatically larger than body text (2x or more)
- **Generous letter-spacing** for uppercase display text; tighter for body copy

### Recommended Web Fonts (Google Fonts)

| Font | Style | Best For |
|------|-------|----------|
| **Space Grotesk** | Geometric sans, quirky details | Headlines, display text -- quintessential neubrutalist feel |
| **Space Mono** | Fixed-width, technical | Code blocks, labels, retro-tech accents |
| **Syne** | Variable-weight, eccentric geometry | Headlines, hero text, display -- bold and unapologetic |
| **Archivo Black** | Heavy compressed grotesque | Massive headlines, section titles, pure impact |
| **Inter** | Clean neo-grotesque, tall x-height | Body text, UI labels, buttons -- reliable readability |
| **Instrument Sans** | Modern geometric, clean | Body text, secondary headings |
| **DM Sans** | Clean geometric sans | Body text, form labels, smaller copy |
| **Poppins** | Geometric sans, rounded | All-purpose, buttons, body text |
| **Sora** | Geometric, modern, variable | Headlines and body, versatile weight range |
| **Unbounded** | Heavy display, stretched forms | Huge display headlines, maximum visual weight |

### Font Pairing Suggestions

| Heading Font | Body Font | Character |
|-------------|-----------|-----------|
| **Archivo Black** (400) | **Inter** (400) | Maximum impact headlines, clean body |
| **Syne** (700-800) | **DM Sans** (400) | Eccentric, bold headers with clean readability |
| **Space Grotesk** (700) | **Space Grotesk** (400) | Cohesive mono-family, techy neubrutalist feel |
| **Unbounded** (700) | **Poppins** (400) | Stretched display type, friendly body text |
| **Sora** (800) | **Instrument Sans** (400) | Modern geometric, balanced hierarchy |

### Typography CSS Example

```css
/* Import fonts */
@import url('https://fonts.googleapis.com/css2?family=Space+Grotesk:wght@400;500;600;700&family=Inter:wght@400;500;600&display=swap');

/* Headings */
h1, h2, h3, h4, h5, h6 {
  font-family: 'Space Grotesk', 'Syne', sans-serif;
  font-weight: 700;
  color: var(--nb-text-dark);
  line-height: 1.1;
  letter-spacing: -0.01em;
}

/* Display / Hero text */
.nb-display {
  font-family: 'Space Grotesk', sans-serif;
  font-size: clamp(3rem, 7vw, 5.5rem);
  font-weight: 700;
  letter-spacing: -0.02em;
  line-height: 1.0;
  text-transform: uppercase;
}

/* Body text */
body {
  font-family: 'Inter', 'DM Sans', sans-serif;
  font-weight: 400;
  font-size: 1.05rem;
  line-height: 1.7;
  color: var(--nb-text-body);
}

/* UI labels and buttons */
.nb-label {
  font-family: 'Space Grotesk', sans-serif;
  font-weight: 600;
  font-size: 0.95rem;
  letter-spacing: 0.04em;
  text-transform: uppercase;
}

/* Monospace accents */
.nb-mono {
  font-family: 'Space Mono', monospace;
  font-size: 0.85rem;
  letter-spacing: 0.02em;
}

/* Subtext / captions */
.nb-caption {
  font-family: 'Inter', sans-serif;
  font-weight: 400;
  font-size: 0.85rem;
  color: var(--nb-text-body);
  line-height: 1.5;
}
```

---

## Layout Principles

### Grid and Structure

- **Blocky, geometric layouts** -- content is organized in rigid rectangular blocks with thick visible borders, not floating cards with subtle shadows
- **Asymmetric and irregular arrangements** -- elements may be deliberately offset, overlapping, or unevenly sized to create visual tension
- **Visible grid structure** -- the underlying layout grid may be exposed as a design feature (graph paper, ruled lines)
- **High density with strategic whitespace** -- content areas can be packed tightly, but generous padding around the entire composition and between major sections prevents chaos
- **Max-width containers** (1000-1200px) keep content focused; generous padding (24-32px margins) on all sides
- **Large, oversized components** -- buttons, inputs, and interactive elements are deliberately bigger than conventional sizing
- **Stacked and tiled sections** -- content blocks sit directly on top of each other, separated by thick borders rather than whitespace alone
- **No decorative dividers** -- structure comes from borders and color blocks, not hairlines or subtle gradients

### Section Organization

- **Navigation**: Bold top bar with thick bottom border; logo and links in strong, uppercase type; no transparency or blur effects
- **Hero**: Massive headline (often full-width uppercase), short supporting text, oversized CTA button with hard shadow; optional bold illustration or geometric shapes
- **Features**: Grid of bordered cards with solid color backgrounds, each with thick outlines and hard shadows
- **Content blocks**: Alternating bold background colors with bordered containers; text and images arranged asymmetrically
- **Statistics / metrics**: Large bold numbers in thick-bordered boxes, arranged in a grid
- **CTA section**: Full-width bold background color + large centered text + oversized button
- **Footer**: Thick top border, bold background color, organized content in bordered columns

### Responsive Approach

- Stack columns vertically on mobile while maintaining thick borders and hard shadows
- Touch targets remain oversized (minimum 48px) for mobile accessibility
- Typography scales down but maintains strong weight and uppercase treatment
- Shadows and borders remain at full intensity at all breakpoints -- never soften for mobile

---

## CSS / Design Techniques

### Neubrutalist Card Component

```css
.nb-card {
  background: var(--nb-white);
  border: 2px solid var(--nb-black);
  box-shadow: 4px 4px 0px 0px var(--nb-black);
  padding: 24px;
  /* No border-radius or minimal radius */
  border-radius: 0;
  transition: box-shadow 0.15s ease, transform 0.15s ease;
}

.nb-card:hover {
  box-shadow: 2px 2px 0px 0px var(--nb-black);
  transform: translate(2px, 2px);
}

/* Colored card variants */
.nb-card--blue { background: var(--nb-blue-bg); }
.nb-card--yellow { background: var(--nb-yellow-bg); }
.nb-card--orange { background: var(--nb-orange-bg); }
.nb-card--red { background: var(--nb-red-bg); }
.nb-card--green { background: var(--nb-green-bg); }
.nb-card--purple { background: var(--nb-purple-bg); }
.nb-card--pink { background: var(--nb-pink-bg); }

/* Vivid card variants (saturated background) */
.nb-card--vivid-blue { background: var(--nb-blue); }
.nb-card--vivid-yellow { background: var(--nb-yellow); }
.nb-card--vivid-orange { background: var(--nb-orange); }

/* Card grid */
.nb-card-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
  gap: 24px;
}
```

### Neubrutalist Button

```css
.nb-button {
  display: inline-flex;
  align-items: center;
  justify-content: center;
  background: var(--nb-yellow);
  color: var(--nb-black);
  border: 2px solid var(--nb-black);
  border-radius: 0;
  padding: 14px 32px;
  font-family: 'Space Grotesk', sans-serif;
  font-weight: 700;
  font-size: 1rem;
  text-transform: uppercase;
  letter-spacing: 0.04em;
  cursor: pointer;
  box-shadow: 4px 4px 0px 0px var(--nb-black);
  transition: box-shadow 0.15s ease, transform 0.15s ease;
  text-decoration: none;
}

.nb-button:hover {
  box-shadow: 2px 2px 0px 0px var(--nb-black);
  transform: translate(2px, 2px);
}

.nb-button:active {
  box-shadow: 0px 0px 0px 0px var(--nb-black);
  transform: translate(4px, 4px);
}

/* Color variants */
.nb-button--blue { background: var(--nb-blue); }
.nb-button--green { background: var(--nb-green); }
.nb-button--orange { background: var(--nb-orange); }
.nb-button--red { background: var(--nb-red); color: var(--nb-white); }
.nb-button--pink { background: var(--nb-pink); }
.nb-button--white { background: var(--nb-white); }

/* Outline / ghost variant */
.nb-button--outline {
  background: transparent;
  color: var(--nb-black);
}

.nb-button--outline:hover {
  background: var(--nb-yellow);
}

/* Large button */
.nb-button--lg {
  padding: 18px 44px;
  font-size: 1.15rem;
  box-shadow: 6px 6px 0px 0px var(--nb-black);
}

/* Disabled state */
.nb-button:disabled {
  opacity: 0.5;
  cursor: not-allowed;
  box-shadow: 4px 4px 0px 0px var(--nb-black);
  transform: none;
}
```

### Navigation Bar

```css
.nb-nav {
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 16px 32px;
  border-bottom: 3px solid var(--nb-black);
  background: var(--nb-white);
}

.nb-nav__logo {
  font-family: 'Space Grotesk', sans-serif;
  font-weight: 700;
  font-size: 1.5rem;
  color: var(--nb-black);
  text-decoration: none;
  text-transform: uppercase;
  letter-spacing: 0.02em;
}

.nb-nav__links {
  display: flex;
  gap: 24px;
  list-style: none;
  margin: 0;
  padding: 0;
}

.nb-nav__links a {
  font-family: 'Space Grotesk', sans-serif;
  font-weight: 600;
  font-size: 0.95rem;
  color: var(--nb-black);
  text-decoration: none;
  text-transform: uppercase;
  letter-spacing: 0.03em;
  padding: 4px 0;
  border-bottom: 2px solid transparent;
  transition: border-color 0.15s ease;
}

.nb-nav__links a:hover {
  border-bottom-color: var(--nb-black);
}

.nb-nav__links a.active {
  border-bottom-color: var(--nb-black);
  background: var(--nb-yellow);
  padding: 4px 8px;
}
```

### Hero Section

```css
.nb-hero {
  display: flex;
  align-items: center;
  justify-content: space-between;
  max-width: 1200px;
  margin: 0 auto;
  padding: 80px 40px;
  gap: 60px;
}

.nb-hero__content {
  flex: 1;
  max-width: 600px;
}

.nb-hero__content h1 {
  font-size: clamp(3rem, 7vw, 5rem);
  font-weight: 700;
  text-transform: uppercase;
  line-height: 1.0;
  margin-bottom: 1.5rem;
  letter-spacing: -0.02em;
}

.nb-hero__content p {
  font-size: 1.2rem;
  line-height: 1.6;
  margin-bottom: 2rem;
  max-width: 480px;
}

.nb-hero__visual {
  flex: 1;
  display: flex;
  justify-content: center;
  align-items: center;
}

@media (max-width: 768px) {
  .nb-hero {
    flex-direction: column;
    text-align: left;
    padding: 40px 20px;
    gap: 40px;
  }
}
```

### Form Input

```css
.nb-input {
  width: 100%;
  padding: 14px 16px;
  border: 2px solid var(--nb-black);
  border-radius: 0;
  font-family: 'Inter', sans-serif;
  font-size: 1rem;
  color: var(--nb-text-dark);
  background: var(--nb-white);
  box-shadow: 3px 3px 0px 0px var(--nb-black);
  transition: box-shadow 0.15s ease, transform 0.15s ease;
  outline: none;
}

.nb-input:focus {
  box-shadow: 1px 1px 0px 0px var(--nb-black);
  transform: translate(2px, 2px);
}

.nb-input::placeholder {
  color: #888888;
}

/* Select dropdown */
.nb-select {
  appearance: none;
  padding: 14px 40px 14px 16px;
  border: 2px solid var(--nb-black);
  border-radius: 0;
  font-family: 'Inter', sans-serif;
  font-size: 1rem;
  background: var(--nb-white) url("data:image/svg+xml;charset=utf-8,%3Csvg xmlns='http://www.w3.org/2000/svg' width='12' height='8'%3E%3Cpath d='M1 1l5 5 5-5' stroke='%23000' stroke-width='2' fill='none'/%3E%3C/svg%3E") no-repeat right 14px center;
  box-shadow: 3px 3px 0px 0px var(--nb-black);
  cursor: pointer;
}
```

### Section Color Blocks

```css
.nb-section {
  padding: 80px 0;
  border-bottom: 3px solid var(--nb-black);
}

.nb-section--white { background: var(--nb-white); }
.nb-section--cream { background: var(--nb-cream); }
.nb-section--blue { background: var(--nb-blue); }
.nb-section--yellow { background: var(--nb-yellow); }
.nb-section--orange { background: var(--nb-orange); }
.nb-section--green { background: var(--nb-green); }
.nb-section--purple { background: var(--nb-purple); }
.nb-section--pink { background: var(--nb-pink); }
.nb-section--dark {
  background: var(--nb-black);
  color: var(--nb-white);
}

/* On dark sections, borders and shadows switch to white */
.nb-section--dark .nb-card {
  border-color: var(--nb-white);
  box-shadow: 4px 4px 0px 0px var(--nb-white);
}

.nb-section--dark .nb-button {
  border-color: var(--nb-white);
  box-shadow: 4px 4px 0px 0px var(--nb-white);
}
```

### Feature Grid

```css
.nb-features {
  padding: 80px 0;
}

.nb-features__grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
  gap: 24px;
  max-width: 1200px;
  margin: 0 auto;
  padding: 0 40px;
}

.nb-feature {
  border: 2px solid var(--nb-black);
  box-shadow: 4px 4px 0px 0px var(--nb-black);
  padding: 28px;
  background: var(--nb-white);
}

.nb-feature__icon {
  width: 56px;
  height: 56px;
  border: 2px solid var(--nb-black);
  margin-bottom: 16px;
  display: flex;
  align-items: center;
  justify-content: center;
  font-size: 1.5rem;
  background: var(--nb-yellow);
}

.nb-feature h3 {
  font-size: 1.2rem;
  text-transform: uppercase;
  margin-bottom: 0.75rem;
  letter-spacing: 0.02em;
}

.nb-feature p {
  font-size: 0.95rem;
  line-height: 1.6;
}
```

### Badge / Tag Component

```css
.nb-badge {
  display: inline-flex;
  align-items: center;
  padding: 4px 12px;
  border: 2px solid var(--nb-black);
  font-family: 'Space Grotesk', sans-serif;
  font-weight: 600;
  font-size: 0.75rem;
  text-transform: uppercase;
  letter-spacing: 0.05em;
  background: var(--nb-yellow);
  color: var(--nb-black);
  box-shadow: 2px 2px 0px 0px var(--nb-black);
}

.nb-badge--blue { background: var(--nb-blue); }
.nb-badge--green { background: var(--nb-green); }
.nb-badge--red { background: var(--nb-red); }
.nb-badge--purple { background: var(--nb-purple); }
```

### Retro Window Component

A signature neubrutalist decorative element: faux OS window frames.

```css
.nb-window {
  border: 2px solid var(--nb-black);
  box-shadow: 6px 6px 0px 0px var(--nb-black);
  background: var(--nb-white);
  overflow: hidden;
}

.nb-window__titlebar {
  display: flex;
  align-items: center;
  gap: 6px;
  padding: 8px 12px;
  background: var(--nb-cream);
  border-bottom: 2px solid var(--nb-black);
}

.nb-window__dot {
  width: 12px;
  height: 12px;
  border-radius: 50%;
  border: 2px solid var(--nb-black);
}

.nb-window__dot--red { background: var(--nb-red); }
.nb-window__dot--yellow { background: var(--nb-yellow); }
.nb-window__dot--green { background: var(--nb-green); }

.nb-window__content {
  padding: 24px;
}
```

---

## Design Do's and Don'ts

### Do

- Use thick, solid black borders (2-3px) on every UI element -- cards, buttons, inputs, images
- Apply hard-offset box shadows with zero blur (`4px 4px 0px 0px #000`)
- Use bold, high-contrast, saturated colors that deliberately clash
- Make interactive elements oversized and impossible to miss
- Use uppercase, heavy-weight typography for headlines
- Employ flat, solid color fills for all surfaces
- Maintain high text contrast for accessibility (check with contrast tools)
- Use hover/active states that shift the shadow (translate the element toward its shadow on press)
- Separate sections with thick borders and bold background color changes
- Embrace asymmetry, overlap, and visual tension in layouts
- Include retro/skeuomorphic UI references (window frames, pixel art, monospace fonts)

### Don't

- Use drop shadows with blur (`box-shadow` blur radius must be 0)
- Apply gradients to any surface, background, or text
- Use rounded pill-shaped buttons or large border-radius values
- Use subtle, low-contrast color palettes or harmonious pastel schemes
- Add glassmorphism, transparency, or backdrop-filter effects
- Use thin, delicate typography or light font weights for headings
- Apply smooth transitions or easing animations that feel polished -- keep interactions snappy
- Use soft, diffused shadows or multiple layered shadows
- Over-complicate layouts with nested containers; keep the structure blocky and direct
- Sacrifice readability for raw aesthetics -- text must always be clearly legible

---

## Related Aesthetics

| Aesthetic | Relationship to Neubrutalism |
|-----------|------------------------------|
| **Brutalism (web)** | Direct ancestor; raw, stripped-down web design with exposed HTML structure, monospace type, and zero decoration. Neubrutalism adds modern usability, color, and refined interaction patterns |
| **Flat Design** | Shares the rejection of gradients and 3D effects, but Flat Design seeks polish and harmony while Neubrutalism embraces rawness and visual confrontation |
| **Corporate Memphis** | The aesthetic Neubrutalism most directly reacts against; Corporate Memphis's smooth, friendly, optimistic illustrations are replaced by thick borders, hard shadows, and aggressive color |
| **Memphis Design** | 1980s Italian movement; shares bold colors, geometric shapes, and playful irreverence but adds pattern, texture, and postmodern ornamentation |
| **Bauhaus** | Shares the form-follows-function philosophy and geometric construction; Neubrutalism adds deliberate imperfection and visual aggression |
| **International Typographic Style** | Shares the grid-based, structured approach; Neubrutalism disrupts the Swiss Style's clean precision with rawness and asymmetry |
| **DIY Punk** | Shares the anti-establishment, raw, hand-made aesthetic; Neubrutalism translates punk's cut-and-paste collage energy into digital UI |
| **Claymorphism** | Contemporary alternative; where Claymorphism adds soft, inflated 3D depth, Neubrutalism uses hard-edged, flat, confrontational depth |
| **Glassmorphism** | Polar opposite in approach; Glassmorphism's translucent, blurred, ethereal surfaces are everything Neubrutalism rejects |
| **Neumorphism** | Both create depth without traditional shadows, but Neumorphism uses subtle same-color extrusion while Neubrutalism uses stark black hard-offset shadows |

---

## Quick-Start: Minimal Neubrutalism Page Template

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Neubrutalism Page</title>
  <link href="https://fonts.googleapis.com/css2?family=Space+Grotesk:wght@400;500;600;700&family=Inter:wght@400;500;600&display=swap" rel="stylesheet">
  <style>
    :root {
      --nb-black: #000000;
      --nb-white: #ffffff;
      --nb-cream: #fdf6ec;
      --nb-blue: #38dbff;
      --nb-yellow: #fff503;
      --nb-orange: #ffb443;
      --nb-red: #ff5d5d;
      --nb-green: #00ff75;
      --nb-purple: #dd7dff;
    }

    * { margin: 0; padding: 0; box-sizing: border-box; }

    body {
      background: var(--nb-cream);
      color: var(--nb-black);
      font-family: 'Inter', sans-serif;
      font-weight: 400;
      line-height: 1.7;
    }

    h1, h2, h3 {
      font-family: 'Space Grotesk', sans-serif;
      font-weight: 700;
      line-height: 1.1;
      text-transform: uppercase;
    }

    /* Navigation */
    nav {
      display: flex;
      align-items: center;
      justify-content: space-between;
      padding: 16px 32px;
      border-bottom: 3px solid var(--nb-black);
      background: var(--nb-white);
    }

    nav a.logo {
      font-family: 'Space Grotesk', sans-serif;
      font-weight: 700;
      font-size: 1.5rem;
      color: var(--nb-black);
      text-decoration: none;
      text-transform: uppercase;
    }

    nav ul {
      display: flex;
      gap: 24px;
      list-style: none;
    }

    nav ul a {
      color: var(--nb-black);
      text-decoration: none;
      font-family: 'Space Grotesk', sans-serif;
      font-weight: 600;
      font-size: 0.95rem;
      text-transform: uppercase;
      letter-spacing: 0.03em;
    }

    nav ul a:hover { background: var(--nb-yellow); padding: 2px 6px; }

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

    .hero-content { flex: 1; max-width: 600px; }

    .hero h1 {
      font-size: clamp(3rem, 7vw, 5rem);
      margin-bottom: 1.5rem;
      line-height: 1.0;
    }

    .hero p {
      font-size: 1.15rem;
      margin-bottom: 2rem;
      max-width: 480px;
    }

    .hero-visual {
      flex: 1;
      display: flex;
      justify-content: center;
    }

    /* Button */
    .btn {
      display: inline-block;
      background: var(--nb-yellow);
      color: var(--nb-black);
      border: 2px solid var(--nb-black);
      border-radius: 0;
      padding: 16px 40px;
      font-family: 'Space Grotesk', sans-serif;
      font-weight: 700;
      font-size: 1.05rem;
      text-transform: uppercase;
      letter-spacing: 0.04em;
      cursor: pointer;
      text-decoration: none;
      box-shadow: 4px 4px 0px 0px var(--nb-black);
      transition: box-shadow 0.15s ease, transform 0.15s ease;
    }

    .btn:hover {
      box-shadow: 2px 2px 0px 0px var(--nb-black);
      transform: translate(2px, 2px);
    }

    .btn:active {
      box-shadow: 0px 0px 0px 0px var(--nb-black);
      transform: translate(4px, 4px);
    }

    /* Features */
    .features {
      background: var(--nb-white);
      padding: 80px 0;
      border-top: 3px solid var(--nb-black);
      border-bottom: 3px solid var(--nb-black);
    }

    .features h2 {
      text-align: center;
      font-size: 2.5rem;
      margin-bottom: 48px;
    }

    .features-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
      gap: 24px;
      max-width: 1200px;
      margin: 0 auto;
      padding: 0 40px;
    }

    .feature {
      border: 2px solid var(--nb-black);
      box-shadow: 4px 4px 0px 0px var(--nb-black);
      padding: 28px;
      background: var(--nb-white);
    }

    .feature-icon {
      width: 48px;
      height: 48px;
      border: 2px solid var(--nb-black);
      margin-bottom: 16px;
      display: flex;
      align-items: center;
      justify-content: center;
    }

    .feature h3 { margin-bottom: 0.5rem; font-size: 1.1rem; }
    .feature p { font-size: 0.95rem; line-height: 1.6; }

    /* CTA section */
    .cta {
      background: var(--nb-blue);
      border-bottom: 3px solid var(--nb-black);
      text-align: center;
      padding: 80px 40px;
    }

    .cta h2 {
      font-size: 2.5rem;
      margin-bottom: 1rem;
    }

    .cta p {
      font-size: 1.1rem;
      margin-bottom: 2rem;
      max-width: 500px;
      margin-left: auto;
      margin-right: auto;
    }

    .cta .btn {
      background: var(--nb-white);
    }

    /* Footer */
    footer {
      background: var(--nb-black);
      color: var(--nb-white);
      text-align: center;
      padding: 32px;
      font-family: 'Space Grotesk', sans-serif;
      font-weight: 600;
      font-size: 0.9rem;
      text-transform: uppercase;
      letter-spacing: 0.05em;
    }

    @media (max-width: 768px) {
      .hero {
        flex-direction: column;
        padding: 40px 20px;
        gap: 40px;
      }
      nav { padding: 12px 20px; }
      nav ul { gap: 16px; }
    }
  </style>
</head>
<body>
  <nav>
    <a href="#" class="logo">BruteCo</a>
    <ul>
      <li><a href="#">Product</a></li>
      <li><a href="#">Features</a></li>
      <li><a href="#">Pricing</a></li>
      <li><a href="#">About</a></li>
    </ul>
  </nav>

  <section class="hero">
    <div class="hero-content">
      <h1>No fluff. Just tools that work.</h1>
      <p>Raw, direct, and built for people who care about getting things done. No polish required.</p>
      <a href="#" class="btn">Get Started</a>
    </div>
    <div class="hero-visual">
      <svg width="400" height="320" viewBox="0 0 400 320" fill="none" xmlns="http://www.w3.org/2000/svg">
        <!-- Window frame -->
        <rect x="40" y="20" width="320" height="240" fill="#FFFFFF" stroke="#000000" stroke-width="3"/>
        <rect x="40" y="20" width="320" height="32" fill="#FDF6EC" stroke="#000000" stroke-width="3"/>
        <!-- Window dots -->
        <circle cx="60" cy="36" r="6" fill="#FF5D5D" stroke="#000" stroke-width="2"/>
        <circle cx="80" cy="36" r="6" fill="#FFF503" stroke="#000" stroke-width="2"/>
        <circle cx="100" cy="36" r="6" fill="#00FF75" stroke="#000" stroke-width="2"/>
        <!-- Content blocks inside window -->
        <rect x="60" y="70" width="120" height="16" fill="#000000"/>
        <rect x="60" y="96" width="280" height="8" fill="#DDDDDD"/>
        <rect x="60" y="112" width="280" height="8" fill="#DDDDDD"/>
        <rect x="60" y="128" width="200" height="8" fill="#DDDDDD"/>
        <!-- Button inside window -->
        <rect x="60" y="156" width="120" height="36" fill="#38DBFF" stroke="#000000" stroke-width="2"/>
        <rect x="64" y="160" width="120" height="36" fill="none" stroke="none"/>
        <!-- Shadow block for button -->
        <rect x="64" y="160" width="120" height="36" fill="#000000" opacity="0"/>
        <!-- Decorative shapes outside window -->
        <rect x="20" y="280" width="60" height="30" fill="#FFB443" stroke="#000" stroke-width="2" transform="rotate(-5 50 295)"/>
        <rect x="24" y="284" width="60" height="30" fill="none">
        </rect>
        <circle cx="370" cy="290" r="20" fill="#DD7DFF" stroke="#000" stroke-width="2"/>
        <rect x="340" y="50" width="40" height="40" fill="#FFF503" stroke="#000" stroke-width="2" transform="rotate(12 360 70)"/>
        <!-- Zig-zag decorative line -->
        <polyline points="60,220 80,200 100,220 120,200 140,220 160,200 180,220 200,200 220,220 240,200 260,220 280,200 300,220 320,200 340,220" stroke="#000" stroke-width="2" fill="none"/>
      </svg>
    </div>
  </section>

  <section class="features">
    <h2>Why us</h2>
    <div class="features-grid">
      <div class="feature">
        <div class="feature-icon" style="background: #38DBFF;">
          <svg width="24" height="24" viewBox="0 0 24 24"><rect x="3" y="7" width="18" height="12" rx="1" stroke="#000" stroke-width="2" fill="none"/><line x1="3" y1="11" x2="21" y2="11" stroke="#000" stroke-width="2"/></svg>
        </div>
        <h3>Direct Interface</h3>
        <p>No filler. Every element earns its place on screen. Clarity is the feature.</p>
      </div>
      <div class="feature" style="background: #FFFBD0;">
        <div class="feature-icon" style="background: #FFF503;">
          <svg width="24" height="24" viewBox="0 0 24 24"><path d="M13 2L3 14h8l-1 8 10-12h-8l1-8z" stroke="#000" stroke-width="2" fill="none"/></svg>
        </div>
        <h3>Built For Speed</h3>
        <p>Lightweight, fast, and zero bloat. Your work deserves tools that keep up.</p>
      </div>
      <div class="feature">
        <div class="feature-icon" style="background: #00FF75;">
          <svg width="24" height="24" viewBox="0 0 24 24"><path d="M9 12l2 2 4-4" stroke="#000" stroke-width="2.5" fill="none" stroke-linecap="round" stroke-linejoin="round"/><circle cx="12" cy="12" r="9" stroke="#000" stroke-width="2" fill="none"/></svg>
        </div>
        <h3>Rock Solid</h3>
        <p>99.9% uptime. Enterprise security. No excuses, no exceptions.</p>
      </div>
    </div>
  </section>

  <section class="cta">
    <h2>Ready to build?</h2>
    <p>Stop scrolling. Start shipping. It really is that simple.</p>
    <a href="#" class="btn">Start Free Trial</a>
  </section>

  <footer>
    <p>Built raw. Built right. No gradients were harmed.</p>
  </footer>
</body>
</html>
```
