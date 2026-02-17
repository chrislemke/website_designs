# Memphis Design Reference

Memphis Design is a bold, postmodern design movement originating from the **Memphis Group**, founded in Milan, Italy in 1981 by Ettore Sottsass. It is characterized by **vibrant neon and pastel colors, bold geometric shapes, playful patterns including squiggly and zig-zag lines**, and a deliberate rejection of the austere minimalism that dominated 1970s design. The movement sought to inject **emotional and symbolic meaning into everyday objects**, blending elements of pop culture, high art, and ironic classicism. Memphis Design prioritizes visual exuberance, pattern density, kitsch-meets-elegance tension, and a joyful, almost chaotic compositional energy.

---

## Visual Characteristics

### Core Design Traits

- **Bold geometric shapes** -- triangles, circles, squares, and distinctive "pill" shapes are the primary visual building blocks, often oversized and layered
- **Zig-zag lines** -- usually rendered with black outlines, creating dynamic, angular energy throughout compositions
- **Squiggly lines and organic curves** -- the signature **Bacterio print** (designed by Sottsass in 1978) is the movement's trademark pattern, featuring freely drawn squiggles
- **Vibrant neon and pastel colors** -- fully saturated hues paired with unexpected pastel accents, never muted or tonal
- **Terrazzo patterns** -- speckled stone-inspired surfaces used extensively, originally on floors but extended to tabletops, furniture, and decorative surfaces
- **Confetti and scattered elements** -- small geometric shapes (triangles, dots, squares) scattered haphazardly across surfaces
- **Clashing pattern combinations** -- multiple conflicting patterns used simultaneously within a single composition
- **Thick strokes and outlines** -- heavy black or colored outlines around shapes and elements, creating graphic punch
- **Laminate and synthetic textures** -- matte surfaces paired against glossy finishes, creating deliberate visual tension
- **Flat, vectorized style** -- minimal photographic content; everything is graphic, constructed, and stylized
- **Offset heavy shadows** -- fully saturated solid shadows creating a dimensional pop effect

### Design Principles

- Reject minimalism and restraint; embrace maximalism, clutter, and visual abundance
- Use clashing colors and patterns deliberately -- discord is the point, not a mistake
- Layer geometric shapes for dimensional, collage-like compositions rather than flat layouts
- Combine high art references with pop culture kitsch freely and without irony about the combination
- Prioritize emotional response (joy, surprise, playfulness) over functional clarity
- Use pattern and color as structural elements, not just decoration
- Create visual tension through contrasting materials: matte vs. glossy, flat vs. dimensional, organic vs. geometric
- Asymmetry and haphazard placement over rigid grids -- elements should feel scattered intentionally
- Animation and subtle motion prevent the aesthetic from looking dated on digital platforms
- Bold, oversized elements dominate the viewport; nothing should feel timid or restrained

---

## Color Palette

### Primary Scheme

Memphis Design uses **intensely saturated neon hues combined with unexpected pastels** on typically white or brightly colored backgrounds. The palette evolved from its original 1981 primaries to incorporate purple and teal by the late 1980s and early 1990s.

| Role | Color | Hex (suggested) |
|------|-------|-----------------|
| **Hot Pink / Magenta** | Neon pink, electric magenta | `#F725A0`, `#FF69B4` |
| **Vibrant Yellow** | Bright golden yellow, lemon | `#FAD141`, `#FFD700` |
| **Teal / Turquoise** | Bright cyan, turquoise | `#0CB2C0`, `#40E0D0` |
| **Deep Purple** | Vivid violet, electric purple | `#672394`, `#8B2FC9` |
| **Coral / Red** | Warm coral, bright red | `#CD2D48`, `#FF7F50` |
| **Royal Blue** | Medium electric blue | `#4458A0`, `#4169E1` |
| **Lime Green** | Bright chartreuse | `#A8E05F`, `#7FFF00` |
| **Orange** | Neon tangerine | `#FF8C42`, `#EC9309` |
| **Background (White)** | Clean white, cream | `#FFFFFF`, `#E8E6D9` |
| **Background (Black)** | Deep charcoal, near-black | `#212436`, `#141414` |
| **Outline / Stroke** | Pure black for outlines | `#000000`, `#1A1A1A` |
| **Pastel Pink** | Soft blush | `#FAD6DA`, `#FEB6DC` |
| **Pastel Blue** | Soft sky | `#A3D9E5`, `#86CCCA` |
| **Pastel Yellow** | Soft butter | `#FAE498`, `#FEF3C7` |
| **Pastel Lavender** | Soft violet | `#C9AECF`, `#C8B4FF` |

### Suggested CSS Custom Properties

```css
:root {
  /* Neon primaries */
  --memphis-pink: #f725a0;
  --memphis-yellow: #fad141;
  --memphis-teal: #0cb2c0;
  --memphis-purple: #672394;
  --memphis-red: #cd2d48;
  --memphis-blue: #4458a0;
  --memphis-lime: #a8e05f;
  --memphis-orange: #ff8c42;
  --memphis-coral: #ff7f50;

  /* Pastels */
  --memphis-pastel-pink: #fad6da;
  --memphis-pastel-blue: #a3d9e5;
  --memphis-pastel-yellow: #fae498;
  --memphis-pastel-lavender: #c9aecf;
  --memphis-pastel-mint: #b5ead7;

  /* Backgrounds */
  --memphis-bg-white: #ffffff;
  --memphis-bg-cream: #e8e6d9;
  --memphis-bg-dark: #212436;
  --memphis-bg-black: #141414;

  /* Strokes and outlines */
  --memphis-black: #000000;
  --memphis-stroke-width: 3px;

  /* Text */
  --memphis-text-dark: #1a1a1a;
  --memphis-text-light: #ffffff;
}
```

### Color Guidelines

- **Always use fully saturated colors** -- avoid tints, tones, or muted variations for primary elements
- **Clash intentionally** -- place complementary or clashing colors adjacent to one another (pink next to yellow, teal next to orange)
- **White backgrounds are canonical** -- the default backdrop is white or off-white/cream, letting neon colors pop
- **Black and white with neon accents** works as an alternative approach for a slightly more restrained version
- **No color should appear timid** -- if using pastels, use them as secondary accents behind bold neon primaries
- **3-5 bold colors minimum** per composition, plus black outlines
- The palette should feel **electric, joyful, and deliberately excessive**

---

## Typography

### Typeface Characteristics

Memphis Design typography should be:

- **Bold, blocky sans-serifs** -- heavy geometric letterforms with strong visual weight
- **Handwriting-style bubble lettering** as an alternative for display use
- **Extreme font-weight contrasts** -- 900 weight for headings, 200 for body text, creating dramatic hierarchy
- **Geometric letterforms** -- type should mirror the geometric shapes used in other design elements
- **High-contrast colored lettering** -- do not hesitate to set text in bright pink, yellow, or teal against busy backgrounds
- **Playful, expressive composition** -- text can be rotated, stacked, or treated as a graphic element
- **No traditional serif fonts** -- serifs conflict with the geometric, constructed feel (unless used ironically)

### Recommended Web Fonts (Google Fonts)

| Font | Style | Usage |
|------|-------|-------|
| **Fredoka** | Rounded, geometric, playful | Display headings, hero text -- captures the bubbly Memphis spirit |
| **Kablammo** | Experimental variable, Memphis-inspired | Display headings, decorative titles -- directly inspired by the Memphis movement |
| **Quicksand** | Soft geometric curves | Headlines, subheadings, UI labels |
| **Baloo 2** | Chunky, rounded, lively | Display headings, section titles |
| **Oswald** | Condensed, bold, geometric | Impactful headlines, all-caps treatments |
| **Rubik** | Slightly rounded geometric | All-purpose: headlines, body, buttons |
| **Archivo Black** | Heavy geometric sans | Bold headlines, oversized display text |
| **Poppins** | Clean geometric sans | Body text, secondary headings |
| **Space Grotesk** | Modern geometric grotesk | Body text, data-heavy layouts |

### Typography CSS Example

```css
/* Import fonts */
@import url('https://fonts.googleapis.com/css2?family=Fredoka:wght@400;500;600;700&family=Quicksand:wght@300;400;500;700&family=Poppins:wght@200;400;700;900&display=swap');

/* Display / Hero headings */
h1, .memphis-display {
  font-family: 'Fredoka', 'Quicksand', sans-serif;
  font-weight: 700;
  font-size: clamp(3rem, 7vw, 6rem);
  line-height: 1.05;
  letter-spacing: -0.02em;
  color: var(--memphis-text-dark);
}

/* Section headings */
h2, h3 {
  font-family: 'Fredoka', 'Quicksand', sans-serif;
  font-weight: 600;
  line-height: 1.2;
}

/* Body text -- extreme weight contrast */
body {
  font-family: 'Poppins', 'Quicksand', sans-serif;
  font-weight: 200;
  font-size: 1rem;
  line-height: 1.7;
  color: var(--memphis-text-dark);
}

/* Bold accent text */
strong, .memphis-bold {
  font-family: 'Poppins', sans-serif;
  font-weight: 900;
}

/* Colored heading treatment */
.memphis-heading--pink { color: var(--memphis-pink); }
.memphis-heading--yellow { color: var(--memphis-yellow); }
.memphis-heading--teal { color: var(--memphis-teal); }
.memphis-heading--purple { color: var(--memphis-purple); }

/* Rotated decorative text */
.memphis-text-rotated {
  display: inline-block;
  transform: rotate(-5deg);
  font-family: 'Fredoka', sans-serif;
  font-weight: 700;
}
```

---

## Layout Principles

### Grid and Structure

- **Asymmetric, off-grid compositions** -- reject rigid grid systems; elements should feel scattered and haphazardly placed
- **Layered, collage-style layouts** -- overlapping geometric shapes, text, and images create depth
- **No traditional content hierarchy** -- visual weight is distributed through color and scale rather than strict top-down organization
- **White or brightly colored backgrounds** serve as a canvas for floating geometric elements
- **Generous use of negative space** between clusters of dense pattern/color activity
- **Full-bleed color blocks** for section separation, using bold, contrasting colors
- **Oversized decorative elements** that break out of containers and overlap section boundaries
- **Diagonal and rotated elements** -- nothing needs to sit perfectly horizontal or vertical
- **Material Design-style layering** adds modern depth to the 80s flat pattern aesthetic
- **Multiple competing focal points** rather than a single visual hierarchy

### Section Organization

- **Hero**: Oversized display text in a bold color + scattered geometric shapes + pattern background. Text can overlap shapes.
- **Content blocks**: Irregularly sized cards or panels with different background colors, offset from grid alignment
- **Feature sections**: Elements arranged asymmetrically with large geometric accents (circles, triangles) filling negative space
- **Dividers**: Zig-zag lines, wavy borders, or rows of geometric shapes instead of straight lines
- **Backgrounds**: Patterned sections using Bacterio squiggles, terrazzo dots, or confetti triangles
- **CTA sections**: Bold solid-color backgrounds (hot pink, teal, yellow) with contrasting text and thick-bordered buttons

### Responsive Approach

- Stack elements vertically on mobile but maintain bold colors, thick outlines, and geometric decoration
- Scale decorative shapes proportionally; do not remove them on smaller screens
- Typography scales aggressively with `clamp()` -- headings should remain oversized even on mobile
- Maintain thick outlines and stroke widths at all breakpoints
- Pattern density can be reduced on mobile but never eliminated

---

## CSS/Design Techniques

### Geometric Shape Decorations (CSS-only)

```css
/* Triangle */
.memphis-triangle {
  width: 0;
  height: 0;
  border-left: 40px solid transparent;
  border-right: 40px solid transparent;
  border-bottom: 70px solid var(--memphis-yellow);
  transform: rotate(15deg);
  position: absolute;
}

/* Circle */
.memphis-circle {
  width: 80px;
  height: 80px;
  border-radius: 50%;
  background: var(--memphis-pink);
  position: absolute;
}

/* Outlined circle */
.memphis-circle-outline {
  width: 100px;
  height: 100px;
  border-radius: 50%;
  border: 4px solid var(--memphis-black);
  background: transparent;
  position: absolute;
}

/* Cross / plus sign */
.memphis-cross {
  width: 60px;
  height: 60px;
  position: absolute;
}
.memphis-cross::before,
.memphis-cross::after {
  content: '';
  position: absolute;
  background: var(--memphis-teal);
}
.memphis-cross::before {
  width: 100%;
  height: 12px;
  top: 50%;
  transform: translateY(-50%);
}
.memphis-cross::after {
  width: 12px;
  height: 100%;
  left: 50%;
  transform: translateX(-50%);
}

/* Pill / capsule shape */
.memphis-pill {
  width: 40px;
  height: 100px;
  border-radius: 20px;
  background: var(--memphis-coral);
  transform: rotate(30deg);
  position: absolute;
}

/* Semi-circle */
.memphis-semicircle {
  width: 80px;
  height: 40px;
  border-radius: 80px 80px 0 0;
  background: var(--memphis-purple);
  position: absolute;
}
```

### Squiggle / Bacterio Pattern (SVG background)

```css
/* Bacterio print -- Memphis's signature squiggle pattern */
.memphis-bacterio-bg {
  background-color: var(--memphis-bg-cream);
  background-image: url("data:image/svg+xml,%3Csvg width='100' height='100' xmlns='http://www.w3.org/2000/svg'%3E%3Cpath d='M20 20 Q30 5 40 20 T60 20 T80 20' stroke='%23000' stroke-width='2.5' fill='none' stroke-linecap='round'/%3E%3Cpath d='M10 50 Q20 35 30 50 T50 50 T70 50' stroke='%23000' stroke-width='2.5' fill='none' stroke-linecap='round'/%3E%3Cpath d='M30 80 Q40 65 50 80 T70 80 T90 80' stroke='%23000' stroke-width='2.5' fill='none' stroke-linecap='round'/%3E%3C/svg%3E");
  background-size: 120px 120px;
}
```

### Terrazzo Pattern (CSS)

```css
/* Terrazzo speckled pattern */
.memphis-terrazzo-bg {
  background-color: var(--memphis-bg-cream);
  background-image:
    radial-gradient(circle 4px, var(--memphis-pink) 100%, transparent 100%),
    radial-gradient(circle 3px, var(--memphis-teal) 100%, transparent 100%),
    radial-gradient(circle 5px, var(--memphis-yellow) 100%, transparent 100%),
    radial-gradient(circle 3px, var(--memphis-purple) 100%, transparent 100%),
    radial-gradient(circle 2px, var(--memphis-black) 100%, transparent 100%),
    radial-gradient(circle 4px, var(--memphis-lime) 100%, transparent 100%);
  background-size: 200px 200px;
  background-position:
    10px 20px,
    50px 70px,
    90px 30px,
    140px 90px,
    30px 130px,
    170px 160px;
}
```

### Confetti Scatter Pattern (CSS)

```css
/* Confetti pattern with scattered triangles and dots */
.memphis-confetti-bg {
  background-color: #ffffff;
  background-image:
    /* Small triangles via linear-gradient */
    linear-gradient(135deg, var(--memphis-pink) 25%, transparent 25%),
    linear-gradient(225deg, var(--memphis-yellow) 25%, transparent 25%),
    linear-gradient(315deg, var(--memphis-teal) 25%, transparent 25%),
    /* Dots */
    radial-gradient(circle 3px, var(--memphis-purple) 100%, transparent 100%),
    radial-gradient(circle 2px, var(--memphis-orange) 100%, transparent 100%);
  background-size:
    30px 30px,
    40px 40px,
    25px 25px,
    180px 180px,
    150px 150px;
  background-position:
    0 0,
    60px 80px,
    120px 40px,
    20px 50px,
    100px 120px;
}
```

### Zig-Zag Border / Divider

```css
/* Zig-zag section divider */
.memphis-zigzag-divider {
  position: relative;
  height: 30px;
  background: linear-gradient(135deg, var(--memphis-yellow) 25%, transparent 25%) -20px 0,
              linear-gradient(225deg, var(--memphis-yellow) 25%, transparent 25%) -20px 0,
              linear-gradient(315deg, var(--memphis-yellow) 25%, transparent 25%),
              linear-gradient(45deg, var(--memphis-yellow) 25%, transparent 25%);
  background-size: 40px 30px;
  background-color: transparent;
}

/* Alternative: SVG zig-zag border */
.memphis-zigzag-svg {
  background-image: url("data:image/svg+xml,%3Csvg width='40' height='20' xmlns='http://www.w3.org/2000/svg'%3E%3Cpolyline points='0,20 20,0 40,20' stroke='%23000' stroke-width='3' fill='none'/%3E%3C/svg%3E");
  background-repeat: repeat-x;
  height: 20px;
}
```

### Memphis Button

```css
.memphis-button {
  display: inline-block;
  background: var(--memphis-yellow);
  color: var(--memphis-black);
  border: 3px solid var(--memphis-black);
  border-radius: 0; /* sharp corners, not rounded */
  padding: 14px 36px;
  font-family: 'Fredoka', sans-serif;
  font-weight: 700;
  font-size: 1.1rem;
  cursor: pointer;
  text-decoration: none;
  text-transform: uppercase;
  letter-spacing: 0.05em;
  position: relative;
  transition: transform 0.15s ease, box-shadow 0.15s ease;
  /* Offset shadow for dimensional pop */
  box-shadow: 4px 4px 0 var(--memphis-black);
}

.memphis-button:hover {
  transform: translate(-2px, -2px);
  box-shadow: 6px 6px 0 var(--memphis-black);
}

.memphis-button:active {
  transform: translate(2px, 2px);
  box-shadow: 2px 2px 0 var(--memphis-black);
}

/* Color variants */
.memphis-button--pink {
  background: var(--memphis-pink);
  color: #ffffff;
}

.memphis-button--teal {
  background: var(--memphis-teal);
  color: #ffffff;
}
```

### Memphis Card Component

```css
.memphis-card {
  background: #ffffff;
  border: 3px solid var(--memphis-black);
  border-radius: 0;
  padding: 28px;
  position: relative;
  box-shadow: 6px 6px 0 var(--memphis-black);
  transition: transform 0.2s ease, box-shadow 0.2s ease;
}

.memphis-card:hover {
  transform: translate(-3px, -3px);
  box-shadow: 9px 9px 0 var(--memphis-black);
}

/* Decorative corner accent */
.memphis-card::before {
  content: '';
  position: absolute;
  top: -8px;
  right: -8px;
  width: 20px;
  height: 20px;
  background: var(--memphis-yellow);
  border: 2px solid var(--memphis-black);
  border-radius: 50%;
}
```

### Hero Section

```css
.memphis-hero {
  position: relative;
  min-height: 90vh;
  display: flex;
  align-items: center;
  padding: 60px 40px;
  overflow: hidden;
  background: var(--memphis-bg-white);
}

.memphis-hero__content {
  max-width: 600px;
  position: relative;
  z-index: 2;
}

.memphis-hero h1 {
  font-family: 'Fredoka', sans-serif;
  font-size: clamp(3.5rem, 8vw, 7rem);
  font-weight: 700;
  line-height: 1.0;
  margin-bottom: 1.5rem;
  /* Multi-color text treatment */
}

.memphis-hero h1 span:nth-child(1) { color: var(--memphis-pink); }
.memphis-hero h1 span:nth-child(2) { color: var(--memphis-teal); }
.memphis-hero h1 span:nth-child(3) { color: var(--memphis-yellow); }

.memphis-hero p {
  font-size: 1.2rem;
  font-weight: 200;
  margin-bottom: 2.5rem;
  max-width: 480px;
}

/* Scattered background shapes */
.memphis-hero__shapes {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  z-index: 1;
  pointer-events: none;
}
```

### Navigation Bar

```css
.memphis-nav {
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 20px 40px;
  border-bottom: 3px solid var(--memphis-black);
  background: var(--memphis-bg-white);
}

.memphis-nav__logo {
  font-family: 'Fredoka', sans-serif;
  font-weight: 700;
  font-size: 1.6rem;
  color: var(--memphis-text-dark);
  text-decoration: none;
}

.memphis-nav__links {
  display: flex;
  gap: 28px;
  list-style: none;
}

.memphis-nav__links a {
  font-family: 'Fredoka', sans-serif;
  font-weight: 500;
  font-size: 1rem;
  color: var(--memphis-text-dark);
  text-decoration: none;
  text-transform: uppercase;
  letter-spacing: 0.03em;
  padding: 4px 8px;
  transition: background 0.2s ease, color 0.2s ease;
}

.memphis-nav__links a:hover {
  background: var(--memphis-yellow);
  color: var(--memphis-black);
}
```

### Section Color Blocks

```css
.memphis-section {
  padding: 80px 40px;
  position: relative;
  overflow: hidden;
}

.memphis-section--white {
  background: var(--memphis-bg-white);
  color: var(--memphis-text-dark);
}

.memphis-section--pink {
  background: var(--memphis-pink);
  color: var(--memphis-text-light);
}

.memphis-section--teal {
  background: var(--memphis-teal);
  color: var(--memphis-text-light);
}

.memphis-section--yellow {
  background: var(--memphis-yellow);
  color: var(--memphis-text-dark);
}

.memphis-section--dark {
  background: var(--memphis-bg-dark);
  color: var(--memphis-text-light);
}

.memphis-section--cream {
  background: var(--memphis-bg-cream);
  color: var(--memphis-text-dark);
}
```

### Animated Floating Shapes

```css
/* Subtle animation to keep the aesthetic feeling alive on screen */
@keyframes memphis-float {
  0%, 100% { transform: translate(0, 0) rotate(0deg); }
  25% { transform: translate(10px, -15px) rotate(5deg); }
  50% { transform: translate(-5px, -25px) rotate(-3deg); }
  75% { transform: translate(-15px, -10px) rotate(4deg); }
}

@keyframes memphis-spin {
  from { transform: rotate(0deg); }
  to { transform: rotate(360deg); }
}

.memphis-shape--float {
  animation: memphis-float 6s ease-in-out infinite;
}

.memphis-shape--float-delayed {
  animation: memphis-float 8s ease-in-out 2s infinite;
}

.memphis-shape--spin-slow {
  animation: memphis-spin 20s linear infinite;
}
```

### Grid Pattern Overlay

```css
/* Mondrian-like grid overlay for contemporary Memphis revivals */
.memphis-grid-overlay {
  background-image:
    linear-gradient(var(--memphis-black) 2px, transparent 2px),
    linear-gradient(90deg, var(--memphis-black) 2px, transparent 2px);
  background-size: 60px 60px;
  background-position: center center;
  opacity: 0.08;
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  pointer-events: none;
}
```

### Wavy Border (SVG)

```css
/* Wavy section separator */
.memphis-wavy-divider {
  width: 100%;
  height: 40px;
  background: url("data:image/svg+xml,%3Csvg width='120' height='40' xmlns='http://www.w3.org/2000/svg'%3E%3Cpath d='M0 20 Q30 0 60 20 T120 20 L120 40 L0 40 Z' fill='%23f725a0'/%3E%3C/svg%3E");
  background-size: 120px 40px;
  background-repeat: repeat-x;
}
```

---

## Signature Patterns Reference

### The Bacterio Print (Sottsass, 1978)

The most iconic Memphis pattern. Free-form squiggly lines scattered across a surface, typically black on a colored background. Translate to web by using it as a repeating SVG background on hero sections, card backgrounds, or full-page overlays at low opacity.

### Terrazzo

Speckled stone-like surfaces with irregular colored chips on a neutral base. Use CSS radial-gradients or SVG patterns for digital terrazzo. Effective for section backgrounds, card surfaces, and decorative panels.

### Grid / Mondrian Compositions

Contemporary Memphis revivals incorporate Mondrian-like grid compositions with bold color-filled rectangles. Use CSS Grid with varying cell sizes and bold, contrasting background colors.

### Confetti / Scattered Shapes

Small triangles, circles, squares, and lines scattered randomly across a surface. Create with positioned pseudo-elements, SVG sprites, or CSS gradient patterns.

---

## Related Aesthetics

| Aesthetic | Relationship to Memphis Design |
|-----------|-------------------------------|
| **Memphis Lite** | Direct commercial successor; softened Memphis motifs adapted for mass-market consumer products in the late 1980s-early 1990s |
| **Corporate Memphis** | Modern namesake descendant; borrows the bright colors and geometric shapes but strips away pattern density, irony, and maximalism |
| **Vaporwave** | Shares neon color palettes and 1980s nostalgia; Vaporwave adds digital glitch, consumerism critique, and Japanese aesthetic elements |
| **Synthwave** | Parallel retro-80s aesthetic with neon colors; focused more on grid lines, sunsets, and chrome rather than geometric patterns |
| **Pop Art** | Shares the embrace of popular culture, bold colors, and irreverence toward "high art" boundaries |
| **Flat Design** | Shares the absence of realistic textures, but Flat Design is restrained and minimal where Memphis is maximalist |
| **Neubrutalism** | Contemporary aesthetic that shares thick outlines, bold colors, and offset shadows; more raw and less playful than Memphis |
| **Kidcore** | Shares bright, primary-color palettes and playful, childlike energy |
| **Bauhaus** | Memphis was a deliberate reaction against Bauhaus-influenced functionalist minimalism; they share geometric foundations but oppose in philosophy |
| **De Stijl** | Shares the use of primary colors and geometric grids; Memphis adds chaos and pattern where De Stijl enforces order |
| **Dopamine** | Contemporary trend that shares the use of joy-inducing bright colors and maximalist aesthetics |
| **Arcadecore** | Shares 1980s-era neon colors and playful, high-energy visual language |
| **Y2K Futurism** | Later aesthetic evolution that carries forward the bold colors and geometric shapes into late-90s/early-2000s digital contexts |

---

## Quick-Start: Minimal Memphis Design Page Template

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Memphis Design Page</title>
  <link href="https://fonts.googleapis.com/css2?family=Fredoka:wght@400;500;600;700&family=Poppins:wght@200;400;700;900&display=swap" rel="stylesheet">
  <style>
    :root {
      --memphis-pink: #f725a0;
      --memphis-yellow: #fad141;
      --memphis-teal: #0cb2c0;
      --memphis-purple: #672394;
      --memphis-red: #cd2d48;
      --memphis-blue: #4458a0;
      --memphis-lime: #a8e05f;
      --memphis-orange: #ff8c42;
      --memphis-black: #000000;
      --memphis-cream: #e8e6d9;
    }

    * { margin: 0; padding: 0; box-sizing: border-box; }

    body {
      background: #ffffff;
      color: #1a1a1a;
      font-family: 'Poppins', sans-serif;
      font-weight: 200;
      line-height: 1.7;
    }

    h1, h2, h3 {
      font-family: 'Fredoka', sans-serif;
      font-weight: 700;
      line-height: 1.1;
    }

    /* Navigation */
    nav {
      display: flex;
      align-items: center;
      justify-content: space-between;
      padding: 20px 40px;
      border-bottom: 3px solid var(--memphis-black);
    }

    nav .logo {
      font-family: 'Fredoka', sans-serif;
      font-weight: 700;
      font-size: 1.5rem;
      color: var(--memphis-pink);
      text-decoration: none;
    }

    nav ul {
      display: flex;
      gap: 24px;
      list-style: none;
    }

    nav ul a {
      color: #1a1a1a;
      text-decoration: none;
      font-family: 'Fredoka', sans-serif;
      font-weight: 500;
      font-size: 0.95rem;
      text-transform: uppercase;
      letter-spacing: 0.03em;
      padding: 4px 8px;
      transition: background 0.2s, color 0.2s;
    }

    nav ul a:hover {
      background: var(--memphis-yellow);
    }

    /* Hero */
    .hero {
      position: relative;
      min-height: 85vh;
      display: flex;
      align-items: center;
      padding: 80px 40px;
      overflow: hidden;
    }

    .hero-content {
      max-width: 600px;
      position: relative;
      z-index: 2;
    }

    .hero h1 {
      font-size: clamp(3rem, 7vw, 6rem);
      margin-bottom: 1.5rem;
    }

    .hero h1 .word-1 { color: var(--memphis-pink); }
    .hero h1 .word-2 { color: var(--memphis-teal); }
    .hero h1 .word-3 { color: var(--memphis-yellow); display: inline-block; transform: rotate(-3deg); }

    .hero p {
      font-size: 1.2rem;
      margin-bottom: 2.5rem;
      max-width: 480px;
    }

    .btn {
      display: inline-block;
      background: var(--memphis-yellow);
      color: var(--memphis-black);
      border: 3px solid var(--memphis-black);
      padding: 14px 36px;
      font-family: 'Fredoka', sans-serif;
      font-weight: 700;
      font-size: 1.1rem;
      text-decoration: none;
      text-transform: uppercase;
      letter-spacing: 0.04em;
      box-shadow: 5px 5px 0 var(--memphis-black);
      transition: transform 0.15s, box-shadow 0.15s;
      cursor: pointer;
    }

    .btn:hover {
      transform: translate(-2px, -2px);
      box-shadow: 7px 7px 0 var(--memphis-black);
    }

    .btn:active {
      transform: translate(2px, 2px);
      box-shadow: 3px 3px 0 var(--memphis-black);
    }

    .btn--pink { background: var(--memphis-pink); color: #fff; }
    .btn--teal { background: var(--memphis-teal); color: #fff; }

    /* Decorative shapes */
    .shape {
      position: absolute;
      z-index: 1;
      pointer-events: none;
    }

    .shape--circle-pink {
      width: 120px; height: 120px;
      background: var(--memphis-pink);
      border-radius: 50%;
      top: 15%;
      right: 10%;
      animation: float 6s ease-in-out infinite;
    }

    .shape--triangle-yellow {
      width: 0; height: 0;
      border-left: 50px solid transparent;
      border-right: 50px solid transparent;
      border-bottom: 87px solid var(--memphis-yellow);
      top: 60%;
      right: 25%;
      transform: rotate(15deg);
      animation: float 8s ease-in-out 1s infinite;
    }

    .shape--circle-teal-outline {
      width: 160px; height: 160px;
      border: 4px solid var(--memphis-teal);
      border-radius: 50%;
      bottom: 20%;
      right: 5%;
      animation: float 7s ease-in-out 0.5s infinite;
    }

    .shape--pill-purple {
      width: 40px; height: 110px;
      background: var(--memphis-purple);
      border-radius: 20px;
      top: 30%;
      right: 40%;
      transform: rotate(30deg);
      animation: float 9s ease-in-out 2s infinite;
    }

    .shape--cross-orange {
      width: 50px; height: 50px;
      top: 70%;
      right: 45%;
      animation: float 7s ease-in-out 3s infinite;
    }
    .shape--cross-orange::before,
    .shape--cross-orange::after {
      content: '';
      position: absolute;
      background: var(--memphis-orange);
    }
    .shape--cross-orange::before {
      width: 100%; height: 10px;
      top: 50%; transform: translateY(-50%);
    }
    .shape--cross-orange::after {
      width: 10px; height: 100%;
      left: 50%; transform: translateX(-50%);
    }

    .shape--dots {
      width: 200px; height: 200px;
      top: 10%;
      right: 30%;
      background-image:
        radial-gradient(circle 4px, var(--memphis-black) 100%, transparent 100%);
      background-size: 25px 25px;
      opacity: 0.15;
    }

    @keyframes float {
      0%, 100% { transform: translate(0, 0) rotate(var(--rotation, 0deg)); }
      25% { transform: translate(8px, -12px) rotate(calc(var(--rotation, 0deg) + 3deg)); }
      50% { transform: translate(-4px, -20px) rotate(calc(var(--rotation, 0deg) - 2deg)); }
      75% { transform: translate(-12px, -8px) rotate(calc(var(--rotation, 0deg) + 2deg)); }
    }

    /* Features */
    .features {
      background: var(--memphis-cream);
      padding: 80px 40px;
      position: relative;
    }

    .features h2 {
      font-size: 2.5rem;
      text-align: center;
      margin-bottom: 3rem;
      color: var(--memphis-purple);
    }

    .features-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
      gap: 32px;
      max-width: 1100px;
      margin: 0 auto;
    }

    .feature-card {
      background: #ffffff;
      border: 3px solid var(--memphis-black);
      padding: 28px;
      box-shadow: 5px 5px 0 var(--memphis-black);
      transition: transform 0.2s, box-shadow 0.2s;
      position: relative;
    }

    .feature-card:hover {
      transform: translate(-3px, -3px);
      box-shadow: 8px 8px 0 var(--memphis-black);
    }

    .feature-card::before {
      content: '';
      position: absolute;
      top: -10px;
      right: -10px;
      width: 24px;
      height: 24px;
      border-radius: 50%;
      border: 2px solid var(--memphis-black);
    }

    .feature-card:nth-child(1)::before { background: var(--memphis-pink); }
    .feature-card:nth-child(2)::before { background: var(--memphis-yellow); }
    .feature-card:nth-child(3)::before { background: var(--memphis-teal); }

    .feature-card h3 {
      font-size: 1.3rem;
      margin-bottom: 0.75rem;
    }

    .feature-card p {
      font-size: 0.95rem;
      line-height: 1.6;
    }

    /* CTA section */
    .cta {
      background: var(--memphis-pink);
      color: #ffffff;
      text-align: center;
      padding: 80px 40px;
      border-top: 3px solid var(--memphis-black);
      border-bottom: 3px solid var(--memphis-black);
    }

    .cta h2 {
      font-size: clamp(2rem, 5vw, 3.5rem);
      margin-bottom: 1rem;
    }

    .cta p {
      font-size: 1.15rem;
      margin-bottom: 2rem;
      font-weight: 200;
      opacity: 0.9;
    }

    .cta .btn {
      background: var(--memphis-yellow);
      color: var(--memphis-black);
    }

    /* Zig-zag divider */
    .zigzag {
      width: 100%;
      height: 20px;
      background: url("data:image/svg+xml,%3Csvg width='40' height='20' xmlns='http://www.w3.org/2000/svg'%3E%3Cpolyline points='0,20 20,0 40,20' stroke='%23000' stroke-width='3' fill='none'/%3E%3C/svg%3E") repeat-x;
    }

    @media (max-width: 768px) {
      .hero {
        min-height: auto;
        padding: 60px 20px;
      }
      .hero h1 { font-size: 3rem; }
      nav { padding: 16px 20px; }
      nav ul { gap: 14px; }
      .shape { opacity: 0.6; }
    }
  </style>
</head>
<body>
  <nav>
    <a href="#" class="logo">MEMPHIS</a>
    <ul>
      <li><a href="#">About</a></li>
      <li><a href="#">Work</a></li>
      <li><a href="#">Contact</a></li>
    </ul>
  </nav>

  <section class="hero">
    <div class="hero-content">
      <h1>
        <span class="word-1">Bold.</span><br>
        <span class="word-2">Playful.</span><br>
        <span class="word-3">Electric.</span>
      </h1>
      <p>Design that rejects the ordinary, embraces the chaotic, and makes you feel something unexpected.</p>
      <a href="#" class="btn">Explore Now</a>
    </div>
    <!-- Scattered decorative shapes -->
    <div class="shape shape--circle-pink"></div>
    <div class="shape shape--triangle-yellow"></div>
    <div class="shape shape--circle-teal-outline"></div>
    <div class="shape shape--pill-purple"></div>
    <div class="shape shape--cross-orange"></div>
    <div class="shape shape--dots"></div>
  </section>

  <div class="zigzag"></div>

  <section class="features">
    <h2>What Makes It Different</h2>
    <div class="features-grid">
      <div class="feature-card">
        <h3>Geometric Chaos</h3>
        <p>Triangles, circles, squiggles, and pills scattered with joyful abandon across every surface.</p>
      </div>
      <div class="feature-card">
        <h3>Neon Palette</h3>
        <p>Hot pink, electric teal, and vibrant yellow collide in combinations that refuse to be ignored.</p>
      </div>
      <div class="feature-card">
        <h3>Pattern Overload</h3>
        <p>Terrazzo, Bacterio squiggles, and confetti layered together in deliberate, beautiful discord.</p>
      </div>
    </div>
  </section>

  <div class="zigzag"></div>

  <section class="cta">
    <h2>Ready to Break the Rules?</h2>
    <p>Memphis Design proves that more is more. Go bold or go home.</p>
    <a href="#" class="btn">Get Started</a>
  </section>
</body>
</html>
```
