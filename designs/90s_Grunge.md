# 90s Grunge Design Reference

90s Grunge is the raw, anti-establishment visual aesthetic born from the Seattle alternative music scene of the early-to-mid 1990s. Rooted in the flannel-wearing, thrift-store culture of bands like Nirvana, Pearl Jam, Soundgarden, and Alice in Chains, it translates the movement's rejection of mainstream polish into a design language defined by **distressed textures, hand-scrawled typography, dark muted earth tones, photocopy artifacts, and deliberate imperfection**. Influenced heavily by David Carson's deconstructed layouts in *Ray Gun* magazine and the wider zine culture of the era, 90s Grunge treats design as emotional expression rather than clean communication. In web and UI design, this aesthetic manifests through noise/grain overlays, torn paper edges, collage-style layouts, irregular typography, and a pervasive sense that the interface was assembled by hand with scissors, glue, and a broken photocopier. Unlike its descendant **Corporate Grunge** -- which adopted grunge textures within rigid corporate layouts -- authentic 90s Grunge is genuinely chaotic, rejecting the grid entirely in favor of raw visual energy and analog authenticity.

---

## Visual Characteristics

### Core Design Traits

- **Distressed and torn textures** -- ripped paper, fraying fabric, crumpled surfaces, and worn-out materials that look physically handled and degraded
- **Xerox/photocopy artifacts** -- high-contrast black-and-white imagery with toner bleed, registration errors, white speckle, and crushed midtones from repeated photocopying
- **Film grain and noise** -- heavy granular noise overlays on backgrounds and images, simulating analog film stock or lo-fi photography
- **Hand-scrawled typography** -- handwritten text, marker lettering, scratchy ink, and typewriter output that rejects digital precision
- **Flannel and plaid patterns** -- the signature textile of grunge fashion, translated into background textures and decorative elements
- **Collage and layered compositions** -- overlapping images, text, and textures piled on top of each other like a physical cut-and-paste assembly
- **Ink splatter and paint drips** -- accidental-looking marks, smudges, coffee stains, and spray-paint overspray suggesting chaotic analog production
- **Dark, moody atmosphere** -- heavy shadows, low-key lighting references, and an overall sense of brooding introspection
- **Halftone dot patterns** -- coarse, visible dot screens from cheap printing and photocopying processes
- **Faded and washed-out imagery** -- desaturated photographs with crushed blacks and blown highlights, as if left in the sun or run through a copier too many times

### Design Principles

- **Authentic imperfection** -- nothing should look digitally perfect; every element should feel touched by human hands, weather, or a malfunctioning machine
- **Emotion over legibility** -- the visceral feeling of the design matters more than clean information delivery; typography can be challenging to read if it serves the mood
- **Anti-grid chaos** -- reject structured layouts in favor of organic, collage-like arrangements where elements overlap, tilt, and fight for space
- **Analog warmth** -- the design should feel physically produced -- photocopied, screen-printed, wheat-pasted, or scrawled in a notebook -- never sterile or digital
- **Muted restraint** -- despite the chaos, the color palette is subdued and earthy; grunge is dark and introspective, not loud and neon
- **Layered depth** -- build visual richness through multiple texture layers (background grain, midground content, foreground noise and artifacts)
- **DIY accessibility** -- the design should look like anyone with basic tools could recreate it; professional polish is actively avoided

---

## Color Palette

| Swatch Name | Hex | Role / Usage |
|-------------|-----|-------------|
| Soot Black | `#0D0D0D` | Deep backgrounds, maximum contrast elements |
| Charcoal | `#1E1E1E` | Primary background, section fills |
| Dark Olive | `#3B3F2B` | Accent background, nature-inspired depth |
| Flannel Green | `#556B2F` | Primary cool accent, earthy green tones |
| Faded Olive | `#6B7B4A` | Secondary cool accent, muted green highlights |
| Rust | `#A0522D` | Primary warm accent, links, emphasis |
| Burnt Mustard | `#B8860B` | Secondary warm accent, headings, callouts |
| Dried Blood | `#6B1010` | Strong emphasis, danger states, intense accent |
| Concrete Gray | `#4A4846` | Borders, dividers, muted UI structure |
| Smoke | `#7A7672` | Body text on dark, captions, metadata |
| Worn Denim | `#4B5D6E` | Cool neutral accent, alternative interactive state |
| Aged Paper | `#D4C9A8` | Primary text on dark, warm off-white |
| Dirty White | `#E5DFD3` | High-emphasis text, hero titles on dark |
| Coffee Stain | `#8B6F4E` | Decorative accent, mid-tone warm neutral |
| Faded Purple | `#5C4A6B` | Rare accent, album-art inspired secondary |

### CSS Custom Properties

```css
:root {
  /* Base tones */
  --grunge-soot: #0d0d0d;
  --grunge-charcoal: #1e1e1e;
  --grunge-concrete: #4a4846;
  --grunge-smoke: #7a7672;

  /* Earthy greens */
  --grunge-dark-olive: #3b3f2b;
  --grunge-flannel: #556b2f;
  --grunge-faded-olive: #6b7b4a;

  /* Warm accents */
  --grunge-rust: #a0522d;
  --grunge-mustard: #b8860b;
  --grunge-blood: #6b1010;
  --grunge-coffee: #8b6f4e;

  /* Cool accents */
  --grunge-denim: #4b5d6e;
  --grunge-faded-purple: #5c4a6b;

  /* Light tones */
  --grunge-paper: #d4c9a8;
  --grunge-white: #e5dfd3;

  /* Functional mappings */
  --grunge-bg-primary: var(--grunge-charcoal);
  --grunge-bg-secondary: var(--grunge-dark-olive);
  --grunge-bg-surface: var(--grunge-concrete);
  --grunge-text-primary: var(--grunge-white);
  --grunge-text-secondary: var(--grunge-paper);
  --grunge-text-muted: var(--grunge-smoke);
  --grunge-accent-warm: var(--grunge-rust);
  --grunge-accent-cool: var(--grunge-flannel);
  --grunge-accent-highlight: var(--grunge-mustard);
  --grunge-border: var(--grunge-concrete);
}
```

---

## Typography

### Recommended Google Fonts

| Font | Style | Usage |
|------|-------|-------|
| **Permanent Marker** | Bold hand-drawn marker | Hero headlines, section titles, scrawled emphasis |
| **Rock Salt** | Rough handwritten scrawl | Subheadings, annotations, handwritten asides |
| **Special Elite** | Distressed typewriter | Display text, analog-feeling body headings |
| **Courier Prime** | Clean typewriter monospace | Body text, long-form readable content |
| **Cutive Mono** | Vintage typewriter monospace | Secondary body text, metadata |
| **Rubik Dirt** | Bold with ink-pressed texture | Display headlines, poster-style titles |
| **Londrina Solid** | Hand-drawn bold sans | Friendly grunge headings, zine-style titles |
| **VT323** | Pixel / CRT screen | Technical elements, counters, retro-digital accents |
| **Share Tech Mono** | Technical monospace | Labels, tags, timestamps, small metadata |

### Font Pairing Suggestions

| Pairing | Headings | Body | Mood |
|---------|----------|------|------|
| **Zine Scrawl** | Permanent Marker | Courier Prime | Raw, aggressive, hand-lettered energy |
| **Typewriter Grunge** | Special Elite | Cutive Mono | Analog, lo-fi, mechanical imperfection |
| **Poster Wall** | Rubik Dirt | Share Tech Mono | Bold, inky, underground show flyer |
| **Notebook Pages** | Rock Salt | Courier Prime | Intimate, personal, journal-like |
| **Digital Decay** | Londrina Solid | VT323 | Hybrid analog-digital, alternative web |

### CSS Example

```css
/* Import grunge-appropriate Google Fonts */
@import url('https://fonts.googleapis.com/css2?family=Permanent+Marker&family=Rock+Salt&family=Special+Elite&family=Courier+Prime:wght@400;700&family=Cutive+Mono&family=Rubik+Dirt&family=Londrina+Solid&family=VT323&family=Share+Tech+Mono&display=swap');

/* Hero / Display -- aggressive marker scrawl */
h1 {
  font-family: 'Permanent Marker', 'Rock Salt', cursive;
  font-size: clamp(2.5rem, 7vw, 5.5rem);
  letter-spacing: -0.02em;
  line-height: 0.95;
  color: var(--grunge-white);
  text-transform: uppercase;
  transform: rotate(-1.5deg);
  text-shadow:
    3px 3px 0 rgba(0, 0, 0, 0.6),
    -1px -1px 0 rgba(0, 0, 0, 0.3);
}

/* Section headings -- handwritten with attitude */
h2 {
  font-family: 'Rock Salt', 'Permanent Marker', cursive;
  font-size: clamp(1.4rem, 3.5vw, 2.2rem);
  color: var(--grunge-mustard);
  text-transform: uppercase;
  letter-spacing: 0.02em;
  transform: rotate(-0.8deg);
  margin-bottom: 1rem;
}

/* Sub-headings -- distressed typewriter */
h3 {
  font-family: 'Special Elite', 'Courier New', monospace;
  font-size: 1.2rem;
  color: var(--grunge-paper);
  letter-spacing: 0.05em;
  text-transform: uppercase;
}

/* Body text -- readable typewriter */
body {
  font-family: 'Courier Prime', 'Cutive Mono', 'Courier New', monospace;
  font-weight: 400;
  font-size: 1rem;
  line-height: 1.75;
  color: var(--grunge-text-secondary);
}

/* Metadata, labels, tags */
.grunge-label {
  font-family: 'Share Tech Mono', 'VT323', monospace;
  font-size: 0.75rem;
  text-transform: uppercase;
  letter-spacing: 0.2em;
  color: var(--grunge-smoke);
}

/* Oversized display -- inky poster text */
.grunge-display {
  font-family: 'Rubik Dirt', 'Permanent Marker', cursive;
  font-size: clamp(3rem, 9vw, 8rem);
  color: var(--grunge-rust);
  text-shadow: 4px 4px 0 rgba(0, 0, 0, 0.5);
  line-height: 0.85;
}
```

---

## Layout Principles

- **Reject the grid** -- 90s Grunge layouts are organic and collage-based; elements are placed by instinct and visual tension rather than mathematical alignment
- **Layered, overlapping compositions** -- content panels, images, and text blocks pile on top of each other like flyers on a telephone pole or pages torn from a notebook
- **Asymmetric visual weight** -- heavy elements cluster unpredictably; nothing is perfectly centered unless ironically
- **Rotated and tilted elements** -- almost everything sits at a slight angle (1-4 degrees), as if physically pinned or taped to a surface
- **Torn and rough dividers** -- sections are separated by ripped paper edges, ink splatters, or rough painted lines rather than clean horizontal rules
- **Full-bleed textures** -- dark, noisy backgrounds extend edge-to-edge while readable content stays within a narrower column (650-800px)
- **Mixed media collage** -- combine photographic elements, hand-drawn marks, typed text, and textured backgrounds in a single composition
- **Visible construction** -- tape strips, staple marks, pin holes, and glue artifacts are decorative elements that celebrate the handmade process
- **Horror vacui meets brooding space** -- some areas are densely layered while others use dark, empty space for atmospheric weight
- **Vertical rhythm through roughness** -- instead of consistent spacing, let the natural irregularity of torn edges and tilted elements create organic rhythm

---

## CSS / Design Techniques

### Card Component

```css
/* Grunge card -- looks like a torn piece of paper pinned to a dark surface */
.grunge-card {
  background:
    /* Subtle paper texture grain */
    radial-gradient(circle at 30% 20%, rgba(180, 160, 120, 0.06) 0%, transparent 50%),
    var(--grunge-dark-olive);
  border: 1px solid rgba(160, 82, 45, 0.25);
  padding: 2rem;
  position: relative;
  overflow: hidden;
  transform: rotate(calc(var(--tilt, -0.8) * 1deg));
  box-shadow:
    4px 4px 0 rgba(0, 0, 0, 0.5),
    0 0 30px rgba(0, 0, 0, 0.3);
}

/* Tape strip holding the card */
.grunge-card::before {
  content: '';
  position: absolute;
  top: -6px;
  left: calc(40% + var(--tape-offset, 0px));
  width: 75px;
  height: 22px;
  background: rgba(212, 201, 168, 0.2);
  border: 1px solid rgba(212, 201, 168, 0.1);
  transform: rotate(calc(var(--tape-tilt, 2) * 1deg));
  z-index: 2;
}

/* Torn bottom edge */
.grunge-card::after {
  content: '';
  position: absolute;
  bottom: -1px;
  left: 0;
  right: 0;
  height: 12px;
  background: var(--grunge-dark-olive);
  clip-path: polygon(
    0% 0%, 4% 65%, 8% 20%, 12% 70%, 17% 30%, 22% 80%,
    27% 15%, 32% 60%, 37% 25%, 42% 75%, 48% 10%, 53% 55%,
    58% 35%, 63% 85%, 68% 20%, 73% 65%, 78% 40%, 83% 75%,
    88% 15%, 93% 60%, 98% 30%, 100% 50%, 100% 100%, 0% 100%
  );
}

/* Card title */
.grunge-card h3 {
  font-family: 'Permanent Marker', cursive;
  color: var(--grunge-mustard);
  margin-bottom: 0.75rem;
  transform: rotate(-0.5deg);
}

/* Card body text */
.grunge-card p {
  font-family: 'Courier Prime', monospace;
  color: var(--grunge-paper);
  line-height: 1.7;
  font-size: 0.95rem;
}
```

### Button Component

```css
/* Primary grunge button -- handmade, rough, confrontational */
.grunge-btn {
  display: inline-block;
  padding: 0.75rem 2rem;
  font-family: 'Permanent Marker', 'Special Elite', cursive;
  font-size: 1rem;
  letter-spacing: 0.06em;
  text-transform: uppercase;
  text-decoration: none;
  color: var(--grunge-white);
  background: var(--grunge-charcoal);
  border: 2px solid var(--grunge-rust);
  cursor: pointer;
  position: relative;
  transform: rotate(-1deg);
  transition: all 0.15s ease;
  box-shadow: 3px 3px 0 rgba(0, 0, 0, 0.5);
}

.grunge-btn:hover {
  background: var(--grunge-rust);
  color: var(--grunge-soot);
  transform: rotate(0.5deg) translate(-1px, -1px);
  box-shadow: 5px 5px 0 rgba(0, 0, 0, 0.6);
}

.grunge-btn:active {
  transform: rotate(0deg) translate(2px, 2px);
  box-shadow: 1px 1px 0 rgba(0, 0, 0, 0.4);
}

/* Ghost/outline variant */
.grunge-btn--ghost {
  background: transparent;
  border: 2px solid var(--grunge-smoke);
  color: var(--grunge-paper);
}

.grunge-btn--ghost:hover {
  border-color: var(--grunge-mustard);
  color: var(--grunge-mustard);
  background: rgba(184, 134, 11, 0.08);
}

/* Sticker variant -- looks like a peeling sticker on a guitar case */
.grunge-btn--sticker {
  background: var(--grunge-mustard);
  color: var(--grunge-soot);
  border: 2px solid var(--grunge-soot);
  transform: rotate(2deg);
}

.grunge-btn--sticker:hover {
  transform: rotate(-1deg) scale(1.05);
  box-shadow: 4px 4px 0 rgba(0, 0, 0, 0.5);
}
```

### Navigation Bar

```css
/* Grunge navigation -- scrawled, rough, anti-corporate */
.grunge-nav {
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 1rem 2rem;
  background: var(--grunge-soot);
  border-bottom: 3px solid var(--grunge-concrete);
  position: relative;
}

/* Noise texture on nav */
.grunge-nav::after {
  content: '';
  position: absolute;
  inset: 0;
  opacity: 0.05;
  background-image: url("data:image/svg+xml,%3Csvg viewBox='0 0 256 256' xmlns='http://www.w3.org/2000/svg'%3E%3Cfilter id='n'%3E%3CfeTurbulence type='fractalNoise' baseFrequency='0.9' numOctaves='4' stitchTiles='stitch'/%3E%3C/filter%3E%3Crect width='100%25' height='100%25' filter='url(%23n)'/%3E%3C/svg%3E");
  background-size: 256px 256px;
  pointer-events: none;
  mix-blend-mode: overlay;
}

.grunge-nav__brand {
  font-family: 'Permanent Marker', cursive;
  font-size: 1.4rem;
  color: var(--grunge-white);
  text-decoration: none;
  transform: rotate(-1deg);
  letter-spacing: 0.03em;
}

.grunge-nav__links {
  display: flex;
  gap: 1.5rem;
  list-style: none;
  margin: 0;
  padding: 0;
}

.grunge-nav__link {
  font-family: 'Special Elite', monospace;
  font-size: 0.9rem;
  color: var(--grunge-smoke);
  text-decoration: none;
  text-transform: uppercase;
  letter-spacing: 0.1em;
  padding: 0.3rem 0;
  border-bottom: 2px solid transparent;
  transition: all 0.15s ease;
}

.grunge-nav__link:hover {
  color: var(--grunge-mustard);
  border-bottom-color: var(--grunge-mustard);
}

.grunge-nav__link--active {
  color: var(--grunge-rust);
  border-bottom-color: var(--grunge-rust);
}
```

### Hero Section

```css
/* Full-bleed grunge hero with layered textures */
.grunge-hero {
  position: relative;
  min-height: 80vh;
  display: flex;
  flex-direction: column;
  justify-content: center;
  padding: 4rem 2rem;
  background:
    /* Vignette */
    radial-gradient(ellipse at center, transparent 40%, rgba(13, 13, 13, 0.7) 100%),
    /* Warm light leak */
    radial-gradient(circle at 20% 80%, rgba(160, 82, 45, 0.08) 0%, transparent 50%),
    /* Cool shadow */
    radial-gradient(circle at 80% 20%, rgba(59, 63, 43, 0.1) 0%, transparent 40%),
    var(--grunge-soot);
  overflow: hidden;
}

/* Heavy noise grain overlay */
.grunge-hero::before {
  content: '';
  position: absolute;
  inset: 0;
  opacity: 0.1;
  background-image: url("data:image/svg+xml,%3Csvg viewBox='0 0 512 512' xmlns='http://www.w3.org/2000/svg'%3E%3Cfilter id='grain'%3E%3CfeTurbulence type='fractalNoise' baseFrequency='0.75' numOctaves='5' stitchTiles='stitch'/%3E%3C/filter%3E%3Crect width='100%25' height='100%25' filter='url(%23grain)'/%3E%3C/svg%3E");
  background-size: 512px 512px;
  pointer-events: none;
  mix-blend-mode: overlay;
  z-index: 1;
}

/* Diagonal scratch lines */
.grunge-hero::after {
  content: '';
  position: absolute;
  inset: 0;
  background:
    repeating-linear-gradient(
      -30deg,
      transparent,
      transparent 10px,
      rgba(255, 255, 255, 0.01) 10px,
      rgba(255, 255, 255, 0.01) 11px
    ),
    repeating-linear-gradient(
      40deg,
      transparent,
      transparent 14px,
      rgba(255, 255, 255, 0.008) 14px,
      rgba(255, 255, 255, 0.008) 15px
    );
  pointer-events: none;
  z-index: 1;
}

.grunge-hero__content {
  position: relative;
  z-index: 2;
  max-width: 800px;
}

.grunge-hero__title {
  font-family: 'Permanent Marker', cursive;
  font-size: clamp(3rem, 8vw, 6rem);
  line-height: 0.9;
  color: var(--grunge-white);
  text-transform: uppercase;
  transform: rotate(-2deg);
  margin-bottom: 1.5rem;
  text-shadow:
    4px 4px 0 rgba(0, 0, 0, 0.6),
    -2px -2px 0 rgba(0, 0, 0, 0.2);
}

.grunge-hero__subtitle {
  font-family: 'Special Elite', monospace;
  font-size: clamp(1rem, 2vw, 1.3rem);
  color: var(--grunge-smoke);
  letter-spacing: 0.15em;
  text-transform: uppercase;
  transform: rotate(0.5deg);
}
```

### Torn Paper Edge Divider

```css
/* Torn paper edge between sections */
.grunge-torn-edge {
  position: relative;
  padding-bottom: 2rem;
}

.grunge-torn-edge::after {
  content: '';
  position: absolute;
  bottom: -2px;
  left: 0;
  right: 0;
  height: 18px;
  background: var(--grunge-charcoal);
  clip-path: polygon(
    0% 0%, 2% 55%, 5% 15%, 8% 70%, 11% 25%, 14% 80%,
    18% 10%, 21% 60%, 24% 30%, 28% 85%, 31% 20%, 34% 65%,
    37% 5%, 40% 50%, 43% 75%, 46% 15%, 49% 60%, 52% 35%,
    55% 80%, 58% 10%, 61% 55%, 64% 25%, 67% 70%, 70% 40%,
    73% 90%, 76% 20%, 79% 60%, 82% 5%, 85% 45%, 88% 75%,
    91% 30%, 94% 65%, 97% 15%, 100% 50%,
    100% 100%, 0% 100%
  );
}

/* Inverse torn edge (dark to light) */
.grunge-torn-edge--inverse::after {
  background: var(--grunge-soot);
}
```

### Xerox / Photocopy Texture Effect

```css
/* Photocopy-degraded background treatment */
.grunge-xerox {
  position: relative;
  background: var(--grunge-charcoal);
}

/* Heavy photocopy grain */
.grunge-xerox::before {
  content: '';
  position: absolute;
  inset: 0;
  opacity: 0.07;
  background-image: url("data:image/svg+xml,%3Csvg viewBox='0 0 512 512' xmlns='http://www.w3.org/2000/svg'%3E%3Cfilter id='xerox'%3E%3CfeTurbulence type='fractalNoise' baseFrequency='0.85' numOctaves='6' stitchTiles='stitch'/%3E%3C/filter%3E%3Crect width='100%25' height='100%25' filter='url(%23xerox)'/%3E%3C/svg%3E");
  background-size: 512px 512px;
  pointer-events: none;
  mix-blend-mode: overlay;
}

/* Halftone dot overlay */
.grunge-xerox::after {
  content: '';
  position: absolute;
  inset: 0;
  background-image: radial-gradient(circle, rgba(0, 0, 0, 0.8) 0.8px, transparent 0.8px);
  background-size: 4px 4px;
  opacity: 0.04;
  mix-blend-mode: multiply;
  pointer-events: none;
}

/* Apply to images for photocopy look */
.grunge-xerox-img {
  filter: contrast(1.8) grayscale(1) brightness(1.15);
  mix-blend-mode: luminosity;
}

/* Extreme photocopy -- run through the copier 10 times */
.grunge-xerox-img--heavy {
  filter: contrast(2.8) grayscale(1) brightness(1.3);
  image-rendering: auto;
  opacity: 0.9;
}
```

### Flannel / Plaid Pattern

```css
/* CSS-only flannel plaid pattern for backgrounds and accents */
.grunge-flannel {
  background-color: #3b3f2b;
  background-image:
    /* Horizontal bands */
    repeating-linear-gradient(
      0deg,
      transparent,
      transparent 18px,
      rgba(160, 82, 45, 0.15) 18px,
      rgba(160, 82, 45, 0.15) 20px,
      transparent 20px,
      transparent 38px,
      rgba(160, 82, 45, 0.25) 38px,
      rgba(160, 82, 45, 0.25) 42px,
      transparent 42px,
      transparent 56px
    ),
    /* Vertical bands */
    repeating-linear-gradient(
      90deg,
      transparent,
      transparent 18px,
      rgba(85, 107, 47, 0.2) 18px,
      rgba(85, 107, 47, 0.2) 20px,
      transparent 20px,
      transparent 38px,
      rgba(85, 107, 47, 0.3) 38px,
      rgba(85, 107, 47, 0.3) 42px,
      transparent 42px,
      transparent 56px
    ),
    /* Thin accent lines */
    repeating-linear-gradient(
      0deg,
      transparent,
      transparent 27px,
      rgba(184, 134, 11, 0.1) 27px,
      rgba(184, 134, 11, 0.1) 29px,
      transparent 29px,
      transparent 56px
    ),
    repeating-linear-gradient(
      90deg,
      transparent,
      transparent 27px,
      rgba(184, 134, 11, 0.1) 27px,
      rgba(184, 134, 11, 0.1) 29px,
      transparent 29px,
      transparent 56px
    );
}

/* Flannel accent strip -- for borders, dividers, or decorative bands */
.grunge-flannel-strip {
  height: 8px;
  background: repeating-linear-gradient(
    90deg,
    var(--grunge-dark-olive) 0px,
    var(--grunge-dark-olive) 6px,
    var(--grunge-rust) 6px,
    var(--grunge-rust) 8px,
    var(--grunge-dark-olive) 8px,
    var(--grunge-dark-olive) 12px,
    var(--grunge-flannel) 12px,
    var(--grunge-flannel) 14px
  );
  opacity: 0.7;
}
```

### Zine-Style Collage Layout

```css
/* Zine-style collage container with scattered, overlapping elements */
.grunge-zine {
  position: relative;
  min-height: 500px;
  padding: 3rem 2rem;
  overflow: hidden;
}

/* Individual collage pieces */
.grunge-zine__piece {
  position: absolute;
  background: var(--grunge-paper);
  color: var(--grunge-soot);
  padding: 1.2rem;
  border: 1px solid rgba(0, 0, 0, 0.15);
  transform: rotate(calc(var(--r, 0) * 1deg));
  z-index: var(--z, 1);
  max-width: 280px;
  box-shadow:
    2px 2px 0 rgba(0, 0, 0, 0.2),
    0 0 15px rgba(0, 0, 0, 0.15);
  font-family: 'Courier Prime', monospace;
  font-size: 0.85rem;
  line-height: 1.6;
}

.grunge-zine__piece:nth-child(even) {
  background: var(--grunge-white);
}

/* Tape on collage pieces */
.grunge-zine__piece::before {
  content: '';
  position: absolute;
  top: -7px;
  right: 15%;
  width: 55px;
  height: 18px;
  background: rgba(212, 201, 168, 0.35);
  border: 1px solid rgba(212, 201, 168, 0.15);
  transform: rotate(calc(var(--tape-r, 4) * 1deg));
}

/* Headline piece -- bold, scrawled, attention-grabbing */
.grunge-zine__piece--headline {
  font-family: 'Permanent Marker', cursive;
  font-size: 1.5rem;
  text-transform: uppercase;
  background: var(--grunge-soot);
  color: var(--grunge-white);
  border: none;
  z-index: 10;
}

/* Photo piece -- xeroxed image placeholder */
.grunge-zine__piece--photo {
  padding: 0;
  filter: contrast(1.6) grayscale(1) brightness(1.1);
  border: 3px solid var(--grunge-soot);
}
```

### Ink Splatter Divider

```css
/* Ink splatter horizontal divider */
.grunge-splatter {
  border: none;
  height: 1px;
  background: var(--grunge-concrete);
  position: relative;
  margin: 3rem 0;
  opacity: 0.4;
}

/* Splatter dots along the divider */
.grunge-splatter::before {
  content: '';
  position: absolute;
  top: -5px;
  left: 15%;
  width: 10px;
  height: 10px;
  border-radius: 50%;
  background: var(--grunge-rust);
  box-shadow:
    25px 3px 0 3px var(--grunge-rust),
    55px -2px 0 1px var(--grunge-rust),
    90px 4px 0 2px var(--grunge-rust),
    140px -1px 0 4px var(--grunge-rust),
    200px 3px 0 1px var(--grunge-rust),
    260px -3px 0 2px var(--grunge-rust);
  opacity: 0.35;
}

/* Additional splatter layer */
.grunge-splatter::after {
  content: '';
  position: absolute;
  top: -3px;
  right: 20%;
  width: 6px;
  height: 6px;
  border-radius: 50%;
  background: var(--grunge-mustard);
  box-shadow:
    -30px 2px 0 1px var(--grunge-mustard),
    -70px -1px 0 2px var(--grunge-mustard),
    -120px 3px 0 1px var(--grunge-mustard);
  opacity: 0.25;
}
```

---

## Design Do's and Don'ts

### Do's

- **Do** use heavy noise/grain overlays on backgrounds and images to create analog texture
- **Do** tilt and rotate elements slightly (1-4 degrees) for a hand-placed, imperfect feel
- **Do** stick to dark, muted earth tones -- olive, rust, charcoal, mustard, and faded denim
- **Do** use typewriter and handwritten fonts for headings; pair with monospace for body text
- **Do** layer textures -- combine noise, scratches, halftone dots, and vignettes for depth
- **Do** reference physical materials -- torn paper, tape strips, coffee stains, Xerox artifacts
- **Do** let the design breathe with dark, moody negative space between chaotic sections
- **Do** use SVG filters (feTurbulence, feDisplacementMap) for realistic grain and distortion
- **Do** apply photocopy treatments to images: high contrast, grayscale, crushed midtones
- **Do** embrace asymmetry and deliberate misalignment in your layouts

### Don'ts

- **Don't** use bright, saturated, or neon colors -- grunge is muted, faded, and desaturated
- **Don't** center-align everything; grunge layouts are organic and asymmetric
- **Don't** use clean geometric shapes with perfect borders -- rough, irregular edges are essential
- **Don't** over-polish; if it looks too clean or too professional, it has lost the grunge spirit
- **Don't** confuse 90s Grunge with Corporate Grunge -- authentic grunge rejects the underlying grid structure that corporate grunge maintains
- **Don't** use smooth gradients or glossy effects -- everything should feel matte, rough, and physical
- **Don't** sacrifice all readability for style -- body text should still be legible even if headings are raw
- **Don't** use stock photography with clean lighting; images should be high-contrast, grainy, and lo-fi
- **Don't** mix in modern flat design or material design elements -- they are fundamentally incompatible
- **Don't** forget the analog origins -- every digital effect should reference a physical process (photocopying, screen-printing, hand-lettering)

---

## Related Aesthetics

| Aesthetic | Relationship to 90s Grunge |
|-----------|---------------------------|
| **Corporate Grunge** | Direct descendant; commercializes grunge textures within rigid corporate layouts, trading chaos for controlled edginess |
| **DIY Punk** | Ideological parent; shares the anti-establishment DIY ethos, cut-and-paste collage, and Xerox culture, but punk is more aggressive and explicitly political |
| **Industrial Gothic** | Shares dark palettes and gritty textures; Industrial adds heavier metallic and mechanical elements with a colder, more oppressive tone |
| **Brutalist Web Design** | Modern spiritual successor; both reject polish in favor of rawness, though Brutalism is more minimal while Grunge is more textured |
| **Dark Academia** | Overlaps in muted earth tones and moody atmosphere, but Dark Academia is scholarly and refined where Grunge is chaotic and anti-intellectual |
| **Early Cyber** | Contemporaneous aesthetic from the same 1990s era; Early Cyber embraces emerging digital technology while Grunge rejects it in favor of analog |
| **Cyberpunk** | Shares dark, dystopian undertones and anti-corporate sentiment, but Cyberpunk adds neon accents and sci-fi futurism |
| **Weirdcore** | Shares the distorted, lo-fi visual quality and embrace of imperfection, but Weirdcore leans surreal and dreamlike rather than moody and raw |
| **Liminal Space** | Both evoke feelings of unease and atmospheric tension through muted tones and emptiness, but through different visual strategies |
| **Terminal CLI Aesthetic** | Shares the monospace typography preference and anti-polish stance, but Terminal is clean and precise where Grunge is messy and organic |

---

## Quick-Start HTML Template

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>90s Grunge</title>
  <link href="https://fonts.googleapis.com/css2?family=Permanent+Marker&family=Rock+Salt&family=Special+Elite&family=Courier+Prime:wght@400;700&family=VT323&family=Share+Tech+Mono&display=swap" rel="stylesheet">
  <style>
    :root {
      --grunge-soot: #0d0d0d;
      --grunge-charcoal: #1e1e1e;
      --grunge-dark-olive: #3b3f2b;
      --grunge-flannel: #556b2f;
      --grunge-faded-olive: #6b7b4a;
      --grunge-rust: #a0522d;
      --grunge-mustard: #b8860b;
      --grunge-blood: #6b1010;
      --grunge-concrete: #4a4846;
      --grunge-smoke: #7a7672;
      --grunge-denim: #4b5d6e;
      --grunge-paper: #d4c9a8;
      --grunge-white: #e5dfd3;
      --grunge-coffee: #8b6f4e;
      --grunge-faded-purple: #5c4a6b;
    }

    * { margin: 0; padding: 0; box-sizing: border-box; }

    body {
      background: var(--grunge-charcoal);
      color: var(--grunge-paper);
      font-family: 'Courier Prime', 'Courier New', monospace;
      font-size: 1rem;
      line-height: 1.75;
      position: relative;
      overflow-x: hidden;
    }

    /* ---- Global noise grain overlay ---- */
    body::before {
      content: '';
      position: fixed;
      inset: 0;
      opacity: 0.07;
      background-image: url("data:image/svg+xml,%3Csvg viewBox='0 0 512 512' xmlns='http://www.w3.org/2000/svg'%3E%3Cfilter id='g'%3E%3CfeTurbulence type='fractalNoise' baseFrequency='0.8' numOctaves='5' stitchTiles='stitch'/%3E%3C/filter%3E%3Crect width='100%25' height='100%25' filter='url(%23g)'/%3E%3C/svg%3E");
      background-size: 512px 512px;
      pointer-events: none;
      mix-blend-mode: overlay;
      z-index: 9999;
    }

    /* ---- Navigation ---- */
    nav {
      display: flex;
      align-items: center;
      justify-content: space-between;
      padding: 1rem 2rem;
      background: var(--grunge-soot);
      border-bottom: 3px solid var(--grunge-concrete);
      position: relative;
      z-index: 100;
    }

    nav .brand {
      font-family: 'Permanent Marker', cursive;
      font-size: 1.3rem;
      color: var(--grunge-white);
      text-decoration: none;
      transform: rotate(-1deg);
      display: inline-block;
    }

    nav ul {
      display: flex;
      gap: 1.5rem;
      list-style: none;
    }

    nav a {
      font-family: 'Special Elite', monospace;
      font-size: 0.85rem;
      color: var(--grunge-smoke);
      text-decoration: none;
      text-transform: uppercase;
      letter-spacing: 0.1em;
      border-bottom: 2px solid transparent;
      padding-bottom: 0.2rem;
      transition: all 0.15s ease;
    }

    nav a:hover, nav a.active {
      color: var(--grunge-mustard);
      border-bottom-color: var(--grunge-mustard);
    }

    /* ---- Hero Section ---- */
    .hero {
      position: relative;
      min-height: 75vh;
      display: flex;
      flex-direction: column;
      justify-content: center;
      padding: 5rem 2rem;
      background:
        radial-gradient(ellipse at center, transparent 40%, rgba(13, 13, 13, 0.7) 100%),
        radial-gradient(circle at 15% 75%, rgba(160, 82, 45, 0.07) 0%, transparent 50%),
        radial-gradient(circle at 85% 25%, rgba(59, 63, 43, 0.09) 0%, transparent 40%),
        var(--grunge-soot);
      overflow: hidden;
    }

    /* Scratch overlay */
    .hero::after {
      content: '';
      position: absolute;
      inset: 0;
      background:
        repeating-linear-gradient(-30deg, transparent, transparent 11px, rgba(255,255,255,0.01) 11px, rgba(255,255,255,0.01) 12px),
        repeating-linear-gradient(35deg, transparent, transparent 15px, rgba(255,255,255,0.008) 15px, rgba(255,255,255,0.008) 16px);
      pointer-events: none;
    }

    .hero-content {
      max-width: 800px;
      position: relative;
      z-index: 2;
    }

    .hero h1 {
      font-family: 'Permanent Marker', cursive;
      font-size: clamp(3rem, 8vw, 6rem);
      line-height: 0.9;
      color: var(--grunge-white);
      text-transform: uppercase;
      transform: rotate(-2deg);
      margin-bottom: 1.5rem;
      text-shadow:
        4px 4px 0 rgba(0, 0, 0, 0.6),
        -2px -2px 0 rgba(0, 0, 0, 0.2);
    }

    .hero h1 em {
      color: var(--grunge-rust);
      font-style: normal;
    }

    .hero .tagline {
      font-family: 'Special Elite', monospace;
      font-size: clamp(0.9rem, 1.8vw, 1.2rem);
      color: var(--grunge-smoke);
      letter-spacing: 0.15em;
      text-transform: uppercase;
      transform: rotate(0.5deg);
      display: inline-block;
      margin-bottom: 2rem;
    }

    /* ---- Torn Edge Divider ---- */
    .torn-edge {
      height: 18px;
      background: var(--grunge-charcoal);
      clip-path: polygon(
        0% 0%, 2% 55%, 5% 15%, 8% 70%, 11% 25%, 14% 80%,
        18% 10%, 21% 60%, 24% 30%, 28% 85%, 31% 20%, 34% 65%,
        37% 5%, 40% 50%, 43% 75%, 46% 15%, 49% 60%, 52% 35%,
        55% 80%, 58% 10%, 61% 55%, 64% 25%, 67% 70%, 70% 40%,
        73% 90%, 76% 20%, 79% 60%, 82% 5%, 85% 45%, 88% 75%,
        91% 30%, 94% 65%, 97% 15%, 100% 50%,
        100% 100%, 0% 100%
      );
    }

    /* ---- Section Styles ---- */
    section {
      max-width: 800px;
      margin: 0 auto;
      padding: 4rem 2rem;
    }

    section h2 {
      font-family: 'Rock Salt', 'Permanent Marker', cursive;
      font-size: clamp(1.3rem, 3vw, 2rem);
      color: var(--grunge-mustard);
      text-transform: uppercase;
      transform: rotate(-0.8deg);
      margin-bottom: 1.5rem;
      letter-spacing: 0.02em;
    }

    section h3 {
      font-family: 'Special Elite', monospace;
      font-size: 1.1rem;
      color: var(--grunge-paper);
      text-transform: uppercase;
      letter-spacing: 0.08em;
      margin: 2rem 0 0.75rem;
    }

    /* ---- Grunge Cards ---- */
    .card-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
      gap: 2rem;
      margin: 2rem 0;
    }

    .card {
      background:
        radial-gradient(circle at 25% 25%, rgba(160, 82, 45, 0.04) 0%, transparent 50%),
        var(--grunge-dark-olive);
      border: 1px solid rgba(160, 82, 45, 0.2);
      padding: 1.8rem;
      position: relative;
      transform: rotate(calc(var(--tilt, -0.5) * 1deg));
      box-shadow:
        4px 4px 0 rgba(0, 0, 0, 0.5),
        0 0 25px rgba(0, 0, 0, 0.25);
      overflow: hidden;
    }

    /* Tape strip */
    .card::before {
      content: '';
      position: absolute;
      top: -6px;
      left: calc(35% + var(--tape-x, 0px));
      width: 70px;
      height: 20px;
      background: rgba(212, 201, 168, 0.18);
      border: 1px solid rgba(212, 201, 168, 0.08);
      transform: rotate(calc(var(--tape-tilt, 2) * 1deg));
      z-index: 2;
    }

    .card h4 {
      font-family: 'Permanent Marker', cursive;
      color: var(--grunge-mustard);
      font-size: 1.15rem;
      margin-bottom: 0.6rem;
      transform: rotate(-0.5deg);
    }

    .card p {
      font-size: 0.9rem;
      line-height: 1.7;
      color: var(--grunge-paper);
    }

    .card .label {
      font-family: 'Share Tech Mono', monospace;
      font-size: 0.7rem;
      text-transform: uppercase;
      letter-spacing: 0.2em;
      color: var(--grunge-smoke);
      margin-bottom: 0.5rem;
      display: block;
    }

    /* ---- Flannel Accent Band ---- */
    .flannel-band {
      height: 8px;
      background: repeating-linear-gradient(
        90deg,
        var(--grunge-dark-olive) 0px,
        var(--grunge-dark-olive) 6px,
        var(--grunge-rust) 6px,
        var(--grunge-rust) 8px,
        var(--grunge-dark-olive) 8px,
        var(--grunge-dark-olive) 12px,
        var(--grunge-flannel) 12px,
        var(--grunge-flannel) 14px
      );
      opacity: 0.6;
    }

    /* ---- Buttons ---- */
    .btn {
      display: inline-block;
      padding: 0.75rem 2rem;
      font-family: 'Permanent Marker', cursive;
      font-size: 1rem;
      letter-spacing: 0.05em;
      text-transform: uppercase;
      text-decoration: none;
      color: var(--grunge-white);
      background: var(--grunge-charcoal);
      border: 2px solid var(--grunge-rust);
      cursor: pointer;
      transform: rotate(-1deg);
      transition: all 0.15s ease;
      box-shadow: 3px 3px 0 rgba(0, 0, 0, 0.5);
    }

    .btn:hover {
      background: var(--grunge-rust);
      color: var(--grunge-soot);
      transform: rotate(0.5deg) translate(-1px, -1px);
      box-shadow: 5px 5px 0 rgba(0, 0, 0, 0.6);
    }

    .btn:active {
      transform: translate(2px, 2px);
      box-shadow: 1px 1px 0 rgba(0, 0, 0, 0.4);
    }

    .btn--ghost {
      background: transparent;
      border-color: var(--grunge-smoke);
      color: var(--grunge-paper);
    }

    .btn--ghost:hover {
      border-color: var(--grunge-mustard);
      color: var(--grunge-mustard);
      background: rgba(184, 134, 11, 0.08);
    }

    .btn--sticker {
      background: var(--grunge-mustard);
      color: var(--grunge-soot);
      border-color: var(--grunge-soot);
      transform: rotate(2deg);
    }

    .btn--sticker:hover {
      transform: rotate(-1deg) scale(1.05);
    }

    .btn-group {
      display: flex;
      gap: 1rem;
      flex-wrap: wrap;
      margin: 2rem 0;
    }

    /* ---- Splatter Divider ---- */
    .splatter-divider {
      border: none;
      height: 1px;
      background: var(--grunge-concrete);
      position: relative;
      margin: 3rem 0;
      opacity: 0.35;
    }

    .splatter-divider::before {
      content: '';
      position: absolute;
      top: -5px;
      left: 18%;
      width: 8px;
      height: 8px;
      border-radius: 50%;
      background: var(--grunge-rust);
      box-shadow:
        30px 3px 0 2px var(--grunge-rust),
        65px -2px 0 1px var(--grunge-rust),
        110px 4px 0 3px var(--grunge-rust),
        170px -1px 0 1px var(--grunge-rust),
        240px 2px 0 2px var(--grunge-rust);
      opacity: 0.3;
    }

    /* ---- Xerox Image Treatment ---- */
    .xerox-img {
      filter: contrast(1.8) grayscale(1) brightness(1.15);
      mix-blend-mode: luminosity;
      border: 3px solid var(--grunge-soot);
      display: block;
      width: 100%;
    }

    /* ---- Zine Collage Section ---- */
    .zine-collage {
      position: relative;
      min-height: 350px;
      margin: 2rem 0;
    }

    .zine-piece {
      position: absolute;
      background: var(--grunge-paper);
      color: var(--grunge-soot);
      padding: 1rem;
      border: 1px solid rgba(0, 0, 0, 0.12);
      transform: rotate(calc(var(--r, 0) * 1deg));
      z-index: var(--z, 1);
      max-width: 250px;
      box-shadow: 2px 2px 0 rgba(0, 0, 0, 0.2);
      font-family: 'Courier Prime', monospace;
      font-size: 0.8rem;
      line-height: 1.6;
    }

    .zine-piece::before {
      content: '';
      position: absolute;
      top: -6px;
      right: 20%;
      width: 50px;
      height: 16px;
      background: rgba(212, 201, 168, 0.3);
      transform: rotate(calc(var(--tape-r, 3) * 1deg));
    }

    .zine-piece--dark {
      background: var(--grunge-soot);
      color: var(--grunge-white);
      font-family: 'Permanent Marker', cursive;
      font-size: 1.2rem;
      text-transform: uppercase;
    }

    /* ---- Scrawled Annotation ---- */
    .scrawl {
      font-family: 'Rock Salt', cursive;
      font-size: 0.75rem;
      color: var(--grunge-rust);
      transform: rotate(-3deg);
      display: inline-block;
    }

    /* ---- Quote / Callout ---- */
    blockquote {
      border-left: 4px solid var(--grunge-rust);
      padding: 1.5rem 1.5rem 1.5rem 2rem;
      margin: 2rem 0;
      background: rgba(59, 63, 43, 0.2);
      transform: rotate(-0.3deg);
      position: relative;
      font-style: italic;
      color: var(--grunge-white);
    }

    blockquote::before {
      content: '\201C';
      position: absolute;
      top: -0.3rem;
      left: 0.5rem;
      font-family: 'Permanent Marker', cursive;
      font-size: 3rem;
      color: var(--grunge-rust);
      opacity: 0.3;
      line-height: 1;
    }

    /* ---- Footer ---- */
    footer {
      text-align: center;
      padding: 3rem 2rem;
      background: var(--grunge-soot);
      border-top: 3px solid var(--grunge-concrete);
      font-family: 'Share Tech Mono', monospace;
      font-size: 0.75rem;
      letter-spacing: 0.15em;
      text-transform: uppercase;
      color: var(--grunge-smoke);
    }

    footer a {
      color: var(--grunge-rust);
      text-decoration: none;
      border-bottom: 1px solid rgba(160, 82, 45, 0.3);
    }

    footer a:hover {
      color: var(--grunge-mustard);
    }

    /* ---- Links ---- */
    a.text-link {
      color: var(--grunge-rust);
      text-decoration: none;
      border-bottom: 1px solid rgba(160, 82, 45, 0.4);
      transition: color 0.15s;
    }

    a.text-link:hover {
      color: var(--grunge-mustard);
      border-bottom-color: var(--grunge-mustard);
    }

    /* ---- Responsive ---- */
    @media (max-width: 640px) {
      nav {
        flex-direction: column;
        gap: 1rem;
        text-align: center;
      }

      nav ul { gap: 1rem; flex-wrap: wrap; justify-content: center; }

      .hero { min-height: 60vh; padding: 3rem 1.5rem; }

      .card-grid { grid-template-columns: 1fr; }

      .zine-collage { min-height: auto; position: static; }

      .zine-piece {
        position: static;
        transform: rotate(calc(var(--r, 0) * 0.5deg));
        max-width: 100%;
        margin-bottom: 1rem;
      }
    }
  </style>
</head>
<body>

  <!-- Navigation -->
  <nav>
    <a href="#" class="brand">grunge.zine</a>
    <ul>
      <li><a href="#" class="active">Home</a></li>
      <li><a href="#">About</a></li>
      <li><a href="#">Music</a></li>
      <li><a href="#">Zines</a></li>
      <li><a href="#">Contact</a></li>
    </ul>
  </nav>

  <!-- Hero -->
  <section class="hero">
    <div class="hero-content">
      <h1>Smells Like<br><em>Raw Design</em></h1>
      <p class="tagline">Seattle // 1991 // Anti-establishment aesthetics</p>
      <div class="btn-group">
        <a href="#" class="btn">Explore</a>
        <a href="#" class="btn btn--ghost">Read Zine</a>
      </div>
    </div>
  </section>

  <div class="torn-edge"></div>

  <!-- About Section -->
  <section>
    <h2>the aesthetic</h2>
    <p>Born from the rain-soaked basements and thrift stores of the Pacific Northwest, 90s Grunge rejected the polished excess of the 1980s in favor of raw, unfiltered expression. It was never about looking good. It was about looking <em>real</em>.</p>

    <hr class="splatter-divider">

    <blockquote>
      Here we are now, in a world of distressed textures, torn edges, and the beautiful imperfection of things made by hand. The grunge aesthetic endures because authenticity never goes out of style.
    </blockquote>
  </section>

  <div class="flannel-band"></div>

  <!-- Cards Section -->
  <section>
    <h2>core elements</h2>
    <div class="card-grid">
      <div class="card" style="--tilt: -1; --tape-tilt: 3; --tape-x: -10px">
        <span class="label">01 // textures</span>
        <h4>Distressed Surfaces</h4>
        <p>Every surface tells a story of wear -- torn paper, crumpled fabric, scratched film. Nothing is pristine. Everything has been touched, used, and lived in.</p>
      </div>
      <div class="card" style="--tilt: 0.8; --tape-tilt: -2; --tape-x: 20px">
        <span class="label">02 // typography</span>
        <h4>Scrawled & Typed</h4>
        <p>Handwritten marker text collides with typewriter output. Letters bounce on uneven baselines. Legibility is secondary to raw emotional expression.</p>
      </div>
      <div class="card" style="--tilt: -0.5; --tape-tilt: 1; --tape-x: 5px">
        <span class="label">03 // palette</span>
        <h4>Dark Earth Tones</h4>
        <p>Olive, rust, charcoal, mustard, and faded denim. The colors of flannel shirts, coffee-stained notebooks, and Pacific Northwest forests in November.</p>
      </div>
    </div>
  </section>

  <div class="torn-edge"></div>

  <!-- Zine Collage Section -->
  <section>
    <h2>zine culture</h2>
    <p>Cut, paste, photocopy, distribute. The zine was the original social media -- self-published, unfiltered, and distributed hand-to-hand outside shows and in record stores.</p>

    <div class="zine-collage">
      <div class="zine-piece" style="--r: -3; --z: 2; --tape-r: 5; top: 10px; left: 5%;">
        Photocopied at 3am on a stolen Kinko's card. Stapled with whatever was in the junk drawer. Distributed for free or traded for other zines.
      </div>
      <div class="zine-piece zine-piece--dark" style="--r: 2; --z: 3; top: 30px; right: 5%;">
        DIY or die
      </div>
      <div class="zine-piece" style="--r: -1.5; --z: 1; --tape-r: -3; top: 180px; left: 15%;">
        The imperfections ARE the design. Every smudge, every misaligned letter, every toner streak is a mark of authenticity.
      </div>
    </div>
  </section>

  <div class="flannel-band"></div>

  <!-- Buttons Section -->
  <section>
    <h2>interactions</h2>
    <h3>Button Variants</h3>
    <div class="btn-group">
      <a href="#" class="btn">Primary</a>
      <a href="#" class="btn btn--ghost">Ghost</a>
      <a href="#" class="btn btn--sticker">Sticker</a>
    </div>
    <br>
    <p>Even interactive elements carry the weight of analog imperfection. Buttons tilt, hover states shift like papers sliding on a table, and nothing snaps to a perfect grid. <span class="scrawl">^ these actually work!</span></p>
  </section>

  <div class="torn-edge"></div>

  <!-- Footer -->
  <footer>
    <p>assembled by hand &mdash; photocopied at midnight &mdash; <a href="#">grunge.zine</a> &mdash; circa 1994</p>
  </footer>

</body>
</html>
```
