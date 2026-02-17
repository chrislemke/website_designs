# Wacky Pomo Design Reference

Wacky Pomo is a marketing aesthetic popular from the **early 1990s to mid-2000s**, primarily in children's entertainment and product branding. It combines cartoonish mid-century visuals with postmodern design principles, rejecting strict grids, muted palettes, and rational order in favor of **clashing colors, zigzags, blobs, fake 3D squiggles, and distorted type**. The aesthetic sells fun, novelty, and a slightly anarchic sense of "kidz culture" -- everything is loud, plastic, toy-like, and deliberately anti-sophisticated. Surfaces feel glossy and hyper-synthetic, typography bends and wobbles, and competing patterns collide without any attempt at harmony. The mood is hyperactive, irreverent, and unapologetically juvenile.

---

## Visual Characteristics

### Core Design Traits

- **Clashing, saturated color blocks** -- bright purples, acidic greens, saturated yellows, oranges, and teals jammed together with no regard for traditional harmony
- **Glossy plastic surfaces** -- everything looks molded, injection-formed, or powder-coated, creating a toy-like sheen
- **Wobbly, distorted typography** -- letters bend, stretch, wobble, and tilt on wavy baselines with exaggerated drop shadows and 3D extrusions
- **Layered competing patterns** -- checkerboards, confetti sprinkles, stripes, and polka dots fighting for attention within the same composition
- **Jagged zigzags and squiggles** -- angular zigzag borders, spiraling lines, and scribble-like decoration used as structural design elements
- **Blob and splat shapes** -- organic, irregular forms used as containers, backgrounds, and decorative accents
- **Fake industrial contraptions** -- non-functional tubes, panels, levers, gears, and consoles creating a pseudo-technical, sci-fi playground feel
- **Oversized toy-like forms** -- exaggerated geometric shapes resembling game pieces, building blocks, or giant playroom props
- **Hard artificial lighting and neon accents** -- harsh, flat lighting with neon edge glows suggesting a TV studio or arcade environment
- **Gross-out and junk food motifs** -- slime, goo, exaggerated cartoon faces, giant crayons, and candy/snack imagery
- **Confetti and scatter elements** -- small shapes (stars, dots, squiggles) thrown haphazardly across backgrounds
- **3D extrusion on everything** -- text, shapes, and UI elements given chunky depth and perspective, looking like plastic toys

### Design Principles

- Reject minimalism, restraint, and "good taste" -- the louder and more chaotic, the better
- Clash colors deliberately; discord and visual overload are features, not bugs
- Typography is a toy, not a tool -- distort, rotate, stretch, and color it freely
- Layer patterns on top of patterns; nothing should sit on a quiet, empty background
- Everything should feel like it could be a physical toy, game piece, or theme park prop
- Mix cartoon illustration with pseudo-industrial/sci-fi hardware for surreal juxtaposition
- Address the viewer with aggressive, in-your-face energy -- nothing is subtle or understated
- Embrace synthetic, artificial materials over anything natural or organic
- Asymmetry, randomness, and visual noise over order, grids, and whitespace
- Fun is the supreme value -- every design decision should serve maximum entertainment energy

---

## Color Palette

### Core Principle

Wacky Pomo uses **fully saturated, clashing hues** presented as flat color blocks or glossy plastic surfaces. Colors are paired with hard, artificial lighting or neon accents. There is no attempt at harmony -- the palette is deliberately garish, like a toy aisle exploded.

### Primary Scheme

| Role | Colors |
|------|--------|
| **Primary pop** | Bright purple, electric violet |
| **Secondary energy** | Acidic green, lime, slime green |
| **Tertiary warmth** | Saturated yellow, golden yellow |
| **Accent heat** | Hot orange, tangerine |
| **Cool accent** | Teal, turquoise, cyan |
| **Highlight / shock** | Hot pink, magenta, fuchsia |
| **Background (light)** | White, off-white, light gray |
| **Background (dark)** | Deep purple-black, charcoal |
| **Outlines / structure** | Pure black, heavy dark outlines |

### Full Palette

| Color | Hex (suggested) | Usage |
|-------|-----------------|-------|
| Electric Purple | `#8B2FC9`, `#7B1FA2` | Primary accent, section backgrounds, display text |
| Bright Violet | `#AA00FF`, `#9C27B0` | Headlines, decorative shapes, gradient endpoints |
| Acidic Green | `#76FF03`, `#64DD17` | Secondary accent, slime motifs, highlights |
| Slime Green | `#69F0AE`, `#00E676` | Goo effects, hover states, badges |
| Saturated Yellow | `#FFD600`, `#FFEA00` | Hero accents, button backgrounds, stars and confetti |
| Hot Orange | `#FF6D00`, `#FF9100` | Call-to-action, tertiary accent, zigzag borders |
| Tangerine | `#FF8F00`, `#FFA000` | Warm highlights, card accents |
| Teal | `#00BFA5`, `#1DE9B6` | Cool counterpoint, link color, alternate section backgrounds |
| Turquoise | `#00E5FF`, `#18FFFF` | Neon accents, glow effects, tertiary decoration |
| Hot Pink | `#FF4081`, `#F50057` | Shock accents, decorative text, splat shapes |
| Fuchsia | `#E040FB`, `#D500F9` | Display headings, neon glow, alternate accent |
| White | `#FFFFFF`, `#FAFAFA` | Card surfaces, light backgrounds |
| Off-White | `#F5F5F5`, `#EEEEEE` | Page canvas, neutral space |
| Charcoal | `#212121`, `#1A1A1A` | Dark backgrounds, text on light surfaces |
| Pure Black | `#000000` | Heavy outlines, stroke borders, drop shadows |

### Suggested CSS Custom Properties

```css
:root {
  /* Purples */
  --wacky-purple: #8b2fc9;
  --wacky-purple-bright: #aa00ff;
  --wacky-violet: #7b1fa2;

  /* Greens */
  --wacky-acid-green: #76ff03;
  --wacky-lime: #64dd17;
  --wacky-slime: #69f0ae;

  /* Yellows */
  --wacky-yellow: #ffd600;
  --wacky-yellow-bright: #ffea00;

  /* Oranges */
  --wacky-orange: #ff6d00;
  --wacky-tangerine: #ff9100;

  /* Cool accents */
  --wacky-teal: #00bfa5;
  --wacky-turquoise: #00e5ff;
  --wacky-cyan: #18ffff;

  /* Pinks */
  --wacky-pink: #ff4081;
  --wacky-fuchsia: #e040fb;
  --wacky-magenta: #d500f9;

  /* Neutrals */
  --wacky-white: #ffffff;
  --wacky-offwhite: #f5f5f5;
  --wacky-charcoal: #212121;
  --wacky-black: #000000;

  /* Functional */
  --wacky-bg-light: var(--wacky-white);
  --wacky-bg-dark: var(--wacky-charcoal);
  --wacky-text-dark: var(--wacky-charcoal);
  --wacky-text-light: var(--wacky-white);
  --wacky-border: var(--wacky-black);
  --wacky-stroke-width: 3px;
  --wacky-shadow-offset: 5px;
}
```

### Color Usage Principles

- **Always clash** -- place complementary or competing hues side by side (purple next to green, orange next to teal, pink next to yellow)
- **Fully saturated only** -- no pastels, no muted tones, no earth tones; everything at maximum chroma
- **Flat blocks of color** -- backgrounds, cards, and sections use solid, unblended fills like plastic panels
- **Neon accents on edges** -- turquoise and cyan glow effects on borders and outlines to simulate arcade/TV-studio lighting
- **Black outlines everywhere** -- thick black strokes separate color zones, like a cartoon coloring book
- **3-5 clashing colors per section minimum** -- visual restraint is the enemy
- **White or light gray as breathing room** -- used sparingly between dense color blocks, never as the dominant surface

---

## Typography

### Typeface Characteristics

Wacky Pomo typography is **distorted, oversized, cartoonish, and physically impossible**. Letters look like plastic toys -- chunky, shiny, and slightly wrong. The style draws from 1990s Nickelodeon title cards, cereal box branding, and children's TV show logos.

- **Chunky, heavy sans-serifs** -- ultra-bold weights with exaggerated thickness and rounded terminals
- **Wobbly, tilted baselines** -- text set on curved or wavy paths; individual letters rotated at different angles
- **3D extrusion and drop shadows** -- letters given chunky plastic depth with bright-colored extrusions (not gray shadows)
- **Bright outlines** -- colored stroke outlines around letterforms (e.g., yellow text with a purple outline)
- **Stretched and squished letterforms** -- individual characters distorted in scale, some tall, some wide, creating visual chaos
- **Cartoon lettering** -- hand-drawn-style type that looks inflated, bouncy, or blob-like
- **Slanted and arranged around shapes** -- text that wraps around circles, follows zigzag paths, or radiates from a central point
- **All-caps for emphasis** -- loud, attention-grabbing headlines in screaming uppercase
- **Multi-color text** -- individual letters or words in different colors within the same heading
- **No professional typographic "correctness"** -- kerning, alignment, and baseline consistency are deliberately violated

### Recommended Web Fonts (Google Fonts)

| Font | Style | Usage |
|------|-------|-------|
| **Boogaloo** | Retro rounded, fun | Display headings -- groovy, bouncy letterforms with 90s energy |
| **Fredoka** | Rounded, chunky, playful | Primary headlines -- bubbly and toy-like |
| **Bangers** | Bold comic-book block | Impact headings, callouts -- maximum loudness |
| **Luckiest Guy** | Chunky comic display | Hero text, section titles -- exaggerated cartoon weight |
| **Rubik Bubbles** | Inflated, bubbly display | Display accents -- letters look like they are made of rubber |
| **Bungee** | Chromatic layered display | Multi-layered display text -- built for stacking colors |
| **Cabin Sketch** | Sketchy hand-drawn | Accent text, labels -- rough, playful, hand-made feel |
| **Lilita One** | Thick, friendly display | Subheadings, card titles -- bold and approachable |
| **Nunito** | Rounded humanist sans | Body text -- readable with playful roundness |
| **Quicksand** | Soft geometric sans | Secondary text, UI labels -- clean but still fun |

### Typography CSS Example

```css
@import url('https://fonts.googleapis.com/css2?family=Boogaloo&family=Fredoka:wght@400;500;600;700&family=Bangers&family=Luckiest+Guy&family=Nunito:wght@400;600;700&display=swap');

/* Hero / Display headings -- maximum cartoon energy */
h1, .wacky-display {
  font-family: 'Luckiest Guy', 'Boogaloo', 'Fredoka', cursive;
  font-size: clamp(3rem, 8vw, 7rem);
  text-transform: uppercase;
  line-height: 1.0;
  letter-spacing: 0.03em;
  color: var(--wacky-yellow);
  text-shadow:
    4px 4px 0 var(--wacky-purple),
    -2px -2px 0 var(--wacky-black),
    2px -2px 0 var(--wacky-black),
    -2px 2px 0 var(--wacky-black);
  transform: rotate(-2deg);
}

/* Section headings */
h2 {
  font-family: 'Fredoka', 'Boogaloo', sans-serif;
  font-weight: 700;
  font-size: clamp(1.8rem, 4vw, 3rem);
  line-height: 1.15;
  color: var(--wacky-acid-green);
  text-shadow:
    3px 3px 0 var(--wacky-black),
    0 0 10px rgba(118, 255, 3, 0.3);
}

/* Subheadings */
h3 {
  font-family: 'Fredoka', 'Bangers', sans-serif;
  font-weight: 600;
  font-size: 1.4rem;
  color: var(--wacky-orange);
  text-transform: uppercase;
  letter-spacing: 0.05em;
}

/* Body text -- readable but still rounded and fun */
body {
  font-family: 'Nunito', 'Quicksand', sans-serif;
  font-weight: 400;
  font-size: 1.05rem;
  line-height: 1.7;
  color: var(--wacky-text-dark);
}

/* Impact callout text */
.wacky-callout {
  font-family: 'Bangers', 'Luckiest Guy', cursive;
  font-size: 1.6rem;
  text-transform: uppercase;
  letter-spacing: 0.06em;
  color: var(--wacky-pink);
  text-shadow: 2px 2px 0 var(--wacky-black);
}

/* Wobbly text -- individual letter rotation */
.wacky-wobble span:nth-child(odd) { display: inline-block; transform: rotate(-4deg) translateY(-2px); }
.wacky-wobble span:nth-child(even) { display: inline-block; transform: rotate(3deg) translateY(2px); }

/* Multi-color heading */
.wacky-rainbow span:nth-child(1) { color: var(--wacky-purple); }
.wacky-rainbow span:nth-child(2) { color: var(--wacky-acid-green); }
.wacky-rainbow span:nth-child(3) { color: var(--wacky-yellow); }
.wacky-rainbow span:nth-child(4) { color: var(--wacky-orange); }
.wacky-rainbow span:nth-child(5) { color: var(--wacky-pink); }
.wacky-rainbow span:nth-child(6) { color: var(--wacky-teal); }
```

---

## Layout Principles

### Grid and Structure

- **Asymmetric, chaotic compositions** -- reject rigid grids; elements should feel thrown together like a hyperactive collage
- **Overlapping and layered elements** -- shapes, text, and decorative elements pile on top of each other with visible z-depth
- **Tilted and rotated containers** -- cards, panels, and sections sit at slight angles (2-5 degrees) rather than perfectly horizontal
- **Jagged, non-straight section dividers** -- zigzag borders, splat edges, and wave-cut separators between content areas
- **Bold, solid-color section backgrounds** -- full-bleed color blocks in clashing hues for each section
- **Oversized decorative shapes breaking boundaries** -- spirals, stars, blobs, and gears that overflow their containers and overlap adjacent sections
- **Dense, pattern-filled backgrounds** -- no section should sit on a plain, empty surface; checkerboards, dots, or stripes fill dead space
- **Competing focal points** -- multiple loud elements within each section fighting for attention, unlike traditional single-focus hierarchy
- **Thick black borders on everything** -- every card, container, and shape outlined in heavy black strokes

### Section Organization

- **Hero**: Oversized, distorted display text in clashing colors over a pattern-dense background with scattered decorative shapes (stars, zigzags, splats). Text should be rotated or on a curved baseline.
- **Content blocks**: Tilted cards with solid-color backgrounds, thick black borders, and exaggerated colored drop shadows. Each card a different accent color.
- **Feature sections**: Elements arranged chaotically with large decorative shapes (gears, spirals, blobs) filling all negative space
- **Dividers**: Zigzag SVG borders, slime-drip edges, or rows of repeating geometric shapes (stars, triangles) -- never simple horizontal lines
- **Backgrounds**: Checkerboard patterns, confetti scatter, polka dots, or stripe patterns at moderate opacity behind content
- **CTA sections**: Extremely bold solid-color backgrounds (hot pink, acid green, bright purple) with contrasting distorted text and chunky buttons

### Responsive Approach

- Stack elements vertically on mobile but keep the rotation, color clash, and decorative chaos intact
- Scale decorative shapes down but never remove them
- Typography scales aggressively with `clamp()` -- headings stay oversized even on small screens
- Maintain thick outlines and stroke widths at all breakpoints
- Pattern density can be reduced on mobile but backgrounds should never be plain

---

## CSS / Design Techniques

### Checkerboard Pattern Background

```css
/* Classic competing checkerboard pattern */
.wacky-checkerboard {
  background-color: var(--wacky-white);
  background-image:
    repeating-conic-gradient(
      var(--wacky-offwhite) 0% 25%,
      transparent 0% 50%
    );
  background-size: 40px 40px;
}

/* Colored checkerboard variant */
.wacky-checkerboard--purple {
  background-color: #e1bee7;
  background-image:
    repeating-conic-gradient(
      #ce93d8 0% 25%,
      transparent 0% 50%
    );
  background-size: 30px 30px;
}
```

### Confetti Scatter Pattern

```css
/* Confetti dots and shapes scattered across backgrounds */
.wacky-confetti-bg {
  background-color: var(--wacky-white);
  background-image:
    radial-gradient(circle 4px, var(--wacky-purple) 100%, transparent 100%),
    radial-gradient(circle 3px, var(--wacky-acid-green) 100%, transparent 100%),
    radial-gradient(circle 5px, var(--wacky-yellow) 100%, transparent 100%),
    radial-gradient(circle 3px, var(--wacky-pink) 100%, transparent 100%),
    radial-gradient(circle 4px, var(--wacky-orange) 100%, transparent 100%),
    radial-gradient(circle 3px, var(--wacky-teal) 100%, transparent 100%);
  background-size: 180px 180px;
  background-position:
    15px 25px,
    60px 90px,
    110px 40px,
    150px 120px,
    35px 150px,
    130px 70px;
}
```

### Polka Dot Pattern

```css
/* Large polka dots on solid background */
.wacky-polkadots {
  background-color: var(--wacky-purple);
  background-image:
    radial-gradient(circle 12px, var(--wacky-yellow) 100%, transparent 100%),
    radial-gradient(circle 12px, var(--wacky-yellow) 100%, transparent 100%);
  background-size: 50px 50px;
  background-position: 0 0, 25px 25px;
}
```

### Stripe Pattern

```css
/* Diagonal candy stripes */
.wacky-stripes {
  background: repeating-linear-gradient(
    -45deg,
    var(--wacky-yellow),
    var(--wacky-yellow) 10px,
    var(--wacky-charcoal) 10px,
    var(--wacky-charcoal) 20px
  );
}

/* Horizontal thick stripes */
.wacky-stripes-h {
  background: repeating-linear-gradient(
    0deg,
    var(--wacky-acid-green),
    var(--wacky-acid-green) 8px,
    var(--wacky-purple) 8px,
    var(--wacky-purple) 16px
  );
}
```

### Zigzag Border / Divider

```css
/* Zigzag section divider */
.wacky-zigzag {
  width: 100%;
  height: 24px;
  background: url("data:image/svg+xml,%3Csvg width='40' height='24' xmlns='http://www.w3.org/2000/svg'%3E%3Cpolyline points='0,24 20,0 40,24' stroke='%23000' stroke-width='3' fill='%23ffd600'/%3E%3C/svg%3E") repeat-x;
}

/* Colored zigzag variants */
.wacky-zigzag--purple {
  background: url("data:image/svg+xml,%3Csvg width='40' height='24' xmlns='http://www.w3.org/2000/svg'%3E%3Cpolyline points='0,24 20,0 40,24' stroke='%23000' stroke-width='3' fill='%238b2fc9'/%3E%3C/svg%3E") repeat-x;
}

.wacky-zigzag--green {
  background: url("data:image/svg+xml,%3Csvg width='40' height='24' xmlns='http://www.w3.org/2000/svg'%3E%3Cpolyline points='0,24 20,0 40,24' stroke='%23000' stroke-width='3' fill='%2376ff03'/%3E%3C/svg%3E") repeat-x;
}
```

### Splat / Blob Shape

```css
/* Irregular blob container -- the signature Wacky Pomo organic shape */
.wacky-splat {
  border-radius: 60% 40% 50% 45% / 45% 55% 40% 55%;
  padding: 2.5rem;
  position: relative;
}

/* Color variants */
.wacky-splat--purple { background: var(--wacky-purple); color: var(--wacky-text-light); }
.wacky-splat--green { background: var(--wacky-acid-green); color: var(--wacky-text-dark); }
.wacky-splat--yellow { background: var(--wacky-yellow); color: var(--wacky-text-dark); }
.wacky-splat--pink { background: var(--wacky-pink); color: var(--wacky-text-light); }

/* Animated blob that subtly morphs */
@keyframes splat-morph {
  0%, 100% { border-radius: 60% 40% 50% 45% / 45% 55% 40% 55%; }
  25% { border-radius: 45% 55% 40% 60% / 55% 40% 60% 45%; }
  50% { border-radius: 50% 45% 55% 40% / 40% 60% 45% 55%; }
  75% { border-radius: 55% 40% 45% 55% / 60% 45% 55% 40%; }
}

.wacky-splat--morph {
  animation: splat-morph 8s ease-in-out infinite;
}
```

### Decorative Shapes

```css
/* Star burst decoration */
.wacky-star {
  width: 60px;
  height: 60px;
  background: var(--wacky-yellow);
  clip-path: polygon(
    50% 0%, 61% 35%, 98% 35%, 68% 57%,
    79% 91%, 50% 70%, 21% 91%, 32% 57%,
    2% 35%, 39% 35%
  );
  position: absolute;
  filter: drop-shadow(2px 2px 0 var(--wacky-black));
}

/* Spiral / squiggle decoration (SVG background) */
.wacky-squiggle {
  width: 80px;
  height: 80px;
  position: absolute;
  background: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 80 80'%3E%3Cpath d='M10 40 Q20 10 40 25 T70 40 T40 65 T10 40' stroke='%238b2fc9' stroke-width='4' fill='none' stroke-linecap='round'/%3E%3C/svg%3E") no-repeat center;
  pointer-events: none;
}

/* Gear decoration */
.wacky-gear {
  width: 70px;
  height: 70px;
  position: absolute;
  background: var(--wacky-teal);
  border-radius: 50%;
  border: 3px solid var(--wacky-black);
}
.wacky-gear::before {
  content: '';
  position: absolute;
  inset: 8px;
  border-radius: 50%;
  border: 3px solid var(--wacky-black);
  background: var(--wacky-white);
}

/* Lightning bolt / zigzag shape */
.wacky-bolt {
  width: 40px;
  height: 70px;
  position: absolute;
  background: var(--wacky-yellow);
  clip-path: polygon(30% 0%, 70% 0%, 50% 40%, 80% 40%, 20% 100%, 40% 55%, 10% 55%);
  filter: drop-shadow(2px 2px 0 var(--wacky-black));
}
```

### Wacky Card Component

```css
/* Tilted, chunky card with exaggerated colored shadow */
.wacky-card {
  background: var(--wacky-white);
  border: 3px solid var(--wacky-black);
  border-radius: 8px;
  padding: 1.5rem 2rem;
  position: relative;
  transform: rotate(-1.5deg);
  box-shadow: 6px 6px 0 var(--wacky-purple);
  transition: transform 0.2s ease, box-shadow 0.2s ease;
}

.wacky-card:hover {
  transform: rotate(0deg) translate(-3px, -3px);
  box-shadow: 9px 9px 0 var(--wacky-purple);
}

/* Alternating card shadow colors */
.wacky-card:nth-child(1) { box-shadow: 6px 6px 0 var(--wacky-purple); transform: rotate(-1.5deg); }
.wacky-card:nth-child(2) { box-shadow: 6px 6px 0 var(--wacky-acid-green); transform: rotate(1deg); }
.wacky-card:nth-child(3) { box-shadow: 6px 6px 0 var(--wacky-pink); transform: rotate(-2deg); }
.wacky-card:nth-child(4) { box-shadow: 6px 6px 0 var(--wacky-orange); transform: rotate(1.5deg); }
.wacky-card:nth-child(5) { box-shadow: 6px 6px 0 var(--wacky-teal); transform: rotate(-1deg); }

/* Colored background card variants */
.wacky-card--purple { background: var(--wacky-purple); color: var(--wacky-text-light); }
.wacky-card--green { background: var(--wacky-acid-green); color: var(--wacky-text-dark); }
.wacky-card--yellow { background: var(--wacky-yellow); color: var(--wacky-text-dark); }
.wacky-card--pink { background: var(--wacky-pink); color: var(--wacky-text-light); }

/* Decorative corner star */
.wacky-card::after {
  content: '\2605'; /* star */
  position: absolute;
  top: -10px;
  right: -10px;
  font-size: 1.6rem;
  color: var(--wacky-yellow);
  filter: drop-shadow(1px 1px 0 var(--wacky-black));
}
```

### Wacky Button

```css
/* Chunky toy-like button with 3D extrusion */
.wacky-button {
  display: inline-block;
  padding: 14px 32px;
  border: 3px solid var(--wacky-black);
  border-radius: 8px;
  background: var(--wacky-yellow);
  color: var(--wacky-charcoal);
  font-family: 'Fredoka', 'Bangers', sans-serif;
  font-weight: 700;
  font-size: 1.15rem;
  text-transform: uppercase;
  letter-spacing: 0.05em;
  text-decoration: none;
  cursor: pointer;
  position: relative;
  box-shadow:
    5px 5px 0 var(--wacky-black),
    inset 0 -3px 0 rgba(0, 0, 0, 0.15);
  transition: transform 0.12s ease, box-shadow 0.12s ease;
  transform: rotate(-1deg);
}

.wacky-button:hover {
  transform: rotate(0deg) translate(-2px, -2px);
  box-shadow:
    7px 7px 0 var(--wacky-black),
    inset 0 -3px 0 rgba(0, 0, 0, 0.15);
}

.wacky-button:active {
  transform: rotate(0deg) translate(2px, 2px);
  box-shadow:
    3px 3px 0 var(--wacky-black),
    inset 0 -3px 0 rgba(0, 0, 0, 0.15);
}

/* Color variants */
.wacky-button--purple {
  background: var(--wacky-purple);
  color: var(--wacky-text-light);
}

.wacky-button--green {
  background: var(--wacky-acid-green);
  color: var(--wacky-text-dark);
}

.wacky-button--pink {
  background: var(--wacky-pink);
  color: var(--wacky-text-light);
}

.wacky-button--orange {
  background: var(--wacky-orange);
  color: var(--wacky-text-light);
}
```

### Hero Section

```css
.wacky-hero {
  position: relative;
  min-height: 90vh;
  display: flex;
  align-items: center;
  justify-content: center;
  text-align: center;
  padding: 80px 40px;
  overflow: hidden;
  background: var(--wacky-purple);
}

/* Checkerboard overlay at low opacity */
.wacky-hero::before {
  content: '';
  position: absolute;
  inset: 0;
  background-image: repeating-conic-gradient(
    rgba(0, 0, 0, 0.06) 0% 25%,
    transparent 0% 50%
  );
  background-size: 40px 40px;
  pointer-events: none;
  z-index: 1;
}

.wacky-hero__content {
  position: relative;
  z-index: 2;
  max-width: 800px;
}

.wacky-hero h1 {
  font-family: 'Luckiest Guy', 'Boogaloo', cursive;
  font-size: clamp(3.5rem, 9vw, 8rem);
  text-transform: uppercase;
  color: var(--wacky-yellow);
  line-height: 0.95;
  text-shadow:
    5px 5px 0 var(--wacky-black),
    -2px -2px 0 var(--wacky-black),
    2px -2px 0 var(--wacky-black),
    -2px 2px 0 var(--wacky-black),
    0 0 20px rgba(255, 214, 0, 0.3);
  transform: rotate(-3deg);
  margin-bottom: 1.5rem;
}

.wacky-hero p {
  font-family: 'Nunito', sans-serif;
  font-size: 1.3rem;
  font-weight: 600;
  color: var(--wacky-text-light);
  margin-bottom: 2.5rem;
  text-shadow: 1px 1px 0 rgba(0, 0, 0, 0.3);
}
```

### Navigation Bar

```css
.wacky-nav {
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 16px 40px;
  background: var(--wacky-yellow);
  border-bottom: 4px solid var(--wacky-black);
  position: relative;
  z-index: 10;
}

.wacky-nav__logo {
  font-family: 'Luckiest Guy', 'Fredoka', sans-serif;
  font-size: 1.6rem;
  color: var(--wacky-purple);
  text-decoration: none;
  text-shadow: 2px 2px 0 var(--wacky-black);
  transform: rotate(-2deg);
  display: inline-block;
}

.wacky-nav__links {
  display: flex;
  gap: 8px;
  list-style: none;
}

.wacky-nav__links a {
  display: inline-block;
  font-family: 'Fredoka', sans-serif;
  font-weight: 600;
  font-size: 0.95rem;
  color: var(--wacky-charcoal);
  text-decoration: none;
  text-transform: uppercase;
  letter-spacing: 0.04em;
  padding: 6px 14px;
  border: 2px solid transparent;
  border-radius: 6px;
  transition: all 0.15s ease;
}

.wacky-nav__links a:hover {
  background: var(--wacky-purple);
  color: var(--wacky-text-light);
  border-color: var(--wacky-black);
  transform: rotate(-2deg) scale(1.05);
}
```

### Section Color Blocks

```css
.wacky-section {
  padding: 80px 40px;
  position: relative;
  overflow: hidden;
}

.wacky-section--purple {
  background: var(--wacky-purple);
  color: var(--wacky-text-light);
}

.wacky-section--green {
  background: var(--wacky-acid-green);
  color: var(--wacky-text-dark);
}

.wacky-section--yellow {
  background: var(--wacky-yellow);
  color: var(--wacky-text-dark);
}

.wacky-section--pink {
  background: var(--wacky-pink);
  color: var(--wacky-text-light);
}

.wacky-section--orange {
  background: var(--wacky-orange);
  color: var(--wacky-text-light);
}

.wacky-section--teal {
  background: var(--wacky-teal);
  color: var(--wacky-text-dark);
}

.wacky-section--white {
  background: var(--wacky-white);
  color: var(--wacky-text-dark);
}

.wacky-section--dark {
  background: var(--wacky-charcoal);
  color: var(--wacky-text-light);
}
```

### Floating Decoration Animations

```css
/* Chaotic floating animation -- more aggressive than Memphis, less smooth */
@keyframes wacky-float {
  0%, 100% { transform: translate(0, 0) rotate(0deg); }
  20% { transform: translate(12px, -18px) rotate(8deg); }
  40% { transform: translate(-8px, -30px) rotate(-5deg); }
  60% { transform: translate(-16px, -12px) rotate(6deg); }
  80% { transform: translate(6px, -22px) rotate(-4deg); }
}

@keyframes wacky-spin {
  from { transform: rotate(0deg); }
  to { transform: rotate(360deg); }
}

@keyframes wacky-bounce {
  0%, 100% { transform: translateY(0) scale(1); }
  50% { transform: translateY(-15px) scale(1.05); }
}

/* Floating shapes container */
.wacky-shapes {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  pointer-events: none;
  z-index: 1;
}

.wacky-shape {
  position: absolute;
  pointer-events: none;
}

.wacky-shape--float { animation: wacky-float 5s ease-in-out infinite; }
.wacky-shape--float-slow { animation: wacky-float 8s ease-in-out 1s infinite; }
.wacky-shape--spin { animation: wacky-spin 15s linear infinite; }
.wacky-shape--bounce { animation: wacky-bounce 2s ease-in-out infinite; }
```

### Slime / Goo Drip Border

```css
/* Slime drip along bottom edge of a section */
.wacky-slime-bottom {
  position: relative;
}

.wacky-slime-bottom::after {
  content: '';
  position: absolute;
  bottom: -18px;
  left: 0;
  right: 0;
  height: 24px;
  background: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 200 24' preserveAspectRatio='none'%3E%3Cpath d='M0,0 Q8,0 10,6 Q12,18 16,20 Q20,22 22,14 Q24,4 28,0 L50,0 Q52,0 54,8 Q56,18 60,22 Q64,24 66,16 Q68,6 72,0 L100,0 Q104,0 106,10 Q108,20 112,22 Q114,24 118,12 Q120,4 124,0 L150,0 Q152,0 154,6 Q156,16 160,20 Q162,22 166,10 Q168,4 172,0 L200,0' fill='%2369f0ae'/%3E%3C/svg%3E") repeat-x;
  background-size: 200px 24px;
  pointer-events: none;
  z-index: 3;
}
```

### Wavy Section Separator

```css
/* Wavy blob-like section separator */
.wacky-wave-divider {
  width: 100%;
  height: 50px;
  background: url("data:image/svg+xml,%3Csvg width='200' height='50' xmlns='http://www.w3.org/2000/svg'%3E%3Cpath d='M0 25 Q25 0 50 25 T100 25 T150 25 T200 25 L200 50 L0 50 Z' fill='%238b2fc9'/%3E%3C/svg%3E") repeat-x;
  background-size: 200px 50px;
}
```

---

## Key Design Elements and Motifs

### Fake Industrial / Sci-Fi Contraptions

A hallmark of Wacky Pomo is the inclusion of non-functional, toy-like "machinery" -- tubes, panels, levers, dials, gears, and control consoles that look like they belong in a cartoon laboratory or space station. On the web, simulate this with:

- Circular "dial" elements with thick borders and colored centers
- Rectangular "panel" sections with heavy outlines and rows of colored dot "indicators"
- Pipe-like connectors between sections using thick CSS borders on narrow elements
- Gear shapes (via `clip-path` or SVG) as decorative backgrounds

### Slime and Goo

Dripping, blobby, viscous forms are everywhere. Use irregular `border-radius` values, SVG drip paths along section edges, and semi-transparent green overlays to create gooey surfaces.

### Junk Food and Candy

References to snack culture -- bright candy-colored blocks, gumball-machine palettes, and shapes that evoke wrappers, packaging, and sugary excess. The overall palette should feel like a bag of mixed candy spilled out.

### Exaggerated Cartoon Faces and Characters

Even without illustration, suggest cartoonish personality through exaggerated proportions, wobbly arrangements, and elements that seem to "look" at the viewer (circles with smaller offset circles as "eyes," etc.).

### Oversized Toy Paraphernalia

Giant crayons, building blocks, game pieces, and playroom props as visual metaphors. Shapes should feel like physical objects you could pick up -- chunky, solid, slightly glossy.

---

## Materials and Textures (Visual Metaphors for Web)

| Physical Material | Web Equivalent |
|-------------------|----------------|
| Glossy injection-molded plastic | Solid bright colors with slight `linear-gradient` highlight (top-lighter, bottom-darker) suggesting sheen |
| Powder-coated metal | Flat, matte solid colors with no gradient, `border-radius: 0` for hard edges |
| Rubbery / silicone surfaces | Rounded corners (`border-radius: 12-20px`), slight squish animation on hover, saturated colors |
| Laminated cardboard prints | Solid color backgrounds with checkerboard or pattern overlay at low opacity, thick borders |
| Neon tube lighting | `box-shadow` glow effects in cyan or pink, `text-shadow` neon glow on headings |
| Toy plastic (chunky, shiny) | Heavy `box-shadow` offsets (5-8px solid color), thick black borders, slight rotation |
| Slime / goo | Irregular `border-radius` blobs, SVG drip shapes, semi-transparent green/purple overlays |
| Confetti / sprinkles | CSS `radial-gradient` dot patterns or scattered small geometric shapes via positioned pseudo-elements |
| Arcade cabinet / TV set | Heavy black bezels (thick borders), screen-like `border-radius` on corners, neon accent glow |

---

## Animation and Motion

- **Wobble and jiggle** -- elements that subtly rock side to side on hover, suggesting loose toy physics
- **Bouncing** -- shapes that bob up and down with spring-like easing
- **Spinning gears** -- decorative gear elements that rotate slowly and continuously
- **Morphing blobs** -- organic shapes that slowly shift their border-radius values
- **Chaotic floating** -- decorative elements that drift around in irregular paths
- **Scale pop on interaction** -- elements that "pop" larger when hovered, like pressing a squishy toy

```css
/* Wobble on hover */
@keyframes wacky-jiggle {
  0%, 100% { transform: rotate(-1deg); }
  25% { transform: rotate(2deg); }
  50% { transform: rotate(-2deg); }
  75% { transform: rotate(1deg); }
}

.wacky-jiggle:hover {
  animation: wacky-jiggle 0.4s ease-in-out;
}

/* Scale pop on hover */
.wacky-pop {
  transition: transform 0.15s ease;
}

.wacky-pop:hover {
  transform: scale(1.08) rotate(1deg);
}
```

---

## Media References

### Television (Core Visual DNA)

- **Pee-Wee's Playhouse** -- the ur-text of Wacky Pomo; a set design made entirely of clashing colors, talking furniture, and toy-scale architecture
- **Double Dare** -- physical obstacle courses rendered in bright primary and neon colors with slime as the centerpiece
- **The Ren & Stimpy Show** -- grotesque-yet-colorful cartoon excess with extreme close-ups and hyper-detailed gross-out
- **Animaniacs** -- rapid-fire cartoon chaos mixing Warner Bros. zany energy with postmodern self-awareness
- **Rocko's Modern Life** -- surreal suburban satire in garish, overlapping color schemes
- **KaBlam!** -- mixed-media anthology show with collage-style title cards and clashing visual formats
- **Cow and Chicken** -- aggressive color palettes and exaggerated body proportions
- **SpongeBob SquarePants** -- undersea environment rendered as a toybox, with chunky shapes and saturated colors
- **The Mask: Animated Series** -- cartoon physics at maximum exaggeration, neon green central motif
- **Cyberchase** -- digital world visualized through geometric shapes and bright, synthetic colors
- **Lazytown** -- hyperactive set design mixing physical props with digital candy-colored environments
- **Smiling Friends** -- contemporary revival of chaotic 90s cartoon energy

### Films

- **Who Framed Roger Rabbit?** -- live-action/cartoon hybrid as postmodern design statement
- **The Mask** -- cartoon logic applied to live action with garish green and yellow
- **Beetlejuice** -- Tim Burton's take on striped, spiraled, warped domestic interiors
- **Ace Ventura: Pet Detective** -- physical comedy rendered in loud, obnoxious visual environments
- **Spy Kids** franchise -- retro-futuristic gadgetry in candy-colored industrial settings
- **The Cat in the Hat** (2003) -- Dr. Seuss aesthetics pushed to maximum synthetic loudness

### Video Games

- **Kid Pix** -- the Wacky Pomo design tool; deliberately chaotic, stamp-based digital art for children
- **ToeJam & Earl** -- funky alien cartoon aesthetic in oversaturated color schemes
- **Day of the Tentacle** -- hand-drawn adventure game in warped, exaggerated environments
- **PaRappa the Rapper** -- paper-cutout visual style with bright flat colors and cartoon characters
- **Yoshi's Story** -- storybook/craft-material aesthetic in vivid colors
- **Psychonauts** -- surreal mental landscapes rendered in distorted, colorful geometry
- **Fall Guys** -- contemporary jelly-bean characters in bubblegum-bright obstacle courses

### Brands and Products

- **Nickelodeon** (1990s era) -- the defining brand of Wacky Pomo; orange splat logo, green slime, chaotic energy
- **Cartoon Network** (early era) -- checkerboard patterns, bold sans-serif type, black-and-white-with-color accents
- **YTV** -- Canadian children's network with alien mascot and neon-on-dark branding
- **Gushers** -- fruit snack packaging as concentrated Wacky Pomo design (neon colors, blob shapes, extreme flavor language)
- **CBeebies** -- UK children's brand with rounded, bright, toy-like design language

---

## Related Aesthetics

| Aesthetic | Relationship to Wacky Pomo |
|-----------|---------------------------|
| **Memphis Design** | Direct ancestor; Wacky Pomo commercializes and cartoonifies Memphis's postmodern geometric rebellion for kids' markets |
| **Memphis Lite** | Intermediate step; softened Memphis motifs that evolved into Wacky Pomo's toy-market applications |
| **Kidcore** | Close sibling; shares bright colors and child-oriented energy, but Kidcore is nostalgic and sweet where Wacky Pomo is aggressive and anarchic |
| **Kid Science** | Overlapping era and audience; Kid Science channels the same bright, chunky visual language toward educational content |
| **Neon Ooze** | Shares 90s kid-culture roots and slime/goo motifs; Neon Ooze is the dark, gross-out variant where Wacky Pomo is the bright, manic one |
| **Slimepunk** | Shares the goo/slime aesthetic and synthetic material feel, with a more subversive, punk attitude |
| **Googie Kitsch** | Shares the retro-futuristic, exaggerated, fun-over-function design philosophy |
| **Vectordelia** | Shares swirling, colorful, maximalist digital design energy |
| **Frutiger Aero** | Later aesthetic evolution; cleaner and more tech-optimistic but carries forward the glossy, bright, synthetic feel |
| **Y2K Futurism** | Chronological successor; inherits the plastic textures and neon accents but aims for sleek rather than chaotic |
| **Factory Pomo** | Industrial postmodernism; shares the playful violation of modernist rules, but applied to architecture rather than kids' media |
| **Festival Marketplace** | Shares the colorful, overstimulating, commerce-driven postmodern visual environment |
| **Vaporwave** | Nostalgic reimagination of the same 90s visual culture, but melancholic and ironic rather than manic and sincere |
| **Fleischer Style** | Shares the rubberhose animation aesthetic and surreal, stretchy cartoon physics |
| **Global Village Coffeehouse** | Shares the 90s postmodern eclecticism, but adult-oriented and "worldly" rather than kid-targeted |
| **Lowbrow** | Shares the anti-highbrow, cartoon-influenced, deliberately "tasteless" visual philosophy |

---

## Quick-Start: Minimal Wacky Pomo Page Template

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Wacky Pomo Page</title>
  <link href="https://fonts.googleapis.com/css2?family=Luckiest+Guy&family=Fredoka:wght@400;500;600;700&family=Bangers&family=Nunito:wght@400;600;700&display=swap" rel="stylesheet">
  <style>
    :root {
      --wacky-purple: #8b2fc9;
      --wacky-acid-green: #76ff03;
      --wacky-yellow: #ffd600;
      --wacky-orange: #ff6d00;
      --wacky-teal: #00bfa5;
      --wacky-pink: #ff4081;
      --wacky-fuchsia: #e040fb;
      --wacky-cyan: #18ffff;
      --wacky-white: #ffffff;
      --wacky-charcoal: #212121;
      --wacky-black: #000000;
    }

    * { margin: 0; padding: 0; box-sizing: border-box; }

    body {
      background: var(--wacky-white);
      color: var(--wacky-charcoal);
      font-family: 'Nunito', sans-serif;
      font-weight: 400;
      font-size: 1.05rem;
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
      padding: 16px 40px;
      background: var(--wacky-yellow);
      border-bottom: 4px solid var(--wacky-black);
    }

    nav .logo {
      font-family: 'Luckiest Guy', cursive;
      font-size: 1.6rem;
      color: var(--wacky-purple);
      text-decoration: none;
      text-shadow: 2px 2px 0 var(--wacky-black);
      display: inline-block;
      transform: rotate(-2deg);
    }

    nav ul {
      display: flex;
      gap: 8px;
      list-style: none;
    }

    nav ul a {
      display: inline-block;
      font-family: 'Fredoka', sans-serif;
      font-weight: 600;
      font-size: 0.95rem;
      color: var(--wacky-charcoal);
      text-decoration: none;
      text-transform: uppercase;
      letter-spacing: 0.04em;
      padding: 6px 14px;
      border: 2px solid transparent;
      border-radius: 6px;
      transition: all 0.15s;
    }

    nav ul a:hover {
      background: var(--wacky-purple);
      color: var(--wacky-white);
      border-color: var(--wacky-black);
      transform: rotate(-2deg) scale(1.05);
    }

    /* Hero */
    .hero {
      position: relative;
      min-height: 85vh;
      display: flex;
      align-items: center;
      justify-content: center;
      text-align: center;
      padding: 80px 40px;
      overflow: hidden;
      background: var(--wacky-purple);
    }

    .hero::before {
      content: '';
      position: absolute;
      inset: 0;
      background-image: repeating-conic-gradient(
        rgba(0, 0, 0, 0.05) 0% 25%, transparent 0% 50%
      );
      background-size: 40px 40px;
      pointer-events: none;
    }

    .hero-content {
      position: relative;
      z-index: 2;
      max-width: 800px;
    }

    .hero h1 {
      font-family: 'Luckiest Guy', cursive;
      font-size: clamp(3.5rem, 9vw, 8rem);
      text-transform: uppercase;
      color: var(--wacky-yellow);
      text-shadow:
        5px 5px 0 var(--wacky-black),
        -2px -2px 0 var(--wacky-black),
        2px -2px 0 var(--wacky-black),
        -2px 2px 0 var(--wacky-black);
      transform: rotate(-3deg);
      margin-bottom: 1.5rem;
      line-height: 0.95;
    }

    .hero p {
      font-size: 1.3rem;
      font-weight: 600;
      color: rgba(255, 255, 255, 0.95);
      margin-bottom: 2.5rem;
      text-shadow: 1px 1px 0 rgba(0, 0, 0, 0.3);
    }

    .btn {
      display: inline-block;
      padding: 14px 32px;
      border: 3px solid var(--wacky-black);
      border-radius: 8px;
      background: var(--wacky-yellow);
      color: var(--wacky-charcoal);
      font-family: 'Fredoka', sans-serif;
      font-weight: 700;
      font-size: 1.15rem;
      text-transform: uppercase;
      letter-spacing: 0.05em;
      text-decoration: none;
      cursor: pointer;
      box-shadow: 5px 5px 0 var(--wacky-black);
      transition: transform 0.12s, box-shadow 0.12s;
      transform: rotate(-1deg);
    }

    .btn:hover {
      transform: rotate(0deg) translate(-2px, -2px);
      box-shadow: 7px 7px 0 var(--wacky-black);
    }

    .btn:active {
      transform: rotate(0deg) translate(2px, 2px);
      box-shadow: 3px 3px 0 var(--wacky-black);
    }

    .btn--pink { background: var(--wacky-pink); color: var(--wacky-white); }
    .btn--green { background: var(--wacky-acid-green); color: var(--wacky-charcoal); }

    /* Decorative shapes */
    .shape {
      position: absolute;
      z-index: 1;
      pointer-events: none;
    }

    .shape--star-yellow {
      width: 70px; height: 70px;
      background: var(--wacky-yellow);
      clip-path: polygon(50% 0%, 61% 35%, 98% 35%, 68% 57%, 79% 91%, 50% 70%, 21% 91%, 32% 57%, 2% 35%, 39% 35%);
      top: 15%; right: 12%;
      filter: drop-shadow(2px 2px 0 var(--wacky-black));
      animation: wacky-float 5s ease-in-out infinite;
    }

    .shape--blob-pink {
      width: 120px; height: 100px;
      background: var(--wacky-pink);
      border-radius: 60% 40% 50% 45% / 45% 55% 40% 55%;
      top: 60%; right: 8%;
      border: 3px solid var(--wacky-black);
      animation: wacky-float 7s ease-in-out 1s infinite;
    }

    .shape--zigzag-teal {
      width: 100px; height: 40px;
      top: 25%; left: 8%;
      background: url("data:image/svg+xml,%3Csvg width='100' height='40' xmlns='http://www.w3.org/2000/svg'%3E%3Cpolyline points='0,40 12,0 24,40 36,0 48,40 60,0 72,40 84,0 100,40' stroke='%2300bfa5' stroke-width='4' fill='none'/%3E%3C/svg%3E") no-repeat;
      animation: wacky-float 6s ease-in-out 0.5s infinite;
    }

    .shape--gear-orange {
      width: 80px; height: 80px;
      background: var(--wacky-orange);
      border-radius: 50%;
      border: 3px solid var(--wacky-black);
      bottom: 20%; left: 15%;
      animation: wacky-spin 15s linear infinite;
    }
    .shape--gear-orange::before {
      content: '';
      position: absolute;
      inset: 12px;
      border-radius: 50%;
      border: 3px solid var(--wacky-black);
      background: var(--wacky-purple);
    }

    .shape--circle-green {
      width: 50px; height: 50px;
      border: 4px solid var(--wacky-acid-green);
      border-radius: 50%;
      top: 70%; right: 35%;
      animation: wacky-float 8s ease-in-out 2s infinite;
    }

    @keyframes wacky-float {
      0%, 100% { transform: translate(0, 0) rotate(0deg); }
      20% { transform: translate(12px, -18px) rotate(8deg); }
      40% { transform: translate(-8px, -30px) rotate(-5deg); }
      60% { transform: translate(-16px, -12px) rotate(6deg); }
      80% { transform: translate(6px, -22px) rotate(-4deg); }
    }

    @keyframes wacky-spin {
      from { transform: rotate(0deg); }
      to { transform: rotate(360deg); }
    }

    /* Zigzag divider */
    .zigzag {
      width: 100%;
      height: 24px;
      background: url("data:image/svg+xml,%3Csvg width='40' height='24' xmlns='http://www.w3.org/2000/svg'%3E%3Cpolyline points='0,24 20,0 40,24' stroke='%23000' stroke-width='3' fill='%23ffd600'/%3E%3C/svg%3E") repeat-x;
    }

    /* Features section */
    .features {
      padding: 80px 40px;
      position: relative;
      overflow: hidden;
      /* Confetti background */
      background-color: var(--wacky-white);
      background-image:
        radial-gradient(circle 4px, var(--wacky-purple) 100%, transparent 100%),
        radial-gradient(circle 3px, var(--wacky-acid-green) 100%, transparent 100%),
        radial-gradient(circle 5px, var(--wacky-yellow) 100%, transparent 100%),
        radial-gradient(circle 3px, var(--wacky-pink) 100%, transparent 100%);
      background-size: 200px 200px;
      background-position: 15px 25px, 70px 100px, 120px 50px, 170px 140px;
    }

    .features h2 {
      font-family: 'Luckiest Guy', cursive;
      font-size: clamp(2rem, 5vw, 3.5rem);
      text-align: center;
      margin-bottom: 3rem;
      color: var(--wacky-purple);
      text-shadow: 3px 3px 0 var(--wacky-yellow);
      transform: rotate(1deg);
    }

    .features-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
      gap: 32px;
      max-width: 1100px;
      margin: 0 auto;
    }

    .card {
      background: var(--wacky-white);
      border: 3px solid var(--wacky-black);
      border-radius: 8px;
      padding: 1.5rem 2rem;
      position: relative;
      transition: transform 0.2s, box-shadow 0.2s;
    }

    .card:nth-child(1) {
      box-shadow: 6px 6px 0 var(--wacky-purple);
      transform: rotate(-1.5deg);
    }
    .card:nth-child(2) {
      box-shadow: 6px 6px 0 var(--wacky-acid-green);
      transform: rotate(1deg);
    }
    .card:nth-child(3) {
      box-shadow: 6px 6px 0 var(--wacky-pink);
      transform: rotate(-2deg);
    }

    .card:hover {
      transform: rotate(0deg) translate(-3px, -3px) !important;
      box-shadow: 9px 9px 0 var(--wacky-orange) !important;
    }

    .card::after {
      content: '\2605';
      position: absolute;
      top: -10px;
      right: -10px;
      font-size: 1.5rem;
      color: var(--wacky-yellow);
      filter: drop-shadow(1px 1px 0 var(--wacky-black));
    }

    .card h3 {
      font-size: 1.3rem;
      margin-bottom: 0.5rem;
      color: var(--wacky-purple);
    }

    .card:nth-child(2) h3 { color: var(--wacky-teal); }
    .card:nth-child(3) h3 { color: var(--wacky-pink); }

    /* CTA section */
    .cta {
      background: var(--wacky-acid-green);
      color: var(--wacky-charcoal);
      text-align: center;
      padding: 80px 40px;
      border-top: 4px solid var(--wacky-black);
      border-bottom: 4px solid var(--wacky-black);
    }

    .cta h2 {
      font-family: 'Luckiest Guy', cursive;
      font-size: clamp(2rem, 5vw, 3.5rem);
      margin-bottom: 1rem;
      text-shadow: 3px 3px 0 var(--wacky-purple);
      color: var(--wacky-charcoal);
      transform: rotate(2deg);
    }

    .cta p {
      font-size: 1.15rem;
      font-weight: 600;
      margin-bottom: 2rem;
    }

    @media (max-width: 768px) {
      .hero { min-height: auto; padding: 60px 20px; }
      .hero h1 { font-size: 3rem; }
      nav { padding: 12px 20px; }
      nav ul { gap: 6px; }
      .shape { opacity: 0.6; }
      .features { padding: 60px 20px; }
    }
  </style>
</head>
<body>
  <nav>
    <a href="#" class="logo">WACKY!</a>
    <ul>
      <li><a href="#">About</a></li>
      <li><a href="#">Stuff</a></li>
      <li><a href="#">Contact</a></li>
    </ul>
  </nav>

  <section class="hero">
    <div class="hero-content">
      <h1>Totally Radical!</h1>
      <p>Where cartoon chaos meets postmodern design and everything is louder than it needs to be.</p>
      <a href="#" class="btn">Let's Go!</a>
    </div>
    <div class="shape shape--star-yellow"></div>
    <div class="shape shape--blob-pink"></div>
    <div class="shape shape--zigzag-teal"></div>
    <div class="shape shape--gear-orange"></div>
    <div class="shape shape--circle-green"></div>
  </section>

  <div class="zigzag"></div>

  <section class="features">
    <h2>What Makes It Wacky</h2>
    <div class="features-grid">
      <div class="card">
        <h3>Clashing Colors</h3>
        <p>Purple smashes into green, orange screams next to pink. Harmony is for adults -- this is pure chromatic chaos.</p>
      </div>
      <div class="card">
        <h3>Wobbly Everything</h3>
        <p>Nothing sits straight. Text tilts, cards rotate, shapes bounce. It is a playground, not a boardroom.</p>
      </div>
      <div class="card">
        <h3>Toy-Like Surfaces</h3>
        <p>Glossy plastic, chunky shadows, and thick outlines make everything look like you could pick it up and play with it.</p>
      </div>
    </div>
  </section>

  <div class="zigzag"></div>

  <section class="cta">
    <h2>Ready to Get Weird?</h2>
    <p>Wacky Pomo proves that more is more, louder is better, and good taste is overrated.</p>
    <a href="#" class="btn btn--pink">Smash It!</a>
  </section>
</body>
</html>
```
