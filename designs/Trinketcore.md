# Trinketcore -- Design Reference

Trinketcore (also known as **I-Spy**) is an aesthetic defined by its love of small, odd, mismatched objects -- kids' toys, vintage trinkets, buttons, board games, Polaroid photos, handcrafted curiosities, and junk-drawer treasures. It evokes **childlike wonder and nostalgia** through techniques like stop-motion animation, collage, maquettes, and papercraft-style 3D illustration. The mood is cozy, magical, and exploratory: warm lamp-lit rooms overflowing with curiosities, glow-in-the-dark stars on ceilings, autumn rain outside, and the feeling of discovering something delightful in a pile of forgotten objects.

---

## Visual Characteristics

### Core Motifs and Imagery

- **Trinkets and small objects** -- buttons, marbles, thimbles, keys, coins, dice, figurines, tiny toys, miscellaneous junk arranged in dense, layered compositions
- **Handcrafted materials** -- collage, papercraft, felt, yarn, clay, cardboard, stitching, and mixed-media textures that look made-by-hand
- **Stars and space** -- glow-in-the-dark ceiling stars, constellation maps, planets, rockets, and cosmic wonder filtered through a child's imagination
- **Board games and playing cards** -- scattered game pieces, dice, spinners, card suits, puzzle pieces
- **Books and reading** -- open books, stacked spines, bookmarks, dog-eared pages, illuminated reading nooks
- **Polaroid photographs** -- slightly faded snapshots, pinned to walls or scattered on surfaces
- **Lamps and warm lighting** -- desk lamps, string lights, lanterns casting pools of amber/yellow light in otherwise dim rooms
- **Autumn and rainy-day imagery** -- falling leaves, rain-streaked windows, puddles, cozy indoor scenes
- **Vintage and antique objects** -- aged, worn, slightly mysterious items with unknown histories
- **Magic and wonder elements** -- crystal balls, magnifying glasses, kaleidoscopes, snow globes, music boxes
- **Stop-motion and claymation quality** -- slightly imperfect, tactile, dimensional, with visible craft

### Design Principles

- **Maximalist layering** -- surfaces are dense with objects; emptiness is filled with curiosities
- **Handmade over polished** -- deliberate imperfection, visible craft marks, wobbly lines, and uneven edges
- **Warm intimacy** -- small, enclosed, lamp-lit spaces rather than vast open ones
- **Nostalgic wonder** -- everything feels rediscovered, like opening a forgotten box in an attic
- **Eclectic mixing** -- no two objects match; variety and surprise are the organizing principle
- **Tactile dimensionality** -- elements should feel like they have physical depth, texture, and weight (paper layers, shadow offsets, raised surfaces)
- **Playful exploration** -- the eye should wander and discover new details on each viewing

---

## Color Palette

### Primary Scheme

The palette is **muted and warm**, evoking aged objects under lamplight. Colors are never saturated or neon -- they look like they have been softened by time and amber light. Deep purples and blues replace black for dark tones.

| Role | Colors |
|------|--------|
| **Warm lights** | Amber, golden yellow, warm honey, lamplight glow |
| **Earthy base tones** | Warm brown, caramel, tan, kraft paper, cardboard |
| **Deep tones (replacing black)** | Plum purple, deep indigo, midnight blue |
| **Muted accents** | Dusty teal, sage green, faded coral, soft mustard |
| **Glow effects** | Pale yellow-green (glow-in-the-dark), soft phosphor |
| **Neutrals** | Warm cream, aged paper white, soft grey-brown |

### Detailed Color Table

| Color | Hex (suggested) | Usage |
|-------|-----------------|-------|
| Lamplight Gold | `#E8B84B`, `#D4A03C` | Primary accent, headings, glowing highlights |
| Warm Amber | `#C8923A`, `#B57F2E` | Borders, warm UI elements, hover states |
| Honey | `#E5C77D`, `#D9B96A` | Soft highlights, card backgrounds |
| Kraft Brown | `#A0805A`, `#8B6F4E` | Cardboard/paper texture tones, dividers |
| Caramel | `#7A5C3A`, `#6B4D30` | Dark accents, shadows, text on light backgrounds |
| Deep Plum | `#3E2252`, `#4A2D5E` | Primary dark tone (replaces black), deep backgrounds |
| Midnight Indigo | `#2A2545`, `#1E1B3A` | Darkest background, night-sky sections |
| Dusty Teal | `#5A8A7A`, `#4E7B6C` | Secondary accent, links, interactive elements |
| Sage Green | `#7A9A6E`, `#6B8B5E` | Nature accents, subtle highlights |
| Faded Coral | `#C47A6A`, `#B8695A` | Warm accent, buttons, small highlights |
| Glow Green | `#B8D882`, `#A5CC6E` | Glow-in-the-dark effect, star accents |
| Phosphor Yellow | `#E8E4A0`, `#D8D48E` | Soft glow halos, luminous details |
| Cream | `#F5ECD7`, `#EDE3C8` | Light backgrounds, text areas |
| Aged White | `#F0E8D4`, `#E8DFCA` | Page backgrounds |
| Warm Grey | `#8A7E72`, `#7A6E62` | Muted text, secondary elements |

### Suggested CSS Custom Properties

```css
:root {
  /* Warm Light Tones */
  --tc-lamplight: #e8b84b;
  --tc-amber: #c8923a;
  --tc-honey: #e5c77d;

  /* Browns / Kraft */
  --tc-kraft: #a0805a;
  --tc-caramel: #7a5c3a;
  --tc-cardboard: #8b6f4e;

  /* Deep Tones (replacing black) */
  --tc-plum: #3e2252;
  --tc-indigo: #2a2545;
  --tc-midnight: #1e1b3a;

  /* Muted Accents */
  --tc-teal: #5a8a7a;
  --tc-sage: #7a9a6e;
  --tc-coral: #c47a6a;

  /* Glow Effects */
  --tc-glow-green: #b8d882;
  --tc-phosphor: #e8e4a0;

  /* Neutrals */
  --tc-cream: #f5ecd7;
  --tc-aged-white: #f0e8d4;
  --tc-warm-grey: #8a7e72;

  /* Functional */
  --tc-bg-primary: var(--tc-aged-white);
  --tc-bg-dark: var(--tc-midnight);
  --tc-bg-card: var(--tc-cream);
  --tc-text-primary: var(--tc-caramel);
  --tc-text-heading: var(--tc-plum);
  --tc-text-on-dark: var(--tc-honey);
  --tc-accent: var(--tc-lamplight);
  --tc-accent-secondary: var(--tc-teal);
  --tc-border: var(--tc-kraft);
  --tc-glow: var(--tc-glow-green);
}
```

### Color Approach

- **Warm, muted palette** -- colors look like they are seen under a desk lamp in a cozy room
- **No pure black** -- use deep plum, indigo, or midnight tones instead
- **No pure white** -- use cream, aged paper, or honey tones
- **Amber/gold as the signature accent** -- lamplight warmth runs through everything
- **Glow-in-the-dark accents** -- pale green or phosphor yellow used sparingly for magical, luminous highlights
- **Layered warmth** -- multiple shades of brown and gold create depth without coldness

---

## Typography

### Typeface Characteristics

Trinketcore typography feels **handmade, playful, and slightly imperfect** -- as if lettered by hand on cardboard, stamped with mismatched type, or cut from magazine clippings. It should never look corporate or digitally sterile.

- **Handwritten or hand-drawn primary fonts** -- slightly wobbly, organic, with visible personality
- **Rounded, friendly letterforms** -- approachable and warm, never sharp or aggressive
- **Mixed styles** -- combining handwritten headers with cleaner body text mirrors the collage/mixed-media spirit
- **Sticker/stamp quality for accents** -- labels, tags, and callouts can use blocky or typewriter-style fonts
- **Moderate weight variation** -- not too thin (feels fragile) or too heavy (feels industrial)

### Recommended Web Fonts (Google Fonts / Free)

| Font | Style | Usage |
|------|-------|-------|
| **Patrick Hand** | Casual handwriting | Headings, display text |
| **Architects Daughter** | Informal hand-lettered | Headings, feature titles |
| **Caveat** | Natural handwriting | Subheadings, annotations, captions |
| **Comic Neue** | Cleaned-up comic-style | Body text, readable handmade feel |
| **Baloo 2** | Rounded, chunky, playful | Display headings, buttons |
| **Indie Flower** | Loose, informal handwriting | Decorative text, labels |
| **Special Elite** | Typewriter-style | Captions, labels, stamp-like elements |
| **Pangolin** | Rounded handwritten | Body text alternative |
| **Fredericka the Great** | Sketchy, hand-drawn display | Hero titles, large decorative text |
| **Coming Soon** | Childlike handwriting | Annotations, playful accents |

### Typography CSS Example

```css
/* Import fonts */
@import url('https://fonts.googleapis.com/css2?family=Patrick+Hand&family=Caveat:wght@400;600&family=Comic+Neue:wght@400;700&family=Special+Elite&display=swap');

/* Headlines */
h1, h2, h3 {
  font-family: 'Patrick Hand', 'Architects Daughter', cursive;
  color: var(--tc-plum);
  font-weight: 400;
  letter-spacing: 0.02em;
  line-height: 1.3;
}

/* Display / Hero text */
.tc-display {
  font-family: 'Patrick Hand', cursive;
  font-size: clamp(2.5rem, 6vw, 5rem);
  letter-spacing: 0.03em;
  line-height: 1.2;
  color: var(--tc-lamplight);
  text-shadow: 2px 2px 0 var(--tc-caramel);
}

/* Body text */
body {
  font-family: 'Comic Neue', 'Pangolin', 'Trebuchet MS', sans-serif;
  font-size: 1.1rem;
  font-weight: 400;
  letter-spacing: 0.01em;
  line-height: 1.75;
  color: var(--tc-caramel);
}

/* Labels, tags, stamp-like text */
.tc-label {
  font-family: 'Special Elite', 'Courier New', monospace;
  font-size: 0.85rem;
  text-transform: uppercase;
  letter-spacing: 0.1em;
  color: var(--tc-kraft);
}

/* Handwritten annotations */
.tc-annotation {
  font-family: 'Caveat', cursive;
  font-size: 1.25rem;
  color: var(--tc-teal);
  transform: rotate(-2deg);
}
```

---

## Layout Principles

### Grid and Structure

- **Scrapbook / collage-style layouts** -- items appear pinned, taped, or scattered rather than rigidly gridded
- **Layered depth** -- overlapping elements, slight rotations, and shadows create a sense of physical dimension
- **Asymmetric, organic arrangement** -- not perfectly aligned; items feel placed by hand
- **Dense but navigable** -- lots of visual elements, but clear focal points guide the eye
- **Contained in frames** -- sections framed like display boxes, shadow boxes, or shelf compartments
- **Vertical scrolling as exploration** -- each scroll reveals a new "shelf" or "drawer" of discoveries

### Section Organization

- Use **torn paper edges, tape strips, and stitched dividers** between sections
- Apply **slight rotations (1-3 degrees)** to cards and images for a pinned-to-corkboard feel
- Create **shadow-box containers** -- deep inset shadows make panels feel like physical compartments
- **Shelf and grid-of-objects layouts** for collections of items
- **Sticky notes and tags** as supplementary UI elements
- **String-and-pin connections** between related elements

---

## CSS/Design Techniques

### Kraft Paper / Cardboard Background

```css
.tc-kraft-bg {
  background-color: var(--tc-cream);
  background-image:
    url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='6' height='6'%3E%3Crect width='6' height='6' fill='%23f5ecd7'/%3E%3Crect width='2' height='1' x='1' y='2' fill='%23e8dfca' opacity='0.3'/%3E%3Crect width='1' height='2' x='4' y='4' fill='%23ddd4be' opacity='0.2'/%3E%3C/svg%3E");
}
```

### Torn Paper Edge

```css
.tc-torn-edge {
  position: relative;
  background: var(--tc-cream);
  padding: 2rem;
}

.tc-torn-edge::after {
  content: '';
  position: absolute;
  bottom: -8px;
  left: 0;
  right: 0;
  height: 16px;
  background: var(--tc-cream);
  clip-path: polygon(
    0% 0%, 3% 60%, 6% 20%, 9% 70%, 12% 30%,
    15% 80%, 18% 10%, 21% 60%, 24% 40%, 27% 90%,
    30% 20%, 33% 70%, 36% 30%, 39% 80%, 42% 10%,
    45% 60%, 48% 40%, 51% 85%, 54% 15%, 57% 65%,
    60% 25%, 63% 75%, 66% 35%, 69% 80%, 72% 20%,
    75% 70%, 78% 30%, 81% 60%, 84% 10%, 87% 75%,
    90% 40%, 93% 85%, 96% 20%, 100% 55%, 100% 0%
  );
}
```

### Tape Strip Accent

```css
.tc-tape {
  position: relative;
  display: inline-block;
  padding: 0.3em 1.5em;
  background: rgba(232, 228, 160, 0.5);
  transform: rotate(-1.5deg);
  box-shadow: 0 1px 3px rgba(0, 0, 0, 0.1);
}

.tc-tape::before,
.tc-tape::after {
  content: '';
  position: absolute;
  top: 0;
  width: 12px;
  height: 100%;
  background: rgba(232, 228, 160, 0.3);
}

.tc-tape::before { left: -6px; }
.tc-tape::after { right: -6px; }
```

### Shadow Box / Display Case Panel

```css
.tc-shadow-box {
  background: var(--tc-cream);
  border: 2px solid var(--tc-kraft);
  padding: 2rem;
  box-shadow:
    inset 0 2px 8px rgba(122, 92, 58, 0.2),
    inset 0 -2px 8px rgba(122, 92, 58, 0.1),
    3px 4px 0 var(--tc-cardboard),
    5px 6px 12px rgba(30, 27, 58, 0.15);
  border-radius: 4px;
}
```

### Pinned Card (Corkboard Style)

```css
.tc-pinned-card {
  background: var(--tc-cream);
  border: 1px solid var(--tc-kraft);
  padding: 1.5rem;
  transform: rotate(-1.5deg);
  box-shadow: 2px 3px 8px rgba(30, 27, 58, 0.15);
  position: relative;
}

/* Pin dot */
.tc-pinned-card::before {
  content: '';
  position: absolute;
  top: -6px;
  left: 50%;
  transform: translateX(-50%);
  width: 14px;
  height: 14px;
  background: radial-gradient(circle, var(--tc-coral) 40%, #a0524a 60%);
  border-radius: 50%;
  box-shadow: 0 2px 3px rgba(0, 0, 0, 0.3);
}
```

### Glow-in-the-Dark Star Effect

```css
.tc-glow-star {
  color: var(--tc-glow-green);
  text-shadow:
    0 0 4px var(--tc-glow-green),
    0 0 12px rgba(184, 216, 130, 0.5),
    0 0 24px rgba(184, 216, 130, 0.2);
  animation: tc-pulse 3s ease-in-out infinite alternate;
}

@keyframes tc-pulse {
  0% { opacity: 0.7; }
  100% { opacity: 1; }
}
```

### Lamplight Glow Effect

```css
.tc-lamplight {
  position: relative;
}

.tc-lamplight::after {
  content: '';
  position: absolute;
  inset: 0;
  background: radial-gradient(
    ellipse at 50% 20%,
    rgba(232, 184, 75, 0.12) 0%,
    rgba(232, 184, 75, 0.04) 40%,
    transparent 70%
  );
  pointer-events: none;
}
```

### Stitched Border

```css
.tc-stitched {
  border: 2px dashed var(--tc-kraft);
  border-radius: 6px;
  padding: 1.5rem;
  outline: 2px solid var(--tc-cream);
  outline-offset: 4px;
  background: var(--tc-cream);
}
```

### Night Sky / Stars Background

```css
.tc-night-sky {
  background: linear-gradient(
    to bottom,
    var(--tc-midnight) 0%,
    var(--tc-indigo) 40%,
    var(--tc-plum) 100%
  );
  position: relative;
  overflow: hidden;
}

/* Scattered stars via radial gradients */
.tc-night-sky::before {
  content: '';
  position: absolute;
  inset: 0;
  background-image:
    radial-gradient(1px 1px at 10% 15%, var(--tc-glow-green) 50%, transparent 50%),
    radial-gradient(1.5px 1.5px at 25% 45%, var(--tc-phosphor) 50%, transparent 50%),
    radial-gradient(1px 1px at 40% 10%, var(--tc-glow-green) 50%, transparent 50%),
    radial-gradient(2px 2px at 55% 70%, var(--tc-phosphor) 50%, transparent 50%),
    radial-gradient(1px 1px at 70% 30%, var(--tc-glow-green) 50%, transparent 50%),
    radial-gradient(1.5px 1.5px at 85% 55%, var(--tc-phosphor) 50%, transparent 50%),
    radial-gradient(1px 1px at 15% 80%, var(--tc-glow-green) 50%, transparent 50%),
    radial-gradient(1px 1px at 60% 90%, var(--tc-phosphor) 50%, transparent 50%),
    radial-gradient(2px 2px at 90% 15%, var(--tc-glow-green) 50%, transparent 50%),
    radial-gradient(1px 1px at 35% 60%, var(--tc-phosphor) 50%, transparent 50%);
  pointer-events: none;
}
```

### Trinket Collection Grid

```css
.tc-collection {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(200px, 1fr));
  gap: 1.5rem;
  padding: 2rem;
}

.tc-collection > * {
  transform: rotate(calc(var(--rotation, 0) * 1deg));
}

/* Apply varied rotations via inline style --rotation or nth-child */
.tc-collection > *:nth-child(odd) { transform: rotate(-1.5deg); }
.tc-collection > *:nth-child(even) { transform: rotate(1deg); }
.tc-collection > *:nth-child(3n) { transform: rotate(2deg); }
```

### Dark Variant (Night / Attic)

```css
.tc-dark {
  background: var(--tc-midnight);
  color: var(--tc-honey);
}

.tc-dark h1, .tc-dark h2, .tc-dark h3 {
  color: var(--tc-lamplight);
  text-shadow: 0 0 8px rgba(232, 184, 75, 0.3);
}

.tc-dark .tc-shadow-box {
  background: var(--tc-indigo);
  border-color: var(--tc-plum);
  box-shadow:
    inset 0 2px 8px rgba(0, 0, 0, 0.3),
    3px 4px 0 rgba(0, 0, 0, 0.4),
    5px 6px 16px rgba(0, 0, 0, 0.3);
}

.tc-dark .tc-pinned-card {
  background: var(--tc-plum);
  border-color: var(--tc-kraft);
  color: var(--tc-cream);
}
```

---

## Materials and Textures (Visual Metaphors for Web)

| Physical Material | Web Equivalent |
|-------------------|----------------|
| Kraft paper / cardboard | Warm cream/tan backgrounds with subtle fibrous noise texture |
| Felt and fabric | Soft, slightly textured card surfaces with rounded edges |
| Yarn and string | Dashed or dotted connecting lines, stitched borders |
| Clay and plasticine | Rounded elements with soft inner shadows, dimensional feel |
| Aged photographs (Polaroid) | Image containers with thick white borders and slight sepia tint |
| Washi tape / masking tape | Semi-transparent colored strips as decorative accents |
| Cork board | Warm brown-speckled background for pinned element layouts |
| Glow-in-the-dark plastic | Pale green/yellow elements with blur-based glow effects |
| Buttons and beads | Small circular decorative elements, dot patterns |
| Worn book pages | Off-white text areas with subtle discoloration gradients |
| Wooden shelves | Horizontal dividers with wood-grain-like gradient bands |
| Stamp ink | Slightly rough-edged text with typewriter fonts |

---

## Iconic Visual References

### Film and Animation

- **Coraline** (2009) -- stop-motion, button eyes, handcrafted world-building, secret doors and eerie wonder
- **WALL-E** (2008) -- collecting trinkets, curiosity about small objects, lonely lamp-lit spaces
- **Wallace and Gromit** -- claymation, warm domestic settings, inventor's clutter
- **The Little Prince** -- papercraft-style illustration, stars, wonder, intimate scale
- **Flushed Away** -- miniature worlds made from found objects
- **LittleBigPlanet** (game series) -- cardboard, fabric, stickers, buttons, and craft supplies as entire world-building materials

### Game Design References

- **Yoshi's Crafted World** / **Yoshi's Woolly World** -- levels built from yarn, cardboard, and craft supplies
- **Tearaway** -- papercraft world, everything is foldable and tactile
- **Paper Mario** series -- flat paper characters in a dimensional world
- **Katamari Damacy** -- rolling up miscellaneous objects, celebrating the joy of random small things
- **Kirby's Epic Yarn** -- fabric and thread as fundamental visual language
- **Night in the Woods** -- autumn, small-town nostalgia, warm muted palette

---

## Related Aesthetics

| Aesthetic | Relationship to Trinketcore |
|-----------|---------------------------|
| **Cozy Childhood Hideaway** | Overlapping focus on intimate childhood spaces, blanket forts, warm lighting |
| **Indiecraft** | Shared love of handmade, DIY creation, and craft materials |
| **Crowcore** | Shared attraction to collecting shiny, odd, miscellaneous small objects |
| **Whimsigothic** | Shared mystical/magical atmosphere, candles and ambient lighting, eclectic collecting |
| **Twee** | Shared gentle, nostalgic, whimsical tone; handmade and vintage emphasis |
| **Cottagecore** | Overlapping warmth, coziness, and handcraft, but Trinketcore is more cluttered and object-focused |

---

## Quick-Start: Minimal Trinketcore Page Template

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Trinketcore Page</title>
  <link href="https://fonts.googleapis.com/css2?family=Patrick+Hand&family=Comic+Neue:wght@400;700&family=Special+Elite&family=Caveat:wght@400;600&display=swap" rel="stylesheet">
  <style>
    :root {
      --tc-lamplight: #e8b84b;
      --tc-amber: #c8923a;
      --tc-honey: #e5c77d;
      --tc-kraft: #a0805a;
      --tc-caramel: #7a5c3a;
      --tc-cardboard: #8b6f4e;
      --tc-plum: #3e2252;
      --tc-indigo: #2a2545;
      --tc-midnight: #1e1b3a;
      --tc-teal: #5a8a7a;
      --tc-coral: #c47a6a;
      --tc-glow-green: #b8d882;
      --tc-cream: #f5ecd7;
      --tc-aged-white: #f0e8d4;
      --tc-warm-grey: #8a7e72;
    }

    * { margin: 0; padding: 0; box-sizing: border-box; }

    body {
      background: var(--tc-aged-white);
      color: var(--tc-caramel);
      font-family: 'Comic Neue', 'Trebuchet MS', sans-serif;
      font-size: 1.1rem;
      line-height: 1.75;
    }

    h1, h2, h3 {
      font-family: 'Patrick Hand', cursive;
      color: var(--tc-plum);
      font-weight: 400;
      letter-spacing: 0.02em;
    }

    .hero {
      background: linear-gradient(to bottom, var(--tc-midnight), var(--tc-indigo));
      text-align: center;
      padding: 5rem 2rem 4rem;
      position: relative;
      overflow: hidden;
    }

    .hero h1 {
      font-size: clamp(2.5rem, 6vw, 4.5rem);
      color: var(--tc-lamplight);
      text-shadow: 2px 2px 0 var(--tc-caramel), 0 0 20px rgba(232, 184, 75, 0.3);
      margin-bottom: 1rem;
    }

    .hero p {
      font-family: 'Caveat', cursive;
      font-size: 1.4rem;
      color: var(--tc-honey);
    }

    .hero .star {
      color: var(--tc-glow-green);
      text-shadow: 0 0 6px var(--tc-glow-green);
    }

    section {
      max-width: 900px;
      margin: 0 auto;
      padding: 3rem 2rem;
    }

    .tc-card {
      background: var(--tc-cream);
      border: 2px solid var(--tc-kraft);
      padding: 1.5rem;
      margin: 1.5rem 0;
      box-shadow:
        inset 0 2px 6px rgba(122, 92, 58, 0.15),
        3px 4px 0 var(--tc-cardboard);
      border-radius: 4px;
      transform: rotate(-0.5deg);
    }

    .tc-card:nth-child(even) {
      transform: rotate(0.8deg);
    }

    .tc-card h3 {
      font-family: 'Patrick Hand', cursive;
      color: var(--tc-plum);
      margin-bottom: 0.5rem;
    }

    .tc-label {
      font-family: 'Special Elite', monospace;
      font-size: 0.8rem;
      text-transform: uppercase;
      letter-spacing: 0.1em;
      color: var(--tc-kraft);
    }

    .divider {
      border: none;
      border-top: 2px dashed var(--tc-kraft);
      margin: 2rem auto;
      width: 60%;
    }
  </style>
</head>
<body>
  <div class="hero">
    <p class="star">&#9733; &#9733; &#9733;</p>
    <h1>Title Here</h1>
    <p>A subtitle in handwritten style</p>
  </div>
  <section>
    <h2>Section Heading</h2>
    <hr class="divider">
    <div class="tc-card">
      <span class="tc-label">Exhibit A</span>
      <h3>A Curious Discovery</h3>
      <p>Content styled in the Trinketcore tradition -- warm, handcrafted, and full of small wonders.</p>
    </div>
    <div class="tc-card">
      <span class="tc-label">Exhibit B</span>
      <h3>Another Treasure</h3>
      <p>Each card is slightly rotated, like something pinned to a corkboard or tucked into a scrapbook.</p>
    </div>
  </section>
</body>
</html>
```
