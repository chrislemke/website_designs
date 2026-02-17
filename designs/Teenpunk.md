# Teenpunk Design Reference

Teenpunk is the commercial youth aesthetic that dominated late-1990s to early-2010s mall culture, fusing **punk-inspired motifs with accessible, mass-market fashion**. It packages teenage rebellion and non-conformity into a playful, consumer-friendly format -- the visual language of Hot Topic clearance racks, Avril Lavigne music videos, Monster High dolls, and Myspace profile pages. The palette is built on a stark **black-and-hot-pink foundation** with checkerboard patterns, skull-and-crossbones adorned with bows, paint splatters, and fishnet textures. The mood is edgy-but-accessible: punk princess angst filtered through pop hooks and mall retail. Everything looks like it was designed on a composition notebook cover in study hall -- stars, hearts, lightning bolts, and band logos scrawled over every surface. Where authentic punk rejects commercialism, Teenpunk *is* the commercialized rebellion, and it owns that contradiction with neon-streaked confidence.

---

## Visual Characteristics

### Core Motifs and Patterns

- **Skulls with feminine accents** -- the signature Teenpunk icon: skulls adorned with hair bows, hearts for eyes, rhinestones, or lipstick; the juxtaposition of tough and cute defines the entire aesthetic
- **Checkerboard patterns** -- black-and-white checks on everything (inspired by Vans slip-ons and ska punk); used as borders, fills, backgrounds, and accent strips
- **Stars and lightning bolts** -- hand-drawn or stamped star shapes (five-pointed), often scattered as decorative confetti or used as bullet points; lightning bolts as energy symbols
- **Paint splatters and drips** -- graffiti-style splatter effects in hot pink, white, or neon green against black backgrounds
- **Hearts** -- both conventional and edgy variants: broken hearts, hearts with crossbones, hearts with skulls, hearts on fire
- **Fishnet texture** -- the diamond-grid fishnet stocking pattern used as overlay textures, background fills, or border treatments
- **Guitar silhouettes** -- electric guitars (especially Flying V shapes) as decorative motifs referencing pop-punk music culture
- **Plaid / tartan patterns** -- punk-derived plaid in pink-and-black or red-and-black, referencing school-uniform skirts gone rebellious
- **Composition notebook lines** -- ruled and margin-lined paper textures suggesting school notebook doodles
- **Crossbones** -- paired with skulls or used independently; the pirate-punk crossover symbol
- **Safety pins and studs** -- punk hardware used decoratively; rows of studs as borders, safety pins as accents
- **Neon hair streaks** -- bright pink, green, or purple color streaks suggesting dyed hair extensions
- **Band logo typography** -- angular, distressed band-name lettering scattered as background decoration
- **Glitter and sparkle effects** -- MySpace-era glitter graphics: sparkling overlays, rhinestone-like dots, shimmer animations

### Design Principles

- **Black base with hot pink punch** -- the core visual formula is near-black backgrounds or elements with hot pink as the primary accent; this pairing is non-negotiable
- **Tough meets cute** -- every design element should balance edginess with playfulness; skulls wear bows, danger symbols get hearts
- **Maximalist layering** -- pile on the motifs; stars, splatters, checks, and skulls can coexist in the same composition like a sticker-bombed locker
- **Hand-drawn energy** -- elements should look sketched, doodled, or stamped rather than precision-engineered; the vibe is notebook margins, not design studio
- **Commercial rebellion** -- the aesthetic is self-aware about its mass-market nature; it is polished enough for retail packaging but rough enough to feel "alternative"
- **Scrapbook collage** -- compositions feel assembled from cut-out stickers, magazine clippings, and printouts layered on a black or dark surface
- **Myspace-era digital sparkle** -- glitter graphics, sparkle overlays, and animated shine effects reference the social media platform where the aesthetic thrived
- **High contrast, limited palette** -- restrict the palette to black, white, hot pink, and one or two supporting accents; more colors dilute the identity
- **Youth-targeted boldness** -- everything should be legible, loud, and immediately appealing to a teenage audience; subtlety is not the goal

---

## Color Palette

### Primary Scheme

| Role | Colors |
|------|--------|
| **Base / Background** | Jet black, near-black charcoal, dark slate |
| **Primary accent** | Hot pink / magenta (the signature color) |
| **Secondary accent** | Pure white (for contrast and checks) |
| **Tertiary accent** | Punk red, neon green (hair-streak references) |
| **Pattern fill** | Black-and-white checkerboard |
| **Sparkle / highlight** | Silver glitter, rhinestone white |

### Detailed Palette

| Color | Hex | Usage |
|-------|-----|-------|
| Jet Black | `#0D0D0D` | Primary background, text, dominant fill |
| Charcoal | `#1A1A1A` | Secondary backgrounds, card surfaces, layered panels |
| Dark Slate | `#2A2A2A` | Tertiary background, subtle contrast against black |
| Hot Pink | `#FF1493` | Primary accent -- headlines, highlights, icons, borders |
| Neon Pink | `#FF69B4` | Lighter pink variant for gradients and hover states |
| Blush Pink | `#FF85B3` | Soft pink for secondary text accents and glows |
| Pure White | `#FFFFFF` | Checkerboard squares, stark text on black, highlight sparkles |
| Off-White | `#F0E6EF` | Body text on dark backgrounds, slightly warm/pink cast |
| Punk Red | `#CC0000` | Aggressive accent, broken heart motifs, danger elements |
| Neon Green | `#39FF14` | Hair-streak accent, occasional punk energy pop |
| Electric Purple | `#9B30FF` | Alternative accent for variety, scene-kid reference |
| Silver Glitter | `#C0C0C0` | Metallic text, sparkle effects, stud details |
| Notebook Blue | `#6699CC` | Ruled-line accent from composition notebook motif |
| Plaid Red | `#CC3333` | Tartan pattern accent, flannel/plaid references |

### Suggested CSS Custom Properties

```css
:root {
  /* Backgrounds */
  --tp-black: #0d0d0d;
  --tp-charcoal: #1a1a1a;
  --tp-slate: #2a2a2a;

  /* Pink spectrum */
  --tp-hot-pink: #ff1493;
  --tp-neon-pink: #ff69b4;
  --tp-blush: #ff85b3;

  /* Neutrals */
  --tp-white: #ffffff;
  --tp-off-white: #f0e6ef;
  --tp-silver: #c0c0c0;

  /* Accent colors */
  --tp-red: #cc0000;
  --tp-neon-green: #39ff14;
  --tp-purple: #9b30ff;
  --tp-notebook-blue: #6699cc;
  --tp-plaid-red: #cc3333;

  /* Functional mappings */
  --tp-bg-primary: var(--tp-black);
  --tp-bg-surface: var(--tp-charcoal);
  --tp-bg-elevated: var(--tp-slate);
  --tp-text-primary: var(--tp-off-white);
  --tp-text-heading: var(--tp-hot-pink);
  --tp-text-muted: var(--tp-silver);
  --tp-accent: var(--tp-hot-pink);
  --tp-accent-secondary: var(--tp-neon-pink);
  --tp-border: var(--tp-hot-pink);
  --tp-glow: rgba(255, 20, 147, 0.4);
}
```

### Palette Approaches

- **Black-and-pink dominance** -- the overwhelming majority of the design should be black and hot pink; this is the Teenpunk DNA and must not be diluted
- **White as structural contrast** -- pure white appears in checkerboard patterns, skull fills, star outlines, and stark text; it is a functional neutral, not a background
- **One neon accent for variety** -- neon green or electric purple can appear sparingly for energy pops (referencing dyed hair streaks) but must never compete with hot pink
- **No pastels, no earth tones** -- the palette is aggressively artificial and commercial; muted or natural colors break the spell
- **Glitter metallic shimmer** -- silver and white sparkle effects reference rhinestones, glitter graphics, and the MySpace digital culture
- **Pink glow effects** -- hot pink box-shadows and text-shadows create the neon-sign glow that elevates flat elements into the Teenpunk dimension

---

## Typography

### Typeface Characteristics

Teenpunk typography is bold, angular, and slightly distressed -- it looks like band merchandise lettering and notebook scrawl:

- **Chunky, angular display type** -- bold, condensed, slightly distressed letterforms suggesting band logos and concert poster headings
- **Hand-drawn marker text** -- casual, energetic handwriting as if scrawled on a notebook cover or locker door
- **Stencil and block letters** -- military-style stencil type referencing punk flyer culture, often with rough edges
- **Mix of uppercase aggression and lowercase casualness** -- headlines scream in caps; body text is relaxed and conversational
- **Slight distressing / roughness** -- letterforms with subtle wear, ink splatter, or torn edges rather than clean vector precision
- **Star and heart dingbats** -- decorative characters (stars, hearts, skulls) integrated into text as separators and bullet points
- **Pink-on-black color treatment** -- display type in hot pink or white on black is the default; reversed (black on pink) for accent panels

### Recommended Web Fonts (Google Fonts)

| Font | Style | Usage |
|------|-------|-------|
| **Permanent Marker** | Bold hand-drawn marker | Hero headlines, bold statements, notebook scrawl |
| **Bangers** | Comic/pop bold | Section headings, callouts, energetic display text |
| **Rock Salt** | Rough handwritten | Annotations, personal asides, doodle-style labels |
| **Bungee** | Bold block display | Stencil-style headings, band-logo-adjacent display |
| **Londrina Solid** | Hand-drawn bold | Friendly punk headings, casual emphasis |
| **Cabin Sketch** | Sketchy hand-drawn | Notebook doodle headings, illustrated feel |
| **Staatliches** | Condensed block display | Stencil headings, poster-style text |
| **Nunito** | Rounded sans-serif | Body text -- readable, friendly, slightly rounded |
| **Quicksand** | Rounded geometric sans | Alternative body text, softer youth-friendly reading |
| **Patrick Hand** | Clean handwritten | Body text alternative with hand-lettered character |

### Typography CSS Example

```css
/* Import Teenpunk-appropriate Google Fonts */
@import url('https://fonts.googleapis.com/css2?family=Permanent+Marker&family=Bangers&family=Rock+Salt&family=Bungee&family=Londrina+Solid&family=Cabin+Sketch:wght@700&family=Nunito:wght@400;700&family=Patrick+Hand&display=swap');

/* Hero / Display -- aggressive marker scrawl */
h1 {
  font-family: 'Permanent Marker', 'Bangers', cursive;
  font-size: clamp(2.5rem, 8vw, 6rem);
  letter-spacing: 0.02em;
  line-height: 1.0;
  color: var(--tp-hot-pink);
  text-transform: uppercase;
  text-shadow:
    2px 2px 0 rgba(0, 0, 0, 0.8),
    0 0 20px rgba(255, 20, 147, 0.4),
    0 0 40px rgba(255, 20, 147, 0.2);
}

/* Section headings -- bold block style */
h2 {
  font-family: 'Bangers', 'Bungee', Impact, sans-serif;
  font-size: clamp(1.5rem, 4vw, 3rem);
  letter-spacing: 0.06em;
  text-transform: uppercase;
  color: var(--tp-white);
  text-shadow:
    2px 2px 0 var(--tp-hot-pink),
    4px 4px 0 rgba(0, 0, 0, 0.5);
}

/* Subheadings -- handwritten notebook scrawl */
h3 {
  font-family: 'Rock Salt', 'Permanent Marker', cursive;
  font-size: clamp(1rem, 2.5vw, 1.5rem);
  color: var(--tp-neon-pink);
  transform: rotate(-1deg);
  margin-left: -0.3rem;
}

/* Body text -- friendly rounded sans */
body {
  font-family: 'Nunito', 'Quicksand', sans-serif;
  font-weight: 400;
  font-size: 1rem;
  line-height: 1.7;
  color: var(--tp-text-primary);
}

/* Doodle / annotation text */
.tp-doodle {
  font-family: 'Patrick Hand', 'Rock Salt', cursive;
  font-size: 0.85rem;
  color: var(--tp-neon-pink);
  transform: rotate(-2deg);
  display: inline-block;
}

/* Sticker label text */
.tp-label {
  font-family: 'Bangers', cursive;
  font-size: 0.9rem;
  text-transform: uppercase;
  letter-spacing: 0.1em;
  color: var(--tp-black);
}
```

---

## Layout Principles

### Grid and Structure

- **Dark, immersive backdrop** -- the page should feel like a decorated locker interior or a blacked-out bedroom wall covered in posters and stickers
- **Sticker-bomb layering** -- elements overlap, stack, and crowd like stickers, patches, and cutouts plastered across a surface
- **Slight rotations on most elements** -- cards, images, and accent elements should tilt 1--3 degrees in alternating directions for a hand-placed, scrapbook feel
- **Moderate structure with chaotic decoration** -- maintain readable content flow (unlike pure punk chaos) but decorate aggressively around and between content blocks
- **Full-bleed dark backgrounds** -- sections extend edge-to-edge in dark tones; content areas sit within as lighter or accented panels
- **Generous use of decorative borders** -- checkerboard strips, studded lines, star-scattered dividers between sections
- **Asymmetric accent placement** -- decorative skulls, stars, and splatters placed off-center and at angles, breaking formal symmetry
- **Notebook-page containers** -- content cards that look like torn-out notebook pages pinned or taped to the dark background

### Section Organization

- Use **checkerboard strip dividers** between major sections -- horizontal bands of alternating black-and-white squares
- Apply **pink glow borders** around featured content panels for neon-sign emphasis
- Create **hierarchy through the pink spectrum** -- primary content in hot pink, secondary in neon pink, tertiary in blush or white
- Employ **sticker-style elements** -- badges, tags, and labels that look like puffy stickers or iron-on patches
- Use **scattered star and heart decorations** in section gutters and margins
- Apply **splatter accents** at section transitions -- paint-splash shapes in pink or white breaking out of containers
- Frame key content in **notebook-paper styled panels** with ruled lines and margin marks

---

## CSS/Design Techniques

### Checkerboard Pattern

```css
/* Classic Teenpunk checkerboard background */
.tp-checkerboard {
  background-image:
    linear-gradient(45deg, var(--tp-black) 25%, transparent 25%),
    linear-gradient(-45deg, var(--tp-black) 25%, transparent 25%),
    linear-gradient(45deg, transparent 75%, var(--tp-black) 75%),
    linear-gradient(-45deg, transparent 75%, var(--tp-black) 75%);
  background-size: 20px 20px;
  background-position: 0 0, 0 10px, 10px -10px, -10px 0;
  background-color: var(--tp-white);
}

/* Smaller check for borders and accent strips */
.tp-checkerboard-sm {
  background-image:
    linear-gradient(45deg, var(--tp-black) 25%, transparent 25%),
    linear-gradient(-45deg, var(--tp-black) 25%, transparent 25%),
    linear-gradient(45deg, transparent 75%, var(--tp-black) 75%),
    linear-gradient(-45deg, transparent 75%, var(--tp-black) 75%);
  background-size: 12px 12px;
  background-position: 0 0, 0 6px, 6px -6px, -6px 0;
  background-color: var(--tp-white);
}

/* Checkerboard strip divider */
.tp-check-divider {
  height: 16px;
  border: none;
  margin: 2rem 0;
}
```

### Skull with Bow Decorative Element

```css
/* Skull-and-crossbones with a feminine twist (using pseudo-elements) */
.tp-skull-icon {
  position: relative;
  display: inline-block;
  font-size: 2rem;
  color: var(--tp-white);
  text-shadow: 0 0 10px rgba(255, 20, 147, 0.5);
}

.tp-skull-icon::before {
  content: '\2620'; /* skull and crossbones unicode */
  display: block;
}

/* Bow on top of the skull (CSS triangle ribbon) */
.tp-skull-icon::after {
  content: '\2764'; /* heart as stand-in for bow */
  position: absolute;
  top: -8px;
  right: -6px;
  font-size: 0.6em;
  color: var(--tp-hot-pink);
  text-shadow: none;
}
```

### Paint Splatter Effect

```css
/* Paint splatter background decoration */
.tp-splatter {
  position: relative;
}

.tp-splatter::before {
  content: '';
  position: absolute;
  top: -20px;
  right: -15px;
  width: 80px;
  height: 80px;
  border-radius: 60% 40% 55% 45% / 50% 60% 40% 50%;
  background: var(--tp-hot-pink);
  opacity: 0.15;
  transform: rotate(-15deg);
  pointer-events: none;
  z-index: 0;
}

.tp-splatter::after {
  content: '';
  position: absolute;
  bottom: -10px;
  left: 10%;
  width: 40px;
  height: 40px;
  border-radius: 50% 40% 60% 45% / 55% 45% 50% 50%;
  background: var(--tp-neon-pink);
  opacity: 0.12;
  transform: rotate(20deg);
  pointer-events: none;
  z-index: 0;
}
```

### Fishnet Overlay Texture

```css
/* Fishnet stocking pattern overlay */
.tp-fishnet {
  position: relative;
}

.tp-fishnet::after {
  content: '';
  position: absolute;
  inset: 0;
  background-image:
    linear-gradient(45deg, transparent 46%, rgba(255, 20, 147, 0.08) 46%, rgba(255, 20, 147, 0.08) 54%, transparent 54%),
    linear-gradient(-45deg, transparent 46%, rgba(255, 20, 147, 0.08) 46%, rgba(255, 20, 147, 0.08) 54%, transparent 54%);
  background-size: 16px 16px;
  pointer-events: none;
}
```

### Notebook Paper Panel

```css
/* Torn-out notebook page panel */
.tp-notebook {
  background: var(--tp-white);
  color: var(--tp-black);
  padding: 2rem 2rem 2rem 3.5rem;
  position: relative;
  transform: rotate(calc(var(--tilt, -1) * 1deg));
  box-shadow:
    3px 3px 10px rgba(0, 0, 0, 0.5),
    0 0 0 1px rgba(0, 0, 0, 0.05);
}

/* Ruled lines */
.tp-notebook::before {
  content: '';
  position: absolute;
  inset: 1.5rem 1rem 1rem 1rem;
  background-image:
    repeating-linear-gradient(
      transparent,
      transparent 27px,
      #B8D4E8 27px,
      #B8D4E8 28px
    );
  pointer-events: none;
}

/* Red margin line */
.tp-notebook::after {
  content: '';
  position: absolute;
  top: 1rem;
  bottom: 1rem;
  left: 3rem;
  width: 2px;
  background: #CC4444;
  opacity: 0.5;
}
```

### Sticker Badge Element

```css
/* Puffy sticker / badge element */
.tp-sticker {
  display: inline-block;
  padding: 0.5rem 1.3rem;
  font-family: 'Bangers', cursive;
  font-size: 1rem;
  text-transform: uppercase;
  letter-spacing: 0.06em;
  color: var(--tp-white);
  background: var(--tp-hot-pink);
  border: 2px solid var(--tp-white);
  border-radius: 4px;
  transform: rotate(var(--sticker-tilt, 2deg));
  box-shadow:
    2px 2px 0 rgba(0, 0, 0, 0.4),
    0 0 12px rgba(255, 20, 147, 0.3);
  position: relative;
}

/* Alternate sticker style -- black with pink border */
.tp-sticker--dark {
  background: var(--tp-black);
  color: var(--tp-hot-pink);
  border-color: var(--tp-hot-pink);
}
```

### Pink Neon Glow Border

```css
/* Neon-sign-style pink glow on panels */
.tp-glow-panel {
  border: 2px solid var(--tp-hot-pink);
  background: var(--tp-charcoal);
  padding: 2rem;
  box-shadow:
    0 0 5px var(--tp-hot-pink),
    0 0 15px rgba(255, 20, 147, 0.3),
    inset 0 0 20px rgba(255, 20, 147, 0.05);
  border-radius: 2px;
}
```

### Studded Border Divider

```css
/* Row of studs / rivets divider */
.tp-studs {
  border: none;
  height: 12px;
  position: relative;
  margin: 2rem 0;
}

.tp-studs::before {
  content: '';
  position: absolute;
  top: 4px;
  left: 5%;
  right: 5%;
  height: 4px;
  background: repeating-linear-gradient(
    90deg,
    var(--tp-silver) 0px,
    var(--tp-silver) 4px,
    transparent 4px,
    transparent 12px
  );
  border-radius: 2px;
}
```

### Star Scatter Decoration

```css
/* Decorative scattered stars */
.tp-stars {
  position: relative;
}

.tp-stars::before,
.tp-stars::after {
  position: absolute;
  font-size: 1.2rem;
  color: var(--tp-hot-pink);
  pointer-events: none;
  opacity: 0.6;
}

.tp-stars::before {
  content: '\2605 \2605 \2605'; /* filled stars */
  top: -15px;
  right: 10px;
  transform: rotate(8deg);
  letter-spacing: 6px;
  font-size: 0.8rem;
}

.tp-stars::after {
  content: '\2605 \2605';
  bottom: -12px;
  left: 20px;
  transform: rotate(-5deg);
  letter-spacing: 8px;
  font-size: 0.6rem;
}
```

### Teenpunk Button / CTA

```css
.tp-button {
  display: inline-block;
  padding: 0.7rem 2rem;
  font-family: 'Bangers', 'Permanent Marker', cursive;
  font-size: 1.1rem;
  letter-spacing: 0.08em;
  text-transform: uppercase;
  text-decoration: none;
  color: var(--tp-white);
  background: var(--tp-hot-pink);
  border: 2px solid var(--tp-white);
  cursor: pointer;
  position: relative;
  transform: rotate(-1deg);
  box-shadow:
    3px 3px 0 rgba(0, 0, 0, 0.5),
    0 0 15px rgba(255, 20, 147, 0.3);
  transition: all 0.15s ease;
}

.tp-button:hover {
  background: var(--tp-white);
  color: var(--tp-hot-pink);
  border-color: var(--tp-hot-pink);
  transform: rotate(1deg) scale(1.05);
  box-shadow:
    4px 4px 0 rgba(0, 0, 0, 0.5),
    0 0 25px rgba(255, 20, 147, 0.5);
}

.tp-button:active {
  transform: rotate(0deg) scale(0.98);
  box-shadow: 1px 1px 0 rgba(0, 0, 0, 0.5);
}

/* Black variant */
.tp-button--dark {
  background: var(--tp-black);
  border-color: var(--tp-hot-pink);
  color: var(--tp-hot-pink);
}

.tp-button--dark:hover {
  background: var(--tp-hot-pink);
  color: var(--tp-black);
}
```

### Glitter / Sparkle Overlay

```css
/* MySpace-era glitter sparkle effect */
@keyframes tp-sparkle {
  0%, 100% { opacity: 0; transform: scale(0.5) rotate(0deg); }
  50% { opacity: 1; transform: scale(1) rotate(180deg); }
}

.tp-glitter {
  position: relative;
}

.tp-glitter::before,
.tp-glitter::after {
  content: '\2726'; /* four-pointed star */
  position: absolute;
  color: var(--tp-white);
  font-size: 0.6rem;
  animation: tp-sparkle 2s ease-in-out infinite;
  pointer-events: none;
}

.tp-glitter::before {
  top: 5%;
  right: 8%;
  animation-delay: 0s;
}

.tp-glitter::after {
  bottom: 10%;
  left: 12%;
  animation-delay: 1s;
  font-size: 0.4rem;
}
```

### Plaid / Tartan Pattern

```css
/* Punk plaid pattern (pink-and-black tartan) */
.tp-plaid {
  background-color: var(--tp-black);
  background-image:
    repeating-linear-gradient(
      0deg,
      transparent,
      transparent 18px,
      rgba(255, 20, 147, 0.15) 18px,
      rgba(255, 20, 147, 0.15) 20px,
      transparent 20px,
      transparent 28px,
      rgba(255, 20, 147, 0.08) 28px,
      rgba(255, 20, 147, 0.08) 29px
    ),
    repeating-linear-gradient(
      90deg,
      transparent,
      transparent 18px,
      rgba(255, 20, 147, 0.15) 18px,
      rgba(255, 20, 147, 0.15) 20px,
      transparent 20px,
      transparent 28px,
      rgba(255, 20, 147, 0.08) 28px,
      rgba(255, 20, 147, 0.08) 29px
    );
}
```

---

## Animation and Motion

- **Sparkle twinkle** -- small star/diamond shapes that fade in, rotate, and fade out at staggered intervals, referencing MySpace glitter graphics
- **Gentle hover bounces** -- interactive elements that scale up slightly and rotate on hover, like picking up a sticker
- **Pink neon pulse** -- rhythmic brightening and dimming of pink glow borders and text shadows
- **Paint splatter pop-in** -- elements that appear with a quick scale-up animation from center, as if splatted onto the page
- **Skull bobble** -- decorative skull icons that nod/rotate subtly on loop

```css
/* Pink neon pulse on borders */
@keyframes tp-neon-pulse {
  0%, 100% {
    box-shadow:
      0 0 5px var(--tp-hot-pink),
      0 0 15px rgba(255, 20, 147, 0.3);
  }
  50% {
    box-shadow:
      0 0 10px var(--tp-hot-pink),
      0 0 30px rgba(255, 20, 147, 0.5),
      0 0 50px rgba(255, 20, 147, 0.2);
  }
}

.tp-pulse {
  animation: tp-neon-pulse 2.5s ease-in-out infinite;
}

/* Splatter pop-in entrance */
@keyframes tp-splat-in {
  0% { transform: scale(0) rotate(-20deg); opacity: 0; }
  70% { transform: scale(1.15) rotate(3deg); opacity: 1; }
  100% { transform: scale(1) rotate(0deg); opacity: 1; }
}

.tp-splat-enter {
  animation: tp-splat-in 0.4s ease-out forwards;
}
```

---

## Materials and Textures (Visual Metaphors for Web)

Physical Teenpunk materials and their web equivalents:

| Physical Material | Web Equivalent |
|-------------------|----------------|
| Fishnet stockings | Crossed diagonal `linear-gradient` lines at 45deg/-45deg with low-opacity pink |
| Checkerboard Vans | Alternating black-and-white square pattern via `linear-gradient` at 45deg |
| Studded belt / wristband | Repeating small circles or squares in silver along a dark border strip |
| Notebook paper | White background with `repeating-linear-gradient` ruled lines and a red margin line |
| Iron-on patches | Rounded-corner panels with thick borders and slight `rotate` transforms |
| Sticker sheet | Collection of `inline-block` elements with varied rotations, colored borders, and drop shadows |
| Punk plaid skirt | Tartan pattern via crossed `repeating-linear-gradient` in pink on black |
| Paint-splattered black tee | Dark background with irregular `border-radius` blobs in hot pink at low opacity |
| Glitter graphics | Small four-pointed star characters with `@keyframes` opacity/rotation animation |
| Band poster on wall | Cards with slight `rotate`, `box-shadow` depth, and rough-edge treatment |
| Safety pins | Small angled metallic-colored line segments used as decorative list markers |
| Neon hair streak | Thin gradient stripe in neon pink or green used as accent highlights |

---

## Cultural References and Influences

The following define the Teenpunk visual language and serve as design references:

- **Avril Lavigne** (2002--2010) -- the quintessential Teenpunk figurehead; her music videos, album art, and fashion line (Abbey Dawn) are the aesthetic's north star: black tank tops, neckties, checkered wristbands, pink streaks, and bratty pop-punk attitude
- **Hot Topic** (retail stores, peak 2000s) -- the mall retail epicenter of Teenpunk; the store's visual merchandising, product design, and brand identity *are* the aesthetic: skulls, checkers, pink-on-black everything
- **Monster High** (2010--2018) -- Mattel's fashion-doll franchise that crystallized Teenpunk motifs: characters like Draculaura embodied the skull-with-bow, pink-and-black palette, and girly-punk crossover
- **Freaky Friday** (2003) -- Lindsay Lohan's character (Tess's daughter) with her garage band, black-and-pink wardrobe, and rebellious-but-lovable energy
- **MySpace profile pages** (2005--2008) -- the social media platform where Teenpunk thrived digitally: custom CSS profiles with glitter graphics, sparkling cursors, embedded pop-punk playlists, and pink-on-black layouts
- **The Veronicas** -- Australian pop-punk duo whose visual identity exemplified the twin-punk-princess aesthetic
- **Claire's / Justice / Delia's** (retail) -- teen accessories and fashion retailers that mass-produced Teenpunk jewelry, bags, and room decor
- **Pop-punk music scene** -- bands like Paramore, My Chemical Romance (lighter fans), Fall Out Boy, and All Time Low whose merch and visual branding inhabited the Teenpunk space
- **Scene kid culture** (2006--2012) -- the MySpace-era youth subculture adjacent to and overlapping with Teenpunk, adding more extreme hair styling and digital photo editing
- **Olivia Rodrigo** (2020s) -- the modern revival/nostalgia wave, bringing Teenpunk motifs back through Y2K and pop-punk revival aesthetics

---

## Related Aesthetics

| Aesthetic | Relationship to Teenpunk |
|-----------|--------------------------|
| **Emo** | Overlapping 2000s youth subculture; shares the black base and emotional intensity but is more introspective and melancholy; Teenpunk is more extroverted and playful |
| **Scene** | Direct sibling aesthetic; Scene pushes Teenpunk's neon accents and hair styling to extremes; more digitally oriented with heavier MySpace/Photoshop editing |
| **Mallgoth** | Shares the Hot Topic retail origin and dark base palette; Mallgoth leans darker, more gothic, less pink, and less pop |
| **Punk / DIY Punk** | The authentic ancestor; Teenpunk borrows punk's visual vocabulary (skulls, safety pins, studs, plaid) but strips away the anti-commercial ideology |
| **Skater** | Parallel youth subculture; shares checkerboard Vans, casual attitude, and board-sports energy; Skater is more neutral-toned where Teenpunk is pink |
| **Glitter Graphics** | The digital arm of the same era; sparkle GIFs, animated MySpace layouts, and blingy text effects that decorated Teenpunk's online presence |
| **Tweencore** | The younger-skewing variant; same motifs but aimed at 8--12 year olds rather than teenagers; more wholesome, less edgy |
| **Pop-Punk** | The musical genre that provides Teenpunk's soundtrack; the band merch aesthetic feeds directly into the visual identity |
| **Vectordelia** | Shares the 2000s digital era and bold graphic style; more illustrative and psychedelic, but overlaps in the use of stars, hearts, and splatter effects |
| **Parisian Girly** | A softer, more feminine counterpart; shares the pink-and-black palette but replaces punk edge with French romantic elegance |

---

## Quick-Start: Minimal Teenpunk Page Template

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Teenpunk Page</title>
  <link href="https://fonts.googleapis.com/css2?family=Permanent+Marker&family=Bangers&family=Rock+Salt&family=Nunito:wght@400;700&family=Patrick+Hand&display=swap" rel="stylesheet">
  <style>
    :root {
      --tp-black: #0d0d0d;
      --tp-charcoal: #1a1a1a;
      --tp-slate: #2a2a2a;
      --tp-hot-pink: #ff1493;
      --tp-neon-pink: #ff69b4;
      --tp-blush: #ff85b3;
      --tp-white: #ffffff;
      --tp-off-white: #f0e6ef;
      --tp-silver: #c0c0c0;
      --tp-red: #cc0000;
      --tp-neon-green: #39ff14;
    }

    * { margin: 0; padding: 0; box-sizing: border-box; }

    body {
      background: var(--tp-black);
      color: var(--tp-off-white);
      font-family: 'Nunito', sans-serif;
      font-weight: 400;
      line-height: 1.7;
      position: relative;
      overflow-x: hidden;
    }

    /* Fishnet overlay on entire page */
    body::before {
      content: '';
      position: fixed;
      inset: 0;
      background-image:
        linear-gradient(45deg, transparent 46%, rgba(255, 20, 147, 0.03) 46%, rgba(255, 20, 147, 0.03) 54%, transparent 54%),
        linear-gradient(-45deg, transparent 46%, rgba(255, 20, 147, 0.03) 46%, rgba(255, 20, 147, 0.03) 54%, transparent 54%);
      background-size: 20px 20px;
      pointer-events: none;
      z-index: 9999;
    }

    .hero {
      text-align: center;
      padding: 6rem 2rem 4rem;
      position: relative;
      background:
        radial-gradient(ellipse at 30% 50%, rgba(255, 20, 147, 0.08) 0%, transparent 50%),
        radial-gradient(ellipse at 70% 30%, rgba(255, 105, 180, 0.05) 0%, transparent 40%);
    }

    .hero h1 {
      font-family: 'Permanent Marker', cursive;
      font-size: clamp(3rem, 10vw, 7rem);
      line-height: 1.0;
      text-transform: uppercase;
      color: var(--tp-hot-pink);
      text-shadow:
        3px 3px 0 rgba(0, 0, 0, 0.8),
        0 0 30px rgba(255, 20, 147, 0.4),
        0 0 60px rgba(255, 20, 147, 0.2);
      margin-bottom: 1rem;
    }

    .hero .subtitle {
      font-family: 'Rock Salt', cursive;
      font-size: 0.85rem;
      color: var(--tp-neon-pink);
      transform: rotate(-2deg);
      display: inline-block;
    }

    /* Checkerboard strip divider */
    .tp-check-divider {
      height: 16px;
      border: none;
      margin: 0;
      background-image:
        linear-gradient(45deg, var(--tp-black) 25%, transparent 25%),
        linear-gradient(-45deg, var(--tp-black) 25%, transparent 25%),
        linear-gradient(45deg, transparent 75%, var(--tp-black) 75%),
        linear-gradient(-45deg, transparent 75%, var(--tp-black) 75%);
      background-size: 16px 16px;
      background-position: 0 0, 0 8px, 8px -8px, -8px 0;
      background-color: var(--tp-white);
    }

    section {
      max-width: 800px;
      margin: 0 auto;
      padding: 3rem 2rem;
      position: relative;
    }

    h2 {
      font-family: 'Bangers', cursive;
      font-size: clamp(1.8rem, 5vw, 3rem);
      text-transform: uppercase;
      letter-spacing: 0.06em;
      color: var(--tp-white);
      text-shadow:
        2px 2px 0 var(--tp-hot-pink),
        4px 4px 0 rgba(0, 0, 0, 0.5);
      margin-bottom: 1.5rem;
    }

    h3 {
      font-family: 'Rock Salt', cursive;
      font-size: 1.1rem;
      color: var(--tp-neon-pink);
      transform: rotate(-1deg);
      margin: 1.5rem 0 0.75rem;
    }

    /* Notebook page card */
    .tp-notebook-card {
      background: var(--tp-white);
      color: var(--tp-black);
      padding: 2rem 2rem 2rem 3.5rem;
      position: relative;
      transform: rotate(calc(var(--tilt, -1) * 1deg));
      box-shadow:
        3px 3px 12px rgba(0, 0, 0, 0.6),
        0 0 0 1px rgba(0, 0, 0, 0.1);
      margin: 1.5rem 0;
      font-family: 'Patrick Hand', cursive;
      font-size: 1.05rem;
      line-height: 1.8;
    }

    /* Ruled lines on notebook card */
    .tp-notebook-card::before {
      content: '';
      position: absolute;
      inset: 1.5rem 1rem 1rem 1rem;
      background-image: repeating-linear-gradient(
        transparent, transparent 27px, #B8D4E8 27px, #B8D4E8 28px
      );
      pointer-events: none;
    }

    /* Red margin line */
    .tp-notebook-card::after {
      content: '';
      position: absolute;
      top: 1rem;
      bottom: 1rem;
      left: 3rem;
      width: 2px;
      background: #CC4444;
      opacity: 0.4;
    }

    /* Glow panel */
    .tp-glow-panel {
      border: 2px solid var(--tp-hot-pink);
      background: var(--tp-charcoal);
      padding: 2rem;
      margin: 1.5rem 0;
      box-shadow:
        0 0 5px var(--tp-hot-pink),
        0 0 15px rgba(255, 20, 147, 0.3),
        inset 0 0 20px rgba(255, 20, 147, 0.05);
    }

    /* Sticker badge */
    .tp-sticker {
      display: inline-block;
      padding: 0.4rem 1.1rem;
      font-family: 'Bangers', cursive;
      font-size: 0.9rem;
      text-transform: uppercase;
      letter-spacing: 0.06em;
      color: var(--tp-white);
      background: var(--tp-hot-pink);
      border: 2px solid var(--tp-white);
      border-radius: 3px;
      transform: rotate(2deg);
      box-shadow:
        2px 2px 0 rgba(0, 0, 0, 0.4),
        0 0 10px rgba(255, 20, 147, 0.3);
    }

    /* Annotation / doodle */
    .tp-doodle {
      font-family: 'Rock Salt', cursive;
      font-size: 0.7rem;
      color: var(--tp-neon-pink);
      transform: rotate(-3deg);
      display: inline-block;
      margin-left: 0.5rem;
    }

    /* Button */
    .tp-button {
      display: inline-block;
      padding: 0.7rem 2rem;
      font-family: 'Bangers', cursive;
      font-size: 1.1rem;
      letter-spacing: 0.08em;
      text-transform: uppercase;
      text-decoration: none;
      color: var(--tp-white);
      background: var(--tp-hot-pink);
      border: 2px solid var(--tp-white);
      cursor: pointer;
      transform: rotate(-1deg);
      box-shadow:
        3px 3px 0 rgba(0, 0, 0, 0.5),
        0 0 15px rgba(255, 20, 147, 0.3);
      transition: all 0.15s ease;
    }

    .tp-button:hover {
      background: var(--tp-white);
      color: var(--tp-hot-pink);
      border-color: var(--tp-hot-pink);
      transform: rotate(1deg) scale(1.05);
      box-shadow:
        4px 4px 0 rgba(0, 0, 0, 0.5),
        0 0 25px rgba(255, 20, 147, 0.5);
    }

    a {
      color: var(--tp-hot-pink);
      text-decoration: none;
      border-bottom: 2px solid rgba(255, 20, 147, 0.4);
      transition: all 0.15s;
    }

    a:hover {
      color: var(--tp-neon-pink);
      border-bottom-color: var(--tp-neon-pink);
      text-shadow: 0 0 8px rgba(255, 20, 147, 0.4);
    }

    /* Decorative star scatter */
    .star-scatter::before {
      content: '\2605 \2605 \2605';
      position: absolute;
      top: -10px;
      right: 15px;
      font-size: 0.7rem;
      color: var(--tp-hot-pink);
      letter-spacing: 5px;
      transform: rotate(5deg);
      opacity: 0.5;
    }
  </style>
</head>
<body>
  <div class="hero">
    <h1>Title Here</h1>
    <span class="subtitle">a punk princess production</span>
  </div>
  <hr class="tp-check-divider">
  <section>
    <h2>Section One</h2>
    <div class="tp-notebook-card" style="--tilt: -1.5">
      <p>Content styled with the Teenpunk aesthetic. Bold pink on black, notebook scrawl, and mall-punk attitude. <span class="tp-doodle">^ so punk!</span></p>
    </div>
    <div class="tp-glow-panel">
      <p>A glowing panel with neon pink borders. <span class="tp-sticker">Hot Topic Approved</span></p>
    </div>
    <br>
    <a href="#" class="tp-button">Let's Go</a>
  </section>
</body>
</html>
```
