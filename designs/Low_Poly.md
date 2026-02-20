# Low Poly Design Reference

Low Poly is a visual aesthetic rooted in the geometry of early 3D computer graphics, where limited polygon counts produced angular, faceted surfaces that simplified complex forms into readable crystalline shapes. Originating from the technical constraints of 1990s video game hardware -- where consoles could not render high polygon counts in real-time -- the style has evolved from a necessity into a deliberate artistic choice celebrated for its clarity, elegance, and geometric beauty. Low Poly distills the visual world into triangulated meshes, flat-shaded facets, and sharp angular edges, creating landscapes, portraits, and objects that feel simultaneously abstract and recognizable. In web and UI design, the Low Poly aesthetic translates to faceted background textures, geometric hero illustrations, crisp angular shapes, and color palettes inspired by the natural gradients visible across a crystalline surface catching light. The style prizes simplicity, intentional abstraction, and the interplay of flat color planes meeting at hard edges -- a digital origami where every triangle is a deliberate design decision.

---

## Visual Characteristics

### Core Design Traits

- **Faceted surfaces** -- objects and backgrounds composed of visible flat polygonal faces, typically triangles, that approximate curved forms through angular planes
- **Sharp geometric edges** -- hard, clean edges between polygon faces create a crystalline, gem-like quality throughout compositions
- **Flat shading per face** -- each polygon receives a single flat color or subtle gradient, making individual facets clearly visible rather than smoothly blended
- **Triangulated meshes** -- triangles are the dominant polygon type, arranged in irregular Delaunay-style tessellations across surfaces
- **Crystalline landscapes** -- mountains, water, trees, and terrain rendered as angular, faceted forms resembling cut gemstones or mineral formations
- **Visible geometry** -- the polygon structure itself is the decoration; wireframe edges and facet boundaries are features, not flaws
- **Gradient-across-facets** -- color shifts gradually across collections of polygons, with each individual facet holding a single tone, creating a stained-glass mosaic effect
- **Simplified silhouettes** -- complex organic shapes reduced to their essential angular outlines, readable at a glance
- **Depth through shading** -- light and shadow are represented by lighter and darker facets rather than smooth gradients, giving forms a chiseled, sculptural quality
- **Nature-meets-geometry** -- landscapes, animals, and organic subjects are the most iconic Low Poly subjects, bridging natural beauty with mathematical abstraction

### Design Principles

- Embrace visible polygon structure as the core visual feature, not a limitation to hide
- Use flat shading on individual facets to maintain the crystalline, gem-cut appearance
- Create depth and form through value contrast between adjacent polygon faces
- Keep polygon counts intentionally low -- the beauty is in the abstraction, not in approaching realism
- Color transitions should happen across groups of facets, never within a single polygon face
- Compositions should be immediately readable despite geometric simplification
- Light direction should be consistent and purposeful, defining form through facet brightness
- Balance regularity and irregularity in polygon tessellation -- too uniform feels mechanical, too random feels chaotic
- Let negative space and clean backgrounds frame the angular complexity of Low Poly subjects
- Every polygon should contribute to the overall form; no facet should feel arbitrary

---

## Color Palette

### Crystalline Landscape Palette

| Color Name | Hex | Role / Usage |
|------------|-----|-------------|
| **Alpine White** | `#F0EDE8` | Lightest facets, snow highlights, bright surfaces |
| **Glacier Blue** | `#7BBAD4` | Water surfaces, cool highlights, sky facets |
| **Deep Fjord** | `#2D5F7C` | Dark water, deep shadows, cool depth |
| **Twilight Indigo** | `#1B2A4A` | Deep background, night sky facets |
| **Forest Canopy** | `#3A7D44` | Primary green, vegetation facets, nature |
| **Pine Shadow** | `#1E4D2B` | Dark foliage, deep green shadows |
| **Amber Facet** | `#E8A838` | Warm accent, sunlit facets, CTAs |
| **Sunset Coral** | `#E85D3A` | Warm highlight, active states, emphasis |
| **Sandstone** | `#D4A574` | Warm neutral, terrain, earthy mid-tone |
| **Slate Rock** | `#6B7B8D` | Neutral mid-tone, stone surfaces, borders |
| **Charcoal Facet** | `#2C3038` | Dark neutral, card backgrounds, panels |
| **Obsidian** | `#1A1D23` | Primary dark background, deepest tone |
| **Quartz** | `#C8C0D0` | Light text on dark, secondary surfaces |
| **Warm Gray** | `#9B9488` | Secondary text, muted labels, captions |

### CSS Custom Properties

```css
:root {
  /* Cool tones */
  --lp-glacier: #7bbad4;
  --lp-fjord: #2d5f7c;
  --lp-indigo: #1b2a4a;

  /* Nature greens */
  --lp-forest: #3a7d44;
  --lp-pine: #1e4d2b;

  /* Warm accents */
  --lp-amber: #e8a838;
  --lp-coral: #e85d3a;
  --lp-sandstone: #d4a574;

  /* Neutrals */
  --lp-white: #f0ede8;
  --lp-quartz: #c8c0d0;
  --lp-slate: #6b7b8d;
  --lp-warm-gray: #9b9488;
  --lp-charcoal: #2c3038;
  --lp-obsidian: #1a1d23;

  /* Backgrounds */
  --lp-bg-dark: #1a1d23;
  --lp-bg-panel: #22262e;
  --lp-bg-light: #f0ede8;
  --lp-bg-mid: #e4dfd8;

  /* Text */
  --lp-text-on-dark: #e4dfd8;
  --lp-text-on-light: #2c3038;
  --lp-text-muted: #9b9488;

  /* Facet gradients */
  --lp-gradient-sky: linear-gradient(180deg, #7bbad4 0%, #2d5f7c 40%, #1b2a4a 100%);
  --lp-gradient-terrain: linear-gradient(180deg, #3a7d44 0%, #1e4d2b 50%, #2c3038 100%);
  --lp-gradient-sunset: linear-gradient(180deg, #e8a838 0%, #e85d3a 40%, #1b2a4a 100%);
  --lp-gradient-frost: linear-gradient(135deg, #f0ede8 0%, #c8c0d0 50%, #6b7b8d 100%);

  /* Shadows */
  --lp-shadow-soft: 0 4px 20px rgba(26, 29, 35, 0.15);
  --lp-shadow-hard: 4px 4px 0 rgba(26, 29, 35, 0.2);
}
```

---

## Typography

### Typeface Characteristics

Low Poly typography is:

- **Geometric and angular** -- letterforms that echo the faceted, mathematical nature of polygon meshes
- **Clean and modern** -- sans-serif faces with clear geometry that complement angular visuals without competing
- **Bold for display** -- heavy weights for headlines that hold their own against complex geometric backgrounds
- **Moderate letter-spacing** -- slightly open tracking for readability against tessellated backgrounds
- **Mixed case preferred** -- unlike neon-heavy aesthetics, Low Poly uses standard capitalization for a natural, approachable feel
- **Minimal ornamentation** -- no gradients, chrome, or glow on type; clean solid fills that match the flat-shaded polygon philosophy

### Recommended Web Fonts (Google Fonts)

| Font | Style | Best For |
|------|-------|----------|
| **Montserrat** | Geometric sans-serif | Headlines, hero text, strong display |
| **Poppins** | Geometric, rounded | Headlines, subheadings, friendly tone |
| **Raleway** | Elegant geometric | Headlines, elegant display, titles |
| **Josefin Sans** | Geometric, vintage feel | Display text, stylized headings |
| **Work Sans** | Clean geometric | Body text, versatile usage |
| **Source Sans 3** | Neutral, readable | Body text, long-form content |
| **Nunito** | Rounded geometric | Friendly body text, approachable layouts |
| **Barlow** | Slightly condensed geometric | Navigation, labels, compact UI |
| **Outfit** | Modern geometric | Body text, contemporary layouts |
| **Space Grotesk** | Geometric, technical | Code, data displays, technical labels |

### Font Pairing Suggestions

| Heading Font | Body Font | Character |
|-------------|-----------|-----------|
| **Montserrat** (700) | **Work Sans** (400) | Bold geometric, clean and professional |
| **Raleway** (600) | **Source Sans 3** (400) | Elegant angular, highly readable body |
| **Poppins** (600) | **Nunito** (400) | Friendly geometric, approachable feel |
| **Josefin Sans** (600) | **Outfit** (400) | Stylized display, modern body |
| **Barlow** (700) | **Space Grotesk** (400) | Compact bold heads, technical body |

### Typography CSS Example

```css
/* Import fonts */
@import url('https://fonts.googleapis.com/css2?family=Montserrat:wght@400;600;700&family=Work+Sans:wght@400;500&display=swap');

/* Headings */
h1, h2, h3, h4, h5, h6 {
  font-family: 'Montserrat', sans-serif;
  font-weight: 700;
  color: var(--lp-text-on-dark);
  letter-spacing: 0.02em;
  line-height: 1.2;
}

/* Display / Hero text */
.lp-display {
  font-family: 'Montserrat', sans-serif;
  font-size: clamp(2.5rem, 6vw, 5rem);
  font-weight: 700;
  letter-spacing: -0.01em;
  line-height: 1.1;
  color: var(--lp-white);
}

/* Subheading */
.lp-subhead {
  font-family: 'Montserrat', sans-serif;
  font-weight: 600;
  font-size: 1.25rem;
  letter-spacing: 0.02em;
  color: var(--lp-quartz);
}

/* Body text */
body {
  font-family: 'Work Sans', sans-serif;
  font-weight: 400;
  font-size: 1rem;
  line-height: 1.7;
  color: var(--lp-text-on-dark);
}

/* Labels and small caps */
.lp-label {
  font-family: 'Montserrat', sans-serif;
  font-size: 0.75rem;
  font-weight: 600;
  letter-spacing: 0.12em;
  text-transform: uppercase;
  color: var(--lp-text-muted);
}

/* Accent text */
.lp-accent-text {
  font-family: 'Work Sans', sans-serif;
  font-weight: 500;
  color: var(--lp-amber);
}
```

---

## Layout Principles

### Grid and Structure

- **Clean, spacious layouts** -- generous whitespace (or dark space) frames angular visual elements, preventing visual overload
- **Centered containers** -- content at 1000-1200px max-width, letting geometric backgrounds extend full-bleed behind them
- **Polygon-textured backgrounds** -- full-width sections use tessellated polygon patterns as background textures rather than flat fills
- **Angular section dividers** -- instead of horizontal rules, use CSS clip-path polygons or SVG triangles to create angled section transitions
- **Asymmetric accents** -- triangular decorative elements break up rectangular grid rigidity
- **Card-based feature grids** -- content organized into cards with subtle angular details (clipped corners, faceted borders)
- **Strong vertical rhythm** -- consistent spacing creates order that contrasts with the organic irregularity of polygon tessellations

### Section Organization

- **Navigation**: Clean bar with geometric logo mark, minimal links, optional angular underline on hover
- **Hero**: Large Low Poly landscape or abstract illustration as background, bold headline with clean type, angular CTA button
- **Features**: Grid of cards with polygon-clipped decorative accents, flat-color icon areas, concise descriptions
- **Content rows**: Text and geometric illustration side by side, alternating alignment
- **Stats/Metrics**: Large bold numbers with angular accent shapes, minimal decoration
- **CTA section**: Angular background shape (clip-path diagonal) with centered content and prominent button
- **Footer**: Dark background with clean links, small triangular decorative element

### Responsive Approach

- Maintain polygon background patterns at all breakpoints; simplify tessellation density on mobile
- Scale hero illustrations proportionally; switch from landscape to portrait crop on narrow screens
- Use `clamp()` for display typography to ensure readability at all widths
- Stack feature cards vertically on mobile; preserve angular decorative details at reduced scale
- Simplify clip-path section dividers to gentler angles on small screens
- Keep generous padding and spacing -- cramped layouts break the aesthetic

---

## CSS / Design Techniques

### Low Poly Card Component

```css
.lp-card {
  background: var(--lp-bg-panel);
  border: 1px solid rgba(107, 123, 141, 0.2);
  border-radius: 2px;
  padding: 32px;
  position: relative;
  transition: transform 0.3s ease, box-shadow 0.3s ease;
}

.lp-card:hover {
  transform: translateY(-4px);
  box-shadow: var(--lp-shadow-soft);
}

/* Angular top accent -- a triangular clip-path stripe */
.lp-card::before {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  height: 4px;
  background: linear-gradient(90deg, var(--lp-glacier), var(--lp-forest), var(--lp-amber));
}

/* Clipped corner detail */
.lp-card::after {
  content: '';
  position: absolute;
  top: 0;
  right: 0;
  width: 24px;
  height: 24px;
  background: var(--lp-bg-dark);
  clip-path: polygon(100% 0, 0 0, 100% 100%);
}

/* Card grid */
.lp-card-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
  gap: 24px;
}
```

### Low Poly Button

```css
.lp-button {
  display: inline-flex;
  align-items: center;
  justify-content: center;
  background: var(--lp-amber);
  color: var(--lp-obsidian);
  border: none;
  padding: 14px 36px;
  font-family: 'Montserrat', sans-serif;
  font-size: 0.85rem;
  font-weight: 600;
  letter-spacing: 0.06em;
  text-transform: uppercase;
  text-decoration: none;
  cursor: pointer;
  clip-path: polygon(8px 0, 100% 0, calc(100% - 8px) 100%, 0 100%);
  transition: background 0.3s ease, transform 0.2s ease;
}

.lp-button:hover {
  background: var(--lp-coral);
  transform: translateY(-2px);
}

/* Outlined variant */
.lp-button--outline {
  background: transparent;
  color: var(--lp-glacier);
  border: 2px solid var(--lp-glacier);
  clip-path: none;
}

.lp-button--outline:hover {
  background: var(--lp-glacier);
  color: var(--lp-obsidian);
}

/* Dark variant for light backgrounds */
.lp-button--dark {
  background: var(--lp-charcoal);
  color: var(--lp-white);
}

.lp-button--dark:hover {
  background: var(--lp-obsidian);
}
```

### Navigation Bar

```css
.lp-nav {
  display: flex;
  align-items: center;
  justify-content: space-between;
  max-width: 1200px;
  margin: 0 auto;
  padding: 20px 40px;
  position: relative;
  z-index: 10;
}

.lp-nav__logo {
  font-family: 'Montserrat', sans-serif;
  font-size: 1.2rem;
  font-weight: 700;
  color: var(--lp-white);
  text-decoration: none;
  letter-spacing: 0.04em;
  display: flex;
  align-items: center;
  gap: 8px;
}

/* Small diamond / triangle logo mark */
.lp-nav__logo::before {
  content: '';
  display: inline-block;
  width: 12px;
  height: 12px;
  background: var(--lp-amber);
  clip-path: polygon(50% 0%, 100% 50%, 50% 100%, 0% 50%);
}

.lp-nav__links {
  display: flex;
  gap: 28px;
  list-style: none;
  margin: 0;
  padding: 0;
}

.lp-nav__links a {
  font-family: 'Work Sans', sans-serif;
  font-weight: 500;
  font-size: 0.9rem;
  color: var(--lp-text-muted);
  text-decoration: none;
  letter-spacing: 0.03em;
  transition: color 0.2s ease;
  position: relative;
}

.lp-nav__links a:hover {
  color: var(--lp-glacier);
}

/* Angular underline on hover */
.lp-nav__links a::after {
  content: '';
  position: absolute;
  bottom: -4px;
  left: 0;
  right: 0;
  height: 2px;
  background: var(--lp-glacier);
  clip-path: polygon(4px 0, 100% 0, calc(100% - 4px) 100%, 0 100%);
  transform: scaleX(0);
  transform-origin: left;
  transition: transform 0.2s ease;
}

.lp-nav__links a:hover::after {
  transform: scaleX(1);
}
```

### Hero Section with Polygon Background

```css
.lp-hero {
  position: relative;
  min-height: 90vh;
  display: flex;
  align-items: center;
  justify-content: center;
  text-align: center;
  padding: 80px 40px;
  background: var(--lp-bg-dark);
  overflow: hidden;
}

/* Inline SVG polygon mesh background -- use an actual SVG for production */
.lp-hero__mesh {
  position: absolute;
  inset: 0;
  opacity: 0.35;
  background:
    linear-gradient(135deg, var(--lp-fjord) 0%, var(--lp-indigo) 50%, var(--lp-obsidian) 100%);
  z-index: 1;
}

/* Angular bottom edge -- section divider */
.lp-hero::after {
  content: '';
  position: absolute;
  bottom: 0;
  left: 0;
  right: 0;
  height: 80px;
  background: var(--lp-bg-dark);
  clip-path: polygon(0 100%, 100% 100%, 100% 0, 50% 60%, 0 20%);
  z-index: 3;
}

.lp-hero__content {
  position: relative;
  z-index: 5;
  max-width: 800px;
}

.lp-hero__content h1 {
  font-size: clamp(2.5rem, 6vw, 5rem);
  font-weight: 700;
  margin-bottom: 1.5rem;
  color: var(--lp-white);
}

.lp-hero__content p {
  font-size: 1.15rem;
  color: var(--lp-quartz);
  margin-bottom: 2.5rem;
  max-width: 600px;
  margin-left: auto;
  margin-right: auto;
}

@media (max-width: 768px) {
  .lp-hero { min-height: auto; padding: 60px 20px; }
  .lp-hero::after { height: 40px; }
}
```

### CSS Clip-Path Angular Section Divider

```css
/* Angled section transition using clip-path */
.lp-section--angled {
  position: relative;
  padding: 100px 40px 80px;
  background: var(--lp-bg-panel);
  clip-path: polygon(
    0 40px,
    100% 0,
    100% calc(100% - 40px),
    0 100%
  );
  margin: -40px 0;
}

/* Zigzag / mountain-ridge divider */
.lp-divider-ridge {
  width: 100%;
  height: 60px;
  background: var(--lp-bg-dark);
  clip-path: polygon(
    0% 100%,
    8% 40%,
    16% 70%,
    24% 20%,
    32% 55%,
    40% 10%,
    48% 45%,
    56% 15%,
    64% 50%,
    72% 25%,
    80% 60%,
    88% 30%,
    100% 65%,
    100% 100%
  );
}

/* Simple diagonal divider */
.lp-divider-diagonal {
  width: 100%;
  height: 80px;
  background: var(--lp-bg-panel);
  clip-path: polygon(0 0, 100% 100%, 0 100%);
}
```

### Inline SVG Polygon Mesh Background

```css
/*
  For a true Low Poly background, generate an SVG mesh of triangles.
  This technique uses an inline SVG with polygon elements, each
  filled with a slightly different shade. Below is the CSS to
  position and style such a mesh.
*/

.lp-mesh-container {
  position: relative;
  overflow: hidden;
}

.lp-mesh-container svg.lp-mesh {
  position: absolute;
  inset: 0;
  width: 100%;
  height: 100%;
  z-index: 0;
}

.lp-mesh-container svg.lp-mesh polygon {
  stroke: rgba(255, 255, 255, 0.03);
  stroke-width: 0.5;
  transition: fill 0.4s ease;
}

/* Optional: subtle hover interaction on individual facets */
.lp-mesh-container svg.lp-mesh polygon:hover {
  fill-opacity: 0.85;
  stroke: rgba(255, 255, 255, 0.1);
}

/* Content sits above the mesh */
.lp-mesh-container .lp-content {
  position: relative;
  z-index: 1;
}
```

### Faceted Icon / Shape with CSS

```css
/* Diamond shape -- rotated square */
.lp-diamond {
  width: 48px;
  height: 48px;
  background: var(--lp-amber);
  transform: rotate(45deg);
  display: flex;
  align-items: center;
  justify-content: center;
}

.lp-diamond__icon {
  transform: rotate(-45deg);
  color: var(--lp-obsidian);
  font-size: 1.2rem;
}

/* Hexagonal badge */
.lp-hexagon {
  width: 60px;
  height: 60px;
  background: var(--lp-glacier);
  clip-path: polygon(50% 0%, 100% 25%, 100% 75%, 50% 100%, 0% 75%, 0% 25%);
  display: flex;
  align-items: center;
  justify-content: center;
  color: var(--lp-obsidian);
}

/* Triangular accent */
.lp-triangle {
  width: 0;
  height: 0;
  border-left: 20px solid transparent;
  border-right: 20px solid transparent;
  border-bottom: 35px solid var(--lp-coral);
}

/* Pentagon clip */
.lp-pentagon {
  width: 56px;
  height: 56px;
  background: var(--lp-forest);
  clip-path: polygon(50% 0%, 100% 38%, 82% 100%, 18% 100%, 0% 38%);
}
```

---

## Design Do's and Don'ts

### Do

- Use triangulated polygon patterns as background textures and decorative elements
- Apply flat, single-color shading to each polygon facet for the authentic crystalline look
- Create angular section dividers with CSS `clip-path` instead of straight horizontal lines
- Choose color palettes inspired by nature: mountain ranges, oceans, forests, sunsets
- Maintain generous whitespace (or dark space) to let angular geometry breathe
- Use geometric sans-serif typefaces that harmonize with the mathematical aesthetic
- Include subtle variation in facet colors -- adjacent triangles should differ slightly in hue or value
- Keep decorative shapes angular: diamonds, hexagons, pentagons, triangles
- Use consistent light direction across faceted illustrations for believable form

### Don't

- Use rounded corners, circles, or soft organic shapes as primary design elements -- these conflict with the angular aesthetic
- Apply smooth gradients within individual polygon facets -- each face should be flat-shaded
- Over-complicate polygon meshes to the point they approach photorealism -- the beauty is in visible abstraction
- Use overly ornate or decorative typefaces -- keep typography clean and geometric
- Mix too many saturated colors in adjacent facets -- maintain color harmony across the tessellation
- Add drop shadows or heavy depth effects that contradict the flat-faceted philosophy
- Use the same polygon size uniformly -- natural-feeling tessellations vary in triangle size and proportion
- Forget to include a clear visual hierarchy -- angular complexity can overwhelm without structured layout
- Apply blur or soft-focus effects -- Low Poly is defined by sharp, crisp edges

---

## Related Aesthetics

| Aesthetic | Relationship to Low Poly |
|-----------|-------------------------|
| **Geometric** | Both celebrate mathematical shapes; Geometric is broader and includes circles, curves, and patterns; Low Poly is specifically about faceted 3D surfaces |
| **Flat Design** | Shares the flat-color, minimal-shadow approach; Flat Design applies to UI elements and icons broadly, Low Poly specifically to tessellated polygon meshes |
| **Isometric Design** | Both represent 3D forms in 2D; Isometric uses parallel projection and clean cubes, Low Poly uses irregular triangle meshes and faceted surfaces |
| **Material Design** | Both use flat color planes; Material Design adds elevation and shadow hierarchy, Low Poly uses faceted shading for depth |
| **Minimalism** | Low Poly is a form of minimalism applied to 3D representation -- reducing forms to their essential geometric components |
| **Voxel Art** | Both simplify 3D forms; Voxel uses cubes (like 3D pixels), Low Poly uses triangulated polygon meshes for smoother approximations |
| **Origami** | Both create form through flat planes meeting at angles; Origami references paper folding, Low Poly references digital polygon meshes |
| **Crystalline / Gem** | The closest natural analog to Low Poly -- mineral formations with flat crystal faces and sharp edges mirror polygon mesh geometry |
| **Brutalist Web Design** | Both embrace visible structure; Brutalism exposes raw HTML/layout, Low Poly exposes raw polygon geometry |

---

## Quick-Start: Minimal Low Poly Page Template

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Low Poly Page</title>
  <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@400;600;700&family=Work+Sans:wght@400;500&display=swap" rel="stylesheet">
  <style>
    :root {
      --lp-glacier: #7bbad4;
      --lp-fjord: #2d5f7c;
      --lp-indigo: #1b2a4a;
      --lp-forest: #3a7d44;
      --lp-pine: #1e4d2b;
      --lp-amber: #e8a838;
      --lp-coral: #e85d3a;
      --lp-sandstone: #d4a574;
      --lp-white: #f0ede8;
      --lp-quartz: #c8c0d0;
      --lp-slate: #6b7b8d;
      --lp-warm-gray: #9b9488;
      --lp-charcoal: #2c3038;
      --lp-obsidian: #1a1d23;
      --lp-bg-dark: #1a1d23;
      --lp-bg-panel: #22262e;
      --lp-text-on-dark: #e4dfd8;
      --lp-text-muted: #9b9488;
    }

    * { margin: 0; padding: 0; box-sizing: border-box; }

    body {
      background: var(--lp-bg-dark);
      color: var(--lp-text-on-dark);
      font-family: 'Work Sans', sans-serif;
      font-size: 1rem;
      line-height: 1.7;
    }

    h1, h2, h3 {
      font-family: 'Montserrat', sans-serif;
      font-weight: 700;
      letter-spacing: 0.02em;
      line-height: 1.2;
    }

    /* ---- Navigation ---- */
    nav {
      display: flex;
      align-items: center;
      justify-content: space-between;
      max-width: 1200px;
      margin: 0 auto;
      padding: 20px 40px;
      position: relative;
      z-index: 10;
    }

    nav a.logo {
      font-family: 'Montserrat', sans-serif;
      font-size: 1.15rem;
      font-weight: 700;
      color: var(--lp-white);
      text-decoration: none;
      letter-spacing: 0.04em;
      display: flex;
      align-items: center;
      gap: 8px;
    }

    nav a.logo::before {
      content: '';
      display: inline-block;
      width: 12px;
      height: 12px;
      background: var(--lp-amber);
      clip-path: polygon(50% 0%, 100% 50%, 50% 100%, 0% 50%);
    }

    nav ul {
      display: flex;
      gap: 28px;
      list-style: none;
    }

    nav ul a {
      font-family: 'Work Sans', sans-serif;
      font-weight: 500;
      font-size: 0.9rem;
      color: var(--lp-text-muted);
      text-decoration: none;
      transition: color 0.2s;
    }

    nav ul a:hover {
      color: var(--lp-glacier);
    }

    /* ---- Hero with SVG polygon mesh ---- */
    .hero {
      position: relative;
      min-height: 90vh;
      display: flex;
      align-items: center;
      justify-content: center;
      text-align: center;
      padding: 80px 40px;
      overflow: hidden;
    }

    .hero svg.mesh {
      position: absolute;
      inset: 0;
      width: 100%;
      height: 100%;
      z-index: 0;
    }

    .hero svg.mesh polygon {
      stroke: rgba(255, 255, 255, 0.04);
      stroke-width: 0.5;
    }

    .hero-content {
      position: relative;
      z-index: 5;
      max-width: 760px;
    }

    .hero h1 {
      font-size: clamp(2.5rem, 6vw, 4.5rem);
      margin-bottom: 1.5rem;
      color: var(--lp-white);
    }

    .hero p {
      font-size: 1.15rem;
      color: var(--lp-quartz);
      margin-bottom: 2.5rem;
      max-width: 560px;
      margin-left: auto;
      margin-right: auto;
    }

    .btn {
      display: inline-block;
      background: var(--lp-amber);
      color: var(--lp-obsidian);
      border: none;
      padding: 14px 36px;
      font-family: 'Montserrat', sans-serif;
      font-size: 0.85rem;
      font-weight: 600;
      letter-spacing: 0.06em;
      text-transform: uppercase;
      text-decoration: none;
      cursor: pointer;
      clip-path: polygon(8px 0, 100% 0, calc(100% - 8px) 100%, 0 100%);
      transition: background 0.3s, transform 0.2s;
    }

    .btn:hover {
      background: var(--lp-coral);
      transform: translateY(-2px);
    }

    /* ---- Angular Section Divider ---- */
    .divider-ridge {
      width: 100%;
      height: 50px;
      background: var(--lp-bg-panel);
      clip-path: polygon(
        0% 100%,
        5% 50%,
        12% 80%,
        20% 30%,
        28% 65%,
        36% 15%,
        44% 55%,
        52% 10%,
        60% 50%,
        68% 20%,
        76% 60%,
        84% 25%,
        92% 70%,
        100% 40%,
        100% 100%
      );
    }

    /* ---- Features Section ---- */
    .features {
      padding: 80px 0;
      background: var(--lp-bg-panel);
    }

    .features h2 {
      text-align: center;
      font-size: 1.8rem;
      color: var(--lp-glacier);
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
      background: var(--lp-bg-dark);
      border: 1px solid rgba(107, 123, 141, 0.15);
      border-radius: 2px;
      padding: 32px;
      position: relative;
      transition: transform 0.3s, box-shadow 0.3s;
    }

    .feature:hover {
      transform: translateY(-4px);
      box-shadow: 0 8px 30px rgba(0, 0, 0, 0.3);
    }

    .feature::before {
      content: '';
      position: absolute;
      top: 0; left: 0; right: 0;
      height: 3px;
      background: linear-gradient(90deg, var(--lp-glacier), var(--lp-forest), var(--lp-amber));
    }

    .feature::after {
      content: '';
      position: absolute;
      top: 0;
      right: 0;
      width: 20px;
      height: 20px;
      background: var(--lp-bg-panel);
      clip-path: polygon(100% 0, 0 0, 100% 100%);
    }

    .feature-icon {
      width: 44px;
      height: 44px;
      background: var(--lp-fjord);
      clip-path: polygon(50% 0%, 100% 25%, 100% 75%, 50% 100%, 0% 75%, 0% 25%);
      display: flex;
      align-items: center;
      justify-content: center;
      margin-bottom: 20px;
      font-size: 1.1rem;
    }

    .feature h3 {
      font-size: 1.05rem;
      margin-bottom: 0.75rem;
      color: var(--lp-white);
    }

    .feature p {
      color: var(--lp-text-muted);
      font-size: 0.95rem;
    }

    /* ---- Stats Section ---- */
    .stats {
      padding: 60px 40px;
      background: var(--lp-bg-dark);
    }

    .stats-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(160px, 1fr));
      gap: 32px;
      max-width: 900px;
      margin: 0 auto;
      text-align: center;
    }

    .stat-number {
      font-family: 'Montserrat', sans-serif;
      font-size: 2.8rem;
      font-weight: 700;
      color: var(--lp-amber);
      line-height: 1.1;
      margin-bottom: 8px;
    }

    .stat-label {
      font-family: 'Montserrat', sans-serif;
      font-size: 0.75rem;
      font-weight: 600;
      letter-spacing: 0.1em;
      text-transform: uppercase;
      color: var(--lp-text-muted);
    }

    /* ---- CTA Section with angular clip ---- */
    .cta {
      position: relative;
      text-align: center;
      padding: 100px 40px 80px;
      background: var(--lp-indigo);
      clip-path: polygon(0 30px, 100% 0, 100% calc(100% - 30px), 0 100%);
      margin: -30px 0;
    }

    .cta h2 {
      font-size: 2rem;
      color: var(--lp-white);
      margin-bottom: 1rem;
    }

    .cta p {
      color: var(--lp-quartz);
      margin-bottom: 2rem;
      max-width: 500px;
      margin-left: auto;
      margin-right: auto;
    }

    .btn--light {
      background: var(--lp-white);
      color: var(--lp-indigo);
    }

    .btn--light:hover {
      background: var(--lp-glacier);
      color: var(--lp-obsidian);
    }

    /* ---- Footer ---- */
    footer {
      background: #12141a;
      text-align: center;
      padding: 30px 40px;
      color: var(--lp-text-muted);
      font-size: 0.85rem;
    }

    footer span {
      color: var(--lp-slate);
    }

    /* ---- Responsive ---- */
    @media (max-width: 768px) {
      .hero { min-height: auto; padding: 60px 20px; }
      nav { padding: 16px 20px; }
      nav ul { gap: 16px; }
      .cta { clip-path: polygon(0 15px, 100% 0, 100% calc(100% - 15px), 0 100%); }
      .features { padding: 60px 0; }
      .stats { padding: 40px 20px; }
    }
  </style>
</head>
<body>
  <nav>
    <a href="#" class="logo">Vertex</a>
    <ul>
      <li><a href="#">Terrain</a></li>
      <li><a href="#">Craft</a></li>
      <li><a href="#">Gallery</a></li>
      <li><a href="#">About</a></li>
    </ul>
  </nav>

  <!-- Hero with inline SVG polygon mesh -->
  <section class="hero">
    <svg class="mesh" viewBox="0 0 1200 700" preserveAspectRatio="xMidYMid slice" xmlns="http://www.w3.org/2000/svg">
      <!-- Row 1: Sky facets -->
      <polygon points="0,0 200,0 100,90" fill="#1b2a4a"/>
      <polygon points="200,0 100,90 240,110" fill="#1f3358"/>
      <polygon points="200,0 400,0 240,110" fill="#233c66"/>
      <polygon points="400,0 240,110 380,95" fill="#1f3358"/>
      <polygon points="400,0 600,0 380,95" fill="#1b2a4a"/>
      <polygon points="600,0 380,95 550,100" fill="#263f6a"/>
      <polygon points="600,0 800,0 550,100" fill="#2d5f7c"/>
      <polygon points="800,0 550,100 740,85" fill="#233c66"/>
      <polygon points="800,0 1000,0 740,85" fill="#1f3358"/>
      <polygon points="1000,0 740,85 960,95" fill="#1b2a4a"/>
      <polygon points="1000,0 1200,0 960,95" fill="#233c66"/>
      <polygon points="1200,0 960,95 1200,110" fill="#1f3358"/>

      <!-- Row 2: Upper sky -->
      <polygon points="0,0 100,90 0,180" fill="#233c66"/>
      <polygon points="100,90 240,110 160,200" fill="#2d5f7c"/>
      <polygon points="240,110 380,95 300,190" fill="#1b2a4a"/>
      <polygon points="380,95 550,100 470,195" fill="#233c66"/>
      <polygon points="550,100 740,85 630,200" fill="#2d5f7c"/>
      <polygon points="740,85 960,95 820,185" fill="#1f3358"/>
      <polygon points="960,95 1200,110 1060,195" fill="#233c66"/>
      <polygon points="1200,110 1060,195 1200,200" fill="#1b2a4a"/>

      <!-- Row 3: Mountain peaks -->
      <polygon points="0,180 160,200 80,290" fill="#2d5f7c"/>
      <polygon points="160,200 300,190 220,300" fill="#3a7d44"/>
      <polygon points="160,200 220,300 80,290" fill="#1e4d2b"/>
      <polygon points="300,190 470,195 370,310" fill="#2d5f7c"/>
      <polygon points="300,190 370,310 220,300" fill="#3a7d44"/>
      <polygon points="470,195 630,200 540,280" fill="#1e4d2b"/>
      <polygon points="470,195 540,280 370,310" fill="#2d5f7c"/>
      <polygon points="630,200 820,185 710,300" fill="#3a7d44"/>
      <polygon points="630,200 710,300 540,280" fill="#1e4d2b"/>
      <polygon points="820,185 1060,195 920,290" fill="#2d5f7c"/>
      <polygon points="820,185 920,290 710,300" fill="#3a7d44"/>
      <polygon points="1060,195 1200,200 1120,300" fill="#1e4d2b"/>
      <polygon points="1060,195 1120,300 920,290" fill="#2d5f7c"/>
      <polygon points="1200,200 1200,300 1120,300" fill="#3a7d44"/>
      <polygon points="0,180 80,290 0,310" fill="#1e4d2b"/>

      <!-- Row 4: Mountain body -->
      <polygon points="0,310 80,290 60,400" fill="#1e4d2b"/>
      <polygon points="80,290 220,300 150,400" fill="#3a7d44"/>
      <polygon points="220,300 370,310 280,410" fill="#1e4d2b"/>
      <polygon points="370,310 540,280 450,400" fill="#3a7d44"/>
      <polygon points="540,280 710,300 620,395" fill="#2d5f7c"/>
      <polygon points="710,300 920,290 800,400" fill="#1e4d2b"/>
      <polygon points="920,290 1120,300 1000,410" fill="#3a7d44"/>
      <polygon points="1120,300 1200,300 1200,400" fill="#2d5f7c"/>
      <polygon points="1120,300 1200,400 1000,410" fill="#1e4d2b"/>
      <polygon points="0,310 60,400 0,420" fill="#3a7d44"/>

      <!-- Row 5: Foothills -->
      <polygon points="0,420 60,400 150,400" fill="#2d5f7c"/>
      <polygon points="0,420 150,400 120,500" fill="#d4a574"/>
      <polygon points="150,400 280,410 200,510" fill="#9b9488"/>
      <polygon points="280,410 450,400 350,500" fill="#d4a574"/>
      <polygon points="450,400 620,395 530,510" fill="#6b7b8d"/>
      <polygon points="620,395 800,400 700,505" fill="#d4a574"/>
      <polygon points="800,400 1000,410 880,500" fill="#9b9488"/>
      <polygon points="1000,410 1200,400 1080,510" fill="#d4a574"/>
      <polygon points="1200,400 1200,510 1080,510" fill="#6b7b8d"/>
      <polygon points="0,420 120,500 0,520" fill="#9b9488"/>

      <!-- Row 6: Water -->
      <polygon points="0,520 120,500 100,600" fill="#2d5f7c"/>
      <polygon points="120,500 200,510 180,590" fill="#7bbad4"/>
      <polygon points="200,510 350,500 280,600" fill="#2d5f7c"/>
      <polygon points="350,500 530,510 440,595" fill="#7bbad4"/>
      <polygon points="530,510 700,505 610,600" fill="#2d5f7c"/>
      <polygon points="700,505 880,500 780,590" fill="#7bbad4"/>
      <polygon points="880,500 1080,510 960,600" fill="#2d5f7c"/>
      <polygon points="1080,510 1200,510 1200,590" fill="#7bbad4"/>
      <polygon points="1080,510 1200,590 960,600" fill="#2d5f7c"/>
      <polygon points="0,520 100,600 0,610" fill="#7bbad4"/>

      <!-- Row 7: Deep water / bottom -->
      <polygon points="0,610 100,600 80,700" fill="#1b2a4a"/>
      <polygon points="100,600 180,590 200,700" fill="#2d5f7c"/>
      <polygon points="180,590 280,600 300,700" fill="#1b2a4a"/>
      <polygon points="280,600 440,595 400,700" fill="#2d5f7c"/>
      <polygon points="440,595 610,600 560,700" fill="#1b2a4a"/>
      <polygon points="610,600 780,590 720,700" fill="#2d5f7c"/>
      <polygon points="780,590 960,600 880,700" fill="#1b2a4a"/>
      <polygon points="960,600 1200,590 1060,700" fill="#2d5f7c"/>
      <polygon points="1200,590 1200,700 1060,700" fill="#1b2a4a"/>
      <polygon points="0,610 80,700 0,700" fill="#2d5f7c"/>
      <polygon points="80,700 200,700 150,700" fill="#1b2a4a"/>
      <polygon points="300,700 400,700 350,700" fill="#2d5f7c"/>
      <polygon points="560,700 720,700 640,700" fill="#1b2a4a"/>
      <polygon points="880,700 1060,700 970,700" fill="#2d5f7c"/>
    </svg>

    <div class="hero-content">
      <h1>Crystalline Horizons</h1>
      <p>Where geometry meets nature. Every surface tells a story through facets of light and angular beauty.</p>
      <a href="#" class="btn">Explore</a>
    </div>
  </section>

  <div class="divider-ridge"></div>

  <section class="features">
    <h2>Faceted Features</h2>
    <div class="features-grid">
      <div class="feature">
        <div class="feature-icon">&#9650;</div>
        <h3>Polygon Mesh</h3>
        <p>Surfaces built from tessellated triangles, each facet catching light at its own angle. Complexity emerges from simplicity.</p>
      </div>
      <div class="feature">
        <div class="feature-icon">&#9670;</div>
        <h3>Flat Shading</h3>
        <p>Every polygon face carries a single tone. No smooth gradients blur the boundaries between geometric planes.</p>
      </div>
      <div class="feature">
        <div class="feature-icon">&#11042;</div>
        <h3>Angular Forms</h3>
        <p>Sharp edges and clean vertices define every shape. Curves are approximated through carefully arranged straight lines.</p>
      </div>
    </div>
  </section>

  <section class="stats">
    <div class="stats-grid">
      <div>
        <div class="stat-number">2,048</div>
        <div class="stat-label">Polygons</div>
      </div>
      <div>
        <div class="stat-number">1,024</div>
        <div class="stat-label">Vertices</div>
      </div>
      <div>
        <div class="stat-number">3</div>
        <div class="stat-label">Dimensions</div>
      </div>
      <div>
        <div class="stat-number">60</div>
        <div class="stat-label">FPS</div>
      </div>
    </div>
  </section>

  <section class="cta">
    <h2>Build Your Terrain</h2>
    <p>Every mountain begins with a single triangle. Start shaping your crystalline world today.</p>
    <a href="#" class="btn btn--light">Create</a>
  </section>

  <footer>
    <p>VERTEX STUDIO <span>//</span> Crafted in polygons since the first render</p>
  </footer>
</body>
</html>
```
