# Poster Gal

An aesthetic rooted in the deviantART community of roughly 2002-2013, blending anime-influenced
chibi art with early-2000s pop culture fandom, emo/pop-punk fashion, and amateur digital
photography. Poster Gal (also known as Y2K Chibi or deviantARTcore) captures the enthusiastic,
unpolished creative energy of young female fans who covered their bedroom walls in posters of
favorite actors, drew obsessive fanart in a distinctive chibi-meets-Western-cartoon style, and
documented it all with flash-lit digital camera selfies. The mood is feminine, nerdy, earnest,
and unapologetically obsessive -- a collage of fandom passion rendered in airbrush-smudged
digital art, scanned notebook drawings, and Hot Topic fashion.

---

## Visual Characteristics

- **Chibi-Western hybrid art style** -- heavily stylized, exaggerated chibi proportions merged with Western cartoon influences (Invader Zim, Tiny Toon Adventures); not pure anime, not pure cartoon
- **Airbrush / smudge shading** -- low-quality digital airbrush tool applied heavily, creating visible soft-edged shading artifacts with banding and color bleed; deliberately unpolished
- **Visible pixel artifacts** -- scanned traditional artwork or heavily compressed digital images with JPEG artifacts and pixelation treated as part of the visual texture
- **Exaggerated character expressions** -- over-the-top emotions, large emotive eyes, dramatic poses, and theatrical body language
- **Character fangs** -- fangs drawn on characters universally, even on characters that canonically lack them; a signature stylistic embellishment
- **Large feet, simplified hands** -- proportional exaggeration with oversized feet and fingers drawn connected or simplified into mitten-like forms
- **Japanese lettering as decoration** -- katakana and hiragana characters used as visual ornaments despite the aesthetic's American origins; decorative rather than semantic
- **Kawaii embellishments** -- stars, hearts, sparkles, and cute iconography scattered across artwork and page layouts
- **Flash photography** -- amateur-quality selfies and bedroom photos lit by harsh direct flash from early 2000s consumer digital cameras; washed-out highlights, hard shadows, red-eye
- **Poster-covered walls** -- bedroom environments densely layered with movie posters, band posters, printed fanart, magazine clippings, and photos of favorite actors
- **DeviantART ID cards** -- signature profile cards featuring a self-portrait (drawn or photographed), name, birthday, and categorized lists of likes, loves, and dislikes; digitally composed with decorative borders
- **Scanned paper textures** -- traditional pencil and marker drawings scanned at low resolution, preserving paper grain, smudges, and notebook lines
- **Fandom collage compositions** -- multiple characters, logos, and references crammed into single images; horror vacui approach to fan expression

---

## Color Palette

The palette is **saturated and high-contrast**, reflecting the bold color choices of early digital art tools and the emo/pop-punk visual culture of the mid-2000s. Black dominates as a base, with vivid accent colors pulled from anime art, Hot Topic merchandise, and the bright-on-dark sensibility of the era.

### Primary Palette

| Role                    | Color              | Hex       |
|-------------------------|--------------------|-----------|
| Base background         | Jet Black          | `#0D0D0D` |
| Alt background          | Dark Charcoal      | `#1A1A2E` |
| Surface dark            | Deep Plum          | `#2A1B3D` |
| Surface mid             | Slate Purple       | `#3D2C5E` |
| Primary accent          | Hot Pink           | `#FF1493` |
| Secondary accent        | Electric Blue      | `#00BFFF` |
| Tertiary accent         | Neon Green         | `#39FF14` |
| Warm accent             | Emo Red            | `#CC0033` |
| Highlight               | Vivid Purple       | `#9B30FF` |
| Soft accent             | Bubblegum Pink     | `#FF69B4` |

### Kawaii Accent Colors

| Role              | Color            | Hex       |
|-------------------|------------------|-----------|
| Star yellow       | Bright Yellow    | `#FFD700` |
| Sparkle white     | Pure White       | `#FFFFFF` |
| Sky blue          | Anime Sky        | `#87CEEB` |
| Blush pink        | Cheek Blush      | `#FFB6C1` |
| Fang white        | Cream            | `#FFF8F0` |

### Emo / Pop-Punk Accent Colors

| Role              | Color            | Hex       |
|-------------------|------------------|-----------|
| Eyeliner black    | True Black       | `#000000` |
| Crimson           | Blood Red        | `#8B0000` |
| Band tee gray     | Faded Gray       | `#4A4A4A` |
| Safety pin silver | Metallic Silver  | `#C0C0C0` |
| Checkerboard      | Stark White      | `#FFFFFF` |

### Suggested CSS Custom Properties

```css
:root {
  /* Dark base tones */
  --pg-black: #0d0d0d;
  --pg-charcoal: #1a1a2e;
  --pg-plum: #2a1b3d;
  --pg-slate-purple: #3d2c5e;

  /* Vibrant accents */
  --pg-hot-pink: #ff1493;
  --pg-electric-blue: #00bfff;
  --pg-neon-green: #39ff14;
  --pg-emo-red: #cc0033;
  --pg-vivid-purple: #9b30ff;
  --pg-bubblegum: #ff69b4;

  /* Kawaii accents */
  --pg-star-yellow: #ffd700;
  --pg-sparkle-white: #ffffff;
  --pg-sky-blue: #87ceeb;
  --pg-blush-pink: #ffb6c1;
  --pg-cream: #fff8f0;

  /* Emo layer */
  --pg-true-black: #000000;
  --pg-crimson: #8b0000;
  --pg-faded-gray: #4a4a4a;
  --pg-silver: #c0c0c0;

  /* Functional mappings */
  --pg-bg-primary: var(--pg-black);
  --pg-bg-secondary: var(--pg-charcoal);
  --pg-bg-card: var(--pg-plum);
  --pg-text-primary: var(--pg-cream);
  --pg-text-secondary: var(--pg-blush-pink);
  --pg-text-heading: var(--pg-hot-pink);
  --pg-accent-primary: var(--pg-hot-pink);
  --pg-accent-secondary: var(--pg-electric-blue);
  --pg-accent-tertiary: var(--pg-neon-green);
  --pg-border: var(--pg-vivid-purple);
  --pg-link: var(--pg-electric-blue);
  --pg-link-hover: var(--pg-hot-pink);
  --pg-shadow: rgba(255, 20, 147, 0.2);
}
```

### Usage Notes

- **Black dominates** -- dark backgrounds are the default canvas; content glows against darkness like a screen in a dimly-lit bedroom
- **Pink and purple are the backbone** -- hot pink and vivid purple appear most frequently across art, fashion, and UI elements
- **High saturation, no pastels** -- colors are vivid and electric, not soft or muted; this aesthetic predates the pastel internet era
- **Emo red for edge** -- crimson and blood red provide the darker, heavier counterpoint to kawaii pinks
- **Neon green and electric blue as pop accents** -- used sparingly for highlights, links, and decorative sparkle effects
- **White for sparkle and text** -- pure white used for star/sparkle decorations and high-contrast text on dark backgrounds

---

## Typography

### Typeface Characteristics

Poster Gal typography reflects the deviantART era's DIY digital aesthetic:

- **Chunky, rounded display fonts** -- headlines evoke early-2000s web design with bubbly, bold letterforms
- **Handwritten / marker-style fonts** -- mimicking notebook doodles and hand-lettered fanart titles
- **Gothic / emo display fonts** -- blackletter-influenced fonts for band-name styling and edgy headers
- **Japanese-inflected decorative text** -- katakana-style letterforms or actual Japanese characters used ornamentally
- **Pixel and bitmap fonts** -- 8-bit-style type reflecting the early web and gaming culture of the era
- **Heavy drop shadows and outlines** -- text treatments with thick colored outlines or deep drop shadows, a hallmark of 2000s digital art
- **Mixed-case chaos** -- deliberate mixing of capitalization styles (aLtErNaTiNg CaPs, ALL CAPS for emphasis)

### Recommended Web Fonts

| Font                    | Style                                | Usage                                      |
|-------------------------|--------------------------------------|--------------------------------------------|
| **Bangers**             | Chunky comic-book display            | Primary headlines, hero text               |
| **Boogaloo**            | Rounded, playful display             | Section headings, kawaii-inflected titles   |
| **Permanent Marker**    | Hand-drawn marker feel               | Accent text, notebook-style annotations    |
| **Creepster**           | Horror-comic letterforms             | Edgy headings, Halloween/goth accents      |
| **Press Start 2P**      | Pixel/8-bit style                    | Gaming references, retro UI elements       |
| **Indie Flower**        | Handwritten, whimsical               | Diary text, casual annotations, ID cards   |
| **Russo One**           | Bold, geometric sans-serif           | Body text, navigation, UI labels           |
| **Kosugi Maru**         | Rounded Japanese-supporting font     | Japanese decorative text, kawaii labels     |
| **Gloria Hallelujah**   | Scrawled marker handwriting          | Scattered fan comments, doodle labels      |
| **Special Elite**       | Typewriter-style                     | deviantART profile text, bio sections      |

### Typography CSS Example

```css
@import url('https://fonts.googleapis.com/css2?family=Bangers&family=Boogaloo&family=Permanent+Marker&family=Russo+One:wght@400&family=Indie+Flower&family=Press+Start+2P&display=swap');

/* Headlines -- chunky, loud, comic-book energy */
h1, h2, h3 {
  font-family: 'Bangers', 'Boogaloo', cursive;
  color: var(--pg-text-heading);
  line-height: 1.2;
  letter-spacing: 0.04em;
  text-shadow:
    3px 3px 0px var(--pg-true-black),
    -1px -1px 0px var(--pg-vivid-purple);
}

h1 { font-size: clamp(2.4rem, 5vw, 4.2rem); }
h2 { font-size: clamp(1.6rem, 3.5vw, 2.5rem); }
h3 { font-size: clamp(1.2rem, 2.5vw, 1.8rem); }

/* Body text -- clean, readable on dark backgrounds */
body {
  font-family: 'Russo One', sans-serif;
  font-size: 1rem;
  line-height: 1.7;
  color: var(--pg-text-primary);
  background: var(--pg-bg-primary);
}

/* Handwritten notebook-style text */
.pg-handwritten {
  font-family: 'Permanent Marker', 'Gloria Hallelujah', cursive;
  font-size: 1.3em;
  color: var(--pg-bubblegum);
  transform: rotate(-1.5deg);
  display: inline-block;
}

/* Pixel/gaming text */
.pg-pixel {
  font-family: 'Press Start 2P', monospace;
  font-size: 0.7rem;
  color: var(--pg-neon-green);
  letter-spacing: 0.05em;
  text-shadow: 0 0 8px rgba(57, 255, 20, 0.4);
}

/* Decorative Japanese-style text */
.pg-jp-deco {
  font-family: 'Kosugi Maru', sans-serif;
  font-size: 0.85rem;
  color: var(--pg-sky-blue);
  letter-spacing: 0.3em;
  opacity: 0.6;
}

/* Tag / label text */
.pg-tag {
  font-family: 'Russo One', sans-serif;
  font-size: 0.65rem;
  font-weight: 400;
  text-transform: uppercase;
  letter-spacing: 0.08em;
  color: #fff;
}
```

---

## Key Design Elements and Motifs

### Poster Wall / Fandom Collage

The defining environmental motif -- densely layered walls covered in printed media:

- **Movie and band posters** -- Lord of the Rings, My Chemical Romance, Evanescence, Linkin Park
- **Printed fanart** -- character drawings pinned or taped alongside commercial posters
- **Magazine clippings** -- cutout photos of actors (Orlando Bloom, Johnny Depp, Elijah Wood)
- **Overlapping placement** -- no bare wall visible; items pinned at slight angles, edges overlapping
- **Tape and pin marks** -- visible attachment methods (scotch tape corners, pushpin holes)

### DeviantART ID Card

A signature format combining personal expression with community convention:

- **Rectangular card layout** -- portrait or landscape orientation with a decorative border
- **Self-portrait** -- drawn in chibi style or a flash-lit selfie photo
- **Personal info fields** -- Name, Birthday, Location arranged as labeled data
- **Fandom lists** -- categorized columns: "Likes," "Loves," "Dislikes" filled with band names, anime titles, and character crushes
- **Decorative frame** -- borders embellished with stars, hearts, character doodles, and Japanese text
- **Digital collage construction** -- layered in an image editor with text tool, airbrush accents, and imported clipart

### Chibi Character Art

- **Oversized heads** -- classic chibi proportion (head 1/2 to 1/3 of total body height)
- **Large, expressive eyes** -- anime-derived with exaggerated shine/highlight dots
- **Universal fangs** -- small pointed fangs visible in smiles, applied to all characters regardless of canon
- **Simplified mitten hands** -- fingers connected or reduced to basic shapes
- **Oversized feet** -- disproportionately large relative to body
- **Airbrush-shaded hair** -- soft gradient shading with visible tool artifacts
- **Emo/scene hairstyles on characters** -- side-swept bangs, asymmetric cuts, colored streaks applied to fanart subjects

### Kawaii Sparkle Layer

- **Star bursts** -- four-pointed or six-pointed stars scattered as decorative elements
- **Heart clusters** -- small hearts floating around characters or framing text
- **Sparkle dots** -- tiny highlight dots suggesting glitter or magical effects
- **Rainbow accents** -- small rainbow arcs used as cheerful decorative fills
- **Blush marks** -- pink ovals on character cheeks indicating cuteness/embarrassment

### Flash Photography Aesthetic

- **Harsh direct flash** -- washed-out center, deep shadows at edges
- **Red-eye artifacts** -- a hallmark of the era's point-and-shoot cameras
- **Low resolution** -- visible JPEG compression, soft focus, digital noise
- **Bedroom setting** -- unmade beds, poster walls, computer desks in background
- **Mirror selfies** -- captured in bathroom or bedroom mirrors with camera visible in frame
- **Timestamp watermarks** -- orange date stamps from early digital cameras

---

## Layout Principles

### Grid and Structure

- **Collage-over-grid** -- layouts feel pinned-to-a-wall rather than designed; items overlap, rotate, and scatter
- **Horror vacui (fear of empty space)** -- every surface should feel filled with content, stickers, doodles, or decorative elements
- **Dark canvas, bright content** -- black or very dark backgrounds with vivid content elements creating contrast
- **Asymmetric, handmade feel** -- deliberate imperfection; elements are slightly rotated, unevenly spaced, and casually placed
- **Layered z-index stacking** -- elements overlap freely, mimicking pinned posters and taped photos on a wall
- **deviantART-era web proportions** -- fixed-width centered containers (800-1000px), reminiscent of early-2000s web layouts

### Section Organization

- **Poster-wall sections** -- dense image grids with slight rotations and overlapping edges
- **ID card panels** -- structured personal-info blocks with labeled fields and decorative borders
- **Doodle dividers** -- hand-drawn-style separators with stars, hearts, and squiggly lines
- **Flash photo strips** -- rows of square photos mimicking digital camera snapshots
- **Fandom list blocks** -- bulleted or columnar lists of favorites (bands, anime, movies, games)
- **Sparkle scatter overlays** -- decorative star and heart elements positioned absolutely over content sections

---

## CSS/Design Techniques

### Poster Wall Background

```css
/* Dark bedroom wall base with subtle texture */
.pg-wall {
  background-color: var(--pg-black);
  background-image:
    radial-gradient(
      ellipse at 20% 30%,
      rgba(42, 27, 61, 0.4) 0%,
      transparent 50%
    ),
    radial-gradient(
      ellipse at 80% 70%,
      rgba(61, 44, 94, 0.3) 0%,
      transparent 50%
    );
}

/* Subtle wall texture noise overlay */
.pg-wall::before {
  content: '';
  position: absolute;
  inset: 0;
  background-image: url("data:image/svg+xml,%3Csvg viewBox='0 0 256 256' xmlns='http://www.w3.org/2000/svg'%3E%3Cfilter id='n'%3E%3CfeTurbulence type='fractalNoise' baseFrequency='0.9' numOctaves='4' stitchTiles='stitch'/%3E%3C/filter%3E%3Crect width='100%25' height='100%25' filter='url(%23n)' opacity='0.06'/%3E%3C/svg%3E");
  pointer-events: none;
  z-index: 0;
}
```

### Poster / Pinned Item Cards

```css
/* Poster pinned to wall */
.pg-poster {
  background: var(--pg-bg-card);
  border: 2px solid var(--pg-vivid-purple);
  padding: 0.75rem;
  position: relative;
  transform: rotate(-2deg);
  box-shadow:
    4px 4px 12px rgba(0, 0, 0, 0.6),
    0 0 20px rgba(155, 48, 255, 0.1);
  transition: transform 0.3s ease, box-shadow 0.3s ease;
}

.pg-poster:hover {
  transform: rotate(0deg) scale(1.03);
  box-shadow:
    6px 6px 20px rgba(0, 0, 0, 0.7),
    0 0 30px rgba(255, 20, 147, 0.2);
  z-index: 10;
}

/* Tape strip holding poster */
.pg-poster::before {
  content: '';
  position: absolute;
  top: -8px;
  left: 50%;
  transform: translateX(-50%) rotate(2deg);
  width: 60px;
  height: 18px;
  background: rgba(255, 248, 240, 0.25);
  border: 1px solid rgba(255, 248, 240, 0.1);
  z-index: 2;
}

/* Alternating rotations for wall effect */
.pg-poster:nth-child(odd) { transform: rotate(-2deg); }
.pg-poster:nth-child(even) { transform: rotate(1.5deg); }
.pg-poster:nth-child(3n) { transform: rotate(-3.5deg); }
.pg-poster:nth-child(4n) { transform: rotate(2.5deg); }
```

### DeviantART ID Card

```css
/* ID card container */
.pg-id-card {
  background: linear-gradient(
    135deg,
    var(--pg-charcoal) 0%,
    var(--pg-plum) 100%
  );
  border: 3px solid var(--pg-hot-pink);
  border-radius: 8px;
  padding: 1.5rem;
  max-width: 400px;
  position: relative;
  box-shadow:
    0 0 15px rgba(255, 20, 147, 0.15),
    4px 4px 0px var(--pg-true-black);
}

/* ID card header with name */
.pg-id-card .id-header {
  font-family: 'Bangers', cursive;
  font-size: 1.6rem;
  color: var(--pg-hot-pink);
  text-shadow: 2px 2px 0px var(--pg-true-black);
  margin-bottom: 0.5rem;
  border-bottom: 2px dashed var(--pg-vivid-purple);
  padding-bottom: 0.5rem;
}

/* ID field labels */
.pg-id-card .id-label {
  font-family: 'Russo One', sans-serif;
  font-size: 0.7rem;
  text-transform: uppercase;
  letter-spacing: 0.1em;
  color: var(--pg-vivid-purple);
  margin-top: 0.6rem;
}

/* ID field values */
.pg-id-card .id-value {
  font-family: 'Indie Flower', cursive;
  font-size: 1rem;
  color: var(--pg-cream);
  line-height: 1.4;
}

/* Decorative star accents on card */
.pg-id-card::after {
  content: '\2605 \2606 \2605';
  position: absolute;
  bottom: 8px;
  right: 12px;
  font-size: 0.8rem;
  color: var(--pg-star-yellow);
  letter-spacing: 0.3em;
  opacity: 0.7;
}
```

### Chibi / Airbrush Glow Effect

```css
/* Simulates the airbrush glow around character art */
.pg-airbrush-glow {
  position: relative;
  display: inline-block;
}

.pg-airbrush-glow::before {
  content: '';
  position: absolute;
  inset: -20px;
  background: radial-gradient(
    ellipse at center,
    rgba(255, 20, 147, 0.15) 0%,
    rgba(155, 48, 255, 0.08) 40%,
    transparent 70%
  );
  filter: blur(10px);
  pointer-events: none;
  z-index: -1;
}

/* Image treatment for art pieces */
.pg-art-piece {
  border: 3px solid var(--pg-hot-pink);
  box-shadow:
    0 0 12px rgba(255, 20, 147, 0.2),
    0 0 30px rgba(155, 48, 255, 0.1);
  image-rendering: auto; /* deliberately not crisp -- airbrush softness */
}
```

### Flash Photo Effect

```css
/* Flash photography / selfie card */
.pg-flash-photo {
  position: relative;
  border: 4px solid #fff;
  box-shadow: 3px 3px 8px rgba(0, 0, 0, 0.5);
  overflow: hidden;
}

/* Flash wash-out overlay */
.pg-flash-photo::after {
  content: '';
  position: absolute;
  inset: 0;
  background: radial-gradient(
    ellipse at 45% 40%,
    rgba(255, 255, 255, 0.2) 0%,
    transparent 55%
  );
  pointer-events: none;
}

/* Timestamp watermark */
.pg-timestamp {
  position: absolute;
  bottom: 6px;
  right: 8px;
  font-family: 'Courier New', monospace;
  font-size: 0.65rem;
  color: #FF8C00;
  text-shadow: 1px 1px 2px rgba(0, 0, 0, 0.8);
  opacity: 0.8;
  letter-spacing: 0.05em;
}
```

### Sparkle / Star Decorations

```css
/* Floating sparkle overlay */
.pg-sparkles {
  position: relative;
}

.pg-sparkles::before,
.pg-sparkles::after {
  position: absolute;
  pointer-events: none;
  z-index: 5;
}

.pg-sparkles::before {
  content: '\2728';
  top: -6px;
  left: -10px;
  font-size: 1rem;
  color: var(--pg-star-yellow);
  opacity: 0.7;
  animation: pg-twinkle 2s ease-in-out infinite;
}

.pg-sparkles::after {
  content: '\2B50';
  bottom: -8px;
  right: -8px;
  font-size: 0.75rem;
  color: var(--pg-star-yellow);
  opacity: 0.5;
  animation: pg-twinkle 2s ease-in-out 0.5s infinite;
}

@keyframes pg-twinkle {
  0%, 100% { opacity: 0.5; transform: scale(1); }
  50% { opacity: 1; transform: scale(1.2); }
}

/* Scattered star background pattern */
.pg-star-field {
  background-image:
    radial-gradient(circle at 10% 15%, var(--pg-star-yellow) 1px, transparent 1px),
    radial-gradient(circle at 85% 25%, var(--pg-hot-pink) 1.5px, transparent 1.5px),
    radial-gradient(circle at 45% 80%, var(--pg-electric-blue) 1px, transparent 1px),
    radial-gradient(circle at 70% 60%, var(--pg-star-yellow) 0.8px, transparent 0.8px),
    radial-gradient(circle at 25% 55%, var(--pg-vivid-purple) 1.2px, transparent 1.2px),
    radial-gradient(circle at 60% 10%, var(--pg-neon-green) 0.8px, transparent 0.8px);
}
```

### Doodle / Hand-Drawn Divider

```css
/* Squiggly hand-drawn-style divider */
.pg-doodle-divider {
  text-align: center;
  padding: 1.5rem 0;
  user-select: none;
  position: relative;
}

.pg-doodle-divider::before {
  content: '';
  position: absolute;
  top: 50%;
  left: 10%;
  right: 10%;
  height: 2px;
  background: repeating-linear-gradient(
    90deg,
    var(--pg-hot-pink) 0px,
    var(--pg-hot-pink) 6px,
    transparent 6px,
    transparent 10px,
    var(--pg-vivid-purple) 10px,
    var(--pg-vivid-purple) 16px,
    transparent 16px,
    transparent 20px
  );
  opacity: 0.5;
}

/* Star and heart decorative text divider */
.pg-divider-fancy {
  font-size: 0.85rem;
  letter-spacing: 0.6em;
  color: var(--pg-hot-pink);
  text-shadow: 0 0 8px rgba(255, 20, 147, 0.3);
}
```

### Fandom List Block

```css
/* Favorites list styled like an ID card section */
.pg-fandom-list {
  background: rgba(42, 27, 61, 0.6);
  border: 1px solid var(--pg-vivid-purple);
  border-radius: 6px;
  padding: 1rem 1.2rem;
}

.pg-fandom-list h4 {
  font-family: 'Permanent Marker', cursive;
  font-size: 1rem;
  color: var(--pg-electric-blue);
  margin-bottom: 0.5rem;
  text-shadow: 1px 1px 0px var(--pg-true-black);
}

.pg-fandom-list ul {
  list-style: none;
  padding: 0;
}

.pg-fandom-list li {
  font-family: 'Indie Flower', cursive;
  font-size: 0.95rem;
  color: var(--pg-cream);
  padding: 0.15rem 0;
  line-height: 1.5;
}

.pg-fandom-list li::before {
  content: '\2665 ';
  color: var(--pg-hot-pink);
  font-size: 0.8em;
}
```

### Poster Wall Grid Layout

```css
/* Dense poster-wall grid with organic feel */
.pg-wall-grid {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(200px, 1fr));
  gap: 1rem;
  padding: 2rem;
  position: relative;
}

/* Overlapping collage variant */
.pg-collage-grid {
  display: grid;
  grid-template-columns: repeat(12, 1fr);
  grid-auto-rows: 40px;
  gap: 0;
  padding: 1rem;
}

.pg-collage-grid > :nth-child(1) { grid-column: 1 / 5; grid-row: 1 / 5; transform: rotate(-3deg); z-index: 2; }
.pg-collage-grid > :nth-child(2) { grid-column: 4 / 8; grid-row: 1 / 6; transform: rotate(1.5deg); z-index: 3; }
.pg-collage-grid > :nth-child(3) { grid-column: 7 / 11; grid-row: 1 / 5; transform: rotate(-1deg); z-index: 1; }
.pg-collage-grid > :nth-child(4) { grid-column: 9 / 13; grid-row: 2 / 6; transform: rotate(2.5deg); z-index: 4; }
.pg-collage-grid > :nth-child(5) { grid-column: 1 / 6; grid-row: 4 / 9; transform: rotate(0.5deg); z-index: 2; }
.pg-collage-grid > :nth-child(6) { grid-column: 5 / 9; grid-row: 5 / 9; transform: rotate(-2deg); z-index: 5; }
```

### Neon Glow / Bedroom LED Effect

```css
/* Neon-glow border for hero sections */
.pg-neon-border {
  border: 2px solid var(--pg-hot-pink);
  box-shadow:
    0 0 8px var(--pg-hot-pink),
    0 0 20px rgba(255, 20, 147, 0.3),
    inset 0 0 8px rgba(255, 20, 147, 0.05);
}

/* Multi-color neon text glow */
.pg-neon-text {
  color: var(--pg-hot-pink);
  text-shadow:
    0 0 4px var(--pg-hot-pink),
    0 0 12px var(--pg-hot-pink),
    0 0 24px rgba(155, 48, 255, 0.4),
    0 0 48px rgba(0, 191, 255, 0.2);
}

/* Alternating glow colors for emphasis */
@keyframes pg-glow-cycle {
  0%, 100% { text-shadow: 0 0 8px var(--pg-hot-pink), 0 0 20px rgba(255, 20, 147, 0.4); }
  33% { text-shadow: 0 0 8px var(--pg-electric-blue), 0 0 20px rgba(0, 191, 255, 0.4); }
  66% { text-shadow: 0 0 8px var(--pg-vivid-purple), 0 0 20px rgba(155, 48, 255, 0.4); }
}

.pg-glow-animate {
  animation: pg-glow-cycle 6s ease-in-out infinite;
}
```

### JPEG Artifact / Lo-Fi Digital Texture

```css
/* Simulated JPEG compression / low-quality digital feel */
.pg-lo-fi {
  filter: contrast(1.1) saturate(1.15);
  image-rendering: auto;
}

/* Chromatic aberration edge effect */
.pg-glitch-edge {
  position: relative;
}

.pg-glitch-edge::before,
.pg-glitch-edge::after {
  content: '';
  position: absolute;
  inset: 0;
  pointer-events: none;
}

.pg-glitch-edge::before {
  background: linear-gradient(
    90deg,
    transparent 0%,
    rgba(255, 20, 147, 0.1) 2%,
    transparent 4%,
    transparent 96%,
    rgba(0, 191, 255, 0.1) 98%,
    transparent 100%
  );
}
```

---

## Composition and Layout Principles

- **Bedroom-wall metaphor** -- the viewport represents a fan's bedroom wall; content is "pinned," "taped," and "stuck" to a dark surface
- **Dense, layered, overlapping** -- items crowd together at varied angles, creating depth through overlap rather than whitespace
- **Fixed-width, centered container** -- an 800-1000px max-width main column, echoing 2000s-era fixed-width web design
- **Sidebar optional** -- a narrow sidebar for profile/ID-card info, mimicking deviantART's journal layout
- **Dark field composition** -- all content floats on a black or deep purple background
- **Sections feel like different wall zones** -- each content section is a cluster of pinned items rather than a formal layout block
- **Decorative noise everywhere** -- stars, hearts, Japanese text, and doodles fill gaps between content elements
- **Text blocks within bordered containers** -- fandom lists, bios, and descriptions enclosed in colored-border panels

### Layout CSS

```css
/* Main page container -- centered, fixed-width era */
.pg-page {
  max-width: 960px;
  margin: 0 auto;
  background: var(--pg-bg-primary);
  min-height: 100vh;
  padding: 2rem;
  position: relative;
}

/* Hero section -- big statement */
.pg-hero {
  text-align: center;
  padding: 4rem 2rem 3rem;
  position: relative;
  overflow: hidden;
}

/* Two-column layout mimicking dA journal + sidebar */
.pg-two-col {
  display: grid;
  grid-template-columns: 1fr 280px;
  gap: 2rem;
  align-items: start;
}

@media (max-width: 768px) {
  .pg-two-col {
    grid-template-columns: 1fr;
  }
}
```

---

## Materials and Textures (Visual Metaphors for Web)

| Physical / Era Reference       | Web Equivalent                                                                    |
|--------------------------------|-----------------------------------------------------------------------------------|
| Bedroom wall (dark, textured)  | Near-black background with subtle noise SVG overlay and purple radial gradients   |
| Scotch tape holding posters    | Semi-transparent white strip (`::before` pseudo-element) atop card edges          |
| Pushpin marks                  | Small colored circles positioned at card top-center                               |
| Flash photography wash-out     | Radial gradient white overlay at center of image containers                       |
| Airbrush smudge shading        | `filter: blur()` with radial pink/purple gradients behind elements                |
| JPEG compression artifacts     | `filter: contrast(1.1) saturate(1.15)` plus chromatic aberration edge gradients   |
| Notebook / sketchbook paper    | Light cream background (`#FFF8F0`) with faint ruled lines via `repeating-linear-gradient` |
| Scanned art with paper grain   | SVG noise texture overlay at low opacity                                          |
| Hot Topic merchandise          | Bold pink/black color blocking with chunky display type                           |
| Digital camera timestamp       | Orange monospace text positioned in bottom-right corner of photo containers       |
| Star/heart stickers            | Unicode characters (sparkles, stars, hearts) positioned absolutely as decorations |
| DeviantART profile layout      | Fixed-width container with bordered sections, labeled fields, avatar placement    |

---

## Animation and Motion

### Sparkle Twinkle

```css
@keyframes pg-twinkle {
  0%, 100% { opacity: 0.4; transform: scale(0.8); }
  50% { opacity: 1; transform: scale(1.2); }
}

.pg-sparkle-anim {
  animation: pg-twinkle 2s ease-in-out infinite;
}

/* Staggered twinkle for multiple sparkles */
.pg-sparkle-anim:nth-child(2) { animation-delay: 0.3s; }
.pg-sparkle-anim:nth-child(3) { animation-delay: 0.7s; }
.pg-sparkle-anim:nth-child(4) { animation-delay: 1.1s; }
```

### Poster Wobble on Hover

```css
@keyframes pg-wobble {
  0%, 100% { transform: rotate(-2deg); }
  25% { transform: rotate(-0.5deg); }
  75% { transform: rotate(-3deg); }
}

.pg-poster:hover {
  animation: pg-wobble 0.5s ease-in-out;
}
```

### Glow Pulse

```css
@keyframes pg-pulse {
  0%, 100% { box-shadow: 0 0 8px var(--pg-hot-pink), 0 0 20px rgba(255, 20, 147, 0.2); }
  50% { box-shadow: 0 0 16px var(--pg-hot-pink), 0 0 40px rgba(255, 20, 147, 0.35); }
}

.pg-glow-pulse {
  animation: pg-pulse 3s ease-in-out infinite;
}
```

---

## Cultural Context and Media References

### Music (Core to the Identity)

- **Pop-punk / emo** -- My Chemical Romance, Fall Out Boy, Panic! at the Disco, blink-182, AFI, Green Day
- **Nu-metal** -- Linkin Park, System of a Down, Evanescence
- **J-pop / J-rock / Visual Kei** -- Japanese music fandom as a bridge to anime culture
- **Alternative / industrial** -- Nine Inch Nails, Marilyn Manson, Rammstein

### Film and Television

- *Lord of the Rings* trilogy -- Orlando Bloom (Legolas), Elijah Wood, Hugo Weaving (Agent Smith/Elrond) as key crush objects
- *The Matrix* trilogy -- cyberpunk aesthetic crossover
- *Pirates of the Caribbean* -- Johnny Depp as Jack Sparrow
- *Harry Potter* series -- literary and cinematic fandom
- Tim Burton films -- gothic-cute crossover aesthetic
- *Invader Zim* (2001-2006) -- major cartoon influence on art style and humor
- *Clerks: The Animated Series* and Kevin Smith films

### Anime

- *Death Note*, *InuYasha*, *Naruto*, *Sailor Moon*, *Trigun*, *Fullmetal Alchemist*
- Characters redrawn in Poster Gal chibi style as the primary fan-art form

### Video Games

- *Final Fantasy* series, *Legend of Zelda*, *Kingdom Hearts*, *Mega Man*, *Sonic*
- *Neopets*, *World of Warcraft* -- online community games
- *Resident Evil* -- horror gaming crossover

### Platforms and Communities

- **deviantART** (primary home) -- profile customization, art journals, ID cards, community interaction
- **Hot Topic** -- primary fashion retail source
- **ThinkGeek** -- nerd merchandise

### Fashion Influences

- JNCO-style baggy jeans
- Layered long-sleeve under short-sleeve t-shirts (typically band tees)
- Heavy dark eyeliner and emo-influenced makeup
- Band merchandise (wristbands, pins, patches)
- Black as the dominant wardrobe color with splashes of color from accessories

---

## Related Aesthetics

| Aesthetic               | Relationship to Poster Gal                                                                    |
|-------------------------|-----------------------------------------------------------------------------------------------|
| **Olderbrothercore**    | Male counterpart; Poster Gal is described as "a more feminine and nerdier version"            |
| **Scene**               | Overlapping fashion and music tastes; Scene is more flamboyant, Poster Gal more introverted   |
| **Emo**                 | Shared music, fashion (dark makeup, layered shirts), and emotional expression                  |
| **Animecore**           | Shared anime obsession; Poster Gal adds Western cartoon and emo-fashion layers                |
| **Old Web / Webcore**   | Shared deviantART-era digital culture and early-2000s web design sensibilities                 |
| **Y2K Futurism**        | Overlapping time period; Poster Gal is the fan-culture expression of Y2K-era youth            |
| **Mallgoth**            | Shared Hot Topic shopping culture and dark fashion; Mallgoth is heavier, more gothic           |
| **Otaku / Moe**         | Shared anime fandom roots; Otaku is more purely Japanese-culture-focused                      |
| **Metalheart**          | Shared nu-metal music influences and dark-on-bright visual language                           |
| **Teenpunk**            | Overlapping rebellious youth culture and pop-punk music                                       |
| **Frutiger Aero**       | Contemporary Y2K-era aesthetic but with opposite visual language (glossy, corporate, clean)    |
| **Nu-Metal**            | Shared music fandom (Linkin Park, SOAD); Nu-Metal aesthetic is heavier and more masculine     |

---

## Implementation Notes

- The Poster Gal aesthetic is **unpolished by design** -- avoid overly clean, modern CSS effects. The charm comes from imperfection: slightly rotated elements, visible artifacts, and the feeling of a teenager's bedroom wall rather than a professional layout.
- **Dark backgrounds are essential** -- the aesthetic lives on black and deep purple. Bright backgrounds destroy the mood entirely.
- **Pink and purple are non-negotiable** -- hot pink and vivid purple are the visual signatures. Without them, it reads as generic emo or generic anime, not Poster Gal.
- **Fangs on everything** -- if you include any character illustrations, add fangs. It is the single most recognizable art-style quirk.
- **Japanese text as decoration** -- scattered katakana or hiragana characters add authenticity even if non-semantic; they reflect the era's "cool Japan" enthusiasm.
- **The deviantART ID card format** -- reproducing this as a component (name, birthday, likes/dislikes lists) is immediately recognizable to anyone from the era.
- **Flash photo aesthetic** -- if incorporating photography, the white-center radial gradient overlay and orange timestamp are era-defining touches.
- **Horror vacui** -- empty space feels wrong in this aesthetic. Fill gaps with sparkles, stars, doodles, and decorative text.
- **Sound design** -- if audio is relevant, the era's soundtrack is pop-punk and emo rock (My Chemical Romance, Fall Out Boy, Linkin Park) mixed with J-pop.

---

## Quick-Start: Minimal Poster Gal Page Template

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Poster Gal Page</title>
  <link href="https://fonts.googleapis.com/css2?family=Bangers&family=Boogaloo&family=Permanent+Marker&family=Russo+One&family=Indie+Flower&family=Press+Start+2P&display=swap" rel="stylesheet">
  <style>
    :root {
      --pg-black: #0d0d0d;
      --pg-charcoal: #1a1a2e;
      --pg-plum: #2a1b3d;
      --pg-slate-purple: #3d2c5e;
      --pg-hot-pink: #ff1493;
      --pg-electric-blue: #00bfff;
      --pg-neon-green: #39ff14;
      --pg-emo-red: #cc0033;
      --pg-vivid-purple: #9b30ff;
      --pg-bubblegum: #ff69b4;
      --pg-star-yellow: #ffd700;
      --pg-cream: #fff8f0;
      --pg-silver: #c0c0c0;
    }

    * { margin: 0; padding: 0; box-sizing: border-box; }

    body {
      background: var(--pg-black);
      color: var(--pg-cream);
      font-family: 'Russo One', sans-serif;
      font-size: 1rem;
      line-height: 1.7;
      min-height: 100vh;
    }

    h1, h2, h3 {
      font-family: 'Bangers', cursive;
      color: var(--pg-hot-pink);
      text-shadow: 3px 3px 0px #000, -1px -1px 0px var(--pg-vivid-purple);
      letter-spacing: 0.04em;
    }

    /* Hero */
    .hero {
      text-align: center;
      padding: 5rem 2rem 3rem;
      position: relative;
      overflow: hidden;
    }

    .hero::before {
      content: '';
      position: absolute;
      inset: 0;
      background: radial-gradient(
        ellipse at 50% 50%,
        rgba(155, 48, 255, 0.1) 0%,
        transparent 60%
      );
      pointer-events: none;
    }

    .hero h1 {
      font-size: clamp(2.8rem, 6vw, 5rem);
      position: relative;
      z-index: 1;
    }

    .hero .subtitle {
      font-family: 'Permanent Marker', cursive;
      font-size: 1.3rem;
      color: var(--pg-electric-blue);
      transform: rotate(-2deg);
      display: inline-block;
      margin-top: 0.5rem;
      position: relative;
      z-index: 1;
    }

    .sparkle-divider {
      text-align: center;
      padding: 1rem 0;
      font-size: 0.9rem;
      letter-spacing: 0.5em;
      color: var(--pg-star-yellow);
      user-select: none;
      opacity: 0.7;
    }

    /* Poster wall grid */
    .poster-grid {
      display: grid;
      grid-template-columns: repeat(auto-fill, minmax(220px, 1fr));
      gap: 1.5rem;
      max-width: 960px;
      margin: 0 auto;
      padding: 2rem;
    }

    .poster-card {
      background: var(--pg-plum);
      border: 2px solid var(--pg-vivid-purple);
      padding: 1.2rem;
      position: relative;
      box-shadow: 4px 4px 12px rgba(0, 0, 0, 0.6);
      transition: transform 0.3s ease, box-shadow 0.3s ease;
    }

    .poster-card:nth-child(odd) { transform: rotate(-1.5deg); }
    .poster-card:nth-child(even) { transform: rotate(1deg); }

    .poster-card:hover {
      transform: rotate(0deg) scale(1.03);
      box-shadow: 6px 6px 20px rgba(0, 0, 0, 0.7), 0 0 20px rgba(255, 20, 147, 0.15);
      z-index: 10;
    }

    /* Tape effect */
    .poster-card::before {
      content: '';
      position: absolute;
      top: -7px;
      left: 50%;
      transform: translateX(-50%) rotate(1deg);
      width: 50px;
      height: 16px;
      background: rgba(255, 248, 240, 0.2);
      border: 1px solid rgba(255, 248, 240, 0.08);
    }

    .poster-card h3 {
      font-size: 1.2rem;
      margin-bottom: 0.4rem;
    }

    .poster-card p {
      font-family: 'Indie Flower', cursive;
      font-size: 0.95rem;
      color: rgba(255, 248, 240, 0.85);
    }

    .tag {
      display: inline-block;
      padding: 0.15rem 0.6rem;
      font-family: 'Russo One', sans-serif;
      font-size: 0.6rem;
      text-transform: uppercase;
      letter-spacing: 0.06em;
      border-radius: 3px;
      margin-bottom: 0.6rem;
      color: #fff;
    }

    .tag--pink { background: var(--pg-hot-pink); }
    .tag--blue { background: var(--pg-electric-blue); }
    .tag--purple { background: var(--pg-vivid-purple); }
    .tag--green { background: var(--pg-neon-green); color: #000; }

    /* ID Card section */
    .id-section {
      max-width: 960px;
      margin: 2rem auto;
      padding: 0 2rem;
    }

    .id-card {
      background: linear-gradient(135deg, var(--pg-charcoal), var(--pg-plum));
      border: 3px solid var(--pg-hot-pink);
      border-radius: 8px;
      padding: 2rem;
      max-width: 420px;
      margin: 0 auto;
      box-shadow: 0 0 15px rgba(255, 20, 147, 0.12), 4px 4px 0px #000;
      position: relative;
    }

    .id-card::after {
      content: '\2605 \2606 \2605';
      position: absolute;
      bottom: 8px;
      right: 12px;
      font-size: 0.8rem;
      color: var(--pg-star-yellow);
      letter-spacing: 0.3em;
      opacity: 0.6;
    }

    .id-card h2 {
      font-size: 1.6rem;
      border-bottom: 2px dashed var(--pg-vivid-purple);
      padding-bottom: 0.4rem;
      margin-bottom: 0.8rem;
    }

    .id-card .label {
      font-size: 0.65rem;
      text-transform: uppercase;
      letter-spacing: 0.1em;
      color: var(--pg-vivid-purple);
      margin-top: 0.5rem;
    }

    .id-card .value {
      font-family: 'Indie Flower', cursive;
      font-size: 1rem;
      color: var(--pg-cream);
    }
  </style>
</head>
<body>
  <div class="hero">
    <h1>My Wall of Fandom</h1>
    <span class="subtitle">~ where obsession meets art ~</span>
  </div>

  <div class="sparkle-divider">* * * * * * *</div>

  <section class="poster-grid">
    <div class="poster-card">
      <span class="tag tag--pink">Fanart</span>
      <h3>Chibi Collection</h3>
      <p>Every character gets fangs. Every single one. It's the law.</p>
    </div>
    <div class="poster-card">
      <span class="tag tag--blue">Music</span>
      <h3>MCR Forever</h3>
      <p>The Black Parade poster, slightly torn at the corner, held up with three strips of tape.</p>
    </div>
    <div class="poster-card">
      <span class="tag tag--purple">Anime</span>
      <h3>Death Note Corner</h3>
      <p>L sits next to a hand-drawn chibi Legolas. They are neighbors now.</p>
    </div>
    <div class="poster-card">
      <span class="tag tag--green">Gaming</span>
      <h3>Final Fantasy Shrine</h3>
      <p>Printed walkthroughs taped alongside hand-drawn character art.</p>
    </div>
  </section>

  <section class="id-section">
    <div class="id-card">
      <h2>DeviantART ID</h2>
      <div class="label">Name</div>
      <div class="value">xX_StardustGal_Xx</div>
      <div class="label">Birthday</div>
      <div class="value">March 15th</div>
      <div class="label">Loves</div>
      <div class="value">MCR, Death Note, Orlando Bloom, drawing fangs on everything</div>
      <div class="label">Dislikes</div>
      <div class="value">Preps, buffering, running out of printer ink</div>
    </div>
  </section>
</body>
</html>
```
