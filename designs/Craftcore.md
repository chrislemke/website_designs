# Craftcore Design Reference

Craftcore is a maximalist, handmade-forward aesthetic that celebrates **visible artisanal craftsmanship** in finished items. Rooted in traditional textile arts -- knitting, crochet, embroidery, quilting, macrame -- it elevates "granny crafts" into a deliberate style statement. Every piece is proudly, obviously handmade: no two items are alike, imperfections are features, and the human hand behind the work is always visible. Craftcore emerged as a counter-movement to fast fashion and mass-produced uniformity, aligned with slow fashion, sustainability, and mindful creation. Luxury houses like Chloe, Valentino, Dior, Bode, and Chopova Lowena have brought craftcore techniques to mainstream runways, proving that handmade is high fashion.

---

## Visual Characteristics

### Core Motifs and Patterns

- **Patchwork and quilting** -- pieced-together fabric panels in contrasting colors and prints, visible seaming
- **Crochet and chunky knits** -- colossal yarn textures, granny squares, crocheted trims and borders
- **Embroidery and beading** -- hand-stitched motifs, cross-stitch patterns, beaded accents on fabric
- **Macrame** -- knotted cord wall hangings, plant holders, fringe and tassel details
- **Artisanal tie-dye** -- hand-dipped color gradients, wax-resist patterns, shibori techniques
- **Hand-painted surfaces** -- brushstroke textures on pottery, ceramics, and textiles
- **Visible stitching** -- exposed seams, decorative topstitching, running stitch borders
- **Folk art motifs** -- flowers, birds, geometric patterns drawn from traditional craft traditions
- **Collage and layering** -- overlapping textures, cut-and-reassembled compositions
- **Woven textures** -- basket weave, tapestry, loom patterns with visible warp and weft

### Design Principles

- **Handmade over perfection** -- intentional imperfections, wobbly edges, and organic forms are celebrated
- **Visible process** -- the making should be evident in the finished product; construction methods are decorative
- **Texture as primary design element** -- depth comes from layered tactile surfaces, not flat graphics
- **Warm authenticity** -- every element should feel human-touched, soulful, and personal
- **Eclectic mixing** -- different craft traditions, materials, and techniques coexist harmoniously
- **Sustainability narrative** -- repurposed, vintage, and natural materials are preferred over synthetic
- **Nostalgic warmth** -- references traditional domestic crafts without irony; genuine appreciation
- **Individual expression** -- unique, one-of-a-kind compositions over repeatable templates
- **Slow, deliberate composition** -- designs encourage the viewer to linger and notice details
- **Analog texture in digital space** -- risograph effects, letterpress textures, paper grain overlays simulate handmade quality

---

## Color Palette

### Primary Scheme

| Role | Colors |
|------|--------|
| **Base / Background** | Natural linen, warm oatmeal, unbleached cotton, soft cream |
| **Earth tones** | Clay, terracotta, raw sienna, warm brown, ochre |
| **Botanical greens** | Moss, sage, olive, fern, forest green |
| **Craft brights** | Sorbet pink, marigold yellow, cornflower blue, berry purple |
| **Warm neutrals** | Camel, biscuit, sandstone, driftwood |
| **Accent darks** | Indigo, charcoal, espresso, burgundy |

### Detailed Palette

| Color | Hex (suggested) | Usage |
|-------|-----------------|-------|
| Unbleached Linen | `#F4EDE4`, `#EDE6DB` | Primary background, base surface |
| Oatmeal | `#E8DFD0`, `#DDD4C4` | Secondary backgrounds, card surfaces |
| Raw Cotton | `#FAF6F0`, `#F8F3EB` | White-equivalent, clean areas |
| Clay | `#C17A5A`, `#B86E4E` | Primary warm accent, handmade feel |
| Terracotta | `#C25B3F`, `#D4654A` | Warm highlights, borders |
| Ochre | `#CC9B3A`, `#D9A842` | Accent badges, stitch details |
| Marigold | `#E8A832`, `#F0B840` | Bright warm accent, call-to-action |
| Moss Green | `#6B7F56`, `#7A8E64` | Nature accents, secondary elements |
| Sage | `#9CAE8A`, `#A8B898` | Soft green, background tints |
| Sorbet Pink | `#E8889A`, `#F09AAB` | Bright craft accent, yarn-inspired |
| Berry | `#8E4066`, `#A04A76` | Rich accent, embroidery-inspired |
| Cornflower | `#6488B4`, `#7098C4` | Cool accent, links |
| Indigo | `#3A4A6E`, `#44567E` | Deep contrast, text-heavy areas |
| Espresso | `#4A3628`, `#5C4438` | Dark text, frame borders |
| Driftwood | `#8C7B6B`, `#9A8878` | Neutral medium tone, dividers |
| Charcoal | `#3E3A36`, `#4A4642` | Body text, dark accents |

### Suggested CSS Custom Properties

```css
:root {
  /* Natural base tones */
  --craft-linen: #f4ede4;
  --craft-oatmeal: #e8dfd0;
  --craft-cotton: #faf6f0;
  --craft-parchment: #ede6db;

  /* Earth and clay tones */
  --craft-clay: #c17a5a;
  --craft-terracotta: #c25b3f;
  --craft-ochre: #cc9b3a;
  --craft-marigold: #e8a832;

  /* Botanical greens */
  --craft-moss: #6b7f56;
  --craft-sage: #9cae8a;
  --craft-olive: #7a7a50;
  --craft-fern: #5a7a4a;

  /* Craft brights */
  --craft-sorbet: #e8889a;
  --craft-berry: #8e4066;
  --craft-cornflower: #6488b4;
  --craft-lavender: #9888b4;

  /* Warm neutrals and darks */
  --craft-driftwood: #8c7b6b;
  --craft-espresso: #4a3628;
  --craft-charcoal: #3e3a36;
  --craft-camel: #c4a87a;

  /* Functional mappings */
  --craft-bg-primary: var(--craft-linen);
  --craft-bg-secondary: var(--craft-oatmeal);
  --craft-bg-card: var(--craft-cotton);
  --craft-text-primary: var(--craft-charcoal);
  --craft-text-secondary: var(--craft-driftwood);
  --craft-text-heading: var(--craft-espresso);
  --craft-accent: var(--craft-clay);
  --craft-accent-bright: var(--craft-marigold);
  --craft-border: var(--craft-camel);
  --craft-link: var(--craft-cornflower);
  --craft-link-hover: var(--craft-berry);
  --craft-stitch: var(--craft-terracotta);
}
```

### Approaches

- **Natural fiber inspiration** -- colors should feel like they come from natural dyes and unprocessed materials
- **Warm base with handmade pops** -- linen/oatmeal backgrounds anchor vibrant craft-bright accents
- **Sorbet and earth together** -- bright yarn colors (pink, marigold, cornflower) sit alongside earthy clay and moss
- **Muted saturation** -- even bright colors feel slightly softened, as if sun-faded or naturally dyed
- **Textured color application** -- colors appear slightly uneven, as if hand-painted or dyed rather than digitally flat
- **Complementary craft pairs** -- terracotta + sage, marigold + indigo, berry + moss are natural pairings

---

## Typography

### Typeface Characteristics

Craftcore typography emphasizes warmth, tactility, and handmade character:

- **Hand-drawn and script fonts** -- primary stylistic choice; letterforms should look brushed, stitched, or stamped
- **Letterpress and woodblock serifs** -- vintage printing aesthetics with ink bleed and slight irregularity
- **Warm, organic serifs** -- not sharp or geometric; rounded terminals and calligraphic influence
- **Rounded sans-serifs for readability** -- body text stays friendly and approachable
- **Visible texture in type** -- fonts that suggest a printing process (risograph, woodcut, hand-stamp)
- **Mixed font weights and styles** -- headings, accents, and body can each use different font families

### Recommended Web Fonts (Google Fonts / Free)

| Font | Style | Usage |
|------|-------|-------|
| **Amatic SC** | Hand-drawn, condensed | Hero headlines, display text |
| **Caveat** | Handwritten, natural flow | Annotations, decorative labels, captions |
| **Kalam** | Handwritten, warm brush-style | Subheadings, accent text |
| **Patrick Hand** | Handwritten, casual | Callouts, pull quotes |
| **Vollkorn** | Warm, organic serif | Subheadings, long-form body text |
| **Lora** | Calligraphic serif | Block quotes, feature text |
| **Crimson Pro** | Classic, book-style serif | Body text alternative |
| **Nunito** | Rounded, friendly sans-serif | Body text, UI elements |
| **Quicksand** | Rounded geometric sans-serif | Labels, navigation, tags |
| **Special Elite** | Typewriter, vintage feel | Monospace accents, labels |
| **Shadows Into Light** | Script, dreamy handwritten | Decorative pull quotes |
| **DM Serif Display** | Bold display serif | Section headings with weight |

### Typography CSS Example

```css
/* Display headlines -- hand-drawn character */
h1 {
  font-family: 'Amatic SC', 'Caveat', cursive;
  font-weight: 700;
  font-size: clamp(2.8rem, 6vw, 5rem);
  color: var(--craft-text-heading);
  line-height: 1.1;
  letter-spacing: 0.02em;
}

/* Section headings -- warm serif */
h2 {
  font-family: 'Vollkorn', 'Lora', Georgia, serif;
  font-weight: 700;
  font-size: clamp(1.6rem, 3.5vw, 2.4rem);
  color: var(--craft-text-heading);
  line-height: 1.25;
}

/* Subsection headings */
h3 {
  font-family: 'Vollkorn', 'Lora', Georgia, serif;
  font-weight: 600;
  font-size: clamp(1.2rem, 2.5vw, 1.7rem);
  color: var(--craft-clay);
  line-height: 1.3;
}

/* Body text -- rounded and readable */
body {
  font-family: 'Nunito', 'Quicksand', sans-serif;
  font-weight: 400;
  font-size: 1rem;
  line-height: 1.75;
  color: var(--craft-text-primary);
}

/* Handwritten accent text */
.craft-handwritten {
  font-family: 'Caveat', 'Kalam', cursive;
  font-size: 1.4em;
  color: var(--craft-clay);
  transform: rotate(-1.5deg);
  display: inline-block;
}

/* Labels and tags */
.craft-tag {
  font-family: 'Quicksand', 'Nunito', sans-serif;
  font-size: 0.72rem;
  font-weight: 600;
  text-transform: uppercase;
  letter-spacing: 0.1em;
  color: var(--craft-text-secondary);
}

/* Decorative pull quote */
.craft-quote {
  font-family: 'Patrick Hand', 'Shadows Into Light', cursive;
  font-size: 1.5rem;
  line-height: 1.5;
  color: var(--craft-berry);
  border-left: 4px dashed var(--craft-terracotta);
  padding-left: 1.5rem;
}
```

---

## Layout Principles

### Grid and Structure

- **Patchwork grid layouts** -- asymmetric panels of different sizes stitched together, like a quilt
- **Collage-style composition** -- overlapping elements, cut-out shapes, torn-edge frames
- **Organic spacing** -- slightly irregular gaps between elements, avoiding mechanical uniformity
- **Layered depth** -- background textures, mid-ground content, foreground decorative stitching/tape
- **Masonry arrangements** -- items of varying heights fit together naturally, like objects on a craft table
- **Visible construction** -- borders that look like stitching, dividers that look like yarn or thread
- **Rotated and tilted elements** -- slight rotations (1-3 degrees) as if hand-placed, like fabric patches
- **Full surface use** -- the page should feel populated and cozy, not sparse; "blank canvas" is against the ethos

### Section Organization

- Use **varied section backgrounds** -- alternate between linen, tinted washes, and textured panels
- Apply **stitch-like borders** -- dashed lines, dotted lines, and running-stitch SVG borders between sections
- Create **craft-table metaphors** -- sections that look like workbenches strewn with materials
- Employ **fabric-patch shapes** for containers -- rounded corners, slightly irregular borders
- Use **tape, pins, and stitch decorations** to attach elements visually
- Incorporate **collage overlaps** -- elements that break out of their containers slightly

---

## CSS/Design Techniques

### Linen / Fabric Textured Background

```css
/* Natural linen background with subtle woven texture */
.craft-bg {
  background-color: var(--craft-linen);
  background-image:
    repeating-linear-gradient(
      0deg,
      transparent,
      transparent 3px,
      rgba(74, 54, 40, 0.015) 3px,
      rgba(74, 54, 40, 0.015) 4px
    ),
    repeating-linear-gradient(
      90deg,
      transparent,
      transparent 3px,
      rgba(74, 54, 40, 0.015) 3px,
      rgba(74, 54, 40, 0.015) 4px
    );
}

/* Paper grain / risograph texture overlay */
.craft-grain::before {
  content: '';
  position: absolute;
  inset: 0;
  background-image: url("data:image/svg+xml,%3Csvg viewBox='0 0 256 256' xmlns='http://www.w3.org/2000/svg'%3E%3Cfilter id='noise'%3E%3CfeTurbulence type='fractalNoise' baseFrequency='0.85' numOctaves='4' stitchTiles='stitch'/%3E%3C/filter%3E%3Crect width='100%25' height='100%25' filter='url(%23noise)' opacity='0.04'/%3E%3C/svg%3E");
  pointer-events: none;
  z-index: 0;
}
```

### Patchwork / Quilt Grid Layout

```css
/* Patchwork quilt grid -- varied panel sizes */
.craft-patchwork-grid {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(240px, 1fr));
  gap: 0;
  padding: 1rem;
}

/* Panels with visible "seam" borders */
.craft-patch {
  padding: 2rem;
  position: relative;
  border: 2px dashed var(--craft-camel);
}

/* Alternating patch backgrounds for quilt effect */
.craft-patch:nth-child(4n+1) { background: var(--craft-cotton); }
.craft-patch:nth-child(4n+2) { background: rgba(156, 174, 138, 0.12); }
.craft-patch:nth-child(4n+3) { background: rgba(232, 136, 154, 0.08); }
.craft-patch:nth-child(4n+4) { background: rgba(204, 155, 58, 0.08); }

/* Masonry with columns (for varied-height items) */
.craft-masonry {
  columns: 3 280px;
  column-gap: 1.5rem;
  padding: 1rem;
}

.craft-masonry > * {
  break-inside: avoid;
  margin-bottom: 1.5rem;
  display: inline-block;
  width: 100%;
}
```

### Running Stitch Border

```css
/* Simulated hand-stitched border using dashed outline */
.craft-stitched {
  border: none;
  outline: 2px dashed var(--craft-terracotta);
  outline-offset: -6px;
  padding: 2rem;
  position: relative;
}

/* SVG-based running stitch divider */
.craft-stitch-divider {
  width: 100%;
  height: 12px;
  margin: 2rem 0;
  background-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='20' height='4' viewBox='0 0 20 4'%3E%3Cline x1='2' y1='2' x2='8' y2='2' stroke='%23c25b3f' stroke-width='2' stroke-linecap='round'/%3E%3C/svg%3E");
  background-repeat: repeat-x;
  background-position: center;
}

/* Cross-stitch corner decoration */
.craft-cross-stitch::before {
  content: '\00D7';
  position: absolute;
  top: 4px;
  left: 8px;
  font-size: 0.9rem;
  color: var(--craft-terracotta);
  font-weight: bold;
}

.craft-cross-stitch::after {
  content: '\00D7';
  position: absolute;
  bottom: 4px;
  right: 8px;
  font-size: 0.9rem;
  color: var(--craft-terracotta);
  font-weight: bold;
}
```

### Craft Card Styles

```css
/* Base craft card -- fabric patch feel */
.craft-card {
  background: var(--craft-bg-card);
  border: 2px dashed var(--craft-camel);
  border-radius: 6px;
  padding: 1.5rem;
  position: relative;
  transition: transform 0.3s ease, box-shadow 0.3s ease;
  box-shadow: 2px 3px 8px rgba(74, 54, 40, 0.1);
}

/* Slightly hand-placed rotations */
.craft-card:nth-child(odd) { transform: rotate(-0.8deg); }
.craft-card:nth-child(even) { transform: rotate(0.6deg); }
.craft-card:nth-child(3n) { transform: rotate(-0.3deg); }

.craft-card:hover {
  transform: rotate(0deg) translateY(-3px);
  box-shadow: 3px 6px 14px rgba(74, 54, 40, 0.18);
  z-index: 2;
}

/* Embroidered accent card */
.craft-card--embroidered {
  border: 3px solid var(--craft-moss);
  outline: 2px dashed var(--craft-sage);
  outline-offset: 4px;
  border-radius: 8px;
}

/* Yarn-wrapped card */
.craft-card--yarn {
  border: 4px solid var(--craft-sorbet);
  border-style: double;
  border-radius: 12px;
  background: linear-gradient(
    135deg,
    var(--craft-cotton) 0%,
    rgba(232, 136, 154, 0.05) 100%
  );
}
```

### Washi Tape / Fabric Tape Decoration

```css
/* Washi tape strip pinning elements */
.craft-tape {
  position: absolute;
  width: 110px;
  height: 26px;
  opacity: 0.75;
  transform: rotate(-4deg);
  top: -11px;
  left: calc(50% - 55px);
  z-index: 3;
  border-radius: 1px;
}

/* Solid fabric tape */
.craft-tape--clay { background: var(--craft-clay); }
.craft-tape--sage { background: var(--craft-sage); }
.craft-tape--marigold { background: var(--craft-marigold); }

/* Striped washi tape */
.craft-tape--striped {
  background: repeating-linear-gradient(
    90deg,
    var(--craft-sorbet),
    var(--craft-sorbet) 3px,
    rgba(255,255,255,0.5) 3px,
    rgba(255,255,255,0.5) 6px
  );
}

/* Dotted washi tape */
.craft-tape--dotted {
  background-color: var(--craft-ochre);
  background-image: radial-gradient(
    circle,
    rgba(255,255,255,0.5) 2px,
    transparent 2px
  );
  background-size: 8px 8px;
}
```

### Yarn / Thread Divider

```css
/* Wavy yarn divider between sections */
.craft-yarn-divider {
  width: 100%;
  height: 20px;
  margin: 2rem 0;
  background-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 200 20'%3E%3Cpath d='M0 10 Q25 2 50 10 T100 10 T150 10 T200 10' fill='none' stroke='%23cc9b3a' stroke-width='3' stroke-linecap='round'/%3E%3C/svg%3E");
  background-repeat: repeat-x;
  background-size: 200px 20px;
  background-position: center;
}

/* Knotted yarn accent */
.craft-yarn-knot {
  display: inline-block;
  width: 12px;
  height: 12px;
  background: var(--craft-terracotta);
  border-radius: 50%;
  box-shadow: 0 0 0 3px var(--craft-linen), 0 0 0 5px var(--craft-terracotta);
  margin: 0 0.5rem;
  vertical-align: middle;
}
```

### Crochet / Granny Square Pattern Background

```css
/* Granny-square-inspired tiled background */
.craft-granny-bg {
  background-color: var(--craft-oatmeal);
  background-image:
    linear-gradient(45deg, rgba(193, 122, 90, 0.08) 25%, transparent 25%),
    linear-gradient(-45deg, rgba(107, 127, 86, 0.08) 25%, transparent 25%),
    linear-gradient(45deg, transparent 75%, rgba(142, 64, 102, 0.06) 75%),
    linear-gradient(-45deg, transparent 75%, rgba(100, 136, 180, 0.06) 75%);
  background-size: 80px 80px;
  background-position: 0 0, 0 40px, 40px -40px, 40px 0;
}

/* Doily-inspired circular frame */
.craft-doily {
  border-radius: 50%;
  padding: 2rem;
  background: var(--craft-cotton);
  box-shadow:
    0 0 0 4px var(--craft-linen),
    0 0 0 6px var(--craft-camel),
    0 0 0 10px var(--craft-linen),
    0 0 0 12px rgba(196, 168, 122, 0.4);
}
```

### Collage / Layered Composition

```css
/* Collage container with overlapping elements */
.craft-collage {
  display: grid;
  grid-template-columns: repeat(12, 1fr);
  grid-auto-rows: 50px;
  gap: 0;
  padding: 2rem;
  position: relative;
}

.craft-collage-item {
  background: var(--craft-cotton);
  padding: 1rem;
  box-shadow: 2px 3px 8px rgba(74, 54, 40, 0.12);
  z-index: 1;
  transition: z-index 0s, transform 0.3s ease;
  overflow: hidden;
}

/* Torn-edge effect on top */
.craft-collage-item--torn::before {
  content: '';
  position: absolute;
  top: -4px;
  left: 0;
  right: 0;
  height: 8px;
  background: var(--craft-cotton);
  clip-path: polygon(
    0% 100%, 3% 40%, 7% 80%, 12% 30%, 18% 70%, 22% 20%,
    28% 60%, 33% 10%, 38% 50%, 44% 25%, 50% 75%, 55% 15%,
    60% 55%, 66% 30%, 72% 70%, 77% 20%, 82% 65%, 88% 35%,
    93% 80%, 97% 25%, 100% 100%
  );
}

/* Varied collage positions */
.craft-collage-item:nth-child(1) { grid-column: 1 / 5; grid-row: 1 / 4; transform: rotate(-2deg); }
.craft-collage-item:nth-child(2) { grid-column: 4 / 8; grid-row: 1 / 5; transform: rotate(1.5deg); }
.craft-collage-item:nth-child(3) { grid-column: 7 / 10; grid-row: 1 / 3; transform: rotate(-1deg); }
.craft-collage-item:nth-child(4) { grid-column: 9 / 13; grid-row: 2 / 6; transform: rotate(2deg); }
.craft-collage-item:nth-child(5) { grid-column: 1 / 4; grid-row: 3 / 7; transform: rotate(1deg); }
.craft-collage-item:nth-child(6) { grid-column: 3 / 8; grid-row: 5 / 8; transform: rotate(-0.5deg); }

.craft-collage-item:hover {
  transform: rotate(0deg) scale(1.04);
  z-index: 10;
  box-shadow: 4px 6px 18px rgba(74, 54, 40, 0.22);
}
```

### Embroidery Hoop Frame

```css
/* Circular embroidery hoop frame for images or sections */
.craft-hoop {
  width: 280px;
  height: 280px;
  border-radius: 50%;
  overflow: hidden;
  border: 8px solid var(--craft-camel);
  box-shadow:
    inset 0 0 0 3px var(--craft-linen),
    inset 0 0 0 5px var(--craft-driftwood),
    3px 4px 10px rgba(74, 54, 40, 0.2);
  position: relative;
}

.craft-hoop img {
  width: 100%;
  height: 100%;
  object-fit: cover;
}

/* Fabric texture background inside hoop */
.craft-hoop--fabric {
  background-color: var(--craft-cotton);
  background-image:
    repeating-linear-gradient(
      0deg,
      transparent,
      transparent 2px,
      rgba(74, 54, 40, 0.03) 2px,
      rgba(74, 54, 40, 0.03) 3px
    ),
    repeating-linear-gradient(
      90deg,
      transparent,
      transparent 2px,
      rgba(74, 54, 40, 0.03) 2px,
      rgba(74, 54, 40, 0.03) 3px
    );
}
```

### Craft Tag / Label Badges

```css
/* Sewn-on fabric tag */
.craft-label {
  display: inline-block;
  padding: 0.25rem 0.75rem;
  font-family: 'Quicksand', sans-serif;
  font-size: 0.72rem;
  font-weight: 700;
  text-transform: uppercase;
  letter-spacing: 0.06em;
  border-radius: 3px;
  position: relative;
  box-shadow: 1px 2px 4px rgba(74, 54, 40, 0.1);
}

/* Visible stitch marks on tag edges */
.craft-label::before {
  content: '';
  position: absolute;
  inset: 2px;
  border: 1px dashed rgba(255, 255, 255, 0.5);
  border-radius: 2px;
  pointer-events: none;
}

.craft-label--clay {
  background: var(--craft-clay);
  color: #fff;
}

.craft-label--moss {
  background: var(--craft-moss);
  color: #fff;
}

.craft-label--marigold {
  background: var(--craft-marigold);
  color: var(--craft-espresso);
}

.craft-label--sorbet {
  background: var(--craft-sorbet);
  color: #fff;
}

.craft-label--outlined {
  background: transparent;
  border: 2px dashed var(--craft-clay);
  color: var(--craft-clay);
}
```

### Button Styles

```css
/* Stitched fabric button */
.craft-btn {
  display: inline-block;
  padding: 0.7rem 1.6rem;
  font-family: 'Nunito', sans-serif;
  font-weight: 600;
  font-size: 0.95rem;
  border: none;
  border-radius: 6px;
  cursor: pointer;
  position: relative;
  transition: transform 0.2s ease, box-shadow 0.2s ease;
}

.craft-btn::after {
  content: '';
  position: absolute;
  inset: 4px;
  border: 2px dashed rgba(255, 255, 255, 0.4);
  border-radius: 4px;
  pointer-events: none;
}

.craft-btn--primary {
  background: var(--craft-clay);
  color: #fff;
  box-shadow: 2px 3px 6px rgba(193, 122, 90, 0.3);
}

.craft-btn--primary:hover {
  transform: translateY(-2px);
  box-shadow: 2px 5px 12px rgba(193, 122, 90, 0.4);
}

.craft-btn--secondary {
  background: var(--craft-moss);
  color: #fff;
  box-shadow: 2px 3px 6px rgba(107, 127, 86, 0.3);
}

.craft-btn--outline {
  background: transparent;
  color: var(--craft-clay);
  border: 2px solid var(--craft-clay);
}

.craft-btn--outline::after {
  border-color: rgba(193, 122, 90, 0.3);
}
```

---

## Materials and Textures (Visual Metaphors for Web)

Physical Craftcore materials and their web equivalents:

| Physical Material | Web Equivalent |
|-------------------|----------------|
| Linen / unbleached cotton | Warm off-white backgrounds with fine crosshatch repeating gradients |
| Yarn and wool | Thick, rounded borders; wavy SVG dividers; warm saturated accent colors |
| Crochet lace / doilies | Circular frames with layered box-shadows; dotted/dashed ornamental borders |
| Patchwork quilts | Grid layouts with alternating tinted backgrounds and dashed "seam" borders |
| Embroidery thread | Dashed outlines, running-stitch SVG borders, cross-stitch character decorations |
| Macrame rope | Knotted node decorations; hanging / dangling positioned elements |
| Washi / fabric tape | Semi-transparent colored strips with pattern fills, positioned over edges |
| Pottery / ceramics | Rounded containers with earthy solid colors and subtle gradient shading |
| Torn paper / fabric | Irregular clip-path edges on overlapping collage elements |
| Wooden embroidery hoop | Circular overflow containers with thick warm-brown borders and inset shadows |
| Buttons and beads | Small circular elements with radial gradients and subtle box-shadows |
| Stamp / block print | Letterpress-style typography with slight texture overlays |

---

## Key Differences from Related Aesthetics

| Aspect | Craftcore | Cottagecore | Cluttercore |
|--------|-----------|-------------|-------------|
| **Focus** | The craft technique itself; visible handwork | Rural lifestyle and pastoral nostalgia | Accumulation and personal collections |
| **Color approach** | Yarn-bright + earthy naturals | Soft pastels and muted florals | Any color, maximum variety |
| **Material feel** | Textured, tactile, woven, stitched | Soft, floral, vintage linen | Eclectic mix of everything |
| **Organization** | Artfully composed; technique is featured | Curated, idyllic arrangement | Organic, dense accumulation |
| **Emotional goal** | Pride in handmade skill; slow living | Escape to simpler times | Comfort through personal objects |
| **Overall feel** | Artist's studio / craft fair | Country cottage garden | Lived-in maximalist home |

---

## Related Aesthetics

| Aesthetic | Relationship to Craftcore |
|-----------|--------------------------|
| **Boho-Chic** | Shares eclectic mixing, textile focus, and handmade appreciation; Boho leans more toward fashion and global influences |
| **Cottagecore** | Overlaps in warmth, handmade values, and natural materials; Cottagecore emphasizes rural setting rather than craft process |
| **Grandmacore** | Shares nostalgia for traditional domestic crafts (knitting, crochet, quilting); Grandmacore celebrates the maker archetype |
| **Pearlcore** | Adjacent through beading and embellishment techniques; Pearlcore is more delicate and decorative |
| **Whimsicraft** | Shares celebration of handmade and creative process; Whimsicraft leans more fantastical and playful |
| **Arts and Crafts (movement)** | Historical ancestor; the original celebration of handcraft over industrialization |

---

## Quick-Start: Minimal Craftcore Page Template

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Craftcore Page</title>
  <link href="https://fonts.googleapis.com/css2?family=Amatic+SC:wght@400;700&family=Vollkorn:wght@400;600;700&family=Nunito:wght@400;600&family=Caveat:wght@400;700&family=Quicksand:wght@500;700&display=swap" rel="stylesheet">
  <style>
    :root {
      --craft-linen: #f4ede4;
      --craft-oatmeal: #e8dfd0;
      --craft-cotton: #faf6f0;
      --craft-clay: #c17a5a;
      --craft-terracotta: #c25b3f;
      --craft-ochre: #cc9b3a;
      --craft-marigold: #e8a832;
      --craft-moss: #6b7f56;
      --craft-sage: #9cae8a;
      --craft-sorbet: #e8889a;
      --craft-berry: #8e4066;
      --craft-cornflower: #6488b4;
      --craft-camel: #c4a87a;
      --craft-driftwood: #8c7b6b;
      --craft-espresso: #4a3628;
      --craft-charcoal: #3e3a36;
    }

    * { margin: 0; padding: 0; box-sizing: border-box; }

    body {
      background-color: var(--craft-linen);
      background-image:
        repeating-linear-gradient(
          0deg, transparent, transparent 3px,
          rgba(74, 54, 40, 0.015) 3px, rgba(74, 54, 40, 0.015) 4px
        ),
        repeating-linear-gradient(
          90deg, transparent, transparent 3px,
          rgba(74, 54, 40, 0.015) 3px, rgba(74, 54, 40, 0.015) 4px
        );
      color: var(--craft-charcoal);
      font-family: 'Nunito', sans-serif;
      font-weight: 400;
      line-height: 1.75;
    }

    h1, h2, h3 {
      font-family: 'Vollkorn', Georgia, serif;
      font-weight: 700;
      color: var(--craft-espresso);
      line-height: 1.2;
    }

    .hero {
      text-align: center;
      padding: 5rem 2rem 3rem;
      background: var(--craft-oatmeal);
      position: relative;
      overflow: hidden;
    }

    .hero h1 {
      font-family: 'Amatic SC', cursive;
      font-size: clamp(3rem, 6vw, 5.5rem);
      letter-spacing: 0.03em;
      margin-bottom: 0.5rem;
    }

    .hero .subtitle {
      font-family: 'Caveat', cursive;
      font-size: 1.5rem;
      color: var(--craft-clay);
      transform: rotate(-1.5deg);
      display: inline-block;
    }

    /* Yarn divider */
    .yarn-divider {
      width: 100%;
      height: 20px;
      margin: 0;
      background-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 200 20'%3E%3Cpath d='M0 10 Q25 2 50 10 T100 10 T150 10 T200 10' fill='none' stroke='%23cc9b3a' stroke-width='3' stroke-linecap='round'/%3E%3C/svg%3E");
      background-repeat: repeat-x;
      background-size: 200px 20px;
      background-position: center;
      background-color: var(--craft-linen);
    }

    .craft-grid {
      display: grid;
      grid-template-columns: repeat(auto-fill, minmax(260px, 1fr));
      gap: 0;
      max-width: 1100px;
      margin: 0 auto;
      padding: 3rem 2rem;
    }

    .craft-patch {
      padding: 2rem;
      border: 2px dashed var(--craft-camel);
      position: relative;
    }

    .craft-patch:nth-child(4n+1) { background: var(--craft-cotton); }
    .craft-patch:nth-child(4n+2) { background: rgba(156, 174, 138, 0.1); }
    .craft-patch:nth-child(4n+3) { background: rgba(232, 136, 154, 0.06); }
    .craft-patch:nth-child(4n+4) { background: rgba(204, 155, 58, 0.06); }

    .craft-patch h3 {
      font-size: 1.3rem;
      margin-bottom: 0.5rem;
      color: var(--craft-clay);
    }

    .label {
      display: inline-block;
      padding: 0.2rem 0.6rem;
      font-family: 'Quicksand', sans-serif;
      font-size: 0.7rem;
      font-weight: 700;
      text-transform: uppercase;
      border-radius: 3px;
      margin-bottom: 0.8rem;
      position: relative;
    }

    .label::before {
      content: '';
      position: absolute;
      inset: 2px;
      border: 1px dashed rgba(255, 255, 255, 0.4);
      border-radius: 2px;
    }

    .label--clay { background: var(--craft-clay); color: #fff; }
    .label--moss { background: var(--craft-moss); color: #fff; }
    .label--marigold { background: var(--craft-marigold); color: var(--craft-espresso); }
    .label--sorbet { background: var(--craft-sorbet); color: #fff; }
  </style>
</head>
<body>
  <div class="hero">
    <h1>Made by Hand</h1>
    <span class="subtitle">every stitch tells a story</span>
  </div>
  <div class="yarn-divider"></div>
  <section class="craft-grid">
    <div class="craft-patch">
      <span class="label label--clay">Knitting</span>
      <h3>Chunky Wool Blanket</h3>
      <p>Oversized cable-knit throw in natural cream wool, three months of evening work in every row.</p>
    </div>
    <div class="craft-patch">
      <span class="label label--moss">Embroidery</span>
      <h3>Botanical Hoop Art</h3>
      <p>Wildflower meadow stitched on linen in satin stitch and French knots, framed in a birch hoop.</p>
    </div>
    <div class="craft-patch">
      <span class="label label--marigold">Quilting</span>
      <h3>Patchwork Table Runner</h3>
      <p>Pieced from vintage cotton scraps collected over a decade, hand-quilted with a running stitch.</p>
    </div>
    <div class="craft-patch">
      <span class="label label--sorbet">Crochet</span>
      <h3>Granny Square Cardigan</h3>
      <p>Seventy-two granny squares in sorbet and sage, joined with a whip stitch and edged in shell trim.</p>
    </div>
  </section>
</body>
</html>
```
