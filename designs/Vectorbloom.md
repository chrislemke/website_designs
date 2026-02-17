# Vectorbloom Design Reference

Vectorbloom is a digitally-driven decorative aesthetic from the early 2000s through the early 2010s, born from the era's fascination with vector graphic tools and their capacity for intricate image manipulation. It applies **maximalist floral and organic patterns**, **psychedelic color**, and **digitally precise vector ornament** to flat surfaces -- walls, ceilings, furniture, packaging, and screens. Drawing from 1960s Psychedelia, 1970s Supergraphic Ultramodern muralism, and Art Nouveau's organic curves, Vectorbloom translates these influences into a distinctly digital idiom: complex, layered, and seamlessly repeating compositions of flourishes, hybrid creatures, and blooming floral forms rendered with the precision only vector tools can achieve. The aesthetic celebrates **technological opulence**, **visual density**, and **psychedelic fantasy**.

---

## Visual Characteristics

### Core Motifs and Patterns

- **Blooming floral forms** -- elaborate, digitally rendered flowers, petals, and botanical elements that appear to unfurl and expand across surfaces
- **Flourishes and scrollwork** -- sinuous vector curves, tendrils, and ornamental swirls inspired by Art Nouveau whiplash lines
- **Hybrid creatures** -- abstract aquatic or fantastical organisms composed of organic and geometric elements, blending natural and digital forms
- **Multi-layered imagery** -- dense, stacked compositions where elements overlap, interweave, and flow into one another
- **Psychedelic organic shapes** -- amorphous, flowing forms reminiscent of 1960s psychedelic poster art, rendered with digital crispness
- **Seamless, environment-spanning patterns** -- designs that function as continuous imagery across walls, ceilings, floors, and surfaces without visible seams or endpoints
- **Vector-precise linework** -- clean, sharp Bezier curves with no hand-drawn imperfection; the digital tool is part of the aesthetic identity
- **Symmetry and mirroring** -- kaleidoscopic arrangements where motifs mirror and rotate to create complex radial or bilateral compositions
- **Decorative filigree** -- fine, intricate ornamental vector detail filling negative space

### Design Principles

- **Maximalism** -- more is more; every surface is an opportunity for intricate visual density
- **Flat surface application** -- designs are applied to flat planes (walls, screens, furniture panels) rather than sculpted in 3D; occasional pseudo-3D effects add subtle depth
- **Dramatic gradients on flat fills** -- while fundamentally flat, colors transition through bold gradients within shapes, creating luminous, glowing effects
- **Digital precision** -- the cleanness and mathematical perfection of vector software is embraced, not hidden
- **Environmental immersion** -- patterns are designed to envelop and transform entire spaces, not merely decorate isolated objects
- **Organic forms through digital means** -- natural, botanical, and biological shapes rendered with technological precision create the distinctive Vectorbloom tension
- **Color as atmosphere** -- saturated, vivid palettes create psychedelic mood and emotional intensity

---

## Color Palette

### Primary Scheme

Vectorbloom uses a **vivid, saturated, and wide-ranging palette** anchored by pinks, magentas, purples, and blues, with green, yellow, and red accents. Black provides contrast and grounding; white appears as highlights and negative space. Colors are applied in bold gradients and flat fills, never muted or earthy.

| Role | Colors | Hex (suggested) |
|------|--------|-----------------|
| **Hot Pink / Magenta** | Vivid pink, deep magenta | `#FF2D8A`, `#E91E8C` |
| **Fuchsia** | Bright fuchsia, electric pink | `#FF00FF`, `#D946EF` |
| **Deep Purple** | Rich violet, royal purple | `#7B2D8E`, `#6B21A8` |
| **Soft Lavender** | Light purple, mauve | `#C084FC`, `#DDA0DD` |
| **Electric Blue** | Vivid sky blue, cyan-blue | `#00A3FF`, `#38BDF8` |
| **Deep Teal** | Dark aqua, blue-green | `#0D9488`, `#0E7490` |
| **Lime Green** | Vivid chartreuse, acid green | `#84CC16`, `#A3E635` |
| **Emerald Green** | Rich green, botanical | `#10B981`, `#22C55E` |
| **Warm Yellow** | Golden yellow, amber | `#FACC15`, `#F59E0B` |
| **Coral Red** | Warm red, red-orange | `#EF4444`, `#F97316` |
| **Background (Light)** | Soft mauve, pale pink | `#F5D6F5`, `#FDF2F8` |
| **Background (Dark)** | Deep plum, near-black violet | `#1E0A2E`, `#0F0520` |
| **Black** | True black, rich black | `#000000`, `#0A0A12` |
| **White** | Pure white, soft cream | `#FFFFFF`, `#FFF5F9` |

### Suggested CSS Custom Properties

```css
:root {
  /* Signature pinks and magentas */
  --vb-hot-pink: #ff2d8a;
  --vb-magenta: #e91e8c;
  --vb-fuchsia: #d946ef;
  --vb-soft-pink: #f9a8d4;

  /* Purples */
  --vb-deep-purple: #7b2d8e;
  --vb-royal-purple: #6b21a8;
  --vb-lavender: #c084fc;
  --vb-mauve: #dda0dd;

  /* Blues and teals */
  --vb-electric-blue: #00a3ff;
  --vb-sky-blue: #38bdf8;
  --vb-deep-teal: #0d9488;
  --vb-cyan: #06b6d4;

  /* Greens */
  --vb-lime: #84cc16;
  --vb-emerald: #10b981;

  /* Warm accents */
  --vb-yellow: #facc15;
  --vb-coral: #ef4444;
  --vb-orange: #f97316;

  /* Backgrounds */
  --vb-bg-light: #f5d6f5;
  --vb-bg-pale: #fdf2f8;
  --vb-bg-dark: #1e0a2e;
  --vb-bg-deep: #0f0520;

  /* Neutrals */
  --vb-black: #0a0a12;
  --vb-white: #ffffff;
  --vb-off-white: #fff5f9;

  /* Functional mappings */
  --vb-bg-primary: var(--vb-bg-light);
  --vb-bg-secondary: var(--vb-bg-pale);
  --vb-text-primary: var(--vb-black);
  --vb-text-on-dark: var(--vb-off-white);
  --vb-accent: var(--vb-hot-pink);
  --vb-accent-secondary: var(--vb-fuchsia);
}
```

### Color Guidelines

- **Vivid and saturated** -- Vectorbloom colors are bold and electric, never dusty, pastel, or muted
- **Dramatic gradients** within shapes are a defining characteristic; colors flow from hot pink to purple to blue within a single form
- **Multi-hue compositions** -- unlike monochromatic aesthetics, Vectorbloom freely uses the full spectrum within a single composition
- **Black as grounding contrast** -- black outlines, backgrounds, or negative space anchor the vivid colors and prevent visual chaos
- **Pink-purple-blue axis dominates** -- the signature Vectorbloom color story moves through magenta, violet, and blue; green and yellow are supporting accents
- **Light backgrounds** use soft mauves, pale pinks, and lavender tints to maintain the warm, floral atmosphere
- **Dark backgrounds** use deep plum and near-black violet, creating a nocturnal psychedelic mood

---

## Typography

### Typeface Characteristics

Vectorbloom typography balances decorative elegance with digital modernity:

- **Clean, rounded sans-serifs** for body text -- modern and legible, complementing rather than competing with ornate visuals
- **Decorative display typefaces** for headings -- flowing, curvy, or playfully stylized fonts that echo the organic vector motifs
- **Generous, open letter-spacing** -- letting type breathe within dense visual environments
- **No harsh, angular, or industrial type** -- typography should feel organic, fluid, and approachable
- **Color-integrated type** -- headings may use gradient fills or be colored to match the surrounding palette
- **Occasional script or calligraphic accents** -- for decorative labels or short display text, referencing Art Nouveau lettering

### Recommended Web Fonts (Google Fonts)

| Font | Style | Usage |
|------|-------|-------|
| **Rubik** | Rounded geometric sans | Body text, headings (the aesthetic's signature typeface) |
| **Quicksand** | Rounded, soft geometric sans | Headlines, feature titles, display text |
| **Comfortaa** | Rounded, futuristic geometric | Display headings, decorative titles |
| **Nunito** | Soft, rounded sans-serif | Body text, subheadings |
| **Josefin Sans** | Elegant geometric sans with vintage feel | Section titles, navigation |
| **Pacifico** | Flowing brush script | Decorative accents, short display text |
| **Dancing Script** | Casual calligraphic script | Pull quotes, decorative labels |
| **Tenor Sans** | Clean serif-like sans with elegance | Formal headings, refined body copy |
| **Fredoka** | Rounded, playful sans-serif | Friendly display headings, bold accents |

### Typography CSS Example

```css
@import url('https://fonts.googleapis.com/css2?family=Rubik:ital,wght@0,300;0,400;0,600;0,700;1,400&family=Quicksand:wght@400;500;600;700&family=Comfortaa:wght@400;600;700&family=Pacifico&display=swap');

/* Headlines */
h1, h2, h3 {
  font-family: 'Quicksand', 'Comfortaa', 'Rubik', sans-serif;
  font-weight: 700;
  color: var(--vb-deep-purple);
  letter-spacing: 0.02em;
  line-height: 1.15;
}

/* Display / Hero text */
.vb-display {
  font-family: 'Comfortaa', 'Quicksand', sans-serif;
  font-size: clamp(2.5rem, 7vw, 6rem);
  font-weight: 700;
  letter-spacing: 0.04em;
  line-height: 1.05;
  background: linear-gradient(135deg, var(--vb-hot-pink), var(--vb-fuchsia), var(--vb-electric-blue));
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  background-clip: text;
}

/* Decorative script accents */
.vb-script {
  font-family: 'Pacifico', 'Dancing Script', cursive;
  font-size: 1.6em;
  color: var(--vb-magenta);
}

/* Body text */
body {
  font-family: 'Rubik', 'Nunito', sans-serif;
  font-weight: 400;
  letter-spacing: 0.01em;
  line-height: 1.75;
  color: var(--vb-text-primary);
}

/* Labels and secondary text */
.vb-label {
  font-family: 'Rubik', sans-serif;
  font-size: 0.8rem;
  font-weight: 600;
  letter-spacing: 0.08em;
  text-transform: uppercase;
  color: var(--vb-magenta);
}
```

---

## Layout Principles

### Grid and Structure

- **Immersive, full-bleed compositions** -- backgrounds and patterns extend edge-to-edge, filling the viewport
- **Layered depth without 3D** -- multiple overlapping elements at different opacities create depth on a flat plane
- **Generous content margins** within maximalist surroundings -- text and interactive elements need clear space even when borders are ornate
- **Centered, flowing content** -- content areas sit within or atop the dense pattern work, using translucent panels or color overlays for readability
- **Organic section transitions** -- sections blend into one another through flowing pattern elements rather than hard horizontal dividers
- **Radial and circular compositions** -- reflecting the kaleidoscopic, blooming motif, key sections may radiate outward from a center point
- **Large hero areas** dominated by pattern and imagery with text overlaid

### Section Organization

- Use **flowing floral dividers** between sections (vine-like SVG separators, blooming ornaments)
- Apply **translucent overlay panels** over patterned backgrounds for text readability
- Create **hierarchy through color intensity** -- hero sections use full-saturation patterns; secondary sections use lighter, more subdued versions
- Employ **ornamental framing** -- content panels bordered by vector flourishes and floral elements
- **Gradient section backgrounds** that shift hue as the user scrolls, maintaining the psychedelic atmosphere

---

## CSS/Design Techniques

### Psychedelic Gradient Background

```css
/* Signature Vectorbloom multi-color gradient background */
.vb-gradient-bg {
  background: linear-gradient(
    135deg,
    var(--vb-bg-light) 0%,
    #f0b4f0 15%,
    #d8a0f0 30%,
    #b4c8ff 50%,
    #a0f0d0 70%,
    #f0e0a0 85%,
    var(--vb-bg-light) 100%
  );
}

/* Animated gradient shift for immersive sections */
.vb-gradient-animated {
  background: linear-gradient(
    135deg,
    var(--vb-hot-pink),
    var(--vb-fuchsia),
    var(--vb-deep-purple),
    var(--vb-electric-blue),
    var(--vb-deep-teal),
    var(--vb-emerald)
  );
  background-size: 300% 300%;
  animation: vb-gradient-shift 12s ease infinite;
}

@keyframes vb-gradient-shift {
  0% { background-position: 0% 50%; }
  50% { background-position: 100% 50%; }
  100% { background-position: 0% 50%; }
}
```

### Blooming Floral Ornament (SVG + CSS)

```css
/* Floral flourish divider */
.vb-floral-divider {
  height: 60px;
  width: 70%;
  margin: 2.5rem auto;
  background: no-repeat center / contain;
  background-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 500 60'%3E%3Cpath d='M0,30 C40,10 80,50 120,30 S200,10 250,30 S320,50 380,30 S440,10 500,30' fill='none' stroke='%23e91e8c' stroke-width='1.5'/%3E%3Ccircle cx='250' cy='30' r='8' fill='%23d946ef'/%3E%3Ccircle cx='250' cy='30' r='4' fill='%23ff2d8a'/%3E%3Cpath d='M230,30 Q240,15 250,22 Q260,15 270,30 Q260,45 250,38 Q240,45 230,30Z' fill='none' stroke='%23d946ef' stroke-width='1'/%3E%3C/svg%3E");
  opacity: 0.8;
}

/* Double flourish with gradient line */
.vb-flourish-line {
  height: 3px;
  width: 60%;
  margin: 2rem auto;
  background: linear-gradient(
    90deg,
    transparent,
    var(--vb-hot-pink) 20%,
    var(--vb-fuchsia) 50%,
    var(--vb-electric-blue) 80%,
    transparent
  );
  border-radius: 2px;
  position: relative;
}

.vb-flourish-line::after {
  content: '';
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  width: 16px;
  height: 16px;
  background: radial-gradient(circle, var(--vb-fuchsia), var(--vb-hot-pink));
  border-radius: 50% 0 50% 0;
  rotate: 45deg;
}
```

### Translucent Content Panel (Over Pattern Background)

```css
/* Glass-style panel for readable text over busy pattern backgrounds */
.vb-content-panel {
  background: rgba(255, 255, 255, 0.85);
  backdrop-filter: blur(12px);
  -webkit-backdrop-filter: blur(12px);
  border: 1px solid rgba(233, 30, 140, 0.2);
  border-radius: 24px;
  padding: 3rem;
  box-shadow:
    0 8px 32px rgba(123, 45, 142, 0.1),
    inset 0 0 0 1px rgba(255, 255, 255, 0.3);
}

/* Dark variant for light-on-dark sections */
.vb-content-panel--dark {
  background: rgba(30, 10, 46, 0.85);
  border: 1px solid rgba(217, 70, 239, 0.25);
  color: var(--vb-text-on-dark);
}
```

### Vectorbloom Card

```css
.vb-card {
  background: var(--vb-white);
  border-radius: 20px;
  padding: 2.5rem;
  position: relative;
  overflow: hidden;
  box-shadow: 0 8px 30px rgba(123, 45, 142, 0.12);
  transition: transform 0.3s ease, box-shadow 0.3s ease;
}

.vb-card:hover {
  transform: translateY(-4px);
  box-shadow: 0 16px 50px rgba(233, 30, 140, 0.18);
}

/* Decorative gradient corner bloom */
.vb-card::before {
  content: '';
  position: absolute;
  top: -40px;
  right: -40px;
  width: 120px;
  height: 120px;
  background: radial-gradient(
    circle,
    rgba(217, 70, 239, 0.15),
    rgba(255, 45, 138, 0.08),
    transparent 70%
  );
  border-radius: 50%;
  pointer-events: none;
}

/* Bottom-left complementary bloom */
.vb-card::after {
  content: '';
  position: absolute;
  bottom: -30px;
  left: -30px;
  width: 100px;
  height: 100px;
  background: radial-gradient(
    circle,
    rgba(0, 163, 255, 0.1),
    rgba(13, 148, 136, 0.06),
    transparent 70%
  );
  border-radius: 50%;
  pointer-events: none;
}
```

### Floral Overlay Pattern

```css
/* Subtle repeating floral pattern for backgrounds */
.vb-pattern-bg {
  background-color: var(--vb-bg-light);
  background-image:
    radial-gradient(ellipse at 25% 25%, rgba(217, 70, 239, 0.06) 0%, transparent 50%),
    radial-gradient(ellipse at 75% 75%, rgba(255, 45, 138, 0.06) 0%, transparent 50%),
    radial-gradient(ellipse at 50% 50%, rgba(0, 163, 255, 0.04) 0%, transparent 40%);
}

/* Dense vine/filigree pattern using repeating SVG */
.vb-filigree-bg {
  background-color: var(--vb-bg-pale);
  background-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 80 80'%3E%3Cpath d='M40,0 C45,20 60,25 40,40 C20,25 35,20 40,0Z' fill='%23d946ef' opacity='0.04'/%3E%3Cpath d='M0,40 C20,35 25,20 40,40 C25,60 20,45 0,40Z' fill='%23e91e8c' opacity='0.03'/%3E%3C/svg%3E");
  background-size: 80px 80px;
}
```

### Gradient Border with Bloom Glow

```css
/* Gradient border using background-clip technique */
.vb-gradient-border {
  position: relative;
  background: var(--vb-white);
  border-radius: 20px;
  padding: 2.5rem;
}

.vb-gradient-border::before {
  content: '';
  position: absolute;
  inset: -2px;
  border-radius: 22px;
  background: linear-gradient(
    135deg,
    var(--vb-hot-pink),
    var(--vb-fuchsia),
    var(--vb-electric-blue),
    var(--vb-emerald)
  );
  z-index: -1;
}

/* Glowing bloom shadow */
.vb-bloom-glow {
  box-shadow:
    0 0 20px rgba(233, 30, 140, 0.15),
    0 0 60px rgba(217, 70, 239, 0.08),
    0 0 100px rgba(0, 163, 255, 0.05);
}
```

### Vectorbloom Button

```css
.vb-button {
  display: inline-flex;
  align-items: center;
  justify-content: center;
  padding: 14px 36px;
  background: linear-gradient(135deg, var(--vb-hot-pink), var(--vb-fuchsia));
  color: var(--vb-white);
  border: none;
  border-radius: 50px;
  font-family: 'Quicksand', 'Rubik', sans-serif;
  font-weight: 700;
  font-size: 1rem;
  letter-spacing: 0.03em;
  cursor: pointer;
  transition: all 0.3s ease;
  box-shadow: 0 4px 20px rgba(233, 30, 140, 0.3);
}

.vb-button:hover {
  background: linear-gradient(135deg, var(--vb-fuchsia), var(--vb-electric-blue));
  transform: translateY(-2px);
  box-shadow: 0 8px 30px rgba(217, 70, 239, 0.4);
}

/* Outline variant */
.vb-button--outline {
  background: transparent;
  border: 2px solid var(--vb-hot-pink);
  color: var(--vb-hot-pink);
  box-shadow: none;
}

.vb-button--outline:hover {
  background: linear-gradient(135deg, var(--vb-hot-pink), var(--vb-fuchsia));
  color: var(--vb-white);
  border-color: transparent;
}
```

### Kaleidoscopic Radial Background

```css
/* Radiating bloom pattern for hero or feature sections */
.vb-radial-bloom {
  background:
    radial-gradient(circle at 50% 50%, rgba(217, 70, 239, 0.12) 0%, transparent 40%),
    radial-gradient(circle at 20% 80%, rgba(255, 45, 138, 0.1) 0%, transparent 35%),
    radial-gradient(circle at 80% 20%, rgba(0, 163, 255, 0.08) 0%, transparent 35%),
    radial-gradient(circle at 30% 30%, rgba(132, 204, 22, 0.06) 0%, transparent 30%),
    radial-gradient(circle at 70% 70%, rgba(250, 204, 21, 0.06) 0%, transparent 30%);
  background-color: var(--vb-bg-light);
}

/* Dark variant */
.vb-radial-bloom--dark {
  background:
    radial-gradient(circle at 50% 50%, rgba(217, 70, 239, 0.2) 0%, transparent 40%),
    radial-gradient(circle at 20% 80%, rgba(255, 45, 138, 0.15) 0%, transparent 35%),
    radial-gradient(circle at 80% 20%, rgba(0, 163, 255, 0.12) 0%, transparent 35%);
  background-color: var(--vb-bg-dark);
}
```

### Navigation Bar

```css
.vb-nav {
  display: flex;
  align-items: center;
  justify-content: space-between;
  max-width: 1200px;
  margin: 0 auto;
  padding: 20px 40px;
}

.vb-nav-logo {
  font-family: 'Comfortaa', 'Quicksand', sans-serif;
  font-weight: 700;
  font-size: 1.4rem;
  background: linear-gradient(135deg, var(--vb-hot-pink), var(--vb-fuchsia));
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  background-clip: text;
  text-decoration: none;
}

.vb-nav-links {
  display: flex;
  gap: 32px;
  list-style: none;
}

.vb-nav-links a {
  font-family: 'Rubik', sans-serif;
  font-weight: 500;
  font-size: 0.95rem;
  color: var(--vb-deep-purple);
  text-decoration: none;
  transition: color 0.2s ease;
}

.vb-nav-links a:hover {
  color: var(--vb-hot-pink);
}
```

---

## Materials and Textures (Visual Metaphors for Web)

Vectorbloom originated on physical surfaces and objects. Their web equivalents:

| Physical Application | Web Equivalent |
|---------------------|----------------|
| Environmental wall/ceiling/floor murals (Katrin Olina) | Full-bleed gradient backgrounds with layered SVG pattern overlays spanning the viewport |
| Laser-cut plywood furniture (Studio Bility) | Intricate SVG clip-paths and mask patterns creating filigree border effects |
| Frosted yogurt shop interiors (SNOG) | Translucent overlay panels with `backdrop-filter: blur` over vivid pattern backgrounds |
| Painted beauty salon interiors | Saturated gradient section backgrounds with ornamental dividers |
| Glass light fixtures | Translucent gradient shapes with soft radial glows and bloom shadows |
| Decorated plastic sculptures | Gradient-filled SVG shapes with ornamental detail and rounded forms |
| Magazine advertisements and print graphics | Bold typography with gradient fills, dense floral framing, high color saturation |
| Angelfire-era web templates | Tiled pattern backgrounds, ornamental borders, decorative cursor trails |

---

## Notable Practitioners and Influences

| Practitioner / Reference | Contribution |
|-------------------------|-------------|
| **Katrin Olina** | Icelandic graphic artist who pioneered Vectorbloom in interior design; created seamless, immersive vector environments (notably the Cristal Bar, Hong Kong) where a single graphic image functions as wall-to-ceiling lining, morphing across surfaces |
| **SNOG Frozen Yogurt** | Commercial interiors exemplifying "frozen yogurt futurism" -- dense vector patterns applied to retail environments |
| **Studio Bility** | Inner Beauty Bench (2008) -- laser-cut plywood furniture with intricate vector floral patterns |

### Video Game Expressions

| Game | Year | Relevance |
|------|------|-----------|
| **Lumines** | 2004 | Psychedelic vector visuals synchronized to electronic music |
| **Feel the Magic: XY/XX** | 2004 | Stylized vector art direction |
| **PixelJunk Eden** | 2008 | Blooming organic vector garden environments |
| **Child of Eden** | 2011 | Synesthetic vector-bloom visual experience |
| **Hohokum** | 2014 | Flowing vector environments with organic forms |

---

## Related Aesthetics

| Aesthetic | Relationship to Vectorbloom |
|-----------|----------------------------|
| **Art Nouveau** | Major visual ancestor; provides the organic curves, botanical motifs, and ornamental flourishes that Vectorbloom digitalizes |
| **Psychedelia** | 1960s influence; contributes the saturated, multicolor palette, flowing forms, and mind-expanding visual density |
| **Supergraphic Ultramodern** | 1970s influence; provides the concept of large-scale, environment-transforming graphic application |
| **Frutiger Aero** | Contemporary sibling; shares the early-2000s digital optimism but favors glossy naturalism over flat ornamental density |
| **Vectordelia** | Close sibling; shares the psychedelic vector toolkit but Vectorbloom emphasizes floral blooming and maximalist ornament |
| **Superflat Pop** | Related; shares flat, digitally precise rendering and vivid color but draws from Japanese pop culture rather than botanical forms |
| **McBling** | Period contemporary; shares the early-2000s maximalist, flashy sensibility in a pop-culture context |
| **Neo-Vectorheart** | Sibling from the same vector design lineage; Neo-Vectorheart is angular and monochromatic where Vectorbloom is organic and polychromatic |

---

## Quick-Start: Minimal Vectorbloom Page Template

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Vectorbloom Page</title>
  <link href="https://fonts.googleapis.com/css2?family=Quicksand:wght@400;500;600;700&family=Rubik:ital,wght@0,300;0,400;0,600;0,700;1,400&family=Comfortaa:wght@400;600;700&family=Pacifico&display=swap" rel="stylesheet">
  <style>
    :root {
      --vb-hot-pink: #ff2d8a;
      --vb-magenta: #e91e8c;
      --vb-fuchsia: #d946ef;
      --vb-deep-purple: #7b2d8e;
      --vb-lavender: #c084fc;
      --vb-electric-blue: #00a3ff;
      --vb-deep-teal: #0d9488;
      --vb-lime: #84cc16;
      --vb-yellow: #facc15;
      --vb-bg-light: #f5d6f5;
      --vb-bg-pale: #fdf2f8;
      --vb-black: #0a0a12;
      --vb-white: #ffffff;
    }

    * { margin: 0; padding: 0; box-sizing: border-box; }

    body {
      background: var(--vb-bg-light);
      color: var(--vb-black);
      font-family: 'Rubik', sans-serif;
      font-weight: 400;
      letter-spacing: 0.01em;
      line-height: 1.75;
    }

    h1, h2, h3 {
      font-family: 'Quicksand', 'Comfortaa', sans-serif;
      font-weight: 700;
      color: var(--vb-deep-purple);
      letter-spacing: 0.02em;
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
      font-family: 'Comfortaa', sans-serif;
      font-weight: 700;
      font-size: 1.3rem;
      background: linear-gradient(135deg, var(--vb-hot-pink), var(--vb-fuchsia));
      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent;
      background-clip: text;
      text-decoration: none;
    }

    nav ul {
      display: flex;
      gap: 28px;
      list-style: none;
    }

    nav ul a {
      color: var(--vb-deep-purple);
      text-decoration: none;
      font-weight: 500;
      font-size: 0.95rem;
      transition: color 0.2s;
    }

    nav ul a:hover { color: var(--vb-hot-pink); }

    /* Hero with radial bloom background */
    .hero {
      text-align: center;
      padding: 6rem 2rem;
      position: relative;
      overflow: hidden;
      background:
        radial-gradient(circle at 50% 50%, rgba(217, 70, 239, 0.12) 0%, transparent 40%),
        radial-gradient(circle at 20% 80%, rgba(255, 45, 138, 0.1) 0%, transparent 35%),
        radial-gradient(circle at 80% 20%, rgba(0, 163, 255, 0.08) 0%, transparent 35%);
    }

    .hero h1 {
      font-family: 'Comfortaa', sans-serif;
      font-size: clamp(2.5rem, 7vw, 5.5rem);
      font-weight: 700;
      letter-spacing: 0.04em;
      background: linear-gradient(135deg, var(--vb-hot-pink), var(--vb-fuchsia), var(--vb-electric-blue));
      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent;
      background-clip: text;
      line-height: 1.1;
    }

    .hero .subtitle {
      font-family: 'Pacifico', cursive;
      font-size: 1.6rem;
      color: var(--vb-magenta);
      margin-top: 0.75rem;
    }

    /* Gradient flourish divider */
    .vb-divider {
      height: 3px;
      width: 40%;
      margin: 2rem auto;
      background: linear-gradient(
        90deg,
        transparent,
        var(--vb-hot-pink) 20%,
        var(--vb-fuchsia) 50%,
        var(--vb-electric-blue) 80%,
        transparent
      );
      border-radius: 2px;
    }

    /* Content section */
    section {
      max-width: 800px;
      margin: 0 auto;
      padding: 4rem 2rem;
    }

    section h2 {
      text-align: center;
      margin-bottom: 1.5rem;
    }

    section p {
      text-align: center;
      color: var(--vb-deep-purple);
      opacity: 0.85;
    }

    /* Card */
    .card {
      background: var(--vb-white);
      border-radius: 20px;
      padding: 2.5rem;
      margin: 1.5rem 0;
      position: relative;
      overflow: hidden;
      box-shadow: 0 8px 30px rgba(123, 45, 142, 0.12);
    }

    .card::before {
      content: '';
      position: absolute;
      top: -40px;
      right: -40px;
      width: 120px;
      height: 120px;
      background: radial-gradient(circle, rgba(217, 70, 239, 0.15), transparent 70%);
      border-radius: 50%;
      pointer-events: none;
    }

    /* Button */
    .btn {
      display: inline-block;
      padding: 14px 36px;
      background: linear-gradient(135deg, var(--vb-hot-pink), var(--vb-fuchsia));
      color: var(--vb-white);
      border: none;
      border-radius: 50px;
      font-family: 'Quicksand', sans-serif;
      font-weight: 700;
      font-size: 1rem;
      text-decoration: none;
      cursor: pointer;
      transition: all 0.3s ease;
      box-shadow: 0 4px 20px rgba(233, 30, 140, 0.3);
    }

    .btn:hover {
      background: linear-gradient(135deg, var(--vb-fuchsia), var(--vb-electric-blue));
      transform: translateY(-2px);
      box-shadow: 0 8px 30px rgba(217, 70, 239, 0.4);
    }

    /* Feature grid */
    .features {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
      gap: 2rem;
      max-width: 1100px;
      margin: 0 auto;
      padding: 2rem 2rem 4rem;
    }

    @media (max-width: 768px) {
      .hero { padding: 4rem 1.5rem; }
      nav { padding: 16px 20px; }
      nav ul { gap: 16px; }
    }
  </style>
</head>
<body>
  <nav>
    <a href="#" class="logo">Vectorbloom</a>
    <ul>
      <li><a href="#">Gallery</a></li>
      <li><a href="#">Designs</a></li>
      <li><a href="#">About</a></li>
    </ul>
  </nav>

  <div class="hero">
    <h1>Digital Blooms</h1>
    <div class="subtitle">where vectors meet nature</div>
    <div class="vb-divider"></div>
    <p style="margin-top: 1.5rem;">
      <a href="#" class="btn">Explore the Garden</a>
    </p>
  </div>

  <section>
    <h2>Technological Opulence</h2>
    <p>Maximalist vector ornament meets psychedelic botanical fantasy. Every surface becomes a canvas for intricate, blooming digital compositions.</p>
  </section>

  <div class="features">
    <div class="card">
      <h3>Flourishing Patterns</h3>
      <p>Intricate floral forms rendered with digital precision, spreading seamlessly across every surface.</p>
    </div>
    <div class="card">
      <h3>Vivid Palettes</h3>
      <p>Bold gradients flowing from hot pink through deep purple to electric blue create luminous, psychedelic atmospheres.</p>
    </div>
    <div class="card">
      <h3>Immersive Environments</h3>
      <p>Patterns designed to transform entire spaces, enveloping walls, ceilings, and floors in continuous imagery.</p>
    </div>
  </div>
</body>
</html>
```
