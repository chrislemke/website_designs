# Graffiti Pop Design Reference

Graffiti Pop (c. 1970s--present) is a street-art-rooted aesthetic that fuses the raw, rebellious energy of graffiti and hip-hop culture with bold, accessible pop sensibilities. It takes the visual language of urban walls -- spray paint, tags, bubble letters, drip effects, and stencils -- and repackages it into high-contrast, vibrant compositions suitable for galleries, brands, and screens. The style channels the **downtown metropolitan energy** of 1970s--80s New York, merging punk collage rawness with technical graffiti skill. Think MTV bumpers, Fresh Prince opening credits, and Supreme lookbooks: **aggressive neon color on concrete gray**, cartoonish characters in baggy clothes and big trainers, and typography that looks sprayed onto brick walls. The result is maximalist, kinetic, unapologetically loud, and dripping with street credibility.

---

## Visual Characteristics

### Core Motifs and Patterns

- **Graffiti tags and throw-ups** -- stylized signatures, quick spray-painted names, and elaborate wildstyle lettering covering surfaces
- **Bubble letters** -- rounded, inflated, dimensional letterforms with outlines, highlights, and drop shadows
- **Drip and splatter effects** -- paint drips running down from text and shapes, spray-can overspray dots, ink splatters
- **Brick wall and concrete textures** -- urban surfaces as the natural canvas; visible mortar lines, cracks, and weathering
- **Cartoonish characters** -- exaggerated figures with big trainers, baggy clothes, boomboxes, and expressive poses
- **Stencil art** -- sharp-edged spray-paint imagery using cut-out templates, often political or iconic
- **Chain-link fences and street furniture** -- urban environmental elements: street lamps, fire hydrants, manhole covers, trash cans
- **Xerox and photocopy aesthetics** -- high-contrast, grainy reproductions suggesting zine culture and underground flyers
- **Collaged layering** -- overlapping elements stacked like wheat-pasted posters on a wall; torn edges, partial obscuring
- **Spray-can texture and gradients** -- soft-edge fades, cap-width line variations, and valve-splatter patterns unique to aerosol art
- **Run-down cars and urban decay** -- rusted vehicles, crumbling buildings, cracked sidewalks as background staging

### Design Principles

- **Maximum energy, maximum contrast** -- pair the brightest neons against the darkest urban surfaces for visual impact
- **Layered chaos with compositional intent** -- elements should appear spontaneously placed but follow an underlying visual hierarchy
- **Street-level authenticity** -- every element should feel like it could exist on an actual city wall or in a subway car
- **Motion and kinetic energy** -- compositions should feel dynamic, as if captured mid-action; tilted angles, speed lines, overlapping forms
- **Bold over subtle** -- nothing is quiet; type is oversized, colors are saturated, characters are exaggerated
- **Raw over polished** -- embrace imperfection, overspray, drips, and rough edges rather than clean vector precision
- **Cultural specificity** -- root the design in hip-hop, skateboarding, punk, and street culture visual vocabulary
- **Dimensional letterforms** -- text should have weight, shadow, and volume; flat type feels out of place
- **Foreground dominance** -- the graffiti/art elements take visual priority over any background or structural grid

---

## Color Palette

### Primary Scheme

| Role | Colors |
|------|--------|
| **Background / Canvas** | Concrete gray, dark asphalt, brick red-brown, near-black |
| **Primary neon accents** | Hot pink, neon green, electric blue, vivid purple |
| **High-energy primaries** | Fire engine red, pure white, safety yellow |
| **Urban midtones** | Rusted orange, faded teal, dusty khaki |
| **Outline / Structure** | Pure black, dark charcoal |

### Detailed Palette

| Color | Hex | Usage |
|-------|-----|-------|
| Asphalt Black | `#111111` | Deep backgrounds, text outlines, shadows |
| Concrete Gray | `#5A5A5A` | Primary surface color, wall texture base |
| Warm Concrete | `#7A7168` | Weathered wall tones, secondary surfaces |
| Brick Red | `#8B4513` | Background texture accent, urban warmth |
| Brick Mortar | `#A09080` | Mortar lines in brick patterns, subtle detail |
| Hot Pink | `#FF1493` | Primary neon accent, high-impact highlights |
| Neon Green | `#39FF14` | Secondary neon accent, glow effects |
| Electric Blue | `#0080FF` | Tertiary accent, cool-tone highlights |
| Vivid Purple | `#9B30FF` | Accent for variety, bubble letter fills |
| Safety Yellow | `#FFD700` | Warning accents, tag highlights, star bursts |
| Fire Red | `#FF2400` | Aggressive accent, exclamation marks, arrows |
| Pure White | `#FFFFFF` | Highlights, bubble letter shine spots, outlines |
| Spray Can Silver | `#C0C0C0` | Metallic accents, chrome letter effects |
| Rust Orange | `#CC5500` | Warm accent, aged spray paint, urban decay |
| Faded Teal | `#3D8B8B` | Cool midtone, vintage spray paint feel |
| Dusty Khaki | `#BDB76B` | Muted accent, worn surface highlights |
| Subway Cream | `#F5F0E0` | Light surface alternative, poster backgrounds |

### Suggested CSS Custom Properties

```css
:root {
  /* Background tones */
  --gpop-black: #111111;
  --gpop-concrete: #5a5a5a;
  --gpop-concrete-warm: #7a7168;
  --gpop-brick: #8b4513;
  --gpop-mortar: #a09080;

  /* Neon accents */
  --gpop-pink: #ff1493;
  --gpop-neon-green: #39ff14;
  --gpop-blue: #0080ff;
  --gpop-purple: #9b30ff;
  --gpop-yellow: #ffd700;
  --gpop-red: #ff2400;

  /* Neutral utility */
  --gpop-white: #ffffff;
  --gpop-silver: #c0c0c0;
  --gpop-cream: #f5f0e0;

  /* Warm accents */
  --gpop-rust: #cc5500;
  --gpop-teal: #3d8b8b;
  --gpop-khaki: #bdb76b;

  /* Functional mappings */
  --gpop-bg-primary: var(--gpop-black);
  --gpop-bg-surface: var(--gpop-concrete);
  --gpop-bg-wall: var(--gpop-concrete-warm);
  --gpop-text-primary: var(--gpop-white);
  --gpop-text-secondary: var(--gpop-cream);
  --gpop-text-muted: var(--gpop-silver);
  --gpop-accent-1: var(--gpop-pink);
  --gpop-accent-2: var(--gpop-neon-green);
  --gpop-accent-3: var(--gpop-blue);
  --gpop-accent-4: var(--gpop-purple);
  --gpop-border: var(--gpop-black);
  --gpop-glow: rgba(255, 20, 147, 0.4);
}
```

### Palette Approaches

- **Neon-on-dark dominance** -- saturated, electric colors on dark urban surfaces create the signature Graffiti Pop contrast
- **Multi-accent freedom** -- unlike muted aesthetics, Graffiti Pop encourages using 3--5 vivid accent colors simultaneously
- **Black outlines unify** -- thick black outlines and shadows hold the chaotic palette together, mimicking graffiti technique
- **Warm and cool neon balance** -- mix warm neons (pink, yellow, red) with cool neons (green, blue, purple) for full-spectrum energy
- **Concrete as canvas** -- the neutral gray/brown background tones are as important as the accents; they ground the neon chaos
- **No pastels, no muting** -- colors should be at or near full saturation; faded tones appear only on background surfaces representing age

---

## Typography

### Typeface Characteristics

Graffiti Pop typography is loud, dimensional, and hand-made:

- **Bubble letters** -- rounded, inflated letterforms with thick outlines, inner highlights, and cast shadows
- **Wildstyle graffiti** -- interlocking, angular letters with arrows, connections, and decorative extensions
- **Tag-style script** -- flowing, calligraphic marks mimicking spray-can signatures; aggressive slant and speed
- **Stencil capitals** -- bold, military-style cut-out letters suggesting political street art (Banksy lineage)
- **Block letters** -- heavy, geometric, three-dimensional letterforms with visible depth/perspective
- **Dripping text** -- letterforms with paint drips extending downward from baselines and serifs
- **Mixed case and scale** -- deliberate variation in letter size and baseline within words for hand-painted energy
- **Thick outlines** -- all display text benefits from visible dark outlines that separate letters from busy backgrounds

### Named Typefaces from the Era

These are typefaces historically associated with Graffiti Pop (commercial/specialty fonts):

- **Graffonti** -- classic graffiti tag typeface with drip variants
- **Krylon** -- spray-paint-textured display face
- **Bombing** -- bubble-letter graffiti typeface
- **Fresh Prince** -- the sitcom's logo font, a quintessential Graffiti Pop mark
- **Stussy Script** -- the iconic brand's hand-tag logotype, foundational to the style

### Recommended Web Fonts (Google Fonts)

| Font | Style | Usage |
|------|-------|-------|
| **Bungee** | Bold block display | Headlines, hero text, section titles |
| **Bungee Shade** | Layered dimensional display | Oversized display type, posters |
| **Bungee Inline** | Inline-stroked display | Alternate headlines, decorative emphasis |
| **Permanent Marker** | Bold hand-written marker | Subheadings, callouts, tag-style text |
| **Rock Salt** | Rough handwritten | Accent text, annotations, informal labels |
| **Bangers** | Comic/pop bold | Action text, exclamations, button labels |
| **Bowlby One SC** | Rounded bold display | Bubble-letter approximation, titles |
| **Russo One** | Geometric bold sans | Clean urban display, modern graffiti headers |
| **Lilita One** | Heavy rounded display | Friendly bold headlines, cartoonish headers |
| **Luckiest Guy** | Cartoon block letters | Fun display, comic-influenced headings |
| **Press Start 2P** | Pixel/retro display | Retro gaming accent (for 80s crossover) |
| **Share Tech Mono** | Technical monospace | Small labels, metadata, technical details |

### Typography CSS Example

```css
/* Import graffiti-pop-appropriate Google Fonts */
@import url('https://fonts.googleapis.com/css2?family=Bungee&family=Bungee+Shade&family=Permanent+Marker&family=Bangers&family=Rock+Salt&family=Bowlby+One+SC&family=Russo+One&family=Lilita+One&family=Share+Tech+Mono&display=swap');

/* Hero / Display text -- dimensional block letters */
h1 {
  font-family: 'Bungee Shade', 'Bungee', Impact, sans-serif;
  font-size: clamp(3rem, 8vw, 7rem);
  letter-spacing: 0.04em;
  line-height: 1.0;
  color: var(--gpop-white);
  text-shadow:
    3px 3px 0 var(--gpop-pink),
    6px 6px 0 rgba(0, 0, 0, 0.5);
  -webkit-text-stroke: 2px var(--gpop-black);
}

/* Section headings -- bold marker style */
h2 {
  font-family: 'Bangers', 'Permanent Marker', cursive;
  font-size: clamp(2rem, 5vw, 3.5rem);
  letter-spacing: 0.06em;
  text-transform: uppercase;
  color: var(--gpop-neon-green);
  text-shadow:
    2px 2px 0 var(--gpop-black),
    -1px -1px 0 var(--gpop-black),
    1px -1px 0 var(--gpop-black),
    -1px 1px 0 var(--gpop-black);
}

/* Sub-headings -- hand-tag style */
h3 {
  font-family: 'Permanent Marker', cursive;
  font-size: 1.6rem;
  color: var(--gpop-yellow);
  text-shadow: 2px 2px 0 rgba(0, 0, 0, 0.6);
  transform: rotate(-1deg);
}

/* Body text -- readable but with character */
body {
  font-family: 'Russo One', 'Segoe UI', Tahoma, sans-serif;
  font-weight: 400;
  font-size: 1rem;
  line-height: 1.6;
  color: var(--gpop-text-secondary);
}

/* Tag / annotation text */
.gpop-tag {
  font-family: 'Rock Salt', cursive;
  font-size: 0.85rem;
  color: var(--gpop-pink);
  transform: rotate(-3deg);
  display: inline-block;
}

/* Metadata, labels */
.gpop-label {
  font-family: 'Share Tech Mono', monospace;
  font-size: 0.75rem;
  text-transform: uppercase;
  letter-spacing: 0.15em;
  color: var(--gpop-silver);
}

/* Oversized impact stat */
.gpop-stat {
  font-family: 'Bungee', Impact, sans-serif;
  font-size: clamp(4rem, 10vw, 10rem);
  color: var(--gpop-yellow);
  -webkit-text-stroke: 3px var(--gpop-black);
  text-shadow: 5px 5px 0 rgba(0, 0, 0, 0.5);
}
```

---

## Layout Principles

### Grid and Structure

- **Edge-to-edge canvas** -- backgrounds extend full-bleed; the entire viewport is a wall to be painted on
- **Overlapping, collaged composition** -- elements stack on top of each other like layers of wheat-pasted posters and spray paint
- **Asymmetric, organic placement** -- resist rigid grid alignment; elements should feel placed by hand rather than snapped to columns
- **Generous scale contrast** -- oversized headlines next to small labels; huge characters next to tight body text
- **Angled and rotated elements** -- slight tilts (2--5deg) on cards, text blocks, and images suggest street-level spontaneity
- **Foreground-background depth** -- use z-index layering, shadows, and scale to create a sense of physical depth (paint on wall on building)
- **Generous negative space as "wall"** -- leave areas of bare background visible, like unpainted sections of a wall between pieces

### Section Organization

- Use **spray-paint splatter dividers** between sections -- colorful dots, drips, and line streaks rather than clean horizontal rules
- Apply **alternating surface textures** per section -- brick wall, concrete, metal shutter, subway tile to vary the "canvas"
- Create **hierarchy through size and color intensity** -- the most important content gets the biggest, brightest, most dimensional treatment
- Employ **sticker and wheat-paste elements** -- cards and panels that look pasted onto the wall with visible edges and slight peeling
- Use **arrow and pointer elements** -- hand-drawn arrows, spray-painted directional marks guiding the eye through the composition
- Apply **frame-breaking overflow** -- let elements (characters, drips, tags) extend beyond their containers and into adjacent sections
- **Banner and ribbon treatments** -- text on angled banner shapes, mimicking protest signs and hip-hop event flyers

---

## CSS/Design Techniques

### Brick Wall Background Texture

```css
/* Brick wall pattern using CSS gradients */
.gpop-brick-wall {
  background-color: #5a5a5a;
  background-image:
    /* Horizontal mortar lines */
    repeating-linear-gradient(
      0deg,
      transparent,
      transparent 48px,
      #a09080 48px,
      #a09080 52px
    ),
    /* Vertical mortar lines (offset every other row) */
    repeating-linear-gradient(
      90deg,
      transparent,
      transparent 98px,
      #a09080 98px,
      #a09080 102px
    );
  background-size: 200px 100px;
  position: relative;
}

/* Subtle grime overlay */
.gpop-brick-wall::before {
  content: '';
  position: absolute;
  inset: 0;
  background:
    radial-gradient(circle at 15% 25%, rgba(0, 0, 0, 0.15) 0%, transparent 40%),
    radial-gradient(circle at 85% 60%, rgba(0, 0, 0, 0.1) 0%, transparent 35%),
    radial-gradient(circle at 50% 90%, rgba(0, 0, 0, 0.12) 0%, transparent 45%);
  pointer-events: none;
}
```

### Spray Paint Text Effect

```css
/* Spray-painted text with overspray glow */
.gpop-spray-text {
  font-family: 'Bangers', cursive;
  font-size: clamp(3rem, 7vw, 6rem);
  text-transform: uppercase;
  color: var(--gpop-pink);
  text-shadow:
    /* Core glow (overspray) */
    0 0 10px rgba(255, 20, 147, 0.6),
    0 0 30px rgba(255, 20, 147, 0.3),
    0 0 60px rgba(255, 20, 147, 0.15),
    /* Hard shadow for dimension */
    3px 3px 0 var(--gpop-black);
  position: relative;
}

/* Drip effect under text using pseudo-element */
.gpop-spray-text::after {
  content: '';
  position: absolute;
  bottom: -20px;
  left: 15%;
  width: 4px;
  height: 25px;
  background: linear-gradient(to bottom, var(--gpop-pink), transparent);
  border-radius: 0 0 2px 2px;
  box-shadow:
    40px 5px 0 0 var(--gpop-pink),
    120px -3px 0 0 var(--gpop-pink),
    200px 8px 0 0 var(--gpop-pink);
}
```

### Bubble Letter Effect

```css
/* Bubble letter style heading */
.gpop-bubble {
  font-family: 'Lilita One', 'Bowlby One SC', sans-serif;
  font-size: clamp(3rem, 8vw, 7rem);
  color: var(--gpop-blue);
  -webkit-text-stroke: 3px var(--gpop-black);
  text-shadow:
    /* Inner highlight (top-left shine) */
    -2px -2px 0 rgba(255, 255, 255, 0.3),
    /* Outer black outline reinforcement */
    4px 4px 0 var(--gpop-black),
    5px 5px 0 var(--gpop-black),
    /* Drop shadow for depth */
    7px 7px 0 rgba(0, 0, 0, 0.4);
  letter-spacing: 0.03em;
  paint-order: stroke fill;
}

/* Multicolor bubble letters using gradient */
.gpop-bubble-gradient {
  font-family: 'Lilita One', sans-serif;
  font-size: clamp(3rem, 8vw, 7rem);
  background: linear-gradient(135deg, var(--gpop-pink), var(--gpop-purple), var(--gpop-blue));
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  -webkit-text-stroke: 2px var(--gpop-black);
  filter: drop-shadow(4px 4px 0 rgba(0, 0, 0, 0.5));
}
```

### Paint Drip Effect

```css
/* Paint drip decoration element */
.gpop-drips {
  position: relative;
}

.gpop-drips::after {
  content: '';
  position: absolute;
  bottom: -30px;
  left: 0;
  right: 0;
  height: 30px;
  background:
    /* Individual drips at various positions */
    linear-gradient(to bottom, var(--gpop-pink) 0%, transparent 100%) 10% 0 / 3px 28px no-repeat,
    linear-gradient(to bottom, var(--gpop-pink) 0%, transparent 100%) 25% 0 / 4px 20px no-repeat,
    linear-gradient(to bottom, var(--gpop-pink) 0%, transparent 100%) 40% 0 / 3px 30px no-repeat,
    linear-gradient(to bottom, var(--gpop-pink) 0%, transparent 100%) 55% 0 / 5px 15px no-repeat,
    linear-gradient(to bottom, var(--gpop-pink) 0%, transparent 100%) 70% 0 / 3px 25px no-repeat,
    linear-gradient(to bottom, var(--gpop-pink) 0%, transparent 100%) 85% 0 / 4px 22px no-repeat;
  pointer-events: none;
}
```

### Spray Splatter Divider

```css
/* Spray-paint splatter section divider */
.gpop-splatter-divider {
  border: none;
  height: 20px;
  position: relative;
  margin: 3rem 0;
  overflow: visible;
}

.gpop-splatter-divider::before {
  content: '';
  position: absolute;
  top: 0;
  left: 5%;
  width: 10px;
  height: 10px;
  border-radius: 50%;
  background: var(--gpop-pink);
  box-shadow:
    30px -3px 0 3px var(--gpop-neon-green),
    70px 5px 0 1px var(--gpop-blue),
    110px -2px 0 4px var(--gpop-yellow),
    160px 3px 0 2px var(--gpop-purple),
    200px -4px 0 1px var(--gpop-pink),
    250px 2px 0 3px var(--gpop-red),
    310px -1px 0 2px var(--gpop-neon-green),
    360px 4px 0 1px var(--gpop-blue),
    420px -3px 0 4px var(--gpop-yellow),
    480px 1px 0 2px var(--gpop-purple);
}

/* Spray line streak */
.gpop-splatter-divider::after {
  content: '';
  position: absolute;
  top: 8px;
  left: 10%;
  right: 10%;
  height: 3px;
  background: linear-gradient(
    90deg,
    transparent 0%,
    var(--gpop-pink) 5%,
    var(--gpop-pink) 15%,
    transparent 20%,
    transparent 30%,
    var(--gpop-neon-green) 35%,
    var(--gpop-neon-green) 50%,
    transparent 55%,
    transparent 65%,
    var(--gpop-blue) 70%,
    var(--gpop-blue) 80%,
    transparent 85%,
    transparent 90%,
    var(--gpop-yellow) 95%,
    transparent 100%
  );
  opacity: 0.7;
}
```

### Wheat-Pasted Poster Card

```css
/* Card that looks pasted onto a wall */
.gpop-poster-card {
  background: var(--gpop-cream);
  color: var(--gpop-black);
  padding: 2rem;
  position: relative;
  transform: rotate(-1.5deg);
  box-shadow:
    2px 2px 8px rgba(0, 0, 0, 0.4),
    0 0 0 1px rgba(0, 0, 0, 0.1);
  overflow: hidden;
}

/* Torn/peeling corner effect */
.gpop-poster-card::before {
  content: '';
  position: absolute;
  top: 0;
  right: 0;
  width: 40px;
  height: 40px;
  background: linear-gradient(
    225deg,
    var(--gpop-concrete) 50%,
    rgba(245, 240, 224, 0.8) 50%
  );
  box-shadow: -2px 2px 3px rgba(0, 0, 0, 0.15);
}

/* Aged/yellowed paper overlay */
.gpop-poster-card::after {
  content: '';
  position: absolute;
  inset: 0;
  background:
    radial-gradient(circle at 20% 80%, rgba(139, 69, 19, 0.06) 0%, transparent 50%),
    radial-gradient(circle at 80% 20%, rgba(139, 69, 19, 0.04) 0%, transparent 40%);
  pointer-events: none;
}
```

### Sticker / Slap-Tag Element

```css
/* Sticker-style element */
.gpop-sticker {
  display: inline-block;
  padding: 0.5rem 1.2rem;
  font-family: 'Bangers', cursive;
  font-size: 1.1rem;
  letter-spacing: 0.05em;
  text-transform: uppercase;
  color: var(--gpop-black);
  background: var(--gpop-yellow);
  border: 2px solid var(--gpop-black);
  border-radius: 2px;
  transform: rotate(2deg);
  box-shadow:
    2px 2px 0 var(--gpop-black),
    3px 3px 6px rgba(0, 0, 0, 0.3);
  position: relative;
}

/* Peeling edge */
.gpop-sticker::after {
  content: '';
  position: absolute;
  bottom: -3px;
  right: -3px;
  width: 15px;
  height: 15px;
  background: linear-gradient(
    315deg,
    var(--gpop-concrete) 50%,
    var(--gpop-yellow) 50%
  );
  border-bottom-right-radius: 2px;
}
```

### Graffiti Pop Button

```css
.gpop-button {
  display: inline-block;
  padding: 0.8rem 2.5rem;
  font-family: 'Bangers', cursive;
  font-size: 1.2rem;
  letter-spacing: 0.08em;
  text-transform: uppercase;
  color: var(--gpop-black);
  background: var(--gpop-neon-green);
  border: 3px solid var(--gpop-black);
  cursor: pointer;
  position: relative;
  transform: rotate(-1deg);
  box-shadow: 4px 4px 0 var(--gpop-black);
  transition: all 0.1s ease;
  text-shadow: none;
}

.gpop-button:hover {
  background: var(--gpop-pink);
  color: var(--gpop-white);
  transform: rotate(0deg) translate(-2px, -2px);
  box-shadow: 6px 6px 0 var(--gpop-black);
}

.gpop-button:active {
  transform: rotate(0deg) translate(2px, 2px);
  box-shadow: 2px 2px 0 var(--gpop-black);
}

/* Alt color variant */
.gpop-button--alt {
  background: var(--gpop-purple);
  color: var(--gpop-white);
}

.gpop-button--alt:hover {
  background: var(--gpop-yellow);
  color: var(--gpop-black);
}
```

### Neon Glow Accent Line

```css
/* Neon glow line for emphasis */
.gpop-neon-line {
  height: 4px;
  background: var(--gpop-pink);
  border: none;
  box-shadow:
    0 0 5px var(--gpop-pink),
    0 0 15px rgba(255, 20, 147, 0.5),
    0 0 30px rgba(255, 20, 147, 0.2);
  margin: 2rem 0;
}

/* Animated neon flicker */
@keyframes gpop-flicker {
  0%, 100% { opacity: 1; }
  4% { opacity: 0.9; }
  6% { opacity: 1; }
  42% { opacity: 1; }
  44% { opacity: 0.85; }
  46% { opacity: 1; }
  80% { opacity: 1; }
  82% { opacity: 0.9; }
  83% { opacity: 1; }
}

.gpop-neon-flicker {
  animation: gpop-flicker 3s ease-in-out infinite;
}
```

### Tag Scrawl Animation

```css
/* Animated spray-paint "writing" effect using stroke-dasharray */
@keyframes gpop-spray-write {
  from {
    stroke-dashoffset: 1000;
    opacity: 0.3;
  }
  to {
    stroke-dashoffset: 0;
    opacity: 1;
  }
}

.gpop-tag-animated svg path {
  stroke-dasharray: 1000;
  stroke-dashoffset: 1000;
  animation: gpop-spray-write 2s ease-out forwards;
}

/* Overspray dots appearing */
@keyframes gpop-spatter {
  0% { transform: scale(0); opacity: 0; }
  60% { transform: scale(1.3); opacity: 0.8; }
  100% { transform: scale(1); opacity: 0.5; }
}

.gpop-spatter-dot {
  width: 4px;
  height: 4px;
  border-radius: 50%;
  background: var(--gpop-pink);
  animation: gpop-spatter 0.4s ease-out forwards;
}
```

---

## Materials and Textures (Visual Metaphors for Web)

Physical Graffiti Pop materials and their web equivalents:

| Physical Material | Web Equivalent |
|-------------------|----------------|
| Brick wall | CSS `repeating-linear-gradient` grid pattern in warm gray/brown with mortar lines |
| Concrete surface | Neutral gray background with subtle `radial-gradient` blotches and SVG noise overlay |
| Spray paint on wall | Saturated text with `text-shadow` glow and `filter: blur()` overspray halo |
| Paint drips | `linear-gradient` strips from accent color to transparent, positioned below elements |
| Wheat-pasted poster | Light cream cards with `transform: rotate()`, torn corner pseudo-elements, and aged overlay |
| Sticker / slap-tag | Bright-background inline-block with thick black border, slight rotation, and peeling corner effect |
| Chain-link fence | SVG or CSS diamond grid overlay pattern at low opacity |
| Xerox/photocopy | `filter: contrast(1.8) grayscale(1)` on images with halftone dot overlay |
| Chrome/metallic paint | `linear-gradient` with multiple silver/white stops creating reflection bands |
| Marker on paper | `Rock Salt` or `Permanent Marker` font with slight `text-shadow` bleed |

---

## Cultural References and Influences

The following define the Graffiti Pop visual language and serve as design references:

- **Yo! MTV Raps** (1988--1995) -- the show's logo, set design, and bumper graphics are quintessential Graffiti Pop; spray-painted lettering, bright colors, urban backdrops
- **Fresh Prince of Bel-Air opening sequence** -- the neon-colored graffiti title cards over Philadelphia street scenes define the aesthetic's television presence
- **MTV graffiti-heavy sets** (1980s--90s) -- the original MTV studios used graffiti artists for on-set murals; the visual DNA of the channel was Graffiti Pop
- **Supreme brand identity** -- the gallery-meets-streetwear boutique aesthetic, red-on-white Futura Bold logo functioning like a tag
- **JNCO jeans artwork** -- embroidered spray-paint characters, oversized proportions, cartoon graffiti figures on denim
- **Stussy logo and brand graphics** -- the hand-drawn tag-style signature logo; one of the first brands to bridge street graffiti and commercial fashion
- **Keith Haring** -- bold outlines, cartoonish figures, kinetic energy, pop colors on urban surfaces
- **Jean-Michel Basquiat** -- raw, tag-influenced text and imagery elevated to gallery context; the original graffiti-to-fine-art crossover
- **Subway art and wildstyle** -- NYC subway car pieces from the 1970s--80s; the foundational visual source for the entire aesthetic
- **Skateboard deck graphics** -- bold character art, irreverent humor, and high-contrast color combinations

---

## Related Aesthetics

| Aesthetic | Relationship to Graffiti Pop |
|-----------|------------------------------|
| **Hip-Hop / B-Boy** | Parent culture; Graffiti Pop is the visual arm of hip-hop alongside breakdancing, DJing, and MCing |
| **Gangsta Rap** | Shares street-culture roots; darker, more aggressive variant with focus on West Coast/South imagery |
| **Skater / Skate Punk** | Parallel subculture; shares DIY graphics, bold type, irreverent attitude; overlaps heavily in brand aesthetics |
| **Punk / DIY Punk** | Foundational influence; collage, xerox, anti-establishment energy; Graffiti Pop is punk's visual cousin on the street |
| **Grunge** | Shares raw, anti-polish attitude; Grunge is more muted and introspective, Graffiti Pop is bright and extroverted |
| **UrBling** | Hip-hop's luxury evolution; where Graffiti Pop is street-level, UrBling adds gold, diamonds, and aspirational wealth |
| **Vectordelia** | Digital evolution; takes the flowing lines and bright colors into clean vector illustration |
| **Memphis Design** | Shared maximalism and bold color; Memphis brings geometric patterns and pastel variants to similar energy |
| **Rave** | Parallel 90s subculture; shares neon palette and kinetic energy; Rave is more electronic/psychedelic |
| **Alternative** | Broad overlap in 90s counterculture; Alternative tends toward introspection where Graffiti Pop is extroverted |
| **Shibuya Punk** | Japanese interpretation of street culture; blends Graffiti Pop with Harajuku fashion and anime influence |

---

## Quick-Start: Minimal Graffiti Pop Page Template

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Graffiti Pop Page</title>
  <link href="https://fonts.googleapis.com/css2?family=Bungee+Shade&family=Bungee&family=Bangers&family=Permanent+Marker&family=Rock+Salt&family=Russo+One&family=Lilita+One&family=Share+Tech+Mono&display=swap" rel="stylesheet">
  <style>
    :root {
      --gpop-black: #111111;
      --gpop-concrete: #5a5a5a;
      --gpop-concrete-warm: #7a7168;
      --gpop-brick: #8b4513;
      --gpop-mortar: #a09080;
      --gpop-pink: #ff1493;
      --gpop-neon-green: #39ff14;
      --gpop-blue: #0080ff;
      --gpop-purple: #9b30ff;
      --gpop-yellow: #ffd700;
      --gpop-red: #ff2400;
      --gpop-white: #ffffff;
      --gpop-silver: #c0c0c0;
      --gpop-cream: #f5f0e0;
    }

    * { margin: 0; padding: 0; box-sizing: border-box; }

    body {
      background: var(--gpop-black);
      color: var(--gpop-cream);
      font-family: 'Russo One', Tahoma, sans-serif;
      font-weight: 400;
      line-height: 1.6;
      position: relative;
      overflow-x: hidden;
    }

    /* Brick wall texture on body */
    body::before {
      content: '';
      position: fixed;
      inset: 0;
      background-image:
        repeating-linear-gradient(
          0deg,
          transparent, transparent 48px,
          rgba(160, 144, 128, 0.08) 48px,
          rgba(160, 144, 128, 0.08) 52px
        ),
        repeating-linear-gradient(
          90deg,
          transparent, transparent 98px,
          rgba(160, 144, 128, 0.05) 98px,
          rgba(160, 144, 128, 0.05) 102px
        );
      pointer-events: none;
      z-index: 0;
    }

    .hero {
      text-align: center;
      padding: 8rem 2rem 6rem;
      position: relative;
      z-index: 1;
      background:
        radial-gradient(circle at 20% 50%, rgba(255, 20, 147, 0.08) 0%, transparent 40%),
        radial-gradient(circle at 80% 50%, rgba(57, 255, 20, 0.06) 0%, transparent 40%);
    }

    .hero h1 {
      font-family: 'Bungee Shade', Impact, sans-serif;
      font-size: clamp(3rem, 8vw, 7rem);
      line-height: 1.0;
      letter-spacing: 0.04em;
      color: var(--gpop-white);
      text-shadow:
        3px 3px 0 var(--gpop-pink),
        6px 6px 0 rgba(0, 0, 0, 0.5);
      margin-bottom: 1rem;
    }

    .hero p {
      font-family: 'Share Tech Mono', monospace;
      font-size: 0.85rem;
      text-transform: uppercase;
      letter-spacing: 0.2em;
      color: var(--gpop-silver);
    }

    /* Spray splatter divider */
    .gpop-divider {
      border: none;
      height: 20px;
      position: relative;
      margin: 0;
    }

    .gpop-divider::before {
      content: '';
      position: absolute;
      top: 8px;
      left: 5%;
      width: 8px;
      height: 8px;
      border-radius: 50%;
      background: var(--gpop-pink);
      box-shadow:
        40px -3px 0 2px var(--gpop-neon-green),
        90px 4px 0 1px var(--gpop-blue),
        150px -2px 0 3px var(--gpop-yellow),
        220px 3px 0 1px var(--gpop-purple),
        280px -4px 0 2px var(--gpop-pink),
        350px 2px 0 3px var(--gpop-red);
    }

    section {
      max-width: 900px;
      margin: 0 auto;
      padding: 4rem 2rem;
      position: relative;
      z-index: 1;
    }

    h2 {
      font-family: 'Bangers', cursive;
      font-size: clamp(2rem, 5vw, 3.5rem);
      text-transform: uppercase;
      letter-spacing: 0.06em;
      color: var(--gpop-neon-green);
      text-shadow:
        2px 2px 0 var(--gpop-black),
        -1px -1px 0 var(--gpop-black),
        1px -1px 0 var(--gpop-black),
        -1px 1px 0 var(--gpop-black);
      margin-bottom: 1.5rem;
    }

    .gpop-poster-card {
      background: var(--gpop-cream);
      color: var(--gpop-black);
      padding: 2rem;
      position: relative;
      transform: rotate(-1deg);
      box-shadow:
        3px 3px 10px rgba(0, 0, 0, 0.5),
        0 0 0 1px rgba(0, 0, 0, 0.1);
      margin: 2rem 0;
    }

    .gpop-poster-card h3 {
      font-family: 'Permanent Marker', cursive;
      font-size: 1.5rem;
      color: var(--gpop-black);
      margin-bottom: 0.5rem;
    }

    .gpop-sticker {
      display: inline-block;
      padding: 0.4rem 1rem;
      font-family: 'Bangers', cursive;
      font-size: 1rem;
      text-transform: uppercase;
      letter-spacing: 0.05em;
      color: var(--gpop-black);
      background: var(--gpop-yellow);
      border: 2px solid var(--gpop-black);
      transform: rotate(2deg);
      box-shadow: 2px 2px 0 var(--gpop-black);
    }

    .gpop-button {
      display: inline-block;
      padding: 0.8rem 2.5rem;
      font-family: 'Bangers', cursive;
      font-size: 1.2rem;
      letter-spacing: 0.08em;
      text-transform: uppercase;
      text-decoration: none;
      color: var(--gpop-black);
      background: var(--gpop-neon-green);
      border: 3px solid var(--gpop-black);
      transform: rotate(-1deg);
      box-shadow: 4px 4px 0 var(--gpop-black);
      cursor: pointer;
      transition: all 0.1s ease;
    }

    .gpop-button:hover {
      background: var(--gpop-pink);
      color: var(--gpop-white);
      transform: rotate(0deg) translate(-2px, -2px);
      box-shadow: 6px 6px 0 var(--gpop-black);
    }

    a {
      color: var(--gpop-pink);
      text-decoration: none;
      border-bottom: 2px solid rgba(255, 20, 147, 0.4);
      transition: color 0.15s;
    }

    a:hover {
      color: var(--gpop-neon-green);
      border-bottom-color: var(--gpop-neon-green);
    }
  </style>
</head>
<body>
  <div class="hero">
    <h1>Title Here</h1>
    <p>Subheading in monospace uppercase</p>
  </div>
  <hr class="gpop-divider">
  <section>
    <h2>Section Heading</h2>
    <div class="gpop-poster-card">
      <h3>Card Title</h3>
      <p>Content styled with Graffiti Pop aesthetic. Bold neon colors, spray-paint energy, street-level authenticity.</p>
      <br>
      <span class="gpop-sticker">Fresh!</span>
    </div>
    <br>
    <a href="#" class="gpop-button">Get Started</a>
  </section>
</body>
</html>
```
